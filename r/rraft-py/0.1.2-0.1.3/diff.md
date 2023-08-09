# Comparing `tmp/rraft_py-0.1.2.tar.gz` & `tmp/rraft_py-0.1.3.tar.gz`

## Comparing `rraft_py-0.1.2.tar` & `rraft_py-0.1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 rraft_py-0.1.2/Cargo.toml
--rw-r--r--   0      501       20      206 2023-02-27 06:56:36.000000 rraft_py-0.1.2/.editorconfig
--rw-r--r--   0      501       20      788 2023-07-31 07:01:16.000000 rraft_py-0.1.2/.github/workflows/test.yml
--rw-r--r--   0      501       20      700 2023-04-06 07:12:36.000000 rraft_py-0.1.2/.gitignore
--rw-r--r--   0      501       20        7 2023-08-09 02:53:53.000000 rraft_py-0.1.2/.python-version
--rw-r--r--   0      501       20    11345 2023-07-31 07:01:16.000000 rraft_py-0.1.2/LICENSE
--rw-r--r--   0      501       20      599 2023-08-09 04:47:38.000000 rraft_py-0.1.2/Makefile
--rw-r--r--   0      501       20     3061 2023-08-08 00:51:37.000000 rraft_py-0.1.2/README.md
--rw-r--r--   0      501       20      223 2023-07-31 07:01:16.000000 rraft_py-0.1.2/benches/suites/progress.py
--rw-r--r--   0      501       20     4467 2023-07-31 07:01:16.000000 rraft_py-0.1.2/benches/suites/raft.py
--rw-r--r--   0      501       20        0 2023-07-31 07:01:16.000000 rraft_py-0.1.2/benches/suites/raw_node.py
--rw-r--r--   0      501       20    12446 2023-07-31 07:01:34.000000 rraft_py-0.1.2/example/multi_mem_node/main.py
--rw-r--r--   0      501       20     6010 2023-07-31 07:01:16.000000 rraft_py-0.1.2/example/single_mem_node/use_coroutine.py
--rw-r--r--   0      501       20     6293 2023-08-09 04:43:12.000000 rraft_py-0.1.2/example/single_mem_node/use_threading.py
--rw-r--r--   0      501       20      150 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/README.md
--rw-r--r--   0      501       20     2290 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/src/interface.py
--rw-r--r--   0      501       20     6835 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/src/network.py
--rw-r--r--   0      501       20     1004 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_failpoints.py
--rw-r--r--   0      501       20   186320 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raft.py
--rw-r--r--   0      501       20     7732 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raft_flow_control.py
--rw-r--r--   0      501       20    34562 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raft_paper.py
--rw-r--r--   0      501       20     6467 2023-08-04 03:36:56.000000 rraft_py-0.1.2/harness/tests/test_raft_snap.py
--rw-r--r--   0      501       20    59741 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raw_node.py
--rw-r--r--   0      501       20     5874 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/utils.py
--rw-r--r--   0      501       20        0 2023-01-26 07:03:57.000000 rraft_py-0.1.2/py.typed
--rw-r--r--   0      501       20      400 2023-08-09 03:08:57.000000 rraft_py-0.1.2/pyproject.toml
--rw-r--r--   0      501       20       36 2023-07-31 07:01:16.000000 rraft_py-0.1.2/pytest.ini
--rw-r--r--   0      501       20       52 2023-08-09 02:54:19.000000 rraft_py-0.1.2/requirements.txt
--rw-r--r--   0      501       20   114743 2023-08-09 04:46:38.000000 rraft_py-0.1.2/rraft.pyi
--rw-r--r--   0      501       20     9790 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/config.rs
--rw-r--r--   0      501       20     1332 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/get_entries_context.rs
--rw-r--r--   0      501       20     1906 2023-08-09 04:41:47.000000 rraft_py-0.1.2/src/bindings/global.rs
--rw-r--r--   0      501       20     3547 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/inflights.rs
--rw-r--r--   0      501       20     3716 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/joint_config.rs
--rw-r--r--   0      501       20     2989 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/light_ready.rs
--rw-r--r--   0      501       20     5194 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/majority_config.rs
--rw-r--r--   0      501       20      393 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/mod.rs
--rw-r--r--   0      501       20     1652 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/peer.rs
--rw-r--r--   0      501       20     6960 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/progress.rs
--rw-r--r--   0      501       20     1612 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/progress_state.rs
--rw-r--r--   0      501       20     5916 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/progress_tracker.rs
--rw-r--r--   0      501       20     2715 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/raft_state.rs
--rw-r--r--   0      501       20     3069 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/read_state.rs
--rw-r--r--   0      501       20     1388 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/readonly_option.rs
--rw-r--r--   0      501       20     6371 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/ready.rs
--rw-r--r--   0      501       20     1382 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/snapshot_status.rs
--rw-r--r--   0      501       20     2572 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/soft_state.rs
--rw-r--r--   0      501       20     1731 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/state_role.rs
--rw-r--r--   0      501       20     5229 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/unstable.rs
--rw-r--r--   0      501       20       40 2023-08-09 04:38:46.000000 rraft_py-0.1.2/src/external_bindings/mod.rs
--rw-r--r--   0      501       20     3571 2023-08-09 04:28:59.000000 rraft_py-0.1.2/src/external_bindings/slog.rs
--rw-r--r--   0      501       20     1844 2023-08-09 04:44:33.000000 rraft_py-0.1.2/src/external_bindings/thread_safe_slog.rs
--rw-r--r--   0      501       20     8008 2023-08-09 04:40:34.000000 rraft_py-0.1.2/src/lib.rs
--rw-r--r--   0      501       20     4789 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/mem_storage.rs
--rw-r--r--   0      501       20     4031 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/mem_storage_core.rs
--rw-r--r--   0      501       20       97 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/mod.rs
--rw-r--r--   0      501       20    19404 2023-08-09 02:47:04.000000 rraft_py-0.1.2/src/mem_storage_bindings/raft.rs
--rw-r--r--   0      501       20    11619 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/raft_log.rs
--rw-r--r--   0      501       20     8415 2023-08-08 09:59:49.000000 rraft_py-0.1.2/src/mem_storage_bindings/raw_node.rs
--rw-r--r--   0      501       20       70 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/py_storage_bindings/mod.rs
--rw-r--r--   0      501       20    12837 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/py_storage_bindings/py_storage.rs
--rw-r--r--   0      501       20    19208 2023-08-09 02:48:07.000000 rraft_py-0.1.2/src/py_storage_bindings/raft.rs
--rw-r--r--   0      501       20    11469 2023-08-08 05:35:51.000000 rraft_py-0.1.2/src/py_storage_bindings/raft_log.rs
--rw-r--r--   0      501       20     8271 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/py_storage_bindings/raw_node.rs
--rw-r--r--   0      501       20     6870 2023-08-08 07:53:52.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change.rs
--rw-r--r--   0      501       20     4026 2023-08-08 05:33:36.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_single.rs
--rw-r--r--   0      501       20     2239 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_transition.rs
--rw-r--r--   0      501       20     2051 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_type.rs
--rw-r--r--   0      501       20     6846 2023-08-08 08:33:58.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_v2.rs
--rw-r--r--   0      501       20     6511 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_state.rs
--rw-r--r--   0      501       20     6038 2023-08-08 10:20:16.000000 rraft_py-0.1.2/src/raftpb_bindings/entry.rs
--rw-r--r--   0      501       20     1977 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/entry_type.rs
--rw-r--r--   0      501       20     4025 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/hard_state.rs
--rw-r--r--   0      501       20    11400 2023-08-08 07:54:25.000000 rraft_py-0.1.2/src/raftpb_bindings/message.rs
--rw-r--r--   0      501       20     7115 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/message_type.rs
--rw-r--r--   0      501       20      290 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/mod.rs
--rw-r--r--   0      501       20     4634 2023-08-09 02:55:14.000000 rraft_py-0.1.2/src/raftpb_bindings/snapshot.rs
--rw-r--r--   0      501       20     4570 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/snapshot_metadata.rs
--rw-r--r--   0      501       20      475 2023-08-09 02:36:39.000000 rraft_py-0.1.2/src/utils/deserializer.rs
--rw-r--r--   0      501       20     9258 2023-08-04 00:35:31.000000 rraft_py-0.1.2/src/utils/errors.rs
--rw-r--r--   0      501       20       78 2023-08-08 05:00:26.000000 rraft_py-0.1.2/src/utils/mod.rs
--rw-r--r--   0      501       20     4407 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/utils/reference.rs
--rw-r--r--   0      501       20      409 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/utils/unsafe_cast.rs
--rw-r--r--   0      501       20    27236 2023-08-09 04:45:25.000000 rraft_py-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     3632 1970-01-01 00:00:00.000000 rraft_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 rraft_py-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20      206 2023-02-27 06:56:36.000000 rraft_py-0.1.3/.editorconfig
+-rw-r--r--   0      501       20      788 2023-07-31 07:01:16.000000 rraft_py-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0      501       20      700 2023-04-06 07:12:36.000000 rraft_py-0.1.3/.gitignore
+-rw-r--r--   0      501       20        7 2023-08-09 02:53:53.000000 rraft_py-0.1.3/.python-version
+-rw-r--r--   0      501       20    11345 2023-07-31 07:01:16.000000 rraft_py-0.1.3/LICENSE
+-rw-r--r--   0      501       20      599 2023-08-09 04:47:38.000000 rraft_py-0.1.3/Makefile
+-rw-r--r--   0      501       20     3061 2023-08-08 00:51:37.000000 rraft_py-0.1.3/README.md
+-rw-r--r--   0      501       20      223 2023-07-31 07:01:16.000000 rraft_py-0.1.3/benches/suites/progress.py
+-rw-r--r--   0      501       20     4467 2023-07-31 07:01:16.000000 rraft_py-0.1.3/benches/suites/raft.py
+-rw-r--r--   0      501       20        0 2023-07-31 07:01:16.000000 rraft_py-0.1.3/benches/suites/raw_node.py
+-rw-r--r--   0      501       20    12446 2023-07-31 07:01:34.000000 rraft_py-0.1.3/example/multi_mem_node/main.py
+-rw-r--r--   0      501       20     6010 2023-07-31 07:01:16.000000 rraft_py-0.1.3/example/single_mem_node/use_coroutine.py
+-rw-r--r--   0      501       20     6293 2023-08-09 04:43:12.000000 rraft_py-0.1.3/example/single_mem_node/use_threading.py
+-rw-r--r--   0      501       20      150 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/README.md
+-rw-r--r--   0      501       20     2290 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/src/interface.py
+-rw-r--r--   0      501       20     6835 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/src/network.py
+-rw-r--r--   0      501       20     1004 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/tests/test_failpoints.py
+-rw-r--r--   0      501       20   186320 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/tests/test_raft.py
+-rw-r--r--   0      501       20     7732 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/tests/test_raft_flow_control.py
+-rw-r--r--   0      501       20    34562 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/tests/test_raft_paper.py
+-rw-r--r--   0      501       20     6467 2023-08-04 03:36:56.000000 rraft_py-0.1.3/harness/tests/test_raft_snap.py
+-rw-r--r--   0      501       20    59741 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/tests/test_raw_node.py
+-rw-r--r--   0      501       20     5874 2023-07-31 07:01:16.000000 rraft_py-0.1.3/harness/utils.py
+-rw-r--r--   0      501       20        0 2023-01-26 07:03:57.000000 rraft_py-0.1.3/py.typed
+-rw-r--r--   0      501       20      400 2023-08-09 03:08:57.000000 rraft_py-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20       36 2023-07-31 07:01:16.000000 rraft_py-0.1.3/pytest.ini
+-rw-r--r--   0      501       20       52 2023-08-09 02:54:19.000000 rraft_py-0.1.3/requirements.txt
+-rw-r--r--   0      501       20   114957 2023-08-09 05:02:56.000000 rraft_py-0.1.3/rraft.pyi
+-rw-r--r--   0      501       20     9790 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/config.rs
+-rw-r--r--   0      501       20     1332 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/get_entries_context.rs
+-rw-r--r--   0      501       20     1906 2023-08-09 04:41:47.000000 rraft_py-0.1.3/src/bindings/global.rs
+-rw-r--r--   0      501       20     3547 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/inflights.rs
+-rw-r--r--   0      501       20     3716 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/joint_config.rs
+-rw-r--r--   0      501       20     2989 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/light_ready.rs
+-rw-r--r--   0      501       20     5194 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/majority_config.rs
+-rw-r--r--   0      501       20      393 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/mod.rs
+-rw-r--r--   0      501       20     1652 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/peer.rs
+-rw-r--r--   0      501       20     6960 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/progress.rs
+-rw-r--r--   0      501       20     1612 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/progress_state.rs
+-rw-r--r--   0      501       20     5916 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/progress_tracker.rs
+-rw-r--r--   0      501       20     2715 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/raft_state.rs
+-rw-r--r--   0      501       20     3069 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/read_state.rs
+-rw-r--r--   0      501       20     1388 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/readonly_option.rs
+-rw-r--r--   0      501       20     6371 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/ready.rs
+-rw-r--r--   0      501       20     1382 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/snapshot_status.rs
+-rw-r--r--   0      501       20     2572 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/soft_state.rs
+-rw-r--r--   0      501       20     1731 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/state_role.rs
+-rw-r--r--   0      501       20     5229 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/bindings/unstable.rs
+-rw-r--r--   0      501       20       40 2023-08-09 04:38:46.000000 rraft_py-0.1.3/src/external_bindings/mod.rs
+-rw-r--r--   0      501       20     3571 2023-08-09 04:28:59.000000 rraft_py-0.1.3/src/external_bindings/slog.rs
+-rw-r--r--   0      501       20     1844 2023-08-09 04:44:33.000000 rraft_py-0.1.3/src/external_bindings/thread_safe_slog.rs
+-rw-r--r--   0      501       20     8008 2023-08-09 04:40:34.000000 rraft_py-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20     4789 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/mem_storage_bindings/mem_storage.rs
+-rw-r--r--   0      501       20     4031 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/mem_storage_bindings/mem_storage_core.rs
+-rw-r--r--   0      501       20       97 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/mem_storage_bindings/mod.rs
+-rw-r--r--   0      501       20    19404 2023-08-09 02:47:04.000000 rraft_py-0.1.3/src/mem_storage_bindings/raft.rs
+-rw-r--r--   0      501       20    11619 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/mem_storage_bindings/raft_log.rs
+-rw-r--r--   0      501       20     8415 2023-08-08 09:59:49.000000 rraft_py-0.1.3/src/mem_storage_bindings/raw_node.rs
+-rw-r--r--   0      501       20       70 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/py_storage_bindings/mod.rs
+-rw-r--r--   0      501       20    12837 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/py_storage_bindings/py_storage.rs
+-rw-r--r--   0      501       20    19208 2023-08-09 02:48:07.000000 rraft_py-0.1.3/src/py_storage_bindings/raft.rs
+-rw-r--r--   0      501       20    11469 2023-08-08 05:35:51.000000 rraft_py-0.1.3/src/py_storage_bindings/raft_log.rs
+-rw-r--r--   0      501       20     8271 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/py_storage_bindings/raw_node.rs
+-rw-r--r--   0      501       20     6870 2023-08-08 07:53:52.000000 rraft_py-0.1.3/src/raftpb_bindings/conf_change.rs
+-rw-r--r--   0      501       20     4026 2023-08-08 05:33:36.000000 rraft_py-0.1.3/src/raftpb_bindings/conf_change_single.rs
+-rw-r--r--   0      501       20     2239 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/conf_change_transition.rs
+-rw-r--r--   0      501       20     2051 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/conf_change_type.rs
+-rw-r--r--   0      501       20     6846 2023-08-08 08:33:58.000000 rraft_py-0.1.3/src/raftpb_bindings/conf_change_v2.rs
+-rw-r--r--   0      501       20     6511 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/conf_state.rs
+-rw-r--r--   0      501       20     6038 2023-08-08 10:20:16.000000 rraft_py-0.1.3/src/raftpb_bindings/entry.rs
+-rw-r--r--   0      501       20     1977 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/entry_type.rs
+-rw-r--r--   0      501       20     4025 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/hard_state.rs
+-rw-r--r--   0      501       20    11400 2023-08-08 07:54:25.000000 rraft_py-0.1.3/src/raftpb_bindings/message.rs
+-rw-r--r--   0      501       20     7115 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/message_type.rs
+-rw-r--r--   0      501       20      290 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/mod.rs
+-rw-r--r--   0      501       20     4634 2023-08-09 02:55:14.000000 rraft_py-0.1.3/src/raftpb_bindings/snapshot.rs
+-rw-r--r--   0      501       20     4570 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/raftpb_bindings/snapshot_metadata.rs
+-rw-r--r--   0      501       20      475 2023-08-09 02:36:39.000000 rraft_py-0.1.3/src/utils/deserializer.rs
+-rw-r--r--   0      501       20     9258 2023-08-04 00:35:31.000000 rraft_py-0.1.3/src/utils/errors.rs
+-rw-r--r--   0      501       20       78 2023-08-08 05:00:26.000000 rraft_py-0.1.3/src/utils/mod.rs
+-rw-r--r--   0      501       20     4407 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/utils/reference.rs
+-rw-r--r--   0      501       20      409 2023-07-31 07:01:16.000000 rraft_py-0.1.3/src/utils/unsafe_cast.rs
+-rw-r--r--   0      501       20    27236 2023-08-09 05:03:09.000000 rraft_py-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     3632 1970-01-01 00:00:00.000000 rraft_py-0.1.3/PKG-INFO
```

### Comparing `rraft_py-0.1.2/Cargo.toml` & `rraft_py-0.1.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rraft-py"
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Lablup Inc."]
 license = "Apache-2.0"
 repository = "https://github.com/lablup/rraft-py"
 readme = "./README.md"
 homepage = "https://github.com/lablup/rraft-py"
 description = """
 Unofficial Python Binding of the tikv/raft-rs
```

### Comparing `rraft_py-0.1.2/.github/workflows/test.yml` & `rraft_py-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/.gitignore` & `rraft_py-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/LICENSE` & `rraft_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/Makefile` & `rraft_py-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/README.md` & `rraft_py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/benches/suites/raft.py` & `rraft_py-0.1.3/benches/suites/raft.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/example/multi_mem_node/main.py` & `rraft_py-0.1.3/example/multi_mem_node/main.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/example/single_mem_node/use_coroutine.py` & `rraft_py-0.1.3/example/single_mem_node/use_coroutine.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/example/single_mem_node/use_threading.py` & `rraft_py-0.1.3/example/single_mem_node/use_threading.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/src/interface.py` & `rraft_py-0.1.3/harness/src/interface.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/src/network.py` & `rraft_py-0.1.3/harness/src/network.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/tests/test_failpoints.py` & `rraft_py-0.1.3/harness/tests/test_failpoints.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/tests/test_raft.py` & `rraft_py-0.1.3/harness/tests/test_raft.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/tests/test_raft_flow_control.py` & `rraft_py-0.1.3/harness/tests/test_raft_flow_control.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/tests/test_raft_paper.py` & `rraft_py-0.1.3/harness/tests/test_raft_paper.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/tests/test_raft_snap.py` & `rraft_py-0.1.3/harness/tests/test_raft_snap.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/tests/test_raw_node.py` & `rraft_py-0.1.3/harness/tests/test_raw_node.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/harness/utils.py` & `rraft_py-0.1.3/harness/utils.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/rraft.pyi` & `rraft_py-0.1.3/rraft.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -382,6791 +382,6804 @@
 000017d0: 7365 6c66 2920 2d3e 2022 4c6f 6767 6572  self) -> "Logger
 000017e0: 5265 6622 3a20 2e2e 2e0a 0a63 6c61 7373  Ref": .....class
 000017f0: 204c 6f67 6765 7252 6566 285f 5f41 5049   LoggerRef(__API
 00001800: 5f4c 6f67 6765 7229 3a0a 2020 2020 2222  _Logger):.    ""
 00001810: 2220 2222 220a 0a63 6c61 7373 2054 6872  " """..class Thr
 00001820: 6561 6453 6166 654c 6f67 6765 7228 5f5f  eadSafeLogger(__
 00001830: 4150 495f 4c6f 6767 6572 293a 0a20 2020  API_Logger):.   
-00001840: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00001850: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00001860: 2020 2073 656c 662c 2063 6861 6e5f 7369     self, chan_si
-00001870: 7a65 3a20 696e 742c 206f 7665 7266 6c6f  ze: int, overflo
-00001880: 775f 7374 7261 7465 6779 3a20 224f 7665  w_strategy: "Ove
-00001890: 7266 6c6f 7753 7472 6174 6567 7922 0a20  rflowStrategy". 
-000018a0: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-000018b0: 2e0a 0a63 6c61 7373 205f 5f41 5049 5f52  ...class __API_R
-000018c0: 6166 7453 7461 7465 285f 5f43 6c6f 6e65  aftState(__Clone
-000018d0: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
-000018e0: 6c6f 6e65 2873 656c 6629 202d 3e20 2252  lone(self) -> "R
-000018f0: 6166 7453 7461 7465 223a 202e 2e2e 0a20  aftState": .... 
-00001900: 2020 2064 6566 2069 6e69 7469 616c 697a     def initializ
-00001910: 6564 2873 656c 6629 202d 3e20 626f 6f6c  ed(self) -> bool
-00001920: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00001930: 2020 2020 2020 496e 6469 6361 7465 7320        Indicates 
-00001940: 7468 6520 6052 6166 7453 7461 7465 6020  the `RaftState` 
-00001950: 6973 2069 6e69 7469 616c 697a 6564 206f  is initialized o
-00001960: 7220 6e6f 742e 0a20 2020 2020 2020 2022  r not..        "
-00001970: 2222 0a20 2020 2064 6566 2067 6574 5f63  "".    def get_c
-00001980: 6f6e 665f 7374 6174 6528 7365 6c66 2920  onf_state(self) 
-00001990: 2d3e 2022 436f 6e66 5374 6174 6552 6566  -> "ConfStateRef
-000019a0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-000019b0: 2020 2020 2020 2060 636f 6e66 5f73 7461         `conf_sta
-000019c0: 7465 603a 2052 6563 6f72 6473 2074 6865  te`: Records the
-000019d0: 2063 7572 7265 6e74 206e 6f64 6520 4944   current node ID
-000019e0: 7320 6c69 6b65 2060 5b31 2c20 322c 2033  s like `[1, 2, 3
-000019f0: 5d60 2069 6e20 7468 6520 636c 7573 7465  ]` in the cluste
-00001a00: 722e 2045 7665 7279 2052 6166 7420 6e6f  r. Every Raft no
-00001a10: 6465 206d 7573 7420 6861 7665 2061 0a20  de must have a. 
-00001a20: 2020 2020 2020 2075 6e69 7175 6520 4944         unique ID
-00001a30: 2069 6e20 7468 6520 636c 7573 7465 723b   in the cluster;
-00001a40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00001a50: 2064 6566 2073 6574 5f63 6f6e 665f 7374   def set_conf_st
-00001a60: 6174 6528 7365 6c66 2c20 6373 3a20 2243  ate(self, cs: "C
-00001a70: 6f6e 6653 7461 7465 5265 6622 2920 2d3e  onfStateRef") ->
-00001a80: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00001a90: 2222 0a20 2020 2020 2020 2060 636f 6e66  "".        `conf
-00001aa0: 5f73 7461 7465 603a 2052 6563 6f72 6473  _state`: Records
-00001ab0: 2074 6865 2063 7572 7265 6e74 206e 6f64   the current nod
-00001ac0: 6520 4944 7320 6c69 6b65 2060 5b31 2c20  e IDs like `[1, 
-00001ad0: 322c 2033 5d60 2069 6e20 7468 6520 636c  2, 3]` in the cl
-00001ae0: 7573 7465 722e 2045 7665 7279 2052 6166  uster. Every Raf
-00001af0: 7420 6e6f 6465 206d 7573 7420 6861 7665  t node must have
-00001b00: 2061 0a20 2020 2020 2020 2075 6e69 7175   a.        uniqu
-00001b10: 6520 4944 2069 6e20 7468 6520 636c 7573  e ID in the clus
-00001b20: 7465 723b 0a20 2020 2020 2020 2022 2222  ter;.        """
-00001b30: 0a20 2020 2064 6566 2067 6574 5f68 6172  .    def get_har
-00001b40: 645f 7374 6174 6528 7365 6c66 2920 2d3e  d_state(self) ->
-00001b50: 2022 4861 7264 5374 6174 6552 6566 223a   "HardStateRef":
-00001b60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00001b70: 2020 2020 2060 6861 7264 5f73 7461 7465       `hard_state
-00001b80: 603a 2043 6f6e 7461 696e 7320 7468 6520  `: Contains the 
-00001b90: 6c61 7374 206d 6574 6120 696e 666f 726d  last meta inform
-00001ba0: 6174 696f 6e20 696e 636c 7564 696e 6720  ation including 
-00001bb0: 636f 6d6d 6974 2069 6e64 6578 2c20 7468  commit index, th
-00001bc0: 6520 766f 7465 206c 6561 6465 722c 2061  e vote leader, a
-00001bd0: 6e64 2074 6865 2076 6f74 6520 7465 726d  nd the vote term
-00001be0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00001bf0: 2020 6465 6620 7365 745f 6861 7264 5f73    def set_hard_s
-00001c00: 7461 7465 2873 656c 662c 2068 733a 2022  tate(self, hs: "
-00001c10: 4861 7264 5374 6174 6552 6566 2229 202d  HardStateRef") -
-00001c20: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00001c30: 2222 220a 2020 2020 2020 2020 6068 6172  """.        `har
-00001c40: 645f 7374 6174 6560 3a20 436f 6e74 6169  d_state`: Contai
-00001c50: 6e73 2074 6865 206c 6173 7420 6d65 7461  ns the last meta
-00001c60: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e63   information inc
-00001c70: 6c75 6469 6e67 2063 6f6d 6d69 7420 696e  luding commit in
-00001c80: 6465 782c 2074 6865 2076 6f74 6520 6c65  dex, the vote le
-00001c90: 6164 6572 2c20 616e 6420 7468 6520 766f  ader, and the vo
-00001ca0: 7465 2074 6572 6d2e 0a20 2020 2020 2020  te term..       
-00001cb0: 2022 2222 0a0a 636c 6173 7320 5261 6674   """..class Raft
-00001cc0: 5374 6174 6528 5f5f 4150 495f 5261 6674  State(__API_Raft
-00001cd0: 5374 6174 6529 3a0a 2020 2020 2222 220a  State):.    """.
-00001ce0: 2020 2020 486f 6c64 7320 626f 7468 2074      Holds both t
-00001cf0: 6865 2068 6172 6420 7374 6174 6520 2863  he hard state (c
-00001d00: 6f6d 6d69 7420 696e 6465 782c 2076 6f74  ommit index, vot
-00001d10: 6520 6c65 6164 6572 2c20 7465 726d 2920  e leader, term) 
-00001d20: 616e 6420 7468 6520 636f 6e66 6967 7572  and the configur
-00001d30: 6174 696f 6e20 7374 6174 650a 2020 2020  ation state.    
-00001d40: 2843 7572 7265 6e74 206e 6f64 6520 4944  (Current node ID
-00001d50: 7329 0a20 2020 2022 2222 0a0a 2020 2020  s).    """..    
-00001d60: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001d70: 6629 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  f) -> None: ....
-00001d80: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
-00001d90: 2873 656c 6629 202d 3e20 2252 6166 7453  (self) -> "RaftS
-00001da0: 7461 7465 5265 6622 3a20 2e2e 2e0a 2020  tateRef": ....  
-00001db0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-00001dc0: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
-00001dd0: 2920 2d3e 2022 5261 6674 5374 6174 6522  ) -> "RaftState"
-00001de0: 3a20 2e2e 2e0a 0a63 6c61 7373 2052 6166  : .....class Raf
-00001df0: 7453 7461 7465 5265 6628 5f5f 4150 495f  tStateRef(__API_
-00001e00: 5261 6674 5374 6174 6529 3a0a 2020 2020  RaftState):.    
-00001e10: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
-00001e20: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
-00001e30: 3a60 5261 6674 5374 6174 6560 2e0a 2020  :`RaftState`..  
-00001e40: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-00001e50: 5049 5f53 746f 7261 6765 436f 7265 3a0a  PI_StorageCore:.
-00001e60: 2020 2020 6465 6620 6170 7065 6e64 2873      def append(s
-00001e70: 656c 662c 2065 6e74 733a 204c 6973 745b  elf, ents: List[
-00001e80: 2245 6e74 7279 225d 207c 204c 6973 745b  "Entry"] | List[
-00001e90: 2245 6e74 7279 5265 6622 5d29 202d 3e20  "EntryRef"]) -> 
-00001ea0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00001eb0: 220a 2020 2020 2020 2020 4170 7065 6e64  ".        Append
-00001ec0: 2074 6865 206e 6577 2065 6e74 7269 6573   the new entries
-00001ed0: 2074 6f20 7374 6f72 6167 652e 0a0a 2020   to storage...  
-00001ee0: 2020 2020 2020 2320 5061 6e69 6373 0a0a        # Panics..
-00001ef0: 2020 2020 2020 2020 5061 6e69 6373 2069          Panics i
-00001f00: 6620 6065 6e74 7360 2063 6f6e 7461 696e  f `ents` contain
-00001f10: 7320 636f 6d70 6163 7465 6420 656e 7472  s compacted entr
-00001f20: 6965 732c 206f 7220 7468 6572 6527 7320  ies, or there's 
-00001f30: 6120 6761 7020 6265 7477 6565 6e20 6065  a gap between `e
-00001f40: 6e74 7360 2061 6e64 2074 6865 206c 6173  nts` and the las
-00001f50: 740a 2020 2020 2020 2020 7265 6365 6976  t.        receiv
-00001f60: 6564 2065 6e74 7279 2069 6e20 7468 6520  ed entry in the 
-00001f70: 7374 6f72 6167 652e 0a20 2020 2020 2020  storage..       
-00001f80: 2022 2222 0a20 2020 2064 6566 2061 7070   """.    def app
-00001f90: 6c79 5f73 6e61 7073 686f 7428 7365 6c66  ly_snapshot(self
-00001fa0: 2c20 736e 6170 7368 6f74 3a20 2253 6e61  , snapshot: "Sna
-00001fb0: 7073 686f 7422 207c 2022 536e 6170 7368  pshot" | "Snapsh
-00001fc0: 6f74 5265 6622 2920 2d3e 204e 6f6e 653a  otRef") -> None:
-00001fd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00001fe0: 2020 2020 204f 7665 7277 7269 7465 7320       Overwrites 
-00001ff0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
-00002000: 7468 6973 2053 746f 7261 6765 206f 626a  this Storage obj
-00002010: 6563 7420 7769 7468 2074 686f 7365 206f  ect with those o
-00002020: 6620 7468 6520 6769 7665 6e20 736e 6170  f the given snap
-00002030: 7368 6f74 2e0a 0a20 2020 2020 2020 2023  shot...        #
-00002040: 2050 616e 6963 730a 0a20 2020 2020 2020   Panics..       
-00002050: 2050 616e 6963 7320 6966 2074 6865 2073   Panics if the s
-00002060: 6e61 7073 686f 7420 696e 6465 7820 6973  napshot index is
-00002070: 206c 6573 7320 7468 616e 2074 6865 2073   less than the s
-00002080: 746f 7261 6765 2773 2066 6972 7374 2069  torage's first i
-00002090: 6e64 6578 2e0a 2020 2020 2020 2020 2222  ndex..        ""
-000020a0: 220a 2020 2020 6465 6620 636f 6d70 6163  ".    def compac
-000020b0: 7428 7365 6c66 2c20 636f 6d70 6163 745f  t(self, compact_
-000020c0: 696e 6465 783a 2069 6e74 2920 2d3e 204e  index: int) -> N
-000020d0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000020e0: 0a20 2020 2020 2020 2044 6973 6361 7264  .        Discard
-000020f0: 7320 616c 6c20 6c6f 6720 656e 7472 6965  s all log entrie
-00002100: 7320 7072 696f 7220 746f 2063 6f6d 7061  s prior to compa
-00002110: 6374 5f69 6e64 6578 2e0a 2020 2020 2020  ct_index..      
-00002120: 2020 4974 2069 7320 7468 6520 6170 706c    It is the appl
-00002130: 6963 6174 696f 6e27 7320 7265 7370 6f6e  ication's respon
-00002140: 7369 6269 6c69 7479 2074 6f20 6e6f 7420  sibility to not 
-00002150: 6174 7465 6d70 7420 746f 2063 6f6d 7061  attempt to compa
-00002160: 6374 2061 6e20 696e 6465 780a 2020 2020  ct an index.    
-00002170: 2020 2020 6772 6561 7465 7220 7468 616e      greater than
-00002180: 2052 6166 744c 6f67 2e61 7070 6c69 6564   RaftLog.applied
-00002190: 2e0a 0a20 2020 2020 2020 2023 2050 616e  ...        # Pan
-000021a0: 6963 730a 0a20 2020 2020 2020 2050 616e  ics..        Pan
-000021b0: 6963 7320 6966 2060 636f 6d70 6163 745f  ics if `compact_
-000021c0: 696e 6465 7860 2069 7320 6869 6768 6572  index` is higher
-000021d0: 2074 6861 6e20 6053 746f 7261 6765 3a3a   than `Storage::
-000021e0: 6c61 7374 5f69 6e64 6578 2826 7365 6c66  last_index(&self
-000021f0: 2920 2b20 3160 2e0a 2020 2020 2020 2020  ) + 1`..        
-00002200: 2222 220a 2020 2020 6465 6620 636f 6d6d  """.    def comm
-00002210: 6974 5f74 6f28 7365 6c66 2c20 696e 6465  it_to(self, inde
-00002220: 783a 2069 6e74 2920 2d3e 204e 6f6e 653a  x: int) -> None:
-00002230: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00002240: 2020 2020 2043 6f6d 6d69 7420 746f 2061       Commit to a
-00002250: 6e20 696e 6465 782e 0a0a 2020 2020 2020  n index...      
-00002260: 2020 2320 5061 6e69 6373 0a0a 2020 2020    # Panics..    
-00002270: 2020 2020 5061 6e69 6373 2069 6620 7468      Panics if th
-00002280: 6572 6520 6973 206e 6f20 7375 6368 2065  ere is no such e
-00002290: 6e74 7279 2069 6e20 7261 6674 206c 6f67  ntry in raft log
-000022a0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-000022b0: 2020 2064 6566 2063 6f6d 6d69 745f 746f     def commit_to
-000022c0: 5f61 6e64 5f73 6574 5f63 6f6e 665f 7374  _and_set_conf_st
-000022d0: 6174 6573 280a 2020 2020 2020 2020 7365  ates(.        se
-000022e0: 6c66 2c20 6964 783a 2069 6e74 2c20 6373  lf, idx: int, cs
-000022f0: 3a20 4f70 7469 6f6e 616c 5b22 436f 6e66  : Optional["Conf
-00002300: 5374 6174 6522 5d20 7c20 4f70 7469 6f6e  State"] | Option
-00002310: 616c 5b22 436f 6e66 5374 6174 6552 6566  al["ConfStateRef
-00002320: 225d 0a20 2020 2029 202d 3e20 4e6f 6e65  "].    ) -> None
-00002330: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00002340: 2020 2020 2020 436f 6d6d 6974 2074 6f20        Commit to 
-00002350: 6069 6478 6020 616e 6420 7365 7420 636f  `idx` and set co
-00002360: 6e66 6967 7572 6174 696f 6e20 746f 2074  nfiguration to t
-00002370: 6865 2067 6976 656e 2073 7461 7465 732e  he given states.
-00002380: 204f 6e6c 7920 7573 6564 2066 6f72 2074   Only used for t
-00002390: 6573 7473 2e0a 2020 2020 2020 2020 2222  ests..        ""
-000023a0: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
-000023b0: 6e66 5f73 7461 7465 2873 656c 662c 2063  nf_state(self, c
-000023c0: 733a 2022 436f 6e66 5374 6174 6522 207c  s: "ConfState" |
-000023d0: 2022 436f 6e66 5374 6174 6552 6566 2229   "ConfStateRef")
-000023e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000023f0: 2020 2222 220a 2020 2020 2020 2020 5361    """.        Sa
-00002400: 7665 7320 7468 6520 6375 7272 656e 7420  ves the current 
-00002410: 636f 6e66 2073 7461 7465 2e0a 2020 2020  conf state..    
-00002420: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00002430: 6861 7264 5f73 7461 7465 2873 656c 6629  hard_state(self)
-00002440: 202d 3e20 2248 6172 6453 7461 7465 5265   -> "HardStateRe
-00002450: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
-00002460: 2020 2020 2020 2020 4765 7420 7468 6520          Get the 
-00002470: 6861 7264 2073 7461 7465 2e0a 2020 2020  hard state..    
-00002480: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00002490: 7365 745f 6861 7264 7374 6174 6528 7365  set_hardstate(se
-000024a0: 6c66 2c20 6873 3a20 2248 6172 6453 7461  lf, hs: "HardSta
-000024b0: 7465 2220 7c20 2248 6172 6453 7461 7465  te" | "HardState
-000024c0: 5265 6622 2920 2d3e 204e 6f6e 653a 0a20  Ref") -> None:. 
-000024d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000024e0: 2020 2053 6176 6573 2074 6865 2063 7572     Saves the cur
-000024f0: 7265 6e74 2048 6172 6453 7461 7465 2e0a  rent HardState..
-00002500: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002510: 6465 6620 7472 6967 6765 725f 736e 6170  def trigger_snap
-00002520: 5f75 6e61 7661 696c 6162 6c65 2873 656c  _unavailable(sel
-00002530: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00002540: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002550: 5472 6967 6765 7220 6120 536e 6170 7368  Trigger a Snapsh
-00002560: 6f74 5465 6d70 6f72 6172 696c 7955 6e61  otTemporarilyUna
-00002570: 7661 696c 6162 6c65 2065 7272 6f72 2e0a  vailable error..
-00002580: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002590: 6465 6620 7472 6967 6765 725f 6c6f 675f  def trigger_log_
-000025a0: 756e 6176 6169 6c61 626c 6528 7365 6c66  unavailable(self
-000025b0: 2c20 763a 2062 6f6f 6c29 202d 3e20 4e6f  , v: bool) -> No
-000025c0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-000025d0: 2020 2020 2020 2020 5365 7420 6120 4c6f          Set a Lo
-000025e0: 6754 656d 706f 7261 7269 6c79 556e 6176  gTemporarilyUnav
-000025f0: 6169 6c61 626c 6520 6572 726f 722e 0a20  ailable error.. 
-00002600: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00002610: 6566 2074 616b 655f 6765 745f 656e 7472  ef take_get_entr
-00002620: 6965 735f 636f 6e74 6578 7428 7365 6c66  ies_context(self
-00002630: 2920 2d3e 204f 7074 696f 6e61 6c5b 2247  ) -> Optional["G
-00002640: 6574 456e 7472 6965 7343 6f6e 7465 7874  etEntriesContext
-00002650: 225d 3a0a 2020 2020 2020 2020 2222 220a  "]:.        """.
-00002660: 2020 2020 2020 2020 5461 6b65 2067 6574          Take get
-00002670: 2065 6e74 7269 6573 2063 6f6e 7465 7874   entries context
-00002680: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
-00002690: 6c61 7373 204d 656d 5374 6f72 6167 6543  lass MemStorageC
-000026a0: 6f72 6528 5f5f 4150 495f 5374 6f72 6167  ore(__API_Storag
-000026b0: 6543 6f72 6529 3a0a 2020 2020 2222 220a  eCore):.    """.
-000026c0: 2020 2020 5468 6520 4d65 6d6f 7279 2053      The Memory S
-000026d0: 746f 7261 6765 2043 6f72 6520 696e 7374  torage Core inst
-000026e0: 616e 6365 2068 6f6c 6473 2074 6865 2061  ance holds the a
-000026f0: 6374 7561 6c20 7374 6174 6520 6f66 2074  ctual state of t
-00002700: 6865 2073 746f 7261 6765 2073 7472 7563  he storage struc
-00002710: 742e 2054 6f20 6163 6365 7373 2074 6869  t. To access thi
-00002720: 730a 2020 2020 7661 6c75 652c 2075 7365  s.    value, use
-00002730: 2074 6865 2060 726c 6020 616e 6420 6077   the `rl` and `w
-00002740: 6c60 2066 756e 6374 696f 6e73 206f 6e20  l` functions on 
-00002750: 7468 6520 6d61 696e 204d 656d 5374 6f72  the main MemStor
-00002760: 6167 6520 696d 706c 656d 656e 7461 7469  age implementati
-00002770: 6f6e 2e0a 2020 2020 2222 220a 0a20 2020  on..    """..   
-00002780: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
-00002790: 6c66 2920 2d3e 2022 4d65 6d53 746f 7261  lf) -> "MemStora
-000027a0: 6765 436f 7265 5265 6622 3a20 2e2e 2e0a  geCoreRef": ....
-000027b0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-000027c0: 640a 2020 2020 6465 6620 6465 6661 756c  d.    def defaul
-000027d0: 7428 2920 2d3e 2022 4d65 6d53 746f 7261  t() -> "MemStora
-000027e0: 6765 436f 7265 223a 202e 2e2e 0a0a 636c  geCore": .....cl
-000027f0: 6173 7320 4d65 6d53 746f 7261 6765 436f  ass MemStorageCo
-00002800: 7265 5265 6628 5f5f 4150 495f 5374 6f72  reRef(__API_Stor
-00002810: 6167 6543 6f72 6529 3a0a 2020 2020 2222  ageCore):.    ""
-00002820: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
-00002830: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
-00002840: 4d65 6d53 746f 7261 6765 602e 0a20 2020  MemStorage`..   
-00002850: 2022 2222 0a0a 636c 6173 7320 5374 6f72   """..class Stor
-00002860: 6167 6543 6f72 6528 5f5f 4150 495f 5374  ageCore(__API_St
-00002870: 6f72 6167 6543 6f72 6529 3a0a 2020 2020  orageCore):.    
-00002880: 2222 2220 2222 220a 0a20 2020 2064 6566  """ """..    def
-00002890: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
-000028a0: 2d3e 2022 5374 6f72 6167 6543 6f72 6552  -> "StorageCoreR
-000028b0: 6566 223a 202e 2e2e 0a20 2020 2040 7374  ef": ....    @st
-000028c0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-000028d0: 6566 2064 6566 6175 6c74 2829 202d 3e20  ef default() -> 
-000028e0: 2253 746f 7261 6765 436f 7265 223a 202e  "StorageCore": .
-000028f0: 2e2e 0a0a 636c 6173 7320 5374 6f72 6167  ....class Storag
-00002900: 6543 6f72 6552 6566 285f 5f41 5049 5f53  eCoreRef(__API_S
-00002910: 746f 7261 6765 436f 7265 293a 0a20 2020  torageCore):.   
-00002920: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
-00002930: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
-00002940: 733a 6053 746f 7261 6765 436f 7265 602e  s:`StorageCore`.
-00002950: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-00002960: 5f5f 4150 495f 5374 6f72 6167 6528 5f5f  __API_Storage(__
-00002970: 436c 6f6e 6561 626c 6529 3a0a 2020 2020  Cloneable):.    
-00002980: 6465 6620 636c 6f6e 6528 7365 6c66 2920  def clone(self) 
-00002990: 2d3e 2041 6e79 3a20 2e2e 2e0a 2020 2020  -> Any: ....    
-000029a0: 6465 6620 696e 6974 6961 6c69 7a65 5f77  def initialize_w
-000029b0: 6974 685f 636f 6e66 5f73 7461 7465 280a  ith_conf_state(.
-000029c0: 2020 2020 2020 2020 7365 6c66 2c20 636f          self, co
-000029d0: 6e66 5f73 7461 7465 3a20 2243 6f6e 6653  nf_state: "ConfS
-000029e0: 7461 7465 2220 7c20 2243 6f6e 6653 7461  tate" | "ConfSta
-000029f0: 7465 5265 6622 0a20 2020 2029 202d 3e20  teRef".    ) -> 
-00002a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00002a10: 220a 2020 2020 2020 2020 496e 6974 6961  ".        Initia
-00002a20: 6c69 7a65 2061 2060 4d65 6d53 746f 7261  lize a `MemStora
-00002a30: 6765 6020 7769 7468 2061 2067 6976 656e  ge` with a given
-00002a40: 2060 436f 6e66 6967 602e 0a0a 2020 2020   `Config`...    
-00002a50: 2020 2020 596f 7520 7368 6f75 6c64 2075      You should u
-00002a60: 7365 2074 6865 2073 616d 6520 696e 7075  se the same inpu
-00002a70: 7420 746f 2069 6e69 7469 616c 697a 6520  t to initialize 
-00002a80: 616c 6c20 6e6f 6465 732e 0a20 2020 2020  all nodes..     
-00002a90: 2020 2022 2222 0a20 2020 2064 6566 2069     """.    def i
-00002aa0: 6e69 7469 616c 5f73 7461 7465 2873 656c  nitial_state(sel
-00002ab0: 6629 202d 3e20 5261 6674 5374 6174 653a  f) -> RaftState:
-00002ac0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00002ad0: 2020 2020 2049 6d70 6c65 6d65 6e74 7320       Implements 
-00002ae0: 7468 6520 5374 6f72 6167 6520 7472 6169  the Storage trai
-00002af0: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
-00002b00: 2020 2064 6566 2065 6e74 7269 6573 280a     def entries(.
-00002b10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00002b20: 2020 2020 2020 6c6f 773a 2069 6e74 2c0a        low: int,.
-00002b30: 2020 2020 2020 2020 6869 6768 3a20 696e          high: in
-00002b40: 742c 0a20 2020 2020 2020 2063 6f6e 7465  t,.        conte
-00002b50: 7874 3a20 2247 6574 456e 7472 6965 7343  xt: "GetEntriesC
-00002b60: 6f6e 7465 7874 5265 6622 2c0a 2020 2020  ontextRef",.    
-00002b70: 2020 2020 6d61 785f 7369 7a65 3a20 4f70      max_size: Op
-00002b80: 7469 6f6e 616c 5b69 6e74 5d2c 0a20 2020  tional[int],.   
-00002b90: 2029 202d 3e20 4c69 7374 5b22 456e 7472   ) -> List["Entr
-00002ba0: 7922 5d3a 0a20 2020 2020 2020 2022 2222  y"]:.        """
-00002bb0: 0a20 2020 2020 2020 2049 6d70 6c65 6d65  .        Impleme
-00002bc0: 6e74 7320 7468 6520 5374 6f72 6167 6520  nts the Storage 
-00002bd0: 7472 6169 742e 0a20 2020 2020 2020 2022  trait..        "
-00002be0: 2222 0a20 2020 2064 6566 2074 6572 6d28  "".    def term(
-00002bf0: 7365 6c66 2c20 6964 783a 2069 6e74 2920  self, idx: int) 
-00002c00: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00002c10: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
-00002c20: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
-00002c30: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
-00002c40: 2020 2222 220a 2020 2020 6465 6620 6669    """.    def fi
-00002c50: 7273 745f 696e 6465 7828 7365 6c66 2920  rst_index(self) 
-00002c60: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00002c70: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
-00002c80: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
-00002c90: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
-00002ca0: 2020 2222 220a 2020 2020 6465 6620 6c61    """.    def la
-00002cb0: 7374 5f69 6e64 6578 2873 656c 6629 202d  st_index(self) -
-00002cc0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-00002cd0: 2222 0a20 2020 2020 2020 2049 6d70 6c65  "".        Imple
-00002ce0: 6d65 6e74 7320 7468 6520 5374 6f72 6167  ments the Storag
-00002cf0: 6520 7472 6169 742e 0a20 2020 2020 2020  e trait..       
-00002d00: 2022 2222 0a20 2020 2064 6566 2073 6e61   """.    def sna
-00002d10: 7073 686f 7428 7365 6c66 2c20 7265 7175  pshot(self, requ
-00002d20: 6573 745f 696e 6465 783a 2069 6e74 2c20  est_index: int, 
-00002d30: 746f 3a20 696e 7429 202d 3e20 2253 6e61  to: int) -> "Sna
-00002d40: 7073 686f 7422 3a0a 2020 2020 2020 2020  pshot":.        
-00002d50: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
-00002d60: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
-00002d70: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
-00002d80: 2020 2222 220a 0a63 6c61 7373 204d 656d    """..class Mem
-00002d90: 5374 6f72 6167 6528 5f5f 4150 495f 5374  Storage(__API_St
-00002da0: 6f72 6167 6529 3a0a 2020 2020 2222 220a  orage):.    """.
-00002db0: 2020 2020 604d 656d 5374 6f72 6167 6560      `MemStorage`
-00002dc0: 2069 7320 6120 7468 7265 6164 2d73 6166   is a thread-saf
-00002dd0: 6520 6275 7420 696e 636f 6d70 6c65 7465  e but incomplete
-00002de0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00002df0: 6f66 2060 5374 6f72 6167 6560 2c20 6d61  of `Storage`, ma
-00002e00: 696e 6c79 2066 6f72 2074 6573 7473 2e0a  inly for tests..
-00002e10: 0a20 2020 2041 2072 6561 6c20 6053 746f  .    A real `Sto
-00002e20: 7261 6765 6020 7368 6f75 6c64 2073 6176  rage` should sav
-00002e30: 6520 626f 7468 2072 6166 7420 6c6f 6773  e both raft logs
-00002e40: 2061 6e64 2061 7070 6c69 6564 2064 6174   and applied dat
-00002e50: 612e 2048 6f77 6576 6572 2060 4d65 6d53  a. However `MemS
-00002e60: 746f 7261 6765 6020 6f6e 6c79 0a20 2020  torage` only.   
-00002e70: 2063 6f6e 7461 696e 7320 7261 6674 206c   contains raft l
-00002e80: 6f67 732e 2053 6f20 796f 7520 6361 6e20  ogs. So you can 
-00002e90: 6361 6c6c 2060 4d65 6d53 746f 7261 6765  call `MemStorage
-00002ea0: 3a3a 6170 7065 6e64 6020 746f 2070 6572  ::append` to per
-00002eb0: 7369 7374 206e 6577 2072 6563 6569 7665  sist new receive
-00002ec0: 6420 756e 7374 6162 6c65 2072 6166 740a  d unstable raft.
-00002ed0: 2020 2020 6c6f 6773 2061 6e64 2074 6865      logs and the
-00002ee0: 6e20 6163 6365 7373 2074 6865 6d20 7769  n access them wi
-00002ef0: 7468 2060 5374 6f72 6167 6560 2041 5049  th `Storage` API
-00002f00: 732e 2054 6865 206f 6e6c 7920 6578 6365  s. The only exce
-00002f10: 7074 696f 6e20 6973 2060 5374 6f72 6167  ption is `Storag
-00002f20: 653a 3a73 6e61 7073 686f 7460 2e20 5468  e::snapshot`. Th
-00002f30: 6572 650a 2020 2020 6973 206e 6f20 6461  ere.    is no da
-00002f40: 7461 2069 6e20 6053 6e61 7073 686f 7460  ta in `Snapshot`
-00002f50: 2072 6574 7572 6e65 6420 6279 2060 4d65   returned by `Me
-00002f60: 6d53 746f 7261 6765 3a3a 736e 6170 7368  mStorage::snapsh
-00002f70: 6f74 6020 6265 6361 7573 6520 6170 706c  ot` because appl
-00002f80: 6965 6420 6461 7461 2069 7320 6e6f 7420  ied data is not 
-00002f90: 7374 6f72 6564 0a20 2020 2069 6e20 604d  stored.    in `M
-00002fa0: 656d 5374 6f72 6167 6560 2e0a 2020 2020  emStorage`..    
-00002fb0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-00002fc0: 6e69 745f 5f28 7365 6c66 2920 2d3e 204e  nit__(self) -> N
-00002fd0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-00002fe0: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
-00002ff0: 2d3e 2022 4d65 6d53 746f 7261 6765 5265  -> "MemStorageRe
-00003000: 6622 3a20 2e2e 2e0a 2020 2020 6465 6620  f": ....    def 
-00003010: 636c 6f6e 6528 7365 6c66 2920 2d3e 2022  clone(self) -> "
-00003020: 4d65 6d53 746f 7261 6765 223a 202e 2e2e  MemStorage": ...
-00003030: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00003040: 6f64 0a20 2020 2064 6566 2064 6566 6175  od.    def defau
-00003050: 6c74 2829 202d 3e20 224d 656d 5374 6f72  lt() -> "MemStor
-00003060: 6167 6522 3a20 2e2e 2e0a 2020 2020 4073  age": ....    @s
-00003070: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00003080: 6465 6620 6e65 775f 7769 7468 5f63 6f6e  def new_with_con
-00003090: 665f 7374 6174 6528 0a20 2020 2020 2020  f_state(.       
-000030a0: 2063 6f6e 665f 7374 6174 653a 2022 436f   conf_state: "Co
-000030b0: 6e66 5374 6174 6522 207c 2022 436f 6e66  nfState" | "Conf
-000030c0: 5374 6174 6552 6566 222c 0a20 2020 2029  StateRef",.    )
-000030d0: 202d 3e20 224d 656d 5374 6f72 6167 6522   -> "MemStorage"
-000030e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000030f0: 2020 2020 2020 4372 6561 7465 2061 206e        Create a n
-00003100: 6577 2060 4d65 6d53 746f 7261 6765 6020  ew `MemStorage` 
-00003110: 7769 7468 2061 2067 6976 656e 2060 436f  with a given `Co
-00003120: 6e66 6967 602e 2054 6865 2067 6976 656e  nfig`. The given
-00003130: 2060 436f 6e66 6967 6020 7769 6c6c 2062   `Config` will b
-00003140: 6520 7573 6564 2074 6f0a 2020 2020 2020  e used to.      
-00003150: 2020 696e 6974 6961 6c69 7a65 2074 6865    initialize the
-00003160: 2073 746f 7261 6765 2e0a 0a20 2020 2020   storage...     
-00003170: 2020 2059 6f75 2073 686f 756c 6420 7573     You should us
-00003180: 6520 7468 6520 7361 6d65 2069 6e70 7574  e the same input
-00003190: 2074 6f20 696e 6974 6961 6c69 7a65 2061   to initialize a
-000031a0: 6c6c 206e 6f64 6573 2e0a 2020 2020 2020  ll nodes..      
-000031b0: 2020 2222 220a 2020 2020 6465 6620 776c    """.    def wl
-000031c0: 2873 656c 6629 202d 3e20 224d 656d 5374  (self) -> "MemSt
-000031d0: 6f72 6167 6543 6f72 6552 6566 223a 0a20  orageCoreRef":. 
-000031e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000031f0: 2020 204f 7065 6e73 2075 7020 6120 7772     Opens up a wr
-00003200: 6974 6520 6c6f 636b 206f 6e20 7468 6520  ite lock on the 
-00003210: 7374 6f72 6167 6520 616e 6420 7265 7475  storage and retu
-00003220: 726e 7320 6775 6172 6420 6861 6e64 6c65  rns guard handle
-00003230: 2e20 5573 6520 7468 6973 0a20 2020 2020  . Use this.     
-00003240: 2020 2077 6974 6820 6675 6e63 7469 6f6e     with function
-00003250: 7320 7468 6174 2074 616b 6520 6120 6d75  s that take a mu
-00003260: 7461 626c 6520 7265 6665 7265 6e63 6520  table reference 
-00003270: 746f 2073 656c 662e 0a20 2020 2020 2020  to self..       
-00003280: 2022 2222 0a20 2020 2064 6566 2072 6c28   """.    def rl(
-00003290: 7365 6c66 2920 2d3e 2022 4d65 6d53 746f  self) -> "MemSto
-000032a0: 7261 6765 436f 7265 5265 6622 3a0a 2020  rageCoreRef":.  
-000032b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000032c0: 2020 4f70 656e 7320 7570 2061 2072 6561    Opens up a rea
-000032d0: 6420 6c6f 636b 206f 6e20 7468 6520 7374  d lock on the st
-000032e0: 6f72 6167 6520 616e 6420 7265 7475 726e  orage and return
-000032f0: 7320 6120 6775 6172 6420 6861 6e64 6c65  s a guard handle
-00003300: 2e20 5573 6520 7468 6973 0a20 2020 2020  . Use this.     
-00003310: 2020 2077 6974 6820 6675 6e63 7469 6f6e     with function
-00003320: 7320 7468 6174 2064 6f6e 2774 2072 6571  s that don't req
-00003330: 7569 7265 206d 7574 6174 696f 6e2e 0a20  uire mutation.. 
-00003340: 2020 2020 2020 2022 2222 0a0a 636c 6173         """..clas
-00003350: 7320 4d65 6d53 746f 7261 6765 5265 6628  s MemStorageRef(
-00003360: 5f5f 4150 495f 5374 6f72 6167 6529 3a0a  __API_Storage):.
-00003370: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
-00003380: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
-00003390: 6c61 7373 3a60 4d65 6d53 746f 7261 6765  lass:`MemStorage
-000033a0: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
-000033b0: 6465 6620 636c 6f6e 6528 7365 6c66 2920  def clone(self) 
-000033c0: 2d3e 2022 4d65 6d53 746f 7261 6765 223a  -> "MemStorage":
-000033d0: 202e 2e2e 0a20 2020 2064 6566 2077 6c28   ....    def wl(
-000033e0: 7365 6c66 2920 2d3e 2022 4d65 6d53 746f  self) -> "MemSto
-000033f0: 7261 6765 436f 7265 5265 6622 3a0a 2020  rageCoreRef":.  
-00003400: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003410: 2020 4f70 656e 7320 7570 2061 2077 7269    Opens up a wri
-00003420: 7465 206c 6f63 6b20 6f6e 2074 6865 2073  te lock on the s
-00003430: 746f 7261 6765 2061 6e64 2072 6574 7572  torage and retur
-00003440: 6e73 2067 7561 7264 2068 616e 646c 652e  ns guard handle.
-00003450: 2055 7365 2074 6869 730a 2020 2020 2020   Use this.      
-00003460: 2020 7769 7468 2066 756e 6374 696f 6e73    with functions
-00003470: 2074 6861 7420 7461 6b65 2061 206d 7574   that take a mut
-00003480: 6162 6c65 2072 6566 6572 656e 6365 2074  able reference t
-00003490: 6f20 7365 6c66 2e0a 2020 2020 2020 2020  o self..        
-000034a0: 2222 220a 2020 2020 6465 6620 726c 2873  """.    def rl(s
-000034b0: 656c 6629 202d 3e20 224d 656d 5374 6f72  elf) -> "MemStor
-000034c0: 6167 6543 6f72 6552 6566 223a 0a20 2020  ageCoreRef":.   
-000034d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000034e0: 204f 7065 6e73 2075 7020 6120 7265 6164   Opens up a read
-000034f0: 206c 6f63 6b20 6f6e 2074 6865 2073 746f   lock on the sto
-00003500: 7261 6765 2061 6e64 2072 6574 7572 6e73  rage and returns
-00003510: 2061 2067 7561 7264 2068 616e 646c 652e   a guard handle.
-00003520: 2055 7365 2074 6869 730a 2020 2020 2020   Use this.      
-00003530: 2020 7769 7468 2066 756e 6374 696f 6e73    with functions
-00003540: 2074 6861 7420 646f 6e27 7420 7265 7175   that don't requ
-00003550: 6972 6520 6d75 7461 7469 6f6e 2e0a 2020  ire mutation..  
-00003560: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
-00003570: 2053 746f 7261 6765 285f 5f41 5049 5f53   Storage(__API_S
-00003580: 746f 7261 6765 293a 0a20 2020 2022 2222  torage):.    """
-00003590: 0a20 2020 2053 746f 7261 6765 2073 6176  .    Storage sav
-000035a0: 6573 2061 6c6c 2074 6865 2069 6e66 6f72  es all the infor
-000035b0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
-000035c0: 2063 7572 7265 6e74 2052 6166 7420 696d   current Raft im
-000035d0: 706c 656d 656e 7461 7469 6f6e 2c20 696e  plementation, in
-000035e0: 636c 7564 696e 6720 5261 6674 204c 6f67  cluding Raft Log
-000035f0: 2c0a 2020 2020 636f 6d6d 6974 2069 6e64  ,.    commit ind
-00003600: 6578 2c20 7468 6520 6c65 6164 6572 2074  ex, the leader t
-00003610: 6f20 766f 7465 2066 6f72 2c20 6574 632e  o vote for, etc.
-00003620: 0a0a 2020 2020 4966 2061 6e79 2053 746f  ..    If any Sto
-00003630: 7261 6765 206d 6574 686f 6420 7265 7475  rage method retu
-00003640: 726e 7320 616e 2065 7272 6f72 2c20 7468  rns an error, th
-00003650: 6520 7261 6674 2069 6e73 7461 6e63 6520  e raft instance 
-00003660: 7769 6c6c 0a20 2020 2062 6563 6f6d 6520  will.    become 
-00003670: 696e 6f70 6572 6162 6c65 2061 6e64 2072  inoperable and r
-00003680: 6566 7573 6520 746f 2070 6172 7469 6369  efuse to partici
-00003690: 7061 7465 2069 6e20 656c 6563 7469 6f6e  pate in election
-000036a0: 733b 2074 6865 0a20 2020 2061 7070 6c69  s; the.    appli
-000036b0: 6361 7469 6f6e 2069 7320 7265 7370 6f6e  cation is respon
-000036c0: 7369 626c 6520 666f 7220 636c 6561 6e75  sible for cleanu
-000036d0: 7020 616e 6420 7265 636f 7665 7279 2069  p and recovery i
-000036e0: 6e20 7468 6973 2063 6173 652e 0a20 2020  n this case..   
-000036f0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
-00003700: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
-00003710: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
-00003720: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
-00003730: 202d 3e20 2253 746f 7261 6765 5265 6622   -> "StorageRef"
-00003740: 3a20 2e2e 2e0a 2020 2020 6465 6620 636c  : ....    def cl
-00003750: 6f6e 6528 7365 6c66 2920 2d3e 2022 5374  one(self) -> "St
-00003760: 6f72 6167 6522 3a20 2e2e 2e0a 2020 2020  orage": ....    
-00003770: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-00003780: 2020 6465 6620 6465 6661 756c 7428 2920    def default() 
-00003790: 2d3e 2022 5374 6f72 6167 6522 3a20 2e2e  -> "Storage": ..
-000037a0: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-000037b0: 686f 640a 2020 2020 6465 6620 6e65 775f  hod.    def new_
-000037c0: 7769 7468 5f63 6f6e 665f 7374 6174 6528  with_conf_state(
-000037d0: 0a20 2020 2020 2020 2063 6f6e 665f 7374  .        conf_st
-000037e0: 6174 653a 2022 436f 6e66 5374 6174 6522  ate: "ConfState"
-000037f0: 207c 2022 436f 6e66 5374 6174 6552 6566   | "ConfStateRef
-00003800: 222c 0a20 2020 2029 202d 3e20 2253 746f  ",.    ) -> "Sto
-00003810: 7261 6765 223a 0a20 2020 2020 2020 2022  rage":.        "
-00003820: 2222 2022 2222 0a20 2020 2064 6566 2077  "" """.    def w
-00003830: 6c28 7365 6c66 2920 2d3e 2041 6e79 3a0a  l(self) -> Any:.
-00003840: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003850: 2020 2020 4f70 656e 7320 7570 2061 2077      Opens up a w
-00003860: 7269 7465 206c 6f63 6b20 6f6e 2074 6865  rite lock on the
-00003870: 2073 746f 7261 6765 2061 6e64 2072 6574   storage and ret
-00003880: 7572 6e73 2067 7561 7264 2068 616e 646c  urns guard handl
-00003890: 652e 2055 7365 2074 6869 730a 2020 2020  e. Use this.    
-000038a0: 2020 2020 7769 7468 2066 756e 6374 696f      with functio
-000038b0: 6e73 2074 6861 7420 7461 6b65 2061 206d  ns that take a m
-000038c0: 7574 6162 6c65 2072 6566 6572 656e 6365  utable reference
-000038d0: 2074 6f20 7365 6c66 2e0a 2020 2020 2020   to self..      
-000038e0: 2020 2222 220a 2020 2020 6465 6620 726c    """.    def rl
-000038f0: 2873 656c 6629 202d 3e20 416e 793a 0a20  (self) -> Any:. 
-00003900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003910: 2020 204f 7065 6e73 2075 7020 6120 7265     Opens up a re
-00003920: 6164 206c 6f63 6b20 6f6e 2074 6865 2073  ad lock on the s
-00003930: 746f 7261 6765 2061 6e64 2072 6574 7572  torage and retur
-00003940: 6e73 2061 2067 7561 7264 2068 616e 646c  ns a guard handl
-00003950: 652e 2055 7365 2074 6869 730a 2020 2020  e. Use this.    
-00003960: 2020 2020 7769 7468 2066 756e 6374 696f      with functio
-00003970: 6e73 2074 6861 7420 646f 6e27 7420 7265  ns that don't re
-00003980: 7175 6972 6520 6d75 7461 7469 6f6e 2e0a  quire mutation..
-00003990: 2020 2020 2020 2020 2222 220a 0a63 6c61          """..cla
-000039a0: 7373 2053 746f 7261 6765 5265 6628 5f5f  ss StorageRef(__
-000039b0: 4150 495f 5374 6f72 6167 6529 3a0a 2020  API_Storage):.  
-000039c0: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
-000039d0: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
-000039e0: 7373 3a60 5374 6f72 6167 6560 2e0a 2020  ss:`Storage`..  
-000039f0: 2020 2222 220a 0a20 2020 2064 6566 2063    """..    def c
-00003a00: 6c6f 6e65 2873 656c 6629 202d 3e20 2253  lone(self) -> "S
-00003a10: 746f 7261 6765 223a 202e 2e2e 0a20 2020  torage": ....   
-00003a20: 2064 6566 2077 6c28 7365 6c66 2920 2d3e   def wl(self) ->
-00003a30: 2041 6e79 3a0a 2020 2020 2020 2020 2222   Any:.        ""
-00003a40: 220a 2020 2020 2020 2020 4f70 656e 7320  ".        Opens 
-00003a50: 7570 2061 2077 7269 7465 206c 6f63 6b20  up a write lock 
-00003a60: 6f6e 2074 6865 2073 746f 7261 6765 2061  on the storage a
-00003a70: 6e64 2072 6574 7572 6e73 2067 7561 7264  nd returns guard
-00003a80: 2068 616e 646c 652e 2055 7365 2074 6869   handle. Use thi
-00003a90: 730a 2020 2020 2020 2020 7769 7468 2066  s.        with f
-00003aa0: 756e 6374 696f 6e73 2074 6861 7420 7461  unctions that ta
-00003ab0: 6b65 2061 206d 7574 6162 6c65 2072 6566  ke a mutable ref
-00003ac0: 6572 656e 6365 2074 6f20 7365 6c66 2e0a  erence to self..
-00003ad0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003ae0: 6465 6620 726c 2873 656c 6629 202d 3e20  def rl(self) -> 
-00003af0: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
-00003b00: 0a20 2020 2020 2020 204f 7065 6e73 2075  .        Opens u
-00003b10: 7020 6120 7265 6164 206c 6f63 6b20 6f6e  p a read lock on
-00003b20: 2074 6865 2073 746f 7261 6765 2061 6e64   the storage and
-00003b30: 2072 6574 7572 6e73 2061 2067 7561 7264   returns a guard
-00003b40: 2068 616e 646c 652e 2055 7365 2074 6869   handle. Use thi
-00003b50: 730a 2020 2020 2020 2020 7769 7468 2066  s.        with f
-00003b60: 756e 6374 696f 6e73 2074 6861 7420 646f  unctions that do
-00003b70: 6e27 7420 7265 7175 6972 6520 6d75 7461  n't require muta
-00003b80: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
-00003b90: 220a 0a63 6c61 7373 205f 5f41 5049 5f52  "..class __API_R
-00003ba0: 6561 6479 3a0a 2020 2020 6465 6620 6873  eady:.    def hs
-00003bb0: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-00003bc0: 616c 5b22 4861 7264 5374 6174 6552 6566  al["HardStateRef
-00003bd0: 225d 3a0a 2020 2020 2020 2020 2222 220a  "]:.        """.
-00003be0: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
-00003bf0: 656e 7420 7374 6174 6520 6f66 2061 204e  ent state of a N
-00003c00: 6f64 6520 746f 2062 6520 7361 7665 6420  ode to be saved 
-00003c10: 746f 2073 7461 626c 6520 7374 6f72 6167  to stable storag
-00003c20: 652e 0a20 2020 2020 2020 2048 6172 6453  e..        HardS
-00003c30: 7461 7465 2077 696c 6c20 6265 204e 6f6e  tate will be Non
-00003c40: 6520 7374 6174 6520 6966 2074 6865 7265  e state if there
-00003c50: 2069 7320 6e6f 2075 7064 6174 652e 0a20   is no update.. 
-00003c60: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00003c70: 6566 2073 7328 7365 6c66 2920 2d3e 204f  ef ss(self) -> O
-00003c80: 7074 696f 6e61 6c5b 2253 6f66 7453 7461  ptional["SoftSta
-00003c90: 7465 5265 6622 5d3a 0a20 2020 2020 2020  teRef"]:.       
-00003ca0: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
-00003cb0: 2063 7572 7265 6e74 2076 6f6c 6174 696c   current volatil
-00003cc0: 6520 7374 6174 6520 6f66 2061 204e 6f64  e state of a Nod
-00003cd0: 652e 0a20 2020 2020 2020 2053 6f66 7453  e..        SoftS
-00003ce0: 7461 7465 2077 696c 6c20 6265 204e 6f6e  tate will be Non
-00003cf0: 6520 6966 2074 6865 7265 2069 7320 6e6f  e if there is no
-00003d00: 2075 7064 6174 652e 0a20 2020 2020 2020   update..       
-00003d10: 2049 7420 6973 206e 6f74 2072 6571 7569   It is not requi
-00003d20: 7265 6420 746f 2063 6f6e 7375 6d65 206f  red to consume o
-00003d30: 7220 7374 6f72 6520 536f 6674 5374 6174  r store SoftStat
-00003d40: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00003d50: 2020 2064 6566 206d 7573 745f 7379 6e63     def must_sync
-00003d60: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00003d70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003d80: 2020 2020 4d75 7374 5379 6e63 2069 7320      MustSync is 
-00003d90: 6661 6c73 6520 6966 2061 6e64 206f 6e6c  false if and onl
-00003da0: 7920 6966 0a20 2020 2020 2020 2031 2e20  y if.        1. 
-00003db0: 6e6f 2048 6172 6453 7461 7465 206f 7220  no HardState or 
-00003dc0: 6f6e 6c79 2069 7473 2063 6f6d 6d69 7420  only its commit 
-00003dd0: 6973 2064 6966 6665 7265 6e74 2066 726f  is different fro
-00003de0: 6d20 6265 666f 7265 0a20 2020 2020 2020  m before.       
-00003df0: 2032 2e20 6e6f 2045 6e74 7269 6573 2061   2. no Entries a
-00003e00: 6e64 2053 6e61 7073 686f 740a 2020 2020  nd Snapshot.    
-00003e10: 2020 2020 4966 2069 7427 7320 6661 6c73      If it's fals
-00003e20: 652c 2061 6e20 6173 796e 6368 726f 6e6f  e, an asynchrono
-00003e30: 7573 2077 7269 7465 206f 6620 4861 7264  us write of Hard
-00003e40: 5374 6174 6520 6973 2070 6572 6d69 7373  State is permiss
-00003e50: 6962 6c65 2062 6566 6f72 6520 6361 6c6c  ible before call
-00003e60: 696e 670a 2020 2020 2020 2020 5b60 5261  ing.        [`Ra
-00003e70: 774e 6f64 653a 3a6f 6e5f 7065 7273 6973  wNode::on_persis
-00003e80: 745f 7265 6164 7960 5d20 6f72 205b 6052  t_ready`] or [`R
-00003e90: 6177 4e6f 6465 3a3a 6164 7661 6e63 6560  awNode::advance`
-00003ea0: 5d20 6f72 2069 7473 2066 616d 696c 6965  ] or its familie
-00003eb0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00003ec0: 2020 2064 6566 206e 756d 6265 7228 7365     def number(se
-00003ed0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00003ee0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003ef0: 5468 6520 6e75 6d62 6572 206f 6620 6375  The number of cu
-00003f00: 7272 656e 7420 5265 6164 792e 0a20 2020  rrent Ready..   
-00003f10: 2020 2020 2049 7420 6973 2075 7365 6420       It is used 
-00003f20: 666f 7220 6964 656e 7469 6679 696e 6720  for identifying 
-00003f30: 7468 6520 6469 6666 6572 656e 7420 5265  the different Re
-00003f40: 6164 7920 616e 6420 5265 6164 7952 6563  ady and ReadyRec
-00003f50: 6f72 642e 0a20 2020 2020 2020 2022 2222  ord..        """
-00003f60: 0a20 2020 2064 6566 2073 6e61 7073 686f  .    def snapsho
-00003f70: 7428 7365 6c66 2920 2d3e 2022 536e 6170  t(self) -> "Snap
-00003f80: 7368 6f74 5265 6622 3a0a 2020 2020 2020  shotRef":.      
-00003f90: 2020 2222 220a 2020 2020 2020 2020 536e    """.        Sn
-00003fa0: 6170 7368 6f74 2073 7065 6369 6669 6573  apshot specifies
-00003fb0: 2074 6865 2073 6e61 7073 686f 7420 746f   the snapshot to
-00003fc0: 2062 6520 7361 7665 6420 746f 2073 7461   be saved to sta
-00003fd0: 626c 6520 7374 6f72 6167 652e 0a20 2020  ble storage..   
-00003fe0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00003ff0: 2063 6f6d 6d69 7474 6564 5f65 6e74 7269   committed_entri
-00004000: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
-00004010: 5b22 456e 7472 7952 6566 225d 3a0a 2020  ["EntryRef"]:.  
-00004020: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00004030: 2020 436f 6d6d 6974 7465 6445 6e74 7269    CommittedEntri
-00004040: 6573 2073 7065 6369 6669 6573 2065 6e74  es specifies ent
-00004050: 7269 6573 2074 6f20 6265 2063 6f6d 6d69  ries to be commi
-00004060: 7474 6564 2074 6f20 610a 2020 2020 2020  tted to a.      
-00004070: 2020 7374 6f72 652f 7374 6174 652d 6d61    store/state-ma
-00004080: 6368 696e 652e 2054 6865 7365 2068 6176  chine. These hav
-00004090: 6520 7072 6576 696f 7573 6c79 2062 6565  e previously bee
-000040a0: 6e20 636f 6d6d 6974 7465 6420 746f 2073  n committed to s
-000040b0: 7461 626c 650a 2020 2020 2020 2020 7374  table.        st
-000040c0: 6f72 652e 0a20 2020 2020 2020 2022 2222  ore..        """
-000040d0: 0a20 2020 2064 6566 2074 616b 655f 636f  .    def take_co
-000040e0: 6d6d 6974 7465 645f 656e 7472 6965 7328  mmitted_entries(
-000040f0: 7365 6c66 2920 2d3e 204c 6973 745b 2245  self) -> List["E
-00004100: 6e74 7279 225d 3a0a 2020 2020 2020 2020  ntry"]:.        
-00004110: 2222 220a 2020 2020 2020 2020 5461 6b65  """.        Take
-00004120: 2074 6865 2043 6f6d 6d69 7445 6e74 7269   the CommitEntri
-00004130: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-00004140: 2020 2020 6465 6620 656e 7472 6965 7328      def entries(
-00004150: 7365 6c66 2920 2d3e 204c 6973 745b 2245  self) -> List["E
-00004160: 6e74 7279 5265 6622 5d3a 0a20 2020 2020  ntryRef"]:.     
-00004170: 2020 2022 2222 0a20 2020 2020 2020 2045     """.        E
-00004180: 6e74 7269 6573 2073 7065 6369 6669 6573  ntries specifies
-00004190: 2065 6e74 7269 6573 2074 6f20 6265 2073   entries to be s
-000041a0: 6176 6564 2074 6f20 7374 6162 6c65 2073  aved to stable s
-000041b0: 746f 7261 6765 2e0a 2020 2020 2020 2020  torage..        
-000041c0: 2222 220a 2020 2020 6465 6620 7461 6b65  """.    def take
-000041d0: 5f65 6e74 7269 6573 2873 656c 6629 202d  _entries(self) -
-000041e0: 3e20 4c69 7374 5b22 456e 7472 7922 5d3a  > List["Entry"]:
-000041f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004200: 2020 2020 2054 616b 6520 7468 6520 456e       Take the En
-00004210: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
-00004220: 2222 0a20 2020 2064 6566 206d 6573 7361  "".    def messa
-00004230: 6765 7328 7365 6c66 2920 2d3e 204c 6973  ges(self) -> Lis
-00004240: 745b 224d 6573 7361 6765 5265 6622 5d3a  t["MessageRef"]:
-00004250: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004260: 2020 2020 204d 6573 7361 6765 7320 7370       Messages sp
-00004270: 6563 6966 6965 7320 6f75 7462 6f75 6e64  ecifies outbound
-00004280: 206d 6573 7361 6765 7320 746f 2062 6520   messages to be 
-00004290: 7365 6e74 2e0a 2020 2020 2020 2020 4966  sent..        If
-000042a0: 2069 7420 636f 6e74 6169 6e73 2061 204d   it contains a M
-000042b0: 7367 536e 6170 206d 6573 7361 6765 2c20  sgSnap message, 
-000042c0: 7468 6520 6170 706c 6963 6174 696f 6e20  the application 
-000042d0: 4d55 5354 2072 6570 6f72 7420 6261 636b  MUST report back
-000042e0: 2074 6f20 7261 6674 0a20 2020 2020 2020   to raft.       
-000042f0: 2077 6865 6e20 7468 6520 736e 6170 7368   when the snapsh
-00004300: 6f74 2068 6173 2062 6565 6e20 7265 6365  ot has been rece
-00004310: 6976 6564 206f 7220 6861 7320 6661 696c  ived or has fail
-00004320: 6564 2062 7920 6361 6c6c 696e 6720 5265  ed by calling Re
-00004330: 706f 7274 536e 6170 7368 6f74 2e0a 2020  portSnapshot..  
-00004340: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00004350: 6620 7461 6b65 5f6d 6573 7361 6765 7328  f take_messages(
-00004360: 7365 6c66 2920 2d3e 204c 6973 745b 224d  self) -> List["M
-00004370: 6573 7361 6765 225d 3a0a 2020 2020 2020  essage"]:.      
-00004380: 2020 2222 220a 2020 2020 2020 2020 5461    """.        Ta
-00004390: 6b65 2074 6865 204d 6573 7361 6765 732e  ke the Messages.
-000043a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000043b0: 2064 6566 2070 6572 7369 7374 6564 5f6d   def persisted_m
-000043c0: 6573 7361 6765 7328 7365 6c66 2920 2d3e  essages(self) ->
-000043d0: 204c 6973 745b 224d 6573 7361 6765 5265   List["MessageRe
-000043e0: 6622 5d3a 0a20 2020 2020 2020 2022 2222  f"]:.        """
-000043f0: 0a20 2020 2020 2020 2050 6572 7369 7374  .        Persist
-00004400: 6564 204d 6573 7361 6765 7320 7370 6563  ed Messages spec
-00004410: 6966 6965 7320 6f75 7462 6f75 6e64 206d  ifies outbound m
-00004420: 6573 7361 6765 7320 746f 2062 6520 7365  essages to be se
-00004430: 6e74 2041 4654 4552 2074 6865 2048 6172  nt AFTER the Har
-00004440: 6453 7461 7465 2c0a 2020 2020 2020 2020  dState,.        
-00004450: 456e 7472 6965 7320 616e 6420 536e 6170  Entries and Snap
-00004460: 7368 6f74 2061 7265 2070 6572 7369 7374  shot are persist
-00004470: 6564 2074 6f20 7374 6162 6c65 2073 746f  ed to stable sto
-00004480: 7261 6765 2e0a 2020 2020 2020 2020 2222  rage..        ""
-00004490: 220a 2020 2020 6465 6620 7461 6b65 5f70  ".    def take_p
-000044a0: 6572 7369 7374 6564 5f6d 6573 7361 6765  ersisted_message
-000044b0: 7328 7365 6c66 2920 2d3e 204c 6973 745b  s(self) -> List[
-000044c0: 224d 6573 7361 6765 225d 3a0a 2020 2020  "Message"]:.    
-000044d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000044e0: 5461 6b65 2074 6865 2050 6572 7369 7374  Take the Persist
-000044f0: 6564 204d 6573 7361 6765 732e 0a20 2020  ed Messages..   
-00004500: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00004510: 2072 6561 645f 7374 6174 6573 2873 656c   read_states(sel
-00004520: 6629 202d 3e20 4c69 7374 5b22 5265 6164  f) -> List["Read
-00004530: 5374 6174 6552 6566 225d 3a0a 2020 2020  StateRef"]:.    
-00004540: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004550: 5265 6164 5374 6174 6573 2073 7065 6369  ReadStates speci
-00004560: 6669 6573 2074 6865 2073 7461 7465 2066  fies the state f
-00004570: 6f72 2072 6561 6420 6f6e 6c79 2071 7565  or read only que
-00004580: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
-00004590: 2020 2020 6465 6620 7461 6b65 5f72 6561      def take_rea
-000045a0: 645f 7374 6174 6573 2873 656c 6629 202d  d_states(self) -
-000045b0: 3e20 4c69 7374 5b22 5265 6164 5374 6174  > List["ReadStat
-000045c0: 6522 5d3a 0a20 2020 2020 2020 2022 2222  e"]:.        """
-000045d0: 0a20 2020 2020 2020 2052 6561 6453 7461  .        ReadSta
-000045e0: 7465 7320 7370 6563 6966 6965 7320 7468  tes specifies th
-000045f0: 6520 7374 6174 6520 666f 7220 7265 6164  e state for read
-00004600: 206f 6e6c 7920 7175 6572 792e 0a20 2020   only query..   
-00004610: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-00004620: 5265 6164 7928 5f5f 4150 495f 5265 6164  Ready(__API_Read
-00004630: 7929 3a0a 2020 2020 2222 220a 2020 2020  y):.    """.    
-00004640: 5265 6164 7920 656e 6361 7073 756c 6174  Ready encapsulat
-00004650: 6573 2074 6865 2065 6e74 7269 6573 2061  es the entries a
-00004660: 6e64 206d 6573 7361 6765 7320 7468 6174  nd messages that
-00004670: 2061 7265 2072 6561 6479 2074 6f20 7265   are ready to re
-00004680: 6164 2c0a 2020 2020 6265 2073 6176 6564  ad,.    be saved
-00004690: 2074 6f20 7374 6162 6c65 2073 746f 7261   to stable stora
-000046a0: 6765 2c20 636f 6d6d 6974 7465 6420 6f72  ge, committed or
-000046b0: 2073 656e 7420 746f 206f 7468 6572 2070   sent to other p
-000046c0: 6565 7273 2e0a 2020 2020 2222 220a 0a20  eers..    """.. 
-000046d0: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
-000046e0: 7365 6c66 2920 2d3e 2022 5265 6164 7952  self) -> "ReadyR
-000046f0: 6566 223a 202e 2e2e 0a20 2020 2040 7374  ef": ....    @st
-00004700: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00004710: 6566 2064 6566 6175 6c74 2829 202d 3e20  ef default() -> 
-00004720: 2252 6561 6479 223a 202e 2e2e 0a0a 636c  "Ready": .....cl
-00004730: 6173 7320 5265 6164 7952 6566 285f 5f41  ass ReadyRef(__A
-00004740: 5049 5f52 6561 6479 293a 0a20 2020 2022  PI_Ready):.    "
-00004750: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
-00004760: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
-00004770: 6052 6561 6479 602e 0a20 2020 2022 2222  `Ready`..    """
-00004780: 0a0a 636c 6173 7320 5f5f 4150 495f 5261  ..class __API_Ra
-00004790: 774e 6f64 653a 0a20 2020 2064 6566 2061  wNode:.    def a
-000047a0: 6476 616e 6365 5f61 7070 6c79 2873 656c  dvance_apply(sel
-000047b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-000047c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000047d0: 4164 7661 6e63 6520 6170 706c 7920 746f  Advance apply to
-000047e0: 2074 6865 2069 6e64 6578 206f 6620 7468   the index of th
-000047f0: 6520 6c61 7374 2063 6f6d 6d69 7474 6564  e last committed
-00004800: 2065 6e74 7269 6573 2067 6976 656e 2062   entries given b
-00004810: 6566 6f72 652e 0a20 2020 2020 2020 2022  efore..        "
-00004820: 2222 0a20 2020 2064 6566 2061 6476 616e  "".    def advan
-00004830: 6365 5f61 7070 6c79 5f74 6f28 7365 6c66  ce_apply_to(self
-00004840: 2c20 6170 706c 6965 643a 2069 6e74 2920  , applied: int) 
-00004850: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00004860: 2022 2222 0a20 2020 2020 2020 2041 6476   """.        Adv
-00004870: 616e 6365 2061 7070 6c79 2074 6f20 7468  ance apply to th
-00004880: 6520 7061 7373 6564 2069 6e64 6578 2e0a  e passed index..
-00004890: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000048a0: 6465 6620 6164 7661 6e63 6528 7365 6c66  def advance(self
-000048b0: 2c20 7264 3a20 2252 6561 6479 5265 6622  , rd: "ReadyRef"
-000048c0: 2920 2d3e 2022 4c69 6768 7452 6561 6479  ) -> "LightReady
-000048d0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-000048e0: 2020 2020 2020 2041 6476 616e 6365 7320         Advances 
-000048f0: 7468 6520 7265 6164 7920 6166 7465 7220  the ready after 
-00004900: 6675 6c6c 7920 7072 6f63 6573 7369 6e67  fully processing
-00004910: 2069 742e 0a0a 2020 2020 2020 2020 4675   it...        Fu
-00004920: 6c6c 7920 7072 6f63 6573 7369 6e67 2061  lly processing a
-00004930: 2072 6561 6479 2072 6571 7569 7265 7320   ready requires 
-00004940: 746f 2070 6572 7369 7374 2073 6e61 7073  to persist snaps
-00004950: 686f 742c 2065 6e74 7269 6573 2061 6e64  hot, entries and
-00004960: 2068 6172 6420 7374 6174 6573 2c20 6170   hard states, ap
-00004970: 706c 7920 616c 6c0a 2020 2020 2020 2020  ply all.        
-00004980: 636f 6d6d 6974 7465 6420 656e 7472 6965  committed entrie
-00004990: 732c 2073 656e 6420 616c 6c20 6d65 7373  s, send all mess
-000049a0: 6167 6573 2e0a 0a20 2020 2020 2020 2052  ages...        R
-000049b0: 6574 7572 6e73 2074 6865 204c 6967 6874  eturns the Light
-000049c0: 5265 6164 7920 7468 6174 2063 6f6e 7461  Ready that conta
-000049d0: 696e 7320 636f 6d6d 6974 2069 6e64 6578  ins commit index
-000049e0: 2c20 636f 6d6d 6974 7465 6420 656e 7472  , committed entr
-000049f0: 6965 7320 616e 6420 6d65 7373 6167 6573  ies and messages
-00004a00: 2e20 5b60 4c69 6768 7452 6561 6479 605d  . [`LightReady`]
-00004a10: 0a20 2020 2020 2020 2063 6f6e 7461 696e  .        contain
-00004a20: 7320 7570 6461 7465 7320 7468 6174 206f  s updates that o
-00004a30: 6e6c 7920 7661 6c69 6420 6166 7465 7220  nly valid after 
-00004a40: 7065 7273 6973 7469 6e67 206c 6173 7420  persisting last 
-00004a50: 7265 6164 792e 2049 7420 7368 6f75 6c64  ready. It should
-00004a60: 2061 6c73 6f20 6265 2066 756c 6c79 2070   also be fully p
-00004a70: 726f 6365 7373 6564 2e0a 2020 2020 2020  rocessed..      
-00004a80: 2020 5468 656e 205b 6053 656c 663a 3a61    Then [`Self::a
-00004a90: 6476 616e 6365 5f61 7070 6c79 605d 206f  dvance_apply`] o
-00004aa0: 7220 5b60 5365 6c66 3a3a 6164 7661 6e63  r [`Self::advanc
-00004ab0: 655f 6170 706c 795f 746f 605d 2073 686f  e_apply_to`] sho
-00004ac0: 756c 6420 6265 2075 7365 6420 6c61 7465  uld be used late
-00004ad0: 7220 746f 2075 7064 6174 6520 6170 706c  r to update appl
-00004ae0: 7969 6e67 0a20 2020 2020 2020 2070 726f  ying.        pro
-00004af0: 6772 6573 732e 0a20 2020 2020 2020 2022  gress..        "
-00004b00: 2222 0a20 2020 2064 6566 2061 6476 616e  "".    def advan
-00004b10: 6365 5f61 7070 656e 6428 7365 6c66 2c20  ce_append(self, 
-00004b20: 7264 3a20 2252 6561 6479 5265 6622 2920  rd: "ReadyRef") 
-00004b30: 2d3e 2022 4c69 6768 7452 6561 6479 223a  -> "LightReady":
-00004b40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004b50: 2020 2020 2041 6476 616e 6365 7320 7468       Advances th
-00004b60: 6520 7265 6164 7920 7769 7468 6f75 7420  e ready without 
-00004b70: 6170 706c 7969 6e67 2063 6f6d 6d69 7474  applying committ
-00004b80: 6564 2065 6e74 7269 6573 2e20 5b60 5365  ed entries. [`Se
-00004b90: 6c66 3a3a 6164 7661 6e63 655f 6170 706c  lf::advance_appl
-00004ba0: 7960 5d20 6f72 0a20 2020 2020 2020 205b  y`] or.        [
-00004bb0: 6053 656c 663a 3a61 6476 616e 6365 5f61  `Self::advance_a
-00004bc0: 7070 6c79 5f74 6f60 5d20 7368 6f75 6c64  pply_to`] should
-00004bd0: 2062 6520 7573 6564 206c 6174 6572 2074   be used later t
-00004be0: 6f20 7570 6461 7465 2061 7070 6c79 696e  o update applyin
-00004bf0: 6720 7072 6f67 7265 7373 2e0a 0a20 2020  g progress...   
-00004c00: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
-00004c10: 204c 6967 6874 5265 6164 7920 7468 6174   LightReady that
-00004c20: 2063 6f6e 7461 696e 7320 636f 6d6d 6974   contains commit
-00004c30: 2069 6e64 6578 2c20 636f 6d6d 6974 7465   index, committe
-00004c40: 6420 656e 7472 6965 7320 616e 6420 6d65  d entries and me
-00004c50: 7373 6167 6573 2e0a 0a20 2020 2020 2020  ssages...       
-00004c60: 2053 696e 6365 2052 6561 6479 206d 7573   Since Ready mus
-00004c70: 7420 6265 2070 6572 7369 7374 6564 2069  t be persisted i
-00004c80: 6e20 6f72 6465 722c 2063 616c 6c69 6e67  n order, calling
-00004c90: 2074 6869 7320 6675 6e63 7469 6f6e 2069   this function i
-00004ca0: 6d70 6c69 6369 746c 7920 6d65 616e 730a  mplicitly means.
-00004cb0: 2020 2020 2020 2020 616c 6c20 7265 6164          all read
-00004cc0: 7920 636f 6c6c 6563 7465 6420 6265 666f  y collected befo
-00004cd0: 7265 2068 6176 6520 6265 656e 2070 6572  re have been per
-00004ce0: 7369 7374 6564 2e0a 2020 2020 2020 2020  sisted..        
-00004cf0: 2222 220a 2020 2020 6465 6620 6164 7661  """.    def adva
-00004d00: 6e63 655f 6170 7065 6e64 5f61 7379 6e63  nce_append_async
-00004d10: 2873 656c 662c 2072 643a 2022 5265 6164  (self, rd: "Read
-00004d20: 7952 6566 2229 202d 3e20 4e6f 6e65 3a0a  yRef") -> None:.
-00004d30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004d40: 2020 2020 5361 6d65 2061 7320 5b60 5365      Same as [`Se
-00004d50: 6c66 3a3a 6164 7661 6e63 655f 6170 7065  lf::advance_appe
-00004d60: 6e64 605d 2065 7863 6570 7420 7468 6174  nd`] except that
-00004d70: 2069 7420 616c 6c6f 7773 2074 6f20 6f6e   it allows to on
-00004d80: 6c79 2073 746f 7265 2074 6865 2075 7064  ly store the upd
-00004d90: 6174 6573 2069 6e20 6361 6368 652e 0a20  ates in cache.. 
-00004da0: 2020 2020 2020 205b 6053 656c 663a 3a6f         [`Self::o
-00004db0: 6e5f 7065 7273 6973 745f 7265 6164 7960  n_persist_ready`
-00004dc0: 5d20 7368 6f75 6c64 2062 6520 7573 6564  ] should be used
-00004dd0: 206c 6174 6572 2074 6f20 7570 6461 7465   later to update
-00004de0: 2074 6865 2070 6572 7369 7374 696e 6720   the persisting 
-00004df0: 7072 6f67 7265 7373 2e0a 0a20 2020 2020  progress...     
-00004e00: 2020 2052 6166 7420 776f 726b 7320 6f6e     Raft works on
-00004e10: 2061 6e20 6173 7375 6d70 7469 6f6e 2070   an assumption p
-00004e20: 6572 7369 7374 6564 2075 7064 6174 6573  ersisted updates
-00004e30: 2073 686f 756c 6420 6e6f 7420 6265 206c   should not be l
-00004e40: 6f73 742c 2077 6869 6368 2075 7375 616c  ost, which usual
-00004e50: 6c79 2072 6571 7569 7265 7320 6578 7065  ly requires expe
-00004e60: 6e73 6976 650a 2020 2020 2020 2020 6f70  nsive.        op
-00004e70: 6572 6174 696f 6e73 206c 696b 6520 6066  erations like `f
-00004e80: 7379 6e63 602e 2060 6164 7661 6e63 655f  sync`. `advance_
-00004e90: 6170 7065 6e64 5f61 7379 6e63 6020 616c  append_async` al
-00004ea0: 6c6f 7773 2079 6f75 2074 6f20 636f 6e74  lows you to cont
-00004eb0: 726f 6c20 7468 6520 7261 7465 206f 6620  rol the rate of 
-00004ec0: 7375 6368 206f 7065 7261 7469 6f6e 7320  such operations 
-00004ed0: 616e 640a 2020 2020 2020 2020 6765 7420  and.        get 
-00004ee0: 6120 7265 6173 6f6e 6162 6c65 2062 6174  a reasonable bat
-00004ef0: 6368 2073 697a 652e 2048 6f77 6576 6572  ch size. However
-00004f00: 2c20 6974 2773 2073 7469 6c6c 2072 6571  , it's still req
-00004f10: 7569 7265 6420 7468 6174 2074 6865 2075  uired that the u
-00004f20: 7064 6174 6573 2063 616e 2062 6520 7265  pdates can be re
-00004f30: 6164 2062 7920 7261 6674 2066 726f 6d20  ad by raft from 
-00004f40: 7468 650a 2020 2020 2020 2020 6053 746f  the.        `Sto
-00004f50: 7261 6765 6020 7472 6169 7420 6265 666f  rage` trait befo
-00004f60: 7265 2063 616c 6c69 6e67 2060 6164 7661  re calling `adva
-00004f70: 6e63 655f 6170 7065 6e64 5f61 7379 6e63  nce_append_async
-00004f80: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
-00004f90: 2020 2064 6566 2068 6173 5f72 6561 6479     def has_ready
-00004fa0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00004fb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004fc0: 2020 2020 4861 7352 6561 6479 2063 616c      HasReady cal
-00004fd0: 6c65 6420 7768 656e 2052 6177 4e6f 6465  led when RawNode
-00004fe0: 2075 7365 7220 6e65 6564 2074 6f20 6368   user need to ch
-00004ff0: 6563 6b20 6966 2061 6e79 2052 6561 6479  eck if any Ready
-00005000: 2070 656e 6469 6e67 2e0a 2020 2020 2020   pending..      
-00005010: 2020 2222 220a 2020 2020 6465 6620 7469    """.    def ti
-00005020: 636b 2873 656c 6629 202d 3e20 626f 6f6c  ck(self) -> bool
-00005030: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00005040: 2020 2020 2020 5469 636b 2061 6476 616e        Tick advan
-00005050: 6365 7320 7468 6520 696e 7465 726e 616c  ces the internal
-00005060: 206c 6f67 6963 616c 2063 6c6f 636b 2062   logical clock b
-00005070: 7920 6120 7369 6e67 6c65 2074 6963 6b2e  y a single tick.
-00005080: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00005090: 7320 7472 7565 2074 6f20 696e 6469 6361  s true to indica
-000050a0: 7465 2074 6861 7420 7468 6572 6520 7769  te that there wi
-000050b0: 6c6c 2070 726f 6261 626c 7920 6265 2073  ll probably be s
-000050c0: 6f6d 6520 7265 6164 696e 6573 7320 7768  ome readiness wh
-000050d0: 6963 680a 2020 2020 2020 2020 6e65 6564  ich.        need
-000050e0: 7320 746f 2062 6520 6861 6e64 6c65 642e  s to be handled.
-000050f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00005100: 2064 6566 2073 6574 5f62 6174 6368 5f61   def set_batch_a
-00005110: 7070 656e 6428 7365 6c66 2c20 6261 7463  ppend(self, batc
-00005120: 685f 6170 7065 6e64 3a20 626f 6f6c 2920  h_append: bool) 
-00005130: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00005140: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
-00005150: 2077 6865 7468 6572 2074 6f20 6261 7463   whether to batc
-00005160: 6820 6170 7065 6e64 206d 7367 2061 7420  h append msg at 
-00005170: 7275 6e74 696d 652e 0a20 2020 2020 2020  runtime..       
-00005180: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00005190: 5f70 7269 6f72 6974 7928 7365 6c66 2c20  _priority(self, 
-000051a0: 7072 696f 7269 7479 3a20 696e 7429 202d  priority: int) -
-000051b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000051c0: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
-000051d0: 2070 7269 6f72 6974 7920 6f66 206e 6f64   priority of nod
-000051e0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-000051f0: 2020 2064 6566 2072 6570 6f72 745f 736e     def report_sn
-00005200: 6170 7368 6f74 2873 656c 662c 2069 643a  apshot(self, id:
-00005210: 2069 6e74 2c20 736e 6170 7368 6f74 3a20   int, snapshot: 
-00005220: 2253 6e61 7073 686f 7453 7461 7475 7322  "SnapshotStatus"
-00005230: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00005240: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00005250: 6570 6f72 7453 6e61 7073 686f 7420 7265  eportSnapshot re
-00005260: 706f 7274 7320 7468 6520 7374 6174 7573  ports the status
-00005270: 206f 6620 7468 6520 7365 6e74 2073 6e61   of the sent sna
-00005280: 7073 686f 742e 0a20 2020 2020 2020 2022  pshot..        "
-00005290: 2222 0a20 2020 2064 6566 2072 6570 6f72  "".    def repor
-000052a0: 745f 756e 7265 6163 6861 626c 6528 7365  t_unreachable(se
-000052b0: 6c66 2c20 6964 3a20 696e 7429 202d 3e20  lf, id: int) -> 
-000052c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000052d0: 220a 2020 2020 2020 2020 5265 706f 7274  ".        Report
-000052e0: 556e 7265 6163 6861 626c 6520 7265 706f  Unreachable repo
-000052f0: 7274 7320 7468 6520 6769 7665 6e20 6e6f  rts the given no
-00005300: 6465 2069 7320 6e6f 7420 7265 6163 6861  de is not reacha
-00005310: 626c 6520 666f 7220 7468 6520 6c61 7374  ble for the last
-00005320: 2073 656e 642e 0a20 2020 2020 2020 2022   send..        "
-00005330: 2222 0a20 2020 2064 6566 2074 7261 6e73  "".    def trans
-00005340: 6665 725f 6c65 6164 6572 2873 656c 662c  fer_leader(self,
-00005350: 2074 7261 6e73 6665 7265 653a 2069 6e74   transferee: int
-00005360: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00005370: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-00005380: 7261 6e73 6665 724c 6561 6465 7220 7472  ransferLeader tr
-00005390: 6965 7320 746f 2074 7261 6e73 6665 7220  ies to transfer 
-000053a0: 6c65 6164 6572 7368 6970 2074 6f20 7468  leadership to th
-000053b0: 6520 6769 7665 6e20 7472 616e 7366 6572  e given transfer
-000053c0: 6565 2e0a 2020 2020 2020 2020 2222 220a  ee..        """.
-000053d0: 2020 2020 6465 6620 736e 6170 2873 656c      def snap(sel
-000053e0: 6629 202d 3e20 4f70 7469 6f6e 616c 5b22  f) -> Optional["
-000053f0: 536e 6170 7368 6f74 5265 6622 5d3a 0a20  SnapshotRef"]:. 
-00005400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005410: 2020 2047 7261 6273 2074 6865 2073 6e61     Grabs the sna
-00005420: 7073 686f 7420 6672 6f6d 2074 6865 2072  pshot from the r
-00005430: 6166 7420 6966 2061 7661 696c 6162 6c65  aft if available
-00005440: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00005450: 2020 6465 6620 7374 6570 2873 656c 662c    def step(self,
-00005460: 206d 7367 3a20 224d 6573 7361 6765 2220   msg: "Message" 
-00005470: 7c20 224d 6573 7361 6765 5265 6622 2920  | "MessageRef") 
-00005480: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00005490: 2022 2222 0a20 2020 2020 2020 2053 7465   """.        Ste
-000054a0: 7020 6164 7661 6e63 6573 2074 6865 2073  p advances the s
-000054b0: 7461 7465 206d 6163 6869 6e65 2075 7369  tate machine usi
-000054c0: 6e67 2074 6865 2067 6976 656e 206d 6573  ng the given mes
-000054d0: 7361 6765 2e0a 2020 2020 2020 2020 2222  sage..        ""
-000054e0: 220a 2020 2020 6465 6620 736b 6970 5f62  ".    def skip_b
-000054f0: 6361 7374 5f63 6f6d 6d69 7428 7365 6c66  cast_commit(self
-00005500: 2c20 736b 6970 3a20 626f 6f6c 2920 2d3e  , skip: bool) ->
-00005510: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00005520: 2222 0a20 2020 2020 2020 2053 6574 2077  "".        Set w
-00005530: 6865 7468 6572 2073 6b69 7020 6272 6f61  hether skip broa
-00005540: 6463 6173 7420 656d 7074 7920 636f 6d6d  dcast empty comm
-00005550: 6974 206d 6573 7361 6765 7320 6174 2072  it messages at r
-00005560: 756e 7469 6d65 2e0a 2020 2020 2020 2020  untime..        
-00005570: 2222 220a 2020 2020 6465 6620 6361 6d70  """.    def camp
-00005580: 6169 676e 2873 656c 6629 202d 3e20 4e6f  aign(self) -> No
-00005590: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-000055a0: 2020 2020 2020 2020 4361 6d70 6169 676e          Campaign
-000055b0: 2063 6175 7365 7320 7468 6973 2052 6177   causes this Raw
-000055c0: 4e6f 6465 2074 6f20 7472 616e 7369 7469  Node to transiti
-000055d0: 6f6e 2074 6f20 6361 6e64 6964 6174 6520  on to candidate 
-000055e0: 7374 6174 652e 0a20 2020 2020 2020 2022  state..        "
-000055f0: 2222 0a20 2020 2064 6566 2070 726f 706f  "".    def propo
-00005600: 7365 2873 656c 662c 2063 6f6e 7465 7874  se(self, context
-00005610: 3a20 6279 7465 732c 2064 6174 613a 2062  : bytes, data: b
-00005620: 7974 6573 2920 2d3e 204e 6f6e 653a 0a20  ytes) -> None:. 
-00005630: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005640: 2020 2050 726f 706f 7365 2070 726f 706f     Propose propo
-00005650: 7365 7320 6461 7461 2062 6520 6170 7065  ses data be appe
-00005660: 6e64 6564 2074 6f20 7468 6520 7261 6674  nded to the raft
-00005670: 206c 6f67 2e0a 2020 2020 2020 2020 2222   log..        ""
-00005680: 220a 2020 2020 6465 6620 7072 6f70 6f73  ".    def propos
-00005690: 655f 636f 6e66 5f63 6861 6e67 6528 0a20  e_conf_change(. 
-000056a0: 2020 2020 2020 2073 656c 662c 2063 6f6e         self, con
-000056b0: 7465 7874 3a20 6279 7465 732c 2063 633a  text: bytes, cc:
-000056c0: 2022 436f 6e66 4368 616e 6765 2220 7c20   "ConfChange" | 
-000056d0: 2243 6f6e 6643 6861 6e67 6552 6566 220a  "ConfChangeRef".
-000056e0: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-000056f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005700: 2020 2050 726f 706f 7365 436f 6e66 4368     ProposeConfCh
-00005710: 616e 6765 2070 726f 706f 7365 7320 6120  ange proposes a 
-00005720: 636f 6e66 6967 2063 6861 6e67 652e 0a0a  config change...
-00005730: 2020 2020 2020 2020 4966 2074 6865 206e          If the n
-00005740: 6f64 6520 656e 7465 7273 206a 6f69 6e74  ode enters joint
-00005750: 2073 7461 7465 2077 6974 6820 6061 7574   state with `aut
-00005760: 6f5f 6c65 6176 6560 2073 6574 2074 6f20  o_leave` set to 
-00005770: 7472 7565 2c20 6974 2773 0a20 2020 2020  true, it's.     
-00005780: 2020 2063 616c 6c65 7227 7320 7265 7370     caller's resp
-00005790: 6f6e 7369 6269 6c69 7479 2074 6f20 7072  onsibility to pr
-000057a0: 6f70 6f73 6520 616e 2065 6d70 7479 2063  opose an empty c
-000057b0: 6f6e 6620 6368 616e 6765 2061 6761 696e  onf change again
-000057c0: 2074 6f20 666f 7263 650a 2020 2020 2020   to force.      
-000057d0: 2020 6c65 6176 696e 6720 6a6f 696e 7420    leaving joint 
-000057e0: 7374 6174 652e 0a20 2020 2020 2020 2022  state..        "
-000057f0: 2222 0a20 2020 2064 6566 2070 726f 706f  "".    def propo
-00005800: 7365 5f63 6f6e 665f 6368 616e 6765 5f76  se_conf_change_v
-00005810: 3228 0a20 2020 2020 2020 2073 656c 662c  2(.        self,
-00005820: 2063 6f6e 7465 7874 3a20 6279 7465 732c   context: bytes,
-00005830: 2063 633a 2022 436f 6e66 4368 616e 6765   cc: "ConfChange
-00005840: 5632 2220 7c20 2243 6f6e 6643 6861 6e67  V2" | "ConfChang
-00005850: 6556 3252 6566 220a 2020 2020 2920 2d3e  eV2Ref".    ) ->
-00005860: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00005870: 2222 0a20 2020 2020 2020 2050 726f 706f  "".        Propo
-00005880: 7365 436f 6e66 4368 616e 6765 2070 726f  seConfChange pro
-00005890: 706f 7365 7320 6120 636f 6e66 6967 2063  poses a config c
-000058a0: 6861 6e67 652e 0a0a 2020 2020 2020 2020  hange...        
-000058b0: 4966 2074 6865 206e 6f64 6520 656e 7465  If the node ente
-000058c0: 7273 206a 6f69 6e74 2073 7461 7465 2077  rs joint state w
-000058d0: 6974 6820 6061 7574 6f5f 6c65 6176 6560  ith `auto_leave`
-000058e0: 2073 6574 2074 6f20 7472 7565 2c20 6974   set to true, it
-000058f0: 2773 0a20 2020 2020 2020 2063 616c 6c65  's.        calle
-00005900: 7227 7320 7265 7370 6f6e 7369 6269 6c69  r's responsibili
-00005910: 7479 2074 6f20 7072 6f70 6f73 6520 616e  ty to propose an
-00005920: 2065 6d70 7479 2063 6f6e 6620 6368 616e   empty conf chan
-00005930: 6765 2061 6761 696e 2074 6f20 666f 7263  ge again to forc
-00005940: 650a 2020 2020 2020 2020 6c65 6176 696e  e.        leavin
-00005950: 6720 6a6f 696e 7420 7374 6174 652e 0a20  g joint state.. 
-00005960: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00005970: 6566 2061 7070 6c79 5f63 6f6e 665f 6368  ef apply_conf_ch
-00005980: 616e 6765 2873 656c 662c 2063 633a 2022  ange(self, cc: "
-00005990: 436f 6e66 4368 616e 6765 2220 7c20 2243  ConfChange" | "C
-000059a0: 6f6e 6643 6861 6e67 6552 6566 2229 202d  onfChangeRef") -
-000059b0: 3e20 436f 6e66 5374 6174 653a 0a20 2020  > ConfState:.   
-000059c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000059d0: 2041 7070 6c69 6573 2061 2063 6f6e 6669   Applies a confi
-000059e0: 6720 6368 616e 6765 2074 6f20 7468 6520  g change to the 
-000059f0: 6c6f 6361 6c20 6e6f 6465 2e20 5468 6520  local node. The 
-00005a00: 6170 7020 6d75 7374 2063 616c 6c20 7468  app must call th
-00005a10: 6973 2077 6865 6e20 6974 0a20 2020 2020  is when it.     
-00005a20: 2020 2061 7070 6c69 6573 2061 2063 6f6e     applies a con
-00005a30: 6669 6775 7261 7469 6f6e 2063 6861 6e67  figuration chang
-00005a40: 652c 2065 7863 6570 7420 7768 656e 2069  e, except when i
-00005a50: 7420 6465 6369 6465 7320 746f 2072 656a  t decides to rej
-00005a60: 6563 7420 7468 650a 2020 2020 2020 2020  ect the.        
-00005a70: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
-00005a80: 616e 6765 2c20 696e 2077 6869 6368 2063  ange, in which c
-00005a90: 6173 6520 6e6f 2063 616c 6c20 6d75 7374  ase no call must
-00005aa0: 2074 616b 6520 706c 6163 652e 0a20 2020   take place..   
-00005ab0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00005ac0: 2061 7070 6c79 5f63 6f6e 665f 6368 616e   apply_conf_chan
-00005ad0: 6765 5f76 3228 0a20 2020 2020 2020 2073  ge_v2(.        s
-00005ae0: 656c 662c 2063 633a 2022 436f 6e66 4368  elf, cc: "ConfCh
-00005af0: 616e 6765 5632 2220 7c20 2243 6f6e 6643  angeV2" | "ConfC
-00005b00: 6861 6e67 6556 3252 6566 220a 2020 2020  hangeV2Ref".    
-00005b10: 2920 2d3e 2022 436f 6e66 5374 6174 6522  ) -> "ConfState"
-00005b20: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00005b30: 2020 2020 2020 4170 706c 6965 7320 6120        Applies a 
-00005b40: 636f 6e66 6967 2063 6861 6e67 6520 746f  config change to
-00005b50: 2074 6865 206c 6f63 616c 206e 6f64 652e   the local node.
-00005b60: 2054 6865 2061 7070 206d 7573 7420 6361   The app must ca
-00005b70: 6c6c 2074 6869 7320 7768 656e 2069 740a  ll this when it.
-00005b80: 2020 2020 2020 2020 6170 706c 6965 7320          applies 
-00005b90: 6120 636f 6e66 6967 7572 6174 696f 6e20  a configuration 
-00005ba0: 6368 616e 6765 2c20 6578 6365 7074 2077  change, except w
-00005bb0: 6865 6e20 6974 2064 6563 6964 6573 2074  hen it decides t
-00005bc0: 6f20 7265 6a65 6374 2074 6865 0a20 2020  o reject the.   
-00005bd0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-00005be0: 6f6e 2063 6861 6e67 652c 2069 6e20 7768  on change, in wh
-00005bf0: 6963 6820 6361 7365 206e 6f20 6361 6c6c  ich case no call
-00005c00: 206d 7573 7420 7461 6b65 2070 6c61 6365   must take place
-00005c10: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00005c20: 2020 6465 6620 7069 6e67 2873 656c 6629    def ping(self)
-00005c30: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00005c40: 2020 2222 220a 2020 2020 2020 2020 4272    """.        Br
-00005c50: 6f61 6463 6173 7420 6865 6172 7462 6561  oadcast heartbea
-00005c60: 7473 2074 6f20 616c 6c20 7468 6520 666f  ts to all the fo
-00005c70: 6c6c 6f77 6572 732e 0a0a 2020 2020 2020  llowers...      
-00005c80: 2020 4966 2069 7427 7320 6e6f 7420 6c65    If it's not le
-00005c90: 6164 6572 2c20 6e6f 7468 696e 6720 7769  ader, nothing wi
-00005ca0: 6c6c 2068 6170 7065 6e2e 0a20 2020 2020  ll happen..     
-00005cb0: 2020 2022 2222 0a20 2020 2064 6566 206f     """.    def o
-00005cc0: 6e5f 7065 7273 6973 745f 7265 6164 7928  n_persist_ready(
-00005cd0: 7365 6c66 2c20 6e75 6d62 6572 3a20 696e  self, number: in
-00005ce0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00005cf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005d00: 4e6f 7469 6669 6573 2074 6861 7420 7468  Notifies that th
-00005d10: 6520 7265 6164 7920 6f66 2074 6869 7320  e ready of this 
-00005d20: 6e75 6d62 6572 2068 6173 2062 6565 6e20  number has been 
-00005d30: 7065 7273 6973 7465 642e 0a0a 2020 2020  persisted...    
-00005d40: 2020 2020 5369 6e63 6520 5265 6164 7920      Since Ready 
-00005d50: 6d75 7374 2062 6520 7065 7273 6973 7465  must be persiste
-00005d60: 6420 696e 206f 7264 6572 2c20 6361 6c6c  d in order, call
-00005d70: 696e 6720 7468 6973 2066 756e 6374 696f  ing this functio
-00005d80: 6e20 696d 706c 6963 6974 6c79 206d 6561  n implicitly mea
-00005d90: 6e73 0a20 2020 2020 2020 2061 6c6c 2072  ns.        all r
-00005da0: 6561 6469 6573 2077 6974 6820 6e75 6d62  eadies with numb
-00005db0: 6572 7320 736d 616c 6c65 7220 7468 616e  ers smaller than
-00005dc0: 2074 6869 7320 6f6e 6520 6861 7665 2062   this one have b
-00005dd0: 6565 6e20 7065 7273 6973 7465 642e 0a0a  een persisted...
-00005de0: 2020 2020 2020 2020 5b60 5365 6c66 3a3a          [`Self::
-00005df0: 6861 735f 7265 6164 7960 5d20 616e 6420  has_ready`] and 
-00005e00: 5b60 5365 6c66 3a3a 7265 6164 7960 5d20  [`Self::ready`] 
-00005e10: 7368 6f75 6c64 2062 6520 6361 6c6c 6564  should be called
-00005e20: 206c 6174 6572 2074 6f20 6861 6e64 6c65   later to handle
-00005e30: 2066 7572 7468 6572 0a20 2020 2020 2020   further.       
-00005e40: 2075 7064 6174 6573 2074 6861 7420 6265   updates that be
-00005e50: 636f 6d65 2076 616c 6964 2061 6674 6572  come valid after
-00005e60: 2072 6561 6479 2062 6569 6e67 2070 6572   ready being per
-00005e70: 7369 7374 6564 2e0a 2020 2020 2020 2020  sisted..        
-00005e80: 2222 220a 2020 2020 6465 6620 7265 6164  """.    def read
-00005e90: 5f69 6e64 6578 2873 656c 662c 2072 6374  _index(self, rct
-00005ea0: 783a 2062 7974 6573 2920 2d3e 204e 6f6e  x: bytes) -> Non
-00005eb0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00005ec0: 2020 2020 2020 2052 6561 6449 6e64 6578         ReadIndex
-00005ed0: 2072 6571 7565 7374 7320 6120 7265 6164   requests a read
-00005ee0: 2073 7461 7465 2e20 5468 6520 7265 6164   state. The read
-00005ef0: 2073 7461 7465 2077 696c 6c20 6265 2073   state will be s
-00005f00: 6574 2069 6e20 7265 6164 792e 0a20 2020  et in ready..   
-00005f10: 2020 2020 2052 6561 6420 5374 6174 6520       Read State 
-00005f20: 6861 7320 6120 7265 6164 2069 6e64 6578  has a read index
-00005f30: 2e20 4f6e 6365 2074 6865 2061 7070 6c69  . Once the appli
-00005f40: 6361 7469 6f6e 2061 6476 616e 6365 7320  cation advances 
-00005f50: 6675 7274 6865 7220 7468 616e 2074 6865  further than the
-00005f60: 2072 6561 640a 2020 2020 2020 2020 696e   read.        in
-00005f70: 6465 782c 2061 6e79 206c 696e 6561 7269  dex, any lineari
-00005f80: 7a61 626c 6520 7265 6164 2072 6571 7565  zable read reque
-00005f90: 7374 7320 6973 7375 6564 2062 6566 6f72  sts issued befor
-00005fa0: 6520 7468 6520 7265 6164 2072 6571 7565  e the read reque
-00005fb0: 7374 2063 616e 2062 650a 2020 2020 2020  st can be.      
-00005fc0: 2020 7072 6f63 6573 7365 6420 7361 6665    processed safe
-00005fd0: 6c79 2e20 5468 6520 7265 6164 2073 7461  ly. The read sta
-00005fe0: 7465 2077 696c 6c20 6861 7665 2074 6865  te will have the
-00005ff0: 2073 616d 6520 7263 7478 2061 7474 6163   same rctx attac
-00006000: 6865 642e 0a20 2020 2020 2020 2022 2222  hed..        """
-00006010: 0a20 2020 2064 6566 2072 6561 6479 2873  .    def ready(s
-00006020: 656c 6629 202d 3e20 5265 6164 793a 0a20  elf) -> Ready:. 
-00006030: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00006040: 2020 2052 6574 7572 6e73 2074 6865 206f     Returns the o
-00006050: 7574 7374 616e 6469 6e67 2077 6f72 6b20  utstanding work 
-00006060: 7468 6174 2074 6865 2061 7070 6c69 6361  that the applica
-00006070: 7469 6f6e 206e 6565 6473 2074 6f20 6861  tion needs to ha
-00006080: 6e64 6c65 2e0a 0a20 2020 2020 2020 2054  ndle...        T
-00006090: 6869 7320 696e 636c 7564 6573 2061 7070  his includes app
-000060a0: 656e 6469 6e67 2061 6e64 2061 7070 6c79  ending and apply
-000060b0: 696e 6720 656e 7472 6965 7320 6f72 2061  ing entries or a
-000060c0: 2073 6e61 7073 686f 742c 2075 7064 6174   snapshot, updat
-000060d0: 696e 6720 7468 6520 4861 7264 5374 6174  ing the HardStat
-000060e0: 652c 0a20 2020 2020 2020 2061 6e64 2073  e,.        and s
-000060f0: 656e 6469 6e67 206d 6573 7361 6765 732e  ending messages.
-00006100: 2054 6865 2072 6574 7572 6e65 6420 6052   The returned `R
-00006110: 6561 6479 6020 2a4d 5553 542a 2062 6520  eady` *MUST* be 
-00006120: 6861 6e64 6c65 6420 616e 6420 7375 6273  handled and subs
-00006130: 6571 7565 6e74 6c79 0a20 2020 2020 2020  equently.       
-00006140: 2070 6173 7365 6420 6261 636b 2076 6961   passed back via
-00006150: 2060 6164 7661 6e63 6560 206f 7220 6974   `advance` or it
-00006160: 7320 6661 6d69 6c69 6573 2e20 4265 666f  s families. Befo
-00006170: 7265 2074 6861 742c 202a 444f 204e 4f54  re that, *DO NOT
-00006180: 2a20 6361 6c6c 2061 6e79 2066 756e 6374  * call any funct
-00006190: 696f 6e20 6c69 6b65 0a20 2020 2020 2020  ion like.       
-000061a0: 2060 7374 6570 602c 2060 7072 6f70 6f73   `step`, `propos
-000061b0: 6560 2c20 6063 616d 7061 6967 6e60 2074  e`, `campaign` t
-000061c0: 6f20 6368 616e 6765 2069 6e74 6572 6e61  o change interna
-000061d0: 6c20 7374 6174 652e 0a0a 2020 2020 2020  l state...      
-000061e0: 2020 5b60 5365 6c66 3a3a 6861 735f 7265    [`Self::has_re
-000061f0: 6164 7960 5d20 7368 6f75 6c64 2062 6520  ady`] should be 
-00006200: 6361 6c6c 6564 2066 6972 7374 2074 6f20  called first to 
-00006210: 6368 6563 6b20 6966 2069 7427 7320 6e65  check if it's ne
-00006220: 6365 7373 6172 7920 746f 2068 616e 646c  cessary to handl
-00006230: 6520 7468 6520 7265 6164 792e 0a20 2020  e the ready..   
-00006240: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00006250: 2072 6571 7565 7374 5f73 6e61 7073 686f   request_snapsho
-00006260: 7428 7365 6c66 2920 2d3e 2022 5265 6164  t(self) -> "Read
-00006270: 7922 3a0a 2020 2020 2020 2020 2222 220a  y":.        """.
-00006280: 2020 2020 2020 2020 5265 7175 6573 7420          Request 
-00006290: 6120 736e 6170 7368 6f74 2066 726f 6d20  a snapshot from 
-000062a0: 6120 6c65 6164 6572 2e0a 2020 2020 2020  a leader..      
-000062b0: 2020 5468 6520 736e 6170 7368 6f74 2773    The snapshot's
-000062c0: 2069 6e64 6578 206d 7573 7420 6265 2067   index must be g
-000062d0: 7265 6174 6572 206f 7220 6571 7561 6c20  reater or equal 
-000062e0: 746f 2074 6865 2072 6571 7565 7374 5f69  to the request_i
-000062f0: 6e64 6578 2028 6c61 7374 5f69 6e64 6578  ndex (last_index
-00006300: 2920 6f72 0a20 2020 2020 2020 2074 6865  ) or.        the
-00006310: 206c 6561 6465 7227 7320 7465 726d 206d   leader's term m
-00006320: 7573 7420 6265 2067 7265 6174 6572 2074  ust be greater t
-00006330: 6861 6e20 7468 6520 7265 7175 6573 7420  han the request 
-00006340: 7465 726d 2028 6c61 7374 5f69 6e64 6578  term (last_index
-00006350: 2773 2074 6572 6d29 2e0a 2020 2020 2020  's term)..      
-00006360: 2020 2222 220a 2020 2020 6465 6620 6f6e    """.    def on
-00006370: 5f65 6e74 7269 6573 5f66 6574 6368 6564  _entries_fetched
-00006380: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00006390: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000063a0: 2020 2020 4120 6361 6c6c 6261 636b 2077      A callback w
-000063b0: 6865 6e20 656e 7472 6965 7320 6172 6520  hen entries are 
-000063c0: 6665 7463 6865 6420 6173 796e 6368 726f  fetched asynchro
-000063d0: 6e6f 7573 6c79 2e0a 2020 2020 2020 2020  nously..        
-000063e0: 5468 6520 636f 6e74 6578 7420 7368 6f75  The context shou
-000063f0: 6c64 2070 726f 7669 6465 2074 6865 2063  ld provide the c
-00006400: 6f6e 7465 7874 2070 6173 7365 6420 6672  ontext passed fr
-00006410: 6f6d 2053 746f 7261 6765 2e65 6e74 6972  om Storage.entir
-00006420: 6573 2829 2e0a 2020 2020 2020 2020 5365  es()..        Se
-00006430: 6520 6d6f 7265 2069 6e20 7468 6520 636f  e more in the co
-00006440: 6d6d 656e 7420 6f66 2053 746f 7261 6765  mment of Storage
-00006450: 2e65 6e74 6972 6573 2829 2e0a 0a20 2020  .entires()...   
-00006460: 2020 2020 2023 2050 616e 6963 730a 0a20       # Panics.. 
-00006470: 2020 2020 2020 2050 616e 6963 7320 6966         Panics if
-00006480: 2070 6173 7365 6420 7769 7468 2074 6865   passed with the
-00006490: 2063 6f6e 7465 7874 206f 6620 636f 6e74   context of cont
-000064a0: 6578 742e 6361 6e5f 6173 796e 6328 2920  ext.can_async() 
-000064b0: 3d3d 2066 616c 7365 0a20 2020 2020 2020  == false.       
-000064c0: 2022 2222 0a0a 636c 6173 7320 496e 4d65   """..class InMe
-000064d0: 6d6f 7279 5261 774e 6f64 6528 5f5f 4150  moryRawNode(__AP
-000064e0: 495f 5261 774e 6f64 6529 3a0a 2020 2020  I_RawNode):.    
-000064f0: 2222 220a 2020 2020 5261 774e 6f64 6520  """.    RawNode 
-00006500: 6973 2061 2074 6872 6561 642d 756e 7361  is a thread-unsa
-00006510: 6665 204e 6f64 652e 0a20 2020 2054 6865  fe Node..    The
-00006520: 206d 6574 686f 6473 206f 6620 7468 6973   methods of this
-00006530: 2073 7472 7563 7420 636f 7272 6573 706f   struct correspo
-00006540: 6e64 2074 6f20 7468 6520 6d65 7468 6f64  nd to the method
-00006550: 7320 6f66 204e 6f64 6520 616e 6420 6172  s of Node and ar
-00006560: 6520 6465 7363 7269 6265 640a 2020 2020  e described.    
-00006570: 6d6f 7265 2066 756c 6c79 2074 6865 7265  more fully there
-00006580: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00006590: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000065a0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000065b0: 2020 2063 6667 3a20 2243 6f6e 6669 6722     cfg: "Config"
-000065c0: 207c 2022 436f 6e66 6967 5265 6622 2c0a   | "ConfigRef",.
-000065d0: 2020 2020 2020 2020 7374 6f72 653a 2022          store: "
-000065e0: 4d65 6d53 746f 7261 6765 2220 7c20 224d  MemStorage" | "M
-000065f0: 656d 5374 6f72 6167 6552 6566 222c 0a20  emStorageRef",. 
-00006600: 2020 2020 2020 206c 6f67 6765 723a 2022         logger: "
-00006610: 4c6f 6767 6572 2220 7c20 224c 6f67 6765  Logger" | "Logge
-00006620: 7252 6566 222c 0a20 2020 2029 202d 3e20  rRef",.    ) -> 
-00006630: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
-00006640: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
-00006650: 202d 3e20 2249 6e4d 656d 6f72 7952 6177   -> "InMemoryRaw
-00006660: 4e6f 6465 5265 6622 3a20 2e2e 2e0a 2020  NodeRef": ....  
-00006670: 2020 6465 6620 6765 745f 7261 6674 2873    def get_raft(s
-00006680: 656c 6629 202d 3e20 2249 6e4d 656d 6f72  elf) -> "InMemor
-00006690: 7952 6166 7452 6566 223a 0a20 2020 2020  yRaftRef":.     
-000066a0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-000066b0: 6566 2073 746f 7265 2873 656c 6629 202d  ef store(self) -
-000066c0: 3e20 224d 656d 5374 6f72 6167 6552 6566  > "MemStorageRef
-000066d0: 223a 0a20 2020 2020 2020 2022 2222 5265  ":.        """Re
-000066e0: 7475 726e 7320 7468 6520 7374 6f72 6520  turns the store 
-000066f0: 6173 2061 206d 7574 6162 6c65 2072 6566  as a mutable ref
-00006700: 6572 656e 6365 2e22 2222 0a0a 636c 6173  erence."""..clas
-00006710: 7320 496e 4d65 6d6f 7279 5261 774e 6f64  s InMemoryRawNod
-00006720: 6552 6566 285f 5f41 5049 5f52 6177 4e6f  eRef(__API_RawNo
-00006730: 6465 293a 0a20 2020 2022 2222 0a20 2020  de):.    """.   
-00006740: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-00006750: 6f66 203a 636c 6173 733a 6049 6e4d 656d  of :class:`InMem
-00006760: 6f72 7952 6177 4e6f 6465 602e 0a20 2020  oryRawNode`..   
-00006770: 2022 2222 0a0a 2020 2020 6465 6620 6765   """..    def ge
-00006780: 745f 7261 6674 2873 656c 6629 202d 3e20  t_raft(self) -> 
-00006790: 2249 6e4d 656d 6f72 7952 6166 7452 6566  "InMemoryRaftRef
-000067a0: 223a 0a20 2020 2020 2020 2022 2222 2022  ":.        """ "
-000067b0: 2222 0a20 2020 2064 6566 2073 746f 7265  "".    def store
-000067c0: 2873 656c 6629 202d 3e20 224d 656d 5374  (self) -> "MemSt
-000067d0: 6f72 6167 6552 6566 223a 0a20 2020 2020  orageRef":.     
-000067e0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
-000067f0: 6520 7374 6f72 6520 6173 2061 206d 7574  e store as a mut
-00006800: 6162 6c65 2072 6566 6572 656e 6365 2e22  able reference."
-00006810: 2222 0a20 2020 2023 2064 6566 2073 7461  "".    # def sta
-00006820: 7475 7328 7365 6c66 2920 2d3e 2049 6e4d  tus(self) -> InM
-00006830: 656d 6f72 7953 7461 7475 733a 0a20 2020  emoryStatus:.   
-00006840: 2023 2020 2020 2022 2222 0a20 2020 2023   #     """.    #
-00006850: 2020 2020 2053 7461 7475 7320 7265 7475       Status retu
-00006860: 726e 7320 7468 6520 6375 7272 656e 7420  rns the current 
-00006870: 7374 6174 7573 206f 6620 7468 6520 6769  status of the gi
-00006880: 7665 6e20 6772 6f75 702e 0a20 2020 2023  ven group..    #
-00006890: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-000068a0: 5261 774e 6f64 6528 5f5f 4150 495f 5261  RawNode(__API_Ra
-000068b0: 774e 6f64 6529 3a0a 2020 2020 2222 220a  wNode):.    """.
-000068c0: 2020 2020 5261 774e 6f64 6520 6973 2061      RawNode is a
-000068d0: 2074 6872 6561 642d 756e 7361 6665 204e   thread-unsafe N
-000068e0: 6f64 652e 0a20 2020 2054 6865 206d 6574  ode..    The met
-000068f0: 686f 6473 206f 6620 7468 6973 2073 7472  hods of this str
-00006900: 7563 7420 636f 7272 6573 706f 6e64 2074  uct correspond t
-00006910: 6f20 7468 6520 6d65 7468 6f64 7320 6f66  o the methods of
-00006920: 204e 6f64 6520 616e 6420 6172 6520 6465   Node and are de
-00006930: 7363 7269 6265 640a 2020 2020 6d6f 7265  scribed.    more
-00006940: 2066 756c 6c79 2074 6865 7265 2e0a 2020   fully there..  
-00006950: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-00006960: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00006970: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-00006980: 6667 3a20 2243 6f6e 6669 6722 207c 2022  fg: "Config" | "
-00006990: 436f 6e66 6967 5265 6622 2c0a 2020 2020  ConfigRef",.    
-000069a0: 2020 2020 7374 6f72 653a 2022 5374 6f72      store: "Stor
-000069b0: 6167 6522 207c 2022 5374 6f72 6167 6552  age" | "StorageR
-000069c0: 6566 222c 0a20 2020 2020 2020 206c 6f67  ef",.        log
-000069d0: 6765 723a 2022 4c6f 6767 6572 2220 7c20  ger: "Logger" | 
-000069e0: 224c 6f67 6765 7252 6566 222c 0a20 2020  "LoggerRef",.   
-000069f0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-00006a00: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
-00006a10: 2873 656c 6629 202d 3e20 2252 6177 4e6f  (self) -> "RawNo
-00006a20: 6465 5265 6622 3a20 2e2e 2e0a 2020 2020  deRef": ....    
-00006a30: 6465 6620 6765 745f 7261 6674 2873 656c  def get_raft(sel
-00006a40: 6629 202d 3e20 2252 6166 7452 6566 223a  f) -> "RaftRef":
-00006a50: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00006a60: 0a20 2020 2064 6566 2073 746f 7265 2873  .    def store(s
-00006a70: 656c 6629 202d 3e20 2253 746f 7261 6765  elf) -> "Storage
-00006a80: 5265 6622 3a0a 2020 2020 2020 2020 2222  Ref":.        ""
-00006a90: 2252 6574 7572 6e73 2074 6865 2073 746f  "Returns the sto
-00006aa0: 7265 2061 7320 6120 6d75 7461 626c 6520  re as a mutable 
-00006ab0: 7265 6665 7265 6e63 652e 2222 220a 2020  reference.""".  
-00006ac0: 2020 2320 6465 6620 7374 6174 7573 2873    # def status(s
-00006ad0: 656c 6629 202d 3e20 5374 6174 7573 3a0a  elf) -> Status:.
-00006ae0: 2020 2020 2320 2020 2020 2222 220a 2020      #     """.  
-00006af0: 2020 2320 2020 2020 5374 6174 7573 2072    #     Status r
-00006b00: 6574 7572 6e73 2074 6865 2063 7572 7265  eturns the curre
-00006b10: 6e74 2073 7461 7475 7320 6f66 2074 6865  nt status of the
-00006b20: 2067 6976 656e 2067 726f 7570 2e0a 2020   given group..  
-00006b30: 2020 2320 2020 2020 2222 220a 0a63 6c61    #     """..cla
-00006b40: 7373 2052 6177 4e6f 6465 5265 6628 5f5f  ss RawNodeRef(__
-00006b50: 4150 495f 5261 774e 6f64 6529 3a0a 2020  API_RawNode):.  
-00006b60: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
-00006b70: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
-00006b80: 7373 3a60 5261 774e 6f64 6560 2e0a 2020  ss:`RawNode`..  
-00006b90: 2020 2222 220a 0a20 2020 2064 6566 2067    """..    def g
-00006ba0: 6574 5f72 6166 7428 7365 6c66 2920 2d3e  et_raft(self) ->
-00006bb0: 2022 5261 6674 5265 6622 3a0a 2020 2020   "RaftRef":.    
-00006bc0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-00006bd0: 6465 6620 7374 6f72 6528 7365 6c66 2920  def store(self) 
-00006be0: 2d3e 2022 5374 6f72 6167 6552 6566 223a  -> "StorageRef":
-00006bf0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00006c00: 726e 7320 7468 6520 7374 6f72 6520 6173  rns the store as
-00006c10: 2061 206d 7574 6162 6c65 2072 6566 6572   a mutable refer
-00006c20: 656e 6365 2e22 2222 0a20 2020 2023 2064  ence.""".    # d
-00006c30: 6566 2073 7461 7475 7328 7365 6c66 2920  ef status(self) 
-00006c40: 2d3e 2049 6e4d 656d 6f72 7953 7461 7475  -> InMemoryStatu
-00006c50: 733a 0a20 2020 2023 2020 2020 2022 2222  s:.    #     """
-00006c60: 0a20 2020 2023 2020 2020 2053 7461 7475  .    #     Statu
-00006c70: 7320 7265 7475 726e 7320 7468 6520 6375  s returns the cu
-00006c80: 7272 656e 7420 7374 6174 7573 206f 6620  rrent status of 
-00006c90: 7468 6520 6769 7665 6e20 6772 6f75 702e  the given group.
-00006ca0: 0a20 2020 2023 2020 2020 2022 2222 0a0a  .    #     """..
-00006cb0: 636c 6173 7320 5f5f 4150 495f 5065 6572  class __API_Peer
-00006cc0: 3a0a 2020 2020 6465 6620 6765 745f 6964  :.    def get_id
-00006cd0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00006ce0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00006cf0: 2020 2060 6964 603a 2054 6865 2049 4420     `id`: The ID 
-00006d00: 6f66 2074 6865 2070 6565 722e 0a20 2020  of the peer..   
-00006d10: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00006d20: 2073 6574 5f69 6428 7365 6c66 2c20 6964   set_id(self, id
-00006d30: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00006d40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00006d50: 2020 2020 6069 6460 3a20 5468 6520 4944      `id`: The ID
-00006d60: 206f 6620 7468 6520 7065 6572 2e0a 2020   of the peer..  
-00006d70: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00006d80: 6620 6765 745f 636f 6e74 6578 7428 7365  f get_context(se
-00006d90: 6c66 2920 2d3e 2062 7974 6573 3a0a 2020  lf) -> bytes:.  
-00006da0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006db0: 2020 6063 6f6e 7465 7874 603a 2049 6620    `context`: If 
-00006dc0: 7468 6572 6520 6973 2063 6f6e 7465 7874  there is context
-00006dd0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00006de0: 2074 6865 2070 6565 7220 286c 696b 6520   the peer (like 
-00006df0: 636f 6e6e 6563 7469 6f6e 2069 6e66 6f72  connection infor
-00006e00: 6d61 7469 6f6e 292c 2069 7420 6361 6e20  mation), it can 
-00006e10: 6265 0a20 2020 2020 2020 2073 6572 6961  be.        seria
-00006e20: 6c69 7a65 6420 616e 6420 7374 6f72 6564  lized and stored
-00006e30: 2068 6572 652e 0a20 2020 2020 2020 2022   here..        "
-00006e40: 2222 0a20 2020 2064 6566 2073 6574 5f63  "".    def set_c
-00006e50: 6f6e 7465 7874 2873 656c 662c 2063 6f6e  ontext(self, con
-00006e60: 7465 7874 3a20 6279 7465 7329 202d 3e20  text: bytes) -> 
-00006e70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00006e80: 220a 2020 2020 2020 2020 6063 6f6e 7465  ".        `conte
-00006e90: 7874 603a 2049 6620 7468 6572 6520 6973  xt`: If there is
-00006ea0: 2063 6f6e 7465 7874 2061 7373 6f63 6961   context associa
-00006eb0: 7465 6420 7769 7468 2074 6865 2070 6565  ted with the pee
-00006ec0: 7220 286c 696b 6520 636f 6e6e 6563 7469  r (like connecti
-00006ed0: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 292c  on information),
-00006ee0: 2069 7420 6361 6e20 6265 0a20 2020 2020   it can be.     
-00006ef0: 2020 2073 6572 6961 6c69 7a65 6420 616e     serialized an
-00006f00: 6420 7374 6f72 6564 2068 6572 652e 0a20  d stored here.. 
-00006f10: 2020 2020 2020 2022 2222 0a0a 636c 6173         """..clas
-00006f20: 7320 5065 6572 285f 5f41 5049 5f50 6565  s Peer(__API_Pee
-00006f30: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
-00006f40: 5265 7072 6573 656e 7473 2061 2050 6565  Represents a Pee
-00006f50: 7220 6e6f 6465 2069 6e20 7468 6520 636c  r node in the cl
-00006f60: 7573 7465 722e 0a20 2020 2022 2222 0a0a  uster..    """..
-00006f70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00006f80: 2873 656c 6629 202d 3e20 4e6f 6e65 3a20  (self) -> None: 
-00006f90: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-00006fa0: 5f72 6566 2873 656c 6629 202d 3e20 2250  _ref(self) -> "P
-00006fb0: 6565 7252 6566 223a 202e 2e2e 0a0a 636c  eerRef": .....cl
-00006fc0: 6173 7320 5065 6572 5265 6628 5f5f 4150  ass PeerRef(__AP
-00006fd0: 495f 5065 6572 293a 0a20 2020 2022 2222  I_Peer):.    """
-00006fe0: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
-00006ff0: 7970 6520 6f66 203a 636c 6173 733a 6050  ype of :class:`P
-00007000: 6565 7260 2e0a 2020 2020 2222 220a 0a63  eer`..    """..c
-00007010: 6c61 7373 205f 5f41 5049 5f4c 6967 6874  lass __API_Light
-00007020: 5265 6164 793a 0a20 2020 2064 6566 2063  Ready:.    def c
-00007030: 6f6d 6d69 745f 696e 6465 7828 7365 6c66  ommit_index(self
-00007040: 2920 2d3e 204f 7074 696f 6e61 6c5b 696e  ) -> Optional[in
-00007050: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-00007060: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
-00007070: 656e 7420 636f 6d6d 6974 2069 6e64 6578  ent commit index
-00007080: 2e0a 2020 2020 2020 2020 4974 2077 696c  ..        It wil
-00007090: 6c20 6265 204e 6f6e 6520 7374 6174 6520  l be None state 
-000070a0: 6966 2074 6865 7265 2069 7320 6e6f 2075  if there is no u
-000070b0: 7064 6174 652e 0a20 2020 2020 2020 2049  pdate..        I
-000070c0: 7420 6973 206e 6f74 2072 6571 7569 7265  t is not require
-000070d0: 6420 746f 2073 6176 6520 6974 2074 6f20  d to save it to 
-000070e0: 7374 6162 6c65 2073 746f 7261 6765 2e0a  stable storage..
-000070f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007100: 6465 6620 636f 6d6d 6974 7465 645f 656e  def committed_en
-00007110: 7472 6965 7328 7365 6c66 2920 2d3e 204c  tries(self) -> L
-00007120: 6973 745b 2245 6e74 7279 5265 6622 5d3a  ist["EntryRef"]:
-00007130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007140: 2020 2020 2043 6f6d 6d69 7474 6564 456e       CommittedEn
-00007150: 7472 6965 7320 7370 6563 6966 6965 7320  tries specifies 
-00007160: 656e 7472 6965 7320 746f 2062 6520 636f  entries to be co
-00007170: 6d6d 6974 7465 6420 746f 2061 0a20 2020  mmitted to a.   
-00007180: 2020 2020 2073 746f 7265 2f73 7461 7465       store/state
-00007190: 2d6d 6163 6869 6e65 2e20 5468 6573 6520  -machine. These 
-000071a0: 6861 7665 2070 7265 7669 6f75 736c 7920  have previously 
-000071b0: 6265 656e 2063 6f6d 6d69 7474 6564 2074  been committed t
-000071c0: 6f20 7374 6162 6c65 0a20 2020 2020 2020  o stable.       
-000071d0: 2073 746f 7265 2e0a 2020 2020 2020 2020   store..        
-000071e0: 2222 220a 2020 2020 6465 6620 7461 6b65  """.    def take
-000071f0: 5f63 6f6d 6d69 7474 6564 5f65 6e74 7269  _committed_entri
-00007200: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
-00007210: 5b22 456e 7472 7922 5d3a 0a20 2020 2020  ["Entry"]:.     
-00007220: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-00007230: 616b 6520 7468 6520 436f 6d6d 6974 456e  ake the CommitEn
-00007240: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
-00007250: 2222 0a20 2020 2064 6566 206d 6573 7361  "".    def messa
-00007260: 6765 7328 7365 6c66 2920 2d3e 204c 6973  ges(self) -> Lis
-00007270: 745b 224d 6573 7361 6765 5265 6622 5d3a  t["MessageRef"]:
-00007280: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007290: 2020 2020 204d 6573 7361 6765 7320 7370       Messages sp
-000072a0: 6563 6966 6965 7320 6f75 7462 6f75 6e64  ecifies outbound
-000072b0: 206d 6573 7361 6765 7320 746f 2062 6520   messages to be 
-000072c0: 7365 6e74 2e0a 2020 2020 2020 2020 2222  sent..        ""
-000072d0: 220a 2020 2020 6465 6620 7461 6b65 5f6d  ".    def take_m
-000072e0: 6573 7361 6765 7328 7365 6c66 2920 2d3e  essages(self) ->
-000072f0: 204c 6973 745b 224d 6573 7361 6765 225d   List["Message"]
-00007300: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007310: 2020 2020 2020 5461 6b65 2074 6865 204d        Take the M
-00007320: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
-00007330: 2022 2222 0a0a 636c 6173 7320 4c69 6768   """..class Ligh
-00007340: 7452 6561 6479 285f 5f41 5049 5f4c 6967  tReady(__API_Lig
-00007350: 6874 5265 6164 7929 3a0a 2020 2020 2222  htReady):.    ""
-00007360: 220a 2020 2020 4c69 6768 7452 6561 6479  ".    LightReady
-00007370: 2065 6e63 6170 7375 6c61 7465 7320 7468   encapsulates th
-00007380: 6520 636f 6d6d 6974 2069 6e64 6578 2c20  e commit index, 
-00007390: 636f 6d6d 6974 7465 6420 656e 7472 6965  committed entrie
-000073a0: 7320 616e 640a 2020 2020 6d65 7373 6167  s and.    messag
-000073b0: 6573 2074 6861 7420 6172 6520 7265 6164  es that are read
-000073c0: 7920 746f 2062 6520 6170 706c 6965 6420  y to be applied 
-000073d0: 6f72 2062 6520 7365 6e74 2074 6f20 6f74  or be sent to ot
-000073e0: 6865 7220 7065 6572 732e 0a20 2020 2022  her peers..    "
-000073f0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-00007400: 6974 5f5f 2873 656c 6629 202d 3e20 4e6f  it__(self) -> No
-00007410: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00007420: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-00007430: 3e20 224c 6967 6874 5265 6164 7952 6566  > "LightReadyRef
-00007440: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
-00007450: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00007460: 2064 6566 6175 6c74 2829 202d 3e20 224c   default() -> "L
-00007470: 6967 6874 5265 6164 7922 3a20 2e2e 2e0a  ightReady": ....
-00007480: 0a63 6c61 7373 204c 6967 6874 5265 6164  .class LightRead
-00007490: 7952 6566 285f 5f41 5049 5f4c 6967 6874  yRef(__API_Light
-000074a0: 5265 6164 7929 3a0a 2020 2020 2222 220a  Ready):.    """.
-000074b0: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
-000074c0: 7065 206f 6620 3a63 6c61 7373 3a60 4c69  pe of :class:`Li
-000074d0: 6768 7452 6561 6479 602e 0a20 2020 2022  ghtReady`..    "
-000074e0: 2222 0a0a 636c 6173 7320 5f5f 4150 495f  ""..class __API_
-000074f0: 536e 6170 7368 6f74 4d65 7461 6461 7461  SnapshotMetadata
-00007500: 285f 5f43 6c6f 6e65 6162 6c65 2c20 5f5f  (__Cloneable, __
-00007510: 456e 636f 6465 722c 205f 5f44 6563 6f64  Encoder, __Decod
-00007520: 6572 293a 0a20 2020 2064 6566 2063 6c6f  er):.    def clo
-00007530: 6e65 2873 656c 6629 202d 3e20 2253 6e61  ne(self) -> "Sna
-00007540: 7073 686f 744d 6574 6164 6174 6122 3a20  pshotMetadata": 
-00007550: 2e2e 2e0a 2020 2020 6465 6620 6765 745f  ....    def get_
-00007560: 696e 6465 7828 7365 6c66 2920 2d3e 2069  index(self) -> i
-00007570: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-00007580: 2020 2020 2020 2020 6069 6e64 6578 603a          `index`:
-00007590: 2054 6865 2061 7070 6c69 6564 2069 6e64   The applied ind
-000075a0: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
-000075b0: 2020 2020 6465 6620 7365 745f 696e 6465      def set_inde
-000075c0: 7828 7365 6c66 2c20 696e 6465 783a 2069  x(self, index: i
-000075d0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000075e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000075f0: 2060 696e 6465 7860 3a20 5468 6520 6170   `index`: The ap
-00007600: 706c 6965 6420 696e 6465 782e 0a20 2020  plied index..   
-00007610: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00007620: 2063 6c65 6172 5f69 6e64 6578 2873 656c   clear_index(sel
-00007630: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00007640: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007650: 6069 6e64 6578 603a 2054 6865 2061 7070  `index`: The app
-00007660: 6c69 6564 2069 6e64 6578 2e0a 2020 2020  lied index..    
-00007670: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00007680: 6765 745f 7465 726d 2873 656c 6629 202d  get_term(self) -
-00007690: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-000076a0: 2222 0a20 2020 2020 2020 2060 7465 726d  "".        `term
-000076b0: 603a 2054 6865 2074 6572 6d20 6f66 2074  `: The term of t
-000076c0: 6865 2061 7070 6c69 6564 2069 6e64 6578  he applied index
-000076d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000076e0: 2020 6465 6620 7365 745f 7465 726d 2873    def set_term(s
-000076f0: 656c 662c 2074 6572 6d3a 2069 6e74 2920  elf, term: int) 
-00007700: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00007710: 2022 2222 0a20 2020 2020 2020 2060 7465   """.        `te
-00007720: 726d 603a 2054 6865 2074 6572 6d20 6f66  rm`: The term of
-00007730: 2074 6865 2061 7070 6c69 6564 2069 6e64   the applied ind
-00007740: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
-00007750: 2020 2020 6465 6620 636c 6561 725f 7465      def clear_te
-00007760: 726d 2873 656c 6629 202d 3e20 4e6f 6e65  rm(self) -> None
-00007770: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007780: 2020 2020 2020 6074 6572 6d60 3a20 5468        `term`: Th
-00007790: 6520 7465 726d 206f 6620 7468 6520 6170  e term of the ap
-000077a0: 706c 6965 6420 696e 6465 782e 0a20 2020  plied index..   
-000077b0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-000077c0: 2067 6574 5f63 6f6e 665f 7374 6174 6528   get_conf_state(
-000077d0: 7365 6c66 2920 2d3e 2022 436f 6e66 5374  self) -> "ConfSt
-000077e0: 6174 6552 6566 223a 0a20 2020 2020 2020  ateRef":.       
-000077f0: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
-00007800: 6e66 5f73 7461 7465 603a 2054 6865 2063  nf_state`: The c
-00007810: 7572 7265 6e74 2060 436f 6e66 5374 6174  urrent `ConfStat
-00007820: 6560 2e0a 2020 2020 2020 2020 2222 220a  e`..        """.
-00007830: 2020 2020 6465 6620 7365 745f 636f 6e66      def set_conf
-00007840: 5f73 7461 7465 2873 656c 662c 2063 6f6e  _state(self, con
-00007850: 665f 7374 6174 653a 2022 436f 6e66 5374  f_state: "ConfSt
-00007860: 6174 6522 207c 2022 436f 6e66 5374 6174  ate" | "ConfStat
-00007870: 6552 6566 2229 202d 3e20 4e6f 6e65 3a0a  eRef") -> None:.
-00007880: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007890: 2020 2020 6063 6f6e 665f 7374 6174 6560      `conf_state`
-000078a0: 3a20 5468 6520 6375 7272 656e 7420 6043  : The current `C
-000078b0: 6f6e 6653 7461 7465 602e 0a20 2020 2020  onfState`..     
-000078c0: 2020 2022 2222 0a20 2020 2064 6566 2063     """.    def c
-000078d0: 6c65 6172 5f63 6f6e 665f 7374 6174 6528  lear_conf_state(
-000078e0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-000078f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007900: 2020 2060 636f 6e66 5f73 7461 7465 603a     `conf_state`:
-00007910: 2054 6865 2063 7572 7265 6e74 2060 436f   The current `Co
-00007920: 6e66 5374 6174 6560 2e0a 2020 2020 2020  nfState`..      
-00007930: 2020 2222 220a 2020 2020 6465 6620 6861    """.    def ha
-00007940: 735f 636f 6e66 5f73 7461 7465 2873 656c  s_conf_state(sel
-00007950: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
-00007960: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007970: 6063 6f6e 665f 7374 6174 6560 3a20 5468  `conf_state`: Th
-00007980: 6520 6375 7272 656e 7420 6043 6f6e 6653  e current `ConfS
-00007990: 7461 7465 602e 0a20 2020 2020 2020 2022  tate`..        "
-000079a0: 2222 0a0a 636c 6173 7320 536e 6170 7368  ""..class Snapsh
-000079b0: 6f74 4d65 7461 6461 7461 285f 5f41 5049  otMetadata(__API
-000079c0: 5f53 6e61 7073 686f 744d 6574 6164 6174  _SnapshotMetadat
-000079d0: 6129 3a0a 2020 2020 2222 2220 2222 220a  a):.    """ """.
-000079e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000079f0: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00007a00: 202e 2e2e 0a20 2020 2040 7374 6174 6963   ....    @static
-00007a10: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-00007a20: 6566 6175 6c74 2829 202d 3e20 2253 6e61  efault() -> "Sna
-00007a30: 7073 686f 744d 6574 6164 6174 6122 3a20  pshotMetadata": 
-00007a40: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-00007a50: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
-00007a60: 636f 6465 2876 3a20 6279 7465 7329 202d  code(v: bytes) -
-00007a70: 3e20 2253 6e61 7073 686f 744d 6574 6164  > "SnapshotMetad
-00007a80: 6174 6122 3a20 2e2e 2e0a 2020 2020 6465  ata": ....    de
-00007a90: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
-00007aa0: 202d 3e20 2253 6e61 7073 686f 744d 6574   -> "SnapshotMet
-00007ab0: 6164 6174 6152 6566 223a 202e 2e2e 0a0a  adataRef": .....
-00007ac0: 636c 6173 7320 536e 6170 7368 6f74 4d65  class SnapshotMe
-00007ad0: 7461 6461 7461 5265 6628 5f5f 4150 495f  tadataRef(__API_
-00007ae0: 536e 6170 7368 6f74 4d65 7461 6461 7461  SnapshotMetadata
-00007af0: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
-00007b00: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
-00007b10: 203a 636c 6173 733a 6053 6e61 7073 686f   :class:`Snapsho
-00007b20: 744d 6574 6164 6174 6160 2e0a 2020 2020  tMetadata`..    
-00007b30: 2222 220a 0a63 6c61 7373 205f 5f41 5049  """..class __API
-00007b40: 5f53 6e61 7073 686f 7428 5f5f 436c 6f6e  _Snapshot(__Clon
-00007b50: 6561 626c 652c 205f 5f45 6e63 6f64 6572  eable, __Encoder
-00007b60: 2c20 5f5f 4465 636f 6465 7229 3a0a 2020  , __Decoder):.  
-00007b70: 2020 6465 6620 636c 6f6e 6528 7365 6c66    def clone(self
-00007b80: 2920 2d3e 2022 536e 6170 7368 6f74 223a  ) -> "Snapshot":
-00007b90: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
-00007ba0: 5f64 6174 6128 7365 6c66 2920 2d3e 2062  _data(self) -> b
-00007bb0: 7974 6573 3a0a 2020 2020 2020 2020 2222  ytes:.        ""
-00007bc0: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-00007bd0: 745f 6461 7461 2873 656c 662c 2064 6174  t_data(self, dat
-00007be0: 613a 2062 7974 6573 2920 2d3e 204e 6f6e  a: bytes) -> Non
-00007bf0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00007c00: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00007c10: 5f64 6174 6128 7365 6c66 2920 2d3e 204e  _data(self) -> N
-00007c20: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00007c30: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00007c40: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
-00007c50: 2d3e 2022 536e 6170 7368 6f74 4d65 7461  -> "SnapshotMeta
-00007c60: 6461 7461 5265 6622 3a0a 2020 2020 2020  dataRef":.      
-00007c70: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00007c80: 6620 7365 745f 6d65 7461 6461 7461 280a  f set_metadata(.
-00007c90: 2020 2020 2020 2020 7365 6c66 2c20 6d65          self, me
-00007ca0: 7461 5f64 6174 613a 2022 536e 6170 7368  ta_data: "Snapsh
-00007cb0: 6f74 4d65 7461 6461 7461 2220 7c20 2253  otMetadata" | "S
-00007cc0: 6e61 7073 686f 744d 6574 6164 6174 6152  napshotMetadataR
-00007cd0: 6566 220a 2020 2020 2920 2d3e 204e 6f6e  ef".    ) -> Non
-00007ce0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00007cf0: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00007d00: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
-00007d10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00007d20: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00007d30: 2068 6173 5f6d 6574 6164 6174 6128 7365   has_metadata(se
-00007d40: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00007d50: 2020 2020 2022 2222 2022 2222 0a0a 636c       """ """..cl
-00007d60: 6173 7320 536e 6170 7368 6f74 285f 5f41  ass Snapshot(__A
-00007d70: 5049 5f53 6e61 7073 686f 7429 3a0a 2020  PI_Snapshot):.  
-00007d80: 2020 2222 2220 2222 220a 0a20 2020 2064    """ """..    d
-00007d90: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00007da0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00007db0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00007dc0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
-00007dd0: 2829 202d 3e20 2253 6e61 7073 686f 7422  () -> "Snapshot"
-00007de0: 3a20 2e2e 2e0a 2020 2020 4073 7461 7469  : ....    @stati
-00007df0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-00007e00: 6465 636f 6465 2876 3a20 6279 7465 7329  decode(v: bytes)
-00007e10: 202d 3e20 2253 6e61 7073 686f 7422 3a20   -> "Snapshot": 
-00007e20: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-00007e30: 5f72 6566 2873 656c 6629 202d 3e20 2253  _ref(self) -> "S
-00007e40: 6e61 7073 686f 7452 6566 223a 202e 2e2e  napshotRef": ...
-00007e50: 0a0a 636c 6173 7320 536e 6170 7368 6f74  ..class Snapshot
-00007e60: 5265 6628 5f5f 4150 495f 536e 6170 7368  Ref(__API_Snapsh
-00007e70: 6f74 293a 0a20 2020 2022 2222 0a20 2020  ot):.    """.   
-00007e80: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-00007e90: 6f66 203a 636c 6173 733a 6053 6e61 7073  of :class:`Snaps
-00007ea0: 686f 7460 2e0a 2020 2020 2222 220a 0a63  hot`..    """..c
-00007eb0: 6c61 7373 205f 5f41 5049 5f4d 6573 7361  lass __API_Messa
-00007ec0: 6765 285f 5f43 6c6f 6e65 6162 6c65 2c20  ge(__Cloneable, 
-00007ed0: 5f5f 456e 636f 6465 722c 205f 5f44 6563  __Encoder, __Dec
-00007ee0: 6f64 6572 293a 0a20 2020 2064 6566 2063  oder):.    def c
-00007ef0: 6c6f 6e65 2873 656c 6629 202d 3e20 224d  lone(self) -> "M
-00007f00: 6573 7361 6765 223a 202e 2e2e 0a20 2020  essage": ....   
-00007f10: 2064 6566 2067 6574 5f63 6f6d 6d69 7428   def get_commit(
-00007f20: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-00007f30: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-00007f40: 2020 6465 6620 7365 745f 636f 6d6d 6974    def set_commit
-00007f50: 2873 656c 662c 2063 6f6d 6d69 743a 2069  (self, commit: i
-00007f60: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00007f70: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00007f80: 2064 6566 2063 6c65 6172 5f63 6f6d 6d69   def clear_commi
-00007f90: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-00007fa0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00007fb0: 0a20 2020 2064 6566 2067 6574 5f63 6f6d  .    def get_com
-00007fc0: 6d69 745f 7465 726d 2873 656c 6629 202d  mit_term(self) -
-00007fd0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-00007fe0: 2222 2022 2222 0a20 2020 2064 6566 2073  "" """.    def s
-00007ff0: 6574 5f63 6f6d 6d69 745f 7465 726d 2873  et_commit_term(s
-00008000: 656c 662c 2063 6f6d 6d69 745f 7465 726d  elf, commit_term
-00008010: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00008020: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00008030: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
-00008040: 6d6d 6974 5f74 6572 6d28 7365 6c66 2920  mmit_term(self) 
-00008050: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00008060: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00008070: 2067 6574 5f66 726f 6d28 7365 6c66 2920   get_from(self) 
-00008080: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00008090: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-000080a0: 7365 745f 6672 6f6d 2873 656c 662c 2066  set_from(self, f
-000080b0: 726f 6d5f 3a20 696e 7429 202d 3e20 4e6f  rom_: int) -> No
-000080c0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-000080d0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-000080e0: 725f 6672 6f6d 2873 656c 6629 202d 3e20  r_from(self) -> 
-000080f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00008100: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-00008110: 745f 696e 6465 7828 7365 6c66 2920 2d3e  t_index(self) ->
-00008120: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00008130: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-00008140: 745f 696e 6465 7828 7365 6c66 2c20 696e  t_index(self, in
-00008150: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
-00008160: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00008170: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00008180: 5f69 6e64 6578 2873 656c 6629 202d 3e20  _index(self) -> 
-00008190: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000081a0: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-000081b0: 745f 7465 726d 2873 656c 6629 202d 3e20  t_term(self) -> 
-000081c0: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-000081d0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-000081e0: 5f74 6572 6d28 7365 6c66 2c20 7465 726d  _term(self, term
-000081f0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00008200: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00008210: 2020 2020 6465 6620 636c 6561 725f 7465      def clear_te
-00008220: 726d 2873 656c 6629 202d 3e20 4e6f 6e65  rm(self) -> None
-00008230: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00008240: 220a 2020 2020 6465 6620 6765 745f 6c6f  ".    def get_lo
-00008250: 675f 7465 726d 2873 656c 6629 202d 3e20  g_term(self) -> 
-00008260: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00008270: 0a20 2020 2020 2020 2060 6c6f 6754 6572  .        `logTer
-00008280: 6d60 3a20 6c6f 6754 6572 6d20 6973 2067  m`: logTerm is g
-00008290: 656e 6572 616c 6c79 2075 7365 6420 666f  enerally used fo
-000082a0: 7220 6170 7065 6e64 696e 6720 5261 6674  r appending Raft
-000082b0: 206c 6f67 7320 746f 2066 6f6c 6c6f 7765   logs to followe
-000082c0: 7273 2e20 466f 7220 6578 616d 706c 652c  rs. For example,
-000082d0: 0a20 2020 2020 2020 2028 7479 7065 3d4d  .        (type=M
-000082e0: 7367 4170 7065 6e64 2c69 6e64 6578 3d31  sgAppend,index=1
-000082f0: 3030 2c6c 6f67 5f74 6572 6d3d 3529 206d  00,log_term=5) m
-00008300: 6561 6e73 206c 6561 6465 7220 6170 7065  eans leader appe
-00008310: 6e64 7320 656e 7472 6965 7320 7374 6172  nds entries star
-00008320: 7469 6e67 2061 740a 2020 2020 2020 2020  ting at.        
-00008330: 696e 6465 783d 3130 312c 2061 6e64 2074  index=101, and t
-00008340: 6865 2074 6572 6d20 6f66 2065 6e74 7279  he term of entry
-00008350: 2061 7420 696e 6465 7820 3130 3020 6973   at index 100 is
-00008360: 2035 2e0a 2020 2020 2020 2020 2874 7970   5..        (typ
-00008370: 653d 4d73 6741 7070 656e 6452 6573 706f  e=MsgAppendRespo
-00008380: 6e73 652c 7265 6a65 6374 3d74 7275 652c  nse,reject=true,
-00008390: 696e 6465 783d 3130 302c 6c6f 675f 7465  index=100,log_te
-000083a0: 726d 3d35 2920 6d65 616e 7320 666f 6c6c  rm=5) means foll
-000083b0: 6f77 6572 2072 656a 6563 7473 2073 6f6d  ower rejects som
-000083c0: 650a 2020 2020 2020 2020 656e 7472 6965  e.        entrie
-000083d0: 7320 6672 6f6d 2069 7473 206c 6561 6465  s from its leade
-000083e0: 7220 6173 2069 7420 616c 7265 6164 7920  r as it already 
-000083f0: 6861 7320 616e 2065 6e74 7279 2077 6974  has an entry wit
-00008400: 6820 7465 726d 2035 2061 7420 696e 6465  h term 5 at inde
-00008410: 7820 3130 302e 0a20 2020 2020 2020 2022  x 100..        "
-00008420: 2222 0a20 2020 2064 6566 2073 6574 5f6c  "".    def set_l
-00008430: 6f67 5f74 6572 6d28 7365 6c66 2c20 6c6f  og_term(self, lo
-00008440: 675f 696e 6465 783a 2069 6e74 2920 2d3e  g_index: int) ->
-00008450: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00008460: 2222 0a20 2020 2020 2020 2060 6c6f 6754  "".        `logT
-00008470: 6572 6d60 3a20 6c6f 6754 6572 6d20 6973  erm`: logTerm is
-00008480: 2067 656e 6572 616c 6c79 2075 7365 6420   generally used 
-00008490: 666f 7220 6170 7065 6e64 696e 6720 5261  for appending Ra
-000084a0: 6674 206c 6f67 7320 746f 2066 6f6c 6c6f  ft logs to follo
-000084b0: 7765 7273 2e20 466f 7220 6578 616d 706c  wers. For exampl
-000084c0: 652c 0a20 2020 2020 2020 2028 7479 7065  e,.        (type
-000084d0: 3d4d 7367 4170 7065 6e64 2c69 6e64 6578  =MsgAppend,index
-000084e0: 3d31 3030 2c6c 6f67 5f74 6572 6d3d 3529  =100,log_term=5)
-000084f0: 206d 6561 6e73 206c 6561 6465 7220 6170   means leader ap
-00008500: 7065 6e64 7320 656e 7472 6965 7320 7374  pends entries st
-00008510: 6172 7469 6e67 2061 740a 2020 2020 2020  arting at.      
-00008520: 2020 696e 6465 783d 3130 312c 2061 6e64    index=101, and
-00008530: 2074 6865 2074 6572 6d20 6f66 2065 6e74   the term of ent
-00008540: 7279 2061 7420 696e 6465 7820 3130 3020  ry at index 100 
-00008550: 6973 2035 2e0a 2020 2020 2020 2020 2874  is 5..        (t
-00008560: 7970 653d 4d73 6741 7070 656e 6452 6573  ype=MsgAppendRes
-00008570: 706f 6e73 652c 7265 6a65 6374 3d74 7275  ponse,reject=tru
-00008580: 652c 696e 6465 783d 3130 302c 6c6f 675f  e,index=100,log_
-00008590: 7465 726d 3d35 2920 6d65 616e 7320 666f  term=5) means fo
-000085a0: 6c6c 6f77 6572 2072 656a 6563 7473 2073  llower rejects s
-000085b0: 6f6d 650a 2020 2020 2020 2020 656e 7472  ome.        entr
-000085c0: 6965 7320 6672 6f6d 2069 7473 206c 6561  ies from its lea
-000085d0: 6465 7220 6173 2069 7420 616c 7265 6164  der as it alread
-000085e0: 7920 6861 7320 616e 2065 6e74 7279 2077  y has an entry w
-000085f0: 6974 6820 7465 726d 2035 2061 7420 696e  ith term 5 at in
-00008600: 6465 7820 3130 302e 0a20 2020 2020 2020  dex 100..       
-00008610: 2022 2222 0a20 2020 2064 6566 2063 6c65   """.    def cle
-00008620: 6172 5f6c 6f67 5f74 6572 6d28 7365 6c66  ar_log_term(self
-00008630: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00008640: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00008650: 6c6f 6754 6572 6d60 3a20 6c6f 6754 6572  logTerm`: logTer
-00008660: 6d20 6973 2067 656e 6572 616c 6c79 2075  m is generally u
-00008670: 7365 6420 666f 7220 6170 7065 6e64 696e  sed for appendin
-00008680: 6720 5261 6674 206c 6f67 7320 746f 2066  g Raft logs to f
-00008690: 6f6c 6c6f 7765 7273 2e20 466f 7220 6578  ollowers. For ex
-000086a0: 616d 706c 652c 0a20 2020 2020 2020 2028  ample,.        (
-000086b0: 7479 7065 3d4d 7367 4170 7065 6e64 2c69  type=MsgAppend,i
-000086c0: 6e64 6578 3d31 3030 2c6c 6f67 5f74 6572  ndex=100,log_ter
-000086d0: 6d3d 3529 206d 6561 6e73 206c 6561 6465  m=5) means leade
-000086e0: 7220 6170 7065 6e64 7320 656e 7472 6965  r appends entrie
-000086f0: 7320 7374 6172 7469 6e67 2061 740a 2020  s starting at.  
-00008700: 2020 2020 2020 696e 6465 783d 3130 312c        index=101,
-00008710: 2061 6e64 2074 6865 2074 6572 6d20 6f66   and the term of
-00008720: 2065 6e74 7279 2061 7420 696e 6465 7820   entry at index 
-00008730: 3130 3020 6973 2035 2e0a 2020 2020 2020  100 is 5..      
-00008740: 2020 2874 7970 653d 4d73 6741 7070 656e    (type=MsgAppen
-00008750: 6452 6573 706f 6e73 652c 7265 6a65 6374  dResponse,reject
-00008760: 3d74 7275 652c 696e 6465 783d 3130 302c  =true,index=100,
-00008770: 6c6f 675f 7465 726d 3d35 2920 6d65 616e  log_term=5) mean
-00008780: 7320 666f 6c6c 6f77 6572 2072 656a 6563  s follower rejec
-00008790: 7473 2073 6f6d 650a 2020 2020 2020 2020  ts some.        
-000087a0: 656e 7472 6965 7320 6672 6f6d 2069 7473  entries from its
-000087b0: 206c 6561 6465 7220 6173 2069 7420 616c   leader as it al
-000087c0: 7265 6164 7920 6861 7320 616e 2065 6e74  ready has an ent
-000087d0: 7279 2077 6974 6820 7465 726d 2035 2061  ry with term 5 a
-000087e0: 7420 696e 6465 7820 3130 302e 0a20 2020  t index 100..   
-000087f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00008800: 2067 6574 5f70 7269 6f72 6974 7928 7365   get_priority(se
-00008810: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00008820: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008830: 6070 7269 6f72 6974 7960 3a20 4966 2074  `priority`: If t
-00008840: 6869 7320 6e65 7720 6669 656c 6420 6973  his new field is
-00008850: 206e 6f74 2073 6574 2c20 7468 656e 2075   not set, then u
-00008860: 7365 2074 6865 2061 626f 7665 206f 6c64  se the above old
-00008870: 2066 6965 6c64 3b20 6f74 6865 7277 6973   field; otherwis
-00008880: 650a 2020 2020 2020 2020 7573 6520 7468  e.        use th
-00008890: 6520 6e65 7720 6669 656c 642e 2057 6865  e new field. Whe
-000088a0: 6e20 6272 6f61 6463 6173 7469 6e67 2072  n broadcasting r
-000088b0: 6571 7565 7374 2076 6f74 652c 2062 6f74  equest vote, bot
-000088c0: 6820 6669 656c 6473 2061 7265 0a20 2020  h fields are.   
-000088d0: 2020 2020 2073 6574 2069 6620 7468 6520       set if the 
-000088e0: 7072 696f 7269 7479 2069 7320 6c61 7267  priority is larg
-000088f0: 6572 2074 6861 6e20 302e 2054 6869 7320  er than 0. This 
-00008900: 6368 616e 6765 2069 7320 6e6f 7420 6120  change is not a 
-00008910: 6675 6c6c 790a 2020 2020 2020 2020 636f  fully.        co
-00008920: 6d70 6174 6962 6c65 2063 6861 6e67 652c  mpatible change,
-00008930: 2062 7574 2069 7420 6d61 6b65 7320 6d69   but it makes mi
-00008940: 6e69 6d61 6c20 696d 7061 6374 2074 6861  nimal impact tha
-00008950: 7420 6f6e 6c79 206e 6577 2070 7269 6f72  t only new prior
-00008960: 6974 790a 2020 2020 2020 2020 6973 206e  ity.        is n
-00008970: 6f74 2072 6563 6f67 6e69 7a65 6420 6279  ot recognized by
-00008980: 2074 6865 206f 6c64 206e 6f64 6573 2064   the old nodes d
-00008990: 7572 696e 6720 726f 6c6c 696e 6720 7570  uring rolling up
-000089a0: 6461 7465 2e0a 2020 2020 2020 2020 2222  date..        ""
-000089b0: 220a 2020 2020 6465 6620 7365 745f 7072  ".    def set_pr
-000089c0: 696f 7269 7479 2873 656c 662c 2070 7269  iority(self, pri
-000089d0: 6f72 6974 793a 2069 6e74 2920 2d3e 204e  ority: int) -> N
-000089e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000089f0: 0a20 2020 2020 2020 2060 7072 696f 7269  .        `priori
-00008a00: 7479 603a 2049 6620 7468 6973 206e 6577  ty`: If this new
-00008a10: 2066 6965 6c64 2069 7320 6e6f 7420 7365   field is not se
-00008a20: 742c 2074 6865 6e20 7573 6520 7468 6520  t, then use the 
-00008a30: 6162 6f76 6520 6f6c 6420 6669 656c 643b  above old field;
-00008a40: 206f 7468 6572 7769 7365 0a20 2020 2020   otherwise.     
-00008a50: 2020 2075 7365 2074 6865 206e 6577 2066     use the new f
-00008a60: 6965 6c64 2e20 5768 656e 2062 726f 6164  ield. When broad
-00008a70: 6361 7374 696e 6720 7265 7175 6573 7420  casting request 
-00008a80: 766f 7465 2c20 626f 7468 2066 6965 6c64  vote, both field
-00008a90: 7320 6172 650a 2020 2020 2020 2020 7365  s are.        se
-00008aa0: 7420 6966 2074 6865 2070 7269 6f72 6974  t if the priorit
-00008ab0: 7920 6973 206c 6172 6765 7220 7468 616e  y is larger than
-00008ac0: 2030 2e20 5468 6973 2063 6861 6e67 6520   0. This change 
-00008ad0: 6973 206e 6f74 2061 2066 756c 6c79 0a20  is not a fully. 
-00008ae0: 2020 2020 2020 2063 6f6d 7061 7469 626c         compatibl
-00008af0: 6520 6368 616e 6765 2c20 6275 7420 6974  e change, but it
-00008b00: 206d 616b 6573 206d 696e 696d 616c 2069   makes minimal i
-00008b10: 6d70 6163 7420 7468 6174 206f 6e6c 7920  mpact that only 
-00008b20: 6e65 7720 7072 696f 7269 7479 0a20 2020  new priority.   
-00008b30: 2020 2020 2069 7320 6e6f 7420 7265 636f       is not reco
-00008b40: 676e 697a 6564 2062 7920 7468 6520 6f6c  gnized by the ol
-00008b50: 6420 6e6f 6465 7320 6475 7269 6e67 2072  d nodes during r
-00008b60: 6f6c 6c69 6e67 2075 7064 6174 652e 0a20  olling update.. 
-00008b70: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00008b80: 6566 2063 6c65 6172 5f70 7269 6f72 6974  ef clear_priorit
-00008b90: 7928 7365 6c66 2920 2d3e 204e 6f6e 653a  y(self) -> None:
-00008ba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008bb0: 2020 2020 2060 7072 696f 7269 7479 603a       `priority`:
-00008bc0: 2049 6620 7468 6973 206e 6577 2066 6965   If this new fie
-00008bd0: 6c64 2069 7320 6e6f 7420 7365 742c 2074  ld is not set, t
-00008be0: 6865 6e20 7573 6520 7468 6520 6162 6f76  hen use the abov
-00008bf0: 6520 6f6c 6420 6669 656c 643b 206f 7468  e old field; oth
-00008c00: 6572 7769 7365 0a20 2020 2020 2020 2075  erwise.        u
-00008c10: 7365 2074 6865 206e 6577 2066 6965 6c64  se the new field
-00008c20: 2e20 5768 656e 2062 726f 6164 6361 7374  . When broadcast
-00008c30: 696e 6720 7265 7175 6573 7420 766f 7465  ing request vote
-00008c40: 2c20 626f 7468 2066 6965 6c64 7320 6172  , both fields ar
-00008c50: 650a 2020 2020 2020 2020 7365 7420 6966  e.        set if
-00008c60: 2074 6865 2070 7269 6f72 6974 7920 6973   the priority is
-00008c70: 206c 6172 6765 7220 7468 616e 2030 2e20   larger than 0. 
-00008c80: 5468 6973 2063 6861 6e67 6520 6973 206e  This change is n
-00008c90: 6f74 2061 2066 756c 6c79 0a20 2020 2020  ot a fully.     
-00008ca0: 2020 2063 6f6d 7061 7469 626c 6520 6368     compatible ch
-00008cb0: 616e 6765 2c20 6275 7420 6974 206d 616b  ange, but it mak
-00008cc0: 6573 206d 696e 696d 616c 2069 6d70 6163  es minimal impac
-00008cd0: 7420 7468 6174 206f 6e6c 7920 6e65 7720  t that only new 
-00008ce0: 7072 696f 7269 7479 0a20 2020 2020 2020  priority.       
-00008cf0: 2069 7320 6e6f 7420 7265 636f 676e 697a   is not recogniz
-00008d00: 6564 2062 7920 7468 6520 6f6c 6420 6e6f  ed by the old no
-00008d10: 6465 7320 6475 7269 6e67 2072 6f6c 6c69  des during rolli
-00008d20: 6e67 2075 7064 6174 652e 0a20 2020 2020  ng update..     
-00008d30: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-00008d40: 6574 5f63 6f6e 7465 7874 2873 656c 6629  et_context(self)
-00008d50: 202d 3e20 6279 7465 733a 0a20 2020 2020   -> bytes:.     
-00008d60: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00008d70: 6566 2073 6574 5f63 6f6e 7465 7874 2873  ef set_context(s
-00008d80: 656c 662c 2063 6f6e 7465 7874 3a20 6279  elf, context: by
-00008d90: 7465 7329 202d 3e20 4e6f 6e65 3a0a 2020  tes) -> None:.  
-00008da0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-00008db0: 2020 6465 6620 636c 6561 725f 636f 6e74    def clear_cont
-00008dc0: 6578 7428 7365 6c66 2920 2d3e 204e 6f6e  ext(self) -> Non
-00008dd0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00008de0: 2222 0a20 2020 2064 6566 2067 6574 5f72  "".    def get_r
-00008df0: 656a 6563 745f 6869 6e74 2873 656c 6629  eject_hint(self)
-00008e00: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00008e10: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00008e20: 2073 6574 5f72 656a 6563 745f 6869 6e74   set_reject_hint
-00008e30: 2873 656c 662c 2072 656a 6563 745f 6869  (self, reject_hi
-00008e40: 6e74 3a20 626f 6f6c 2920 2d3e 204e 6f6e  nt: bool) -> Non
-00008e50: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00008e60: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00008e70: 5f72 656a 6563 745f 6869 6e74 2873 656c  _reject_hint(sel
-00008e80: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00008e90: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-00008ea0: 6465 6620 6765 745f 656e 7472 6965 7328  def get_entries(
-00008eb0: 7365 6c66 2920 2d3e 204c 6973 745b 2245  self) -> List["E
-00008ec0: 6e74 7279 5265 6622 5d3a 0a20 2020 2020  ntryRef"]:.     
-00008ed0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00008ee0: 6566 2073 6574 5f65 6e74 7269 6573 2873  ef set_entries(s
-00008ef0: 656c 662c 2065 6e74 733a 204c 6973 745b  elf, ents: List[
-00008f00: 2245 6e74 7279 225d 207c 204c 6973 745b  "Entry"] | List[
-00008f10: 2245 6e74 7279 5265 6622 5d29 202d 3e20  "EntryRef"]) -> 
-00008f20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00008f30: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
-00008f40: 6561 725f 656e 7472 6965 7328 7365 6c66  ear_entries(self
-00008f50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00008f60: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00008f70: 6566 2067 6574 5f6d 7367 5f74 7970 6528  ef get_msg_type(
-00008f80: 7365 6c66 2920 2d3e 2022 4d65 7373 6167  self) -> "Messag
-00008f90: 6554 7970 6522 3a0a 2020 2020 2020 2020  eType":.        
-00008fa0: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-00008fb0: 7365 745f 6d73 675f 7479 7065 2873 656c  set_msg_type(sel
-00008fc0: 662c 2074 7970 3a20 224d 6573 7361 6765  f, typ: "Message
-00008fd0: 5479 7065 2229 202d 3e20 4e6f 6e65 3a0a  Type") -> None:.
-00008fe0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00008ff0: 2020 2020 6465 6620 636c 6561 725f 6d73      def clear_ms
-00009000: 675f 7479 7065 2873 656c 6629 202d 3e20  g_type(self) -> 
-00009010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00009020: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-00009030: 745f 7265 6a65 6374 2873 656c 6629 202d  t_reject(self) -
-00009040: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00009050: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-00009060: 7365 745f 7265 6a65 6374 2873 656c 662c  set_reject(self,
-00009070: 2072 656a 6563 743a 2062 6f6f 6c29 202d   reject: bool) -
-00009080: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00009090: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-000090a0: 636c 6561 725f 7265 6a65 6374 2873 656c  clear_reject(sel
-000090b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-000090c0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-000090d0: 6465 6620 6765 745f 736e 6170 7368 6f74  def get_snapshot
-000090e0: 2873 656c 6629 202d 3e20 2253 6e61 7073  (self) -> "Snaps
-000090f0: 686f 7452 6566 223a 0a20 2020 2020 2020  hotRef":.       
-00009100: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00009110: 2073 6574 5f73 6e61 7073 686f 7428 7365   set_snapshot(se
-00009120: 6c66 2c20 736e 6170 7368 6f74 3a20 2253  lf, snapshot: "S
-00009130: 6e61 7073 686f 7422 207c 2022 536e 6170  napshot" | "Snap
-00009140: 7368 6f74 5265 6622 2920 2d3e 204e 6f6e  shotRef") -> Non
-00009150: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00009160: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00009170: 5f73 6e61 7073 686f 7428 7365 6c66 2920  _snapshot(self) 
-00009180: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00009190: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-000091a0: 2067 6574 5f74 6f28 7365 6c66 2920 2d3e   get_to(self) ->
-000091b0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-000091c0: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-000091d0: 745f 746f 2873 656c 662c 2074 6f3a 2069  t_to(self, to: i
-000091e0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000091f0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009200: 2064 6566 2063 6c65 6172 5f74 6f28 7365   def clear_to(se
-00009210: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00009220: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009230: 2064 6566 2067 6574 5f72 6571 7565 7374   def get_request
-00009240: 5f73 6e61 7073 686f 7428 7365 6c66 2920  _snapshot(self) 
-00009250: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00009260: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-00009270: 7365 745f 7265 7175 6573 745f 736e 6170  set_request_snap
-00009280: 7368 6f74 2873 656c 662c 2072 6571 7565  shot(self, reque
-00009290: 7374 5f73 6e61 7073 686f 743a 2069 6e74  st_snapshot: int
-000092a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000092b0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-000092c0: 6566 2063 6c65 6172 5f72 6571 7565 7374  ef clear_request
-000092d0: 5f73 6e61 7073 686f 7428 7365 6c66 2920  _snapshot(self) 
-000092e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000092f0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00009300: 2068 6173 5f73 6e61 7073 686f 7428 7365   has_snapshot(se
-00009310: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00009320: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009330: 2064 6566 2063 6f6d 7075 7465 5f73 697a   def compute_siz
-00009340: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0a  e(self) -> int:.
-00009350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009360: 2020 2020 436f 6d70 7574 6520 616e 6420      Compute and 
-00009370: 6361 6368 6520 7369 7a65 206f 6620 7468  cache size of th
-00009380: 6973 206d 6573 7361 6765 2061 6e64 2061  is message and a
-00009390: 6c6c 206e 6573 7465 6420 6d65 7373 6167  ll nested messag
-000093a0: 6573 0a20 2020 2020 2020 2022 2222 0a0a  es.        """..
-000093b0: 636c 6173 7320 4d65 7373 6167 6528 5f5f  class Message(__
-000093c0: 4150 495f 4d65 7373 6167 6529 3a0a 2020  API_Message):.  
-000093d0: 2020 2222 2220 2222 220a 0a20 2020 2064    """ """..    d
-000093e0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000093f0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00009400: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
-00009410: 7365 6c66 2920 2d3e 2022 4d65 7373 6167  self) -> "Messag
-00009420: 6552 6566 223a 202e 2e2e 0a20 2020 2040  eRef": ....    @
-00009430: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-00009440: 2064 6566 2064 6566 6175 6c74 2829 202d   def default() -
-00009450: 3e20 224d 6573 7361 6765 223a 202e 2e2e  > "Message": ...
-00009460: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00009470: 6f64 0a20 2020 2064 6566 2064 6563 6f64  od.    def decod
-00009480: 6528 763a 2062 7974 6573 2920 2d3e 2022  e(v: bytes) -> "
-00009490: 4d65 7373 6167 6522 3a20 2e2e 2e0a 0a63  Message": .....c
-000094a0: 6c61 7373 204d 6573 7361 6765 5265 6628  lass MessageRef(
-000094b0: 4d65 7373 6167 6529 3a0a 2020 2020 2222  Message):.    ""
-000094c0: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
-000094d0: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
-000094e0: 4d65 7373 6167 6560 2e0a 2020 2020 2222  Message`..    ""
-000094f0: 220a 0a63 6c61 7373 205f 5f41 5049 5f48  "..class __API_H
-00009500: 6172 6453 7461 7465 285f 5f43 6c6f 6e65  ardState(__Clone
-00009510: 6162 6c65 2c20 5f5f 456e 636f 6465 722c  able, __Encoder,
-00009520: 205f 5f44 6563 6f64 6572 293a 0a20 2020   __Decoder):.   
-00009530: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
-00009540: 202d 3e20 2248 6172 6453 7461 7465 223a   -> "HardState":
-00009550: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
-00009560: 5f74 6572 6d28 7365 6c66 2920 2d3e 2069  _term(self) -> i
-00009570: 6e74 3a0a 2020 2020 2020 2020 2222 2220  nt:.        """ 
-00009580: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00009590: 7465 726d 2873 656c 662c 2074 6572 6d3a  term(self, term:
-000095a0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-000095b0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-000095c0: 2020 2064 6566 2063 6c65 6172 5f74 6572     def clear_ter
-000095d0: 6d28 7365 6c66 2920 2d3e 204e 6f6e 653a  m(self) -> None:
-000095e0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-000095f0: 0a20 2020 2064 6566 2067 6574 5f76 6f74  .    def get_vot
-00009600: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0a  e(self) -> int:.
-00009610: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00009620: 2020 2020 6465 6620 7365 745f 766f 7465      def set_vote
-00009630: 2873 656c 662c 2076 6f74 653a 2069 6e74  (self, vote: int
-00009640: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00009650: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00009660: 6566 2063 6c65 6172 5f76 6f74 6528 7365  ef clear_vote(se
-00009670: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00009680: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009690: 2064 6566 2067 6574 5f63 6f6d 6d69 7428   def get_commit(
-000096a0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-000096b0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-000096c0: 2020 6465 6620 7365 745f 636f 6d6d 6974    def set_commit
-000096d0: 2873 656c 662c 2063 6f6d 6d69 743a 2069  (self, commit: i
-000096e0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000096f0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009700: 2064 6566 2063 6c65 6172 5f63 6f6d 6d69   def clear_commi
-00009710: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-00009720: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00009730: 0a0a 636c 6173 7320 4861 7264 5374 6174  ..class HardStat
-00009740: 6528 5f5f 4150 495f 4861 7264 5374 6174  e(__API_HardStat
-00009750: 6529 3a0a 2020 2020 2222 2220 2222 220a  e):.    """ """.
-00009760: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00009770: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00009780: 202e 2e2e 0a20 2020 2064 6566 206d 616b   ....    def mak
-00009790: 655f 7265 6628 7365 6c66 2920 2d3e 2022  e_ref(self) -> "
-000097a0: 4861 7264 5374 6174 6552 6566 223a 202e  HardStateRef": .
-000097b0: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-000097c0: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
-000097d0: 6175 6c74 2829 202d 3e20 2248 6172 6453  ault() -> "HardS
-000097e0: 7461 7465 223a 202e 2e2e 0a20 2020 2040  tate": ....    @
-000097f0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-00009800: 2064 6566 2064 6563 6f64 6528 763a 2062   def decode(v: b
-00009810: 7974 6573 2920 2d3e 2022 4861 7264 5374  ytes) -> "HardSt
-00009820: 6174 6522 3a20 2e2e 2e0a 0a63 6c61 7373  ate": .....class
-00009830: 2048 6172 6453 7461 7465 5265 6628 5f5f   HardStateRef(__
-00009840: 4150 495f 4861 7264 5374 6174 6529 3a0a  API_HardState):.
-00009850: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
-00009860: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
-00009870: 6c61 7373 3a60 4861 7264 5374 6174 6560  lass:`HardState`
-00009880: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
-00009890: 205f 5f41 5049 5f47 6574 456e 7472 6965   __API_GetEntrie
-000098a0: 7343 6f6e 7465 7874 3a0a 2020 2020 6465  sContext:.    de
-000098b0: 6620 6361 6e5f 6173 796e 6328 7365 6c66  f can_async(self
-000098c0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-000098d0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-000098e0: 6865 636b 2069 6620 7468 6520 6361 6c6c  heck if the call
-000098f0: 6572 2773 2063 6f6e 7465 7874 2073 7570  er's context sup
-00009900: 706f 7274 2066 6574 6368 696e 6720 656e  port fetching en
-00009910: 7472 6965 7320 6173 796e 6368 726f 6e6f  tries asynchrono
-00009920: 7573 6c79 2e0a 2020 2020 2020 2020 2222  usly..        ""
-00009930: 220a 0a63 6c61 7373 2047 6574 456e 7472  "..class GetEntr
-00009940: 6965 7343 6f6e 7465 7874 285f 5f41 5049  iesContext(__API
-00009950: 5f47 6574 456e 7472 6965 7343 6f6e 7465  _GetEntriesConte
-00009960: 7874 293a 0a20 2020 2022 2222 0a20 2020  xt):.    """.   
-00009970: 2052 6563 6f72 6473 2074 6865 2063 6f6e   Records the con
-00009980: 7465 7874 206f 6620 7468 6520 6361 6c6c  text of the call
-00009990: 6572 2077 686f 2063 616c 6c73 2065 6e74  er who calls ent
-000099a0: 7269 6573 2829 206f 6620 5374 6f72 6167  ries() of Storag
-000099b0: 6520 7472 6169 742e 0a20 2020 2022 2222  e trait..    """
-000099c0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-000099d0: 686f 640a 2020 2020 6465 6620 656d 7074  hod.    def empt
-000099e0: 7928 6361 6e5f 6173 796e 633a 2062 6f6f  y(can_async: boo
-000099f0: 6c29 202d 3e20 2247 6574 456e 7472 6965  l) -> "GetEntrie
-00009a00: 7343 6f6e 7465 7874 223a 0a20 2020 2020  sContext":.     
-00009a10: 2020 2022 2222 0a20 2020 2020 2020 2055     """.        U
-00009a20: 7365 6420 666f 7220 6361 6c6c 6572 7320  sed for callers 
-00009a30: 6f75 7420 6f66 2072 6166 742e 2043 616c  out of raft. Cal
-00009a40: 6c65 7220 6361 6e20 6375 7374 6f6d 697a  ler can customiz
-00009a50: 6520 6966 2069 7420 7375 7070 6f72 7473  e if it supports
-00009a60: 2061 7379 6e63 2e0a 2020 2020 2020 2020   async..        
-00009a70: 2222 220a 2020 2020 6465 6620 6d61 6b65  """.    def make
-00009a80: 5f72 6566 2873 656c 6629 202d 3e20 2247  _ref(self) -> "G
-00009a90: 6574 456e 7472 6965 7343 6f6e 7465 7874  etEntriesContext
-00009aa0: 5265 6622 3a20 2e2e 2e0a 0a63 6c61 7373  Ref": .....class
-00009ab0: 2047 6574 456e 7472 6965 7343 6f6e 7465   GetEntriesConte
-00009ac0: 7874 5265 6628 5f5f 4150 495f 4765 7445  xtRef(__API_GetE
-00009ad0: 6e74 7269 6573 436f 6e74 6578 7429 3a0a  ntriesContext):.
-00009ae0: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
-00009af0: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
-00009b00: 6c61 7373 3a60 4765 7445 6e74 7269 6573  lass:`GetEntries
-00009b10: 436f 6e74 6578 7460 2e0a 2020 2020 2222  Context`..    ""
-00009b20: 220a 0a63 6c61 7373 205f 5f41 5049 5f45  "..class __API_E
-00009b30: 6e74 7279 285f 5f43 6c6f 6e65 6162 6c65  ntry(__Cloneable
-00009b40: 2c20 5f5f 456e 636f 6465 722c 205f 5f44  , __Encoder, __D
-00009b50: 6563 6f64 6572 293a 0a20 2020 2064 6566  ecoder):.    def
-00009b60: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
-00009b70: 2245 6e74 7279 223a 202e 2e2e 0a20 2020  "Entry": ....   
-00009b80: 2064 6566 2067 6574 5f63 6f6e 7465 7874   def get_context
-00009b90: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
-00009ba0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00009bb0: 0a20 2020 2064 6566 2073 6574 5f63 6f6e  .    def set_con
-00009bc0: 7465 7874 2873 656c 662c 2063 6f6e 7465  text(self, conte
-00009bd0: 7874 3a20 6279 7465 7329 202d 3e20 4e6f  xt: bytes) -> No
-00009be0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-00009bf0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-00009c00: 725f 636f 6e74 6578 7428 7365 6c66 2920  r_context(self) 
-00009c10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00009c20: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00009c30: 2067 6574 5f64 6174 6128 7365 6c66 2920   get_data(self) 
-00009c40: 2d3e 2062 7974 6573 3a0a 2020 2020 2020  -> bytes:.      
-00009c50: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00009c60: 6620 7365 745f 6461 7461 2873 656c 662c  f set_data(self,
-00009c70: 2064 6174 613a 2062 7974 6573 2920 2d3e   data: bytes) ->
-00009c80: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00009c90: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-00009ca0: 6c65 6172 5f64 6174 6128 7365 6c66 2920  lear_data(self) 
-00009cb0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00009cc0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00009cd0: 2067 6574 5f65 6e74 7279 5f74 7970 6528   get_entry_type(
-00009ce0: 7365 6c66 2920 2d3e 2022 456e 7472 7954  self) -> "EntryT
-00009cf0: 7970 6522 3a0a 2020 2020 2020 2020 2222  ype":.        ""
-00009d00: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-00009d10: 745f 656e 7472 795f 7479 7065 2873 656c  t_entry_type(sel
-00009d20: 662c 2074 7970 3a20 2245 6e74 7279 5479  f, typ: "EntryTy
-00009d30: 7065 2229 202d 3e20 4e6f 6e65 3a0a 2020  pe") -> None:.  
-00009d40: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-00009d50: 2020 6465 6620 636c 6561 725f 656e 7472    def clear_entr
-00009d60: 795f 7479 7065 2873 656c 6629 202d 3e20  y_type(self) -> 
-00009d70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00009d80: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-00009d90: 745f 7465 726d 2873 656c 6629 202d 3e20  t_term(self) -> 
-00009da0: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00009db0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00009dc0: 5f74 6572 6d28 7365 6c66 2c20 7465 726d  _term(self, term
-00009dd0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00009de0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00009df0: 2020 2020 6465 6620 636c 6561 725f 7465      def clear_te
-00009e00: 726d 2873 656c 6629 202d 3e20 4e6f 6e65  rm(self) -> None
-00009e10: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00009e20: 220a 2020 2020 6465 6620 6765 745f 696e  ".    def get_in
-00009e30: 6465 7828 7365 6c66 2920 2d3e 2069 6e74  dex(self) -> int
-00009e40: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00009e50: 220a 2020 2020 6465 6620 7365 745f 696e  ".    def set_in
-00009e60: 6465 7828 7365 6c66 2c20 696e 6465 783a  dex(self, index:
-00009e70: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-00009e80: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00009e90: 2020 2064 6566 2063 6c65 6172 5f69 6e64     def clear_ind
-00009ea0: 6578 2873 656c 6629 202d 3e20 4e6f 6e65  ex(self) -> None
-00009eb0: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00009ec0: 220a 2020 2020 6465 6620 6765 745f 7379  ".    def get_sy
-00009ed0: 6e63 5f6c 6f67 2873 656c 6629 202d 3e20  nc_log(self) -> 
-00009ee0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00009ef0: 220a 2020 2020 2020 2020 4465 7072 6563  ".        Deprec
-00009f00: 6174 6564 2120 4974 2069 7320 6b65 7074  ated! It is kept
-00009f10: 2066 6f72 2062 6163 6b77 6172 6420 636f   for backward co
-00009f20: 6d70 6174 6962 696c 6974 792e 0a20 2020  mpatibility..   
-00009f30: 2020 2020 2054 4f44 4f3a 2072 656d 6f76       TODO: remov
-00009f40: 6520 6974 2069 6e20 7468 6520 6e65 7874  e it in the next
-00009f50: 206d 616a 6f72 2072 656c 6561 7365 2e0a   major release..
-00009f60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009f70: 6465 6620 7365 745f 7379 6e63 5f6c 6f67  def set_sync_log
-00009f80: 2873 656c 662c 2073 796e 635f 6c6f 673a  (self, sync_log:
-00009f90: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
-00009fa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009fb0: 2020 2020 4465 7072 6563 6174 6564 2120      Deprecated! 
-00009fc0: 4974 2069 7320 6b65 7074 2066 6f72 2062  It is kept for b
-00009fd0: 6163 6b77 6172 6420 636f 6d70 6174 6962  ackward compatib
-00009fe0: 696c 6974 792e 0a20 2020 2020 2020 2054  ility..        T
-00009ff0: 4f44 4f3a 2072 656d 6f76 6520 6974 2069  ODO: remove it i
-0000a000: 6e20 7468 6520 6e65 7874 206d 616a 6f72  n the next major
-0000a010: 2072 656c 6561 7365 2e0a 2020 2020 2020   release..      
-0000a020: 2020 2222 220a 2020 2020 6465 6620 636c    """.    def cl
-0000a030: 6561 725f 7379 6e63 5f6c 6f67 2873 656c  ear_sync_log(sel
-0000a040: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000a050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a060: 4465 7072 6563 6174 6564 2120 4974 2069  Deprecated! It i
-0000a070: 7320 6b65 7074 2066 6f72 2062 6163 6b77  s kept for backw
-0000a080: 6172 6420 636f 6d70 6174 6962 696c 6974  ard compatibilit
-0000a090: 792e 0a20 2020 2020 2020 2054 4f44 4f3a  y..        TODO:
-0000a0a0: 2072 656d 6f76 6520 6974 2069 6e20 7468   remove it in th
-0000a0b0: 6520 6e65 7874 206d 616a 6f72 2072 656c  e next major rel
-0000a0c0: 6561 7365 2e0a 2020 2020 2020 2020 2222  ease..        ""
-0000a0d0: 220a 0a63 6c61 7373 2045 6e74 7279 285f  "..class Entry(_
-0000a0e0: 5f41 5049 5f45 6e74 7279 293a 0a20 2020  _API_Entry):.   
-0000a0f0: 2022 2222 0a20 2020 2054 6865 2065 6e74   """.    The ent
-0000a100: 7279 2069 7320 6120 7479 7065 206f 6620  ry is a type of 
-0000a110: 6368 616e 6765 2074 6861 7420 6e65 6564  change that need
-0000a120: 7320 746f 2062 6520 6170 706c 6965 642e  s to be applied.
-0000a130: 2049 7420 636f 6e74 6169 6e73 2074 776f   It contains two
-0000a140: 2064 6174 6120 6669 656c 6473 2e0a 2020   data fields..  
-0000a150: 2020 5768 696c 6520 7468 6520 6669 656c    While the fiel
-0000a160: 6473 2061 7265 2062 7569 6c74 2069 6e74  ds are built int
-0000a170: 6f20 7468 6520 6d6f 6465 6c3b 2074 6865  o the model; the
-0000a180: 6972 2075 7361 6765 2069 7320 6465 7465  ir usage is dete
-0000a190: 726d 696e 6564 2062 7920 7468 6520 656e  rmined by the en
-0000a1a0: 7472 795f 7479 7065 2e0a 0a20 2020 2046  try_type...    F
-0000a1b0: 6f72 206e 6f72 6d61 6c20 656e 7472 6965  or normal entrie
-0000a1c0: 732c 2074 6865 2064 6174 6120 6669 656c  s, the data fiel
-0000a1d0: 6420 7368 6f75 6c64 2063 6f6e 7461 696e  d should contain
-0000a1e0: 2074 6865 2064 6174 6120 6368 616e 6765   the data change
-0000a1f0: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
-0000a200: 6170 706c 6965 642e 0a20 2020 2054 6865  applied..    The
-0000a210: 2063 6f6e 7465 7874 2066 6965 6c64 2063   context field c
-0000a220: 616e 2062 6520 7573 6564 2066 6f72 2061  an be used for a
-0000a230: 6e79 2063 6f6e 7465 7874 7561 6c20 6461  ny contextual da
-0000a240: 7461 2074 6861 7420 6d69 6768 7420 6265  ta that might be
-0000a250: 2072 656c 6576 616e 7420 746f 2074 6865   relevant to the
-0000a260: 0a20 2020 2061 7070 6c69 6361 7469 6f6e  .    application
-0000a270: 206f 6620 7468 6520 6461 7461 2e0a 0a20   of the data... 
-0000a280: 2020 2046 6f72 2063 6f6e 6669 6775 7261     For configura
-0000a290: 7469 6f6e 2063 6861 6e67 6573 2c20 7468  tion changes, th
-0000a2a0: 6520 6461 7461 2077 696c 6c20 636f 6e74  e data will cont
-0000a2b0: 6169 6e20 7468 6520 436f 6e66 4368 616e  ain the ConfChan
-0000a2c0: 6765 206d 6573 7361 6765 2061 6e64 2074  ge message and t
-0000a2d0: 6865 0a20 2020 2063 6f6e 7465 7874 2077  he.    context w
-0000a2e0: 696c 6c20 7072 6f76 6964 6520 616e 7974  ill provide anyt
-0000a2f0: 6869 6e67 206e 6565 6465 6420 746f 2061  hing needed to a
-0000a300: 7373 6973 7420 7468 6520 636f 6e66 6967  ssist the config
-0000a310: 7572 6174 696f 6e20 6368 616e 6765 2e20  uration change. 
-0000a320: 5468 6520 636f 6e74 6578 740a 2020 2020  The context.    
-0000a330: 6966 2066 6f72 2074 6865 2075 7365 7220  if for the user 
-0000a340: 746f 2073 6574 2061 6e64 2075 7365 2069  to set and use i
-0000a350: 6e20 7468 6973 2063 6173 652e 0a20 2020  n this case..   
-0000a360: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
-0000a370: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
-0000a380: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
-0000a390: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
-0000a3a0: 202d 3e20 2245 6e74 7279 5265 6622 3a20   -> "EntryRef": 
-0000a3b0: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-0000a3c0: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
-0000a3d0: 6661 756c 7428 2920 2d3e 2022 456e 7472  fault() -> "Entr
-0000a3e0: 7922 3a20 2e2e 2e0a 2020 2020 4073 7461  y": ....    @sta
-0000a3f0: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0000a400: 6620 6465 636f 6465 2876 3a20 6279 7465  f decode(v: byte
-0000a410: 7329 202d 3e20 2245 6e74 7279 223a 202e  s) -> "Entry": .
-0000a420: 2e2e 0a0a 636c 6173 7320 456e 7472 7952  ....class EntryR
-0000a430: 6566 285f 5f41 5049 5f45 6e74 7279 293a  ef(__API_Entry):
-0000a440: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
-0000a450: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
-0000a460: 636c 6173 733a 6045 6e74 7279 602e 0a20  class:`Entry`.. 
-0000a470: 2020 2022 2222 0a0a 636c 6173 7320 5f5f     """..class __
-0000a480: 4150 495f 436f 6e66 5374 6174 6528 5f5f  API_ConfState(__
-0000a490: 436c 6f6e 6561 626c 652c 205f 5f45 6e63  Cloneable, __Enc
-0000a4a0: 6f64 6572 2c20 5f5f 4465 636f 6465 7229  oder, __Decoder)
-0000a4b0: 3a0a 2020 2020 6465 6620 636c 6f6e 6528  :.    def clone(
-0000a4c0: 7365 6c66 2920 2d3e 2022 436f 6e66 5374  self) -> "ConfSt
-0000a4d0: 6174 6522 3a20 2e2e 2e0a 2020 2020 6465  ate": ....    de
-0000a4e0: 6620 6765 745f 6175 746f 5f6c 6561 7665  f get_auto_leave
-0000a4f0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-0000a500: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000a510: 2020 2020 6465 6620 7365 745f 6175 746f      def set_auto
-0000a520: 5f6c 6561 7665 2873 656c 662c 2061 7574  _leave(self, aut
-0000a530: 6f5f 6c65 6176 653a 2062 6f6f 6c29 202d  o_leave: bool) -
-0000a540: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000a550: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-0000a560: 636c 6561 725f 6175 746f 5f6c 6561 7665  clear_auto_leave
-0000a570: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0000a580: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000a590: 2020 2020 6465 6620 6765 745f 6c65 6172      def get_lear
-0000a5a0: 6e65 7273 2873 656c 6629 202d 3e20 4c69  ners(self) -> Li
-0000a5b0: 7374 5b69 6e74 5d3a 0a20 2020 2020 2020  st[int]:.       
-0000a5c0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000a5d0: 2073 6574 5f6c 6561 726e 6572 7328 7365   set_learners(se
-0000a5e0: 6c66 2c20 6c65 6172 6e65 7273 3a20 4c69  lf, learners: Li
-0000a5f0: 7374 5b69 6e74 5d29 202d 3e20 4e6f 6e65  st[int]) -> None
-0000a600: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-0000a610: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
-0000a620: 6c65 6172 6e65 7273 2873 656c 6629 202d  learners(self) -
-0000a630: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000a640: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-0000a650: 6765 745f 6c65 6172 6e65 7273 5f6e 6578  get_learners_nex
-0000a660: 7428 7365 6c66 2920 2d3e 204c 6973 745b  t(self) -> List[
-0000a670: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
-0000a680: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-0000a690: 745f 6c65 6172 6e65 7273 5f6e 6578 7428  t_learners_next(
-0000a6a0: 7365 6c66 2c20 6c65 6172 6e65 7273 5f6e  self, learners_n
-0000a6b0: 6578 743a 204c 6973 745b 696e 745d 2920  ext: List[int]) 
-0000a6c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000a6d0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000a6e0: 2063 6c65 6172 5f6c 6561 726e 6572 735f   clear_learners_
-0000a6f0: 6e65 7874 2873 656c 6629 202d 3e20 4e6f  next(self) -> No
-0000a700: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000a710: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-0000a720: 766f 7465 7273 2873 656c 6629 202d 3e20  voters(self) -> 
-0000a730: 4c69 7374 5b69 6e74 5d3a 0a20 2020 2020  List[int]:.     
-0000a740: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-0000a750: 6566 2073 6574 5f76 6f74 6572 7328 7365  ef set_voters(se
-0000a760: 6c66 2c20 766f 7465 7273 3a20 4c69 7374  lf, voters: List
-0000a770: 5b69 6e74 5d29 202d 3e20 4e6f 6e65 3a0a  [int]) -> None:.
-0000a780: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000a790: 2020 2020 6465 6620 636c 6561 725f 766f      def clear_vo
-0000a7a0: 7465 7273 2873 656c 6629 202d 3e20 4e6f  ters(self) -> No
-0000a7b0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000a7c0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-0000a7d0: 766f 7465 7273 5f6f 7574 676f 696e 6728  voters_outgoing(
-0000a7e0: 7365 6c66 2920 2d3e 204c 6973 745b 696e  self) -> List[in
-0000a7f0: 745d 3a0a 2020 2020 2020 2020 2222 2220  t]:.        """ 
-0000a800: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-0000a810: 766f 7465 7273 5f6f 7574 676f 696e 6728  voters_outgoing(
-0000a820: 7365 6c66 2c20 766f 7465 7273 5f6f 7574  self, voters_out
-0000a830: 676f 696e 673a 204c 6973 745b 696e 745d  going: List[int]
-0000a840: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000a850: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-0000a860: 6566 2063 6c65 6172 5f76 6f74 6572 735f  ef clear_voters_
-0000a870: 6f75 7467 6f69 6e67 2873 656c 6629 202d  outgoing(self) -
-0000a880: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000a890: 2222 2220 2222 220a 0a63 6c61 7373 2043  """ """..class C
-0000a8a0: 6f6e 6653 7461 7465 285f 5f41 5049 5f43  onfState(__API_C
-0000a8b0: 6f6e 6653 7461 7465 293a 0a20 2020 2022  onfState):.    "
-0000a8c0: 2222 2022 2222 0a0a 2020 2020 6465 6620  "" """..    def 
-0000a8d0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0000a8e0: 2020 7365 6c66 2c20 766f 7465 7273 3a20    self, voters: 
-0000a8f0: 4f70 7469 6f6e 616c 5b4c 6973 745b 696e  Optional[List[in
-0000a900: 745d 5d2c 206c 6561 726e 6572 733a 204f  t]], learners: O
-0000a910: 7074 696f 6e61 6c5b 4c69 7374 5b69 6e74  ptional[List[int
-0000a920: 5d5d 0a20 2020 2029 202d 3e20 4e6f 6e65  ]].    ) -> None
-0000a930: 3a20 2e2e 2e0a 2020 2020 6465 6620 6d61  : ....    def ma
-0000a940: 6b65 5f72 6566 2873 656c 6629 202d 3e20  ke_ref(self) -> 
-0000a950: 2243 6f6e 6653 7461 7465 5265 6622 3a20  "ConfStateRef": 
-0000a960: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-0000a970: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
-0000a980: 6661 756c 7428 2920 2d3e 2022 436f 6e66  fault() -> "Conf
-0000a990: 5374 6174 6522 3a20 2e2e 2e0a 2020 2020  State": ....    
-0000a9a0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-0000a9b0: 2020 6465 6620 6465 636f 6465 2876 3a20    def decode(v: 
-0000a9c0: 6279 7465 7329 202d 3e20 2243 6f6e 6653  bytes) -> "ConfS
-0000a9d0: 7461 7465 223a 202e 2e2e 0a0a 636c 6173  tate": .....clas
-0000a9e0: 7320 436f 6e66 5374 6174 6552 6566 285f  s ConfStateRef(_
-0000a9f0: 5f41 5049 5f43 6f6e 6653 7461 7465 293a  _API_ConfState):
-0000aa00: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
-0000aa10: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
-0000aa20: 636c 6173 733a 6043 6f6e 6653 7461 7465  class:`ConfState
-0000aa30: 602e 0a20 2020 2022 2222 0a0a 636c 6173  `..    """..clas
-0000aa40: 7320 5f5f 4150 495f 436f 6e66 4368 616e  s __API_ConfChan
-0000aa50: 6765 5632 285f 5f43 6c6f 6e65 6162 6c65  geV2(__Cloneable
-0000aa60: 2c20 5f5f 456e 636f 6465 722c 205f 5f44  , __Encoder, __D
-0000aa70: 6563 6f64 6572 293a 0a20 2020 2064 6566  ecoder):.    def
-0000aa80: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
-0000aa90: 2243 6f6e 6643 6861 6e67 6556 3222 3a20  "ConfChangeV2": 
-0000aaa0: 2e2e 2e0a 2020 2020 6465 6620 6765 745f  ....    def get_
-0000aab0: 6368 616e 6765 7328 7365 6c66 2920 2d3e  changes(self) ->
-0000aac0: 204c 6973 745b 2243 6f6e 6643 6861 6e67   List["ConfChang
-0000aad0: 6553 696e 676c 6552 6566 225d 3a0a 2020  eSingleRef"]:.  
-0000aae0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-0000aaf0: 2020 6465 6620 7365 745f 6368 616e 6765    def set_change
-0000ab00: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-0000ab10: 2063 6861 6e67 6573 3a20 4c69 7374 5b22   changes: List["
-0000ab20: 436f 6e66 4368 616e 6765 5369 6e67 6c65  ConfChangeSingle
-0000ab30: 225d 207c 204c 6973 745b 2243 6f6e 6643  "] | List["ConfC
-0000ab40: 6861 6e67 6553 696e 676c 6552 6566 225d  hangeSingleRef"]
-0000ab50: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-0000ab60: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000ab70: 2020 2020 6465 6620 636c 6561 725f 6368      def clear_ch
-0000ab80: 616e 6765 7328 7365 6c66 2920 2d3e 204e  anges(self) -> N
-0000ab90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000aba0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-0000abb0: 5f63 6f6e 7465 7874 2873 656c 6629 202d  _context(self) -
-0000abc0: 3e20 6279 7465 733a 0a20 2020 2020 2020  > bytes:.       
-0000abd0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000abe0: 2073 6574 5f63 6f6e 7465 7874 2873 656c   set_context(sel
-0000abf0: 662c 2063 6f6e 7465 7874 3a20 6279 7465  f, context: byte
-0000ac00: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
-0000ac10: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-0000ac20: 6465 6620 636c 6561 725f 636f 6e74 6578  def clear_contex
-0000ac30: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-0000ac40: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-0000ac50: 0a20 2020 2064 6566 2067 6574 5f74 7261  .    def get_tra
-0000ac60: 6e73 6974 696f 6e28 7365 6c66 2920 2d3e  nsition(self) ->
-0000ac70: 2022 436f 6e66 4368 616e 6765 5472 616e   "ConfChangeTran
-0000ac80: 7369 7469 6f6e 223a 0a20 2020 2020 2020  sition":.       
-0000ac90: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000aca0: 2073 6574 5f74 7261 6e73 6974 696f 6e28   set_transition(
-0000acb0: 7365 6c66 2c20 7472 616e 7369 7469 6f6e  self, transition
-0000acc0: 3a20 2243 6f6e 6643 6861 6e67 6554 7261  : "ConfChangeTra
-0000acd0: 6e73 6974 696f 6e22 2920 2d3e 204e 6f6e  nsition") -> Non
-0000ace0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-0000acf0: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-0000ad00: 5f74 7261 6e73 6974 696f 6e28 7365 6c66  _transition(self
-0000ad10: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000ad20: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-0000ad30: 6566 2065 6e74 6572 5f6a 6f69 6e74 2873  ef enter_joint(s
-0000ad40: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-0000ad50: 5b62 6f6f 6c5d 3a0a 2020 2020 2020 2020  [bool]:.        
-0000ad60: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
-0000ad70: 6b73 2069 6620 7573 6573 204a 6f69 6e74  ks if uses Joint
-0000ad80: 2043 6f6e 7365 6e73 7573 2e0a 0a20 2020   Consensus...   
-0000ad90: 2020 2020 2049 7420 7769 6c6c 2072 6574       It will ret
-0000ada0: 7572 6e20 536f 6d65 2069 6620 616e 6420  urn Some if and 
-0000adb0: 6f6e 6c79 2069 6620 7468 6973 2063 6f6e  only if this con
-0000adc0: 6669 6720 6368 616e 6765 2077 696c 6c20  fig change will 
-0000add0: 7573 6520 4a6f 696e 7420 436f 6e73 656e  use Joint Consen
-0000ade0: 7375 732c 0a20 2020 2020 2020 2077 6869  sus,.        whi
-0000adf0: 6368 2069 7320 7468 6520 6361 7365 2069  ch is the case i
-0000ae00: 6620 6974 2063 6f6e 7461 696e 7320 6d6f  f it contains mo
-0000ae10: 7265 2074 6861 6e20 6f6e 6520 6368 616e  re than one chan
-0000ae20: 6765 206f 7220 6966 2074 6865 2075 7365  ge or if the use
-0000ae30: 206f 6620 4a6f 696e 740a 2020 2020 2020   of Joint.      
-0000ae40: 2020 436f 6e73 656e 7375 7320 7761 7320    Consensus was 
-0000ae50: 7265 7175 6573 7465 6420 6578 706c 6963  requested explic
-0000ae60: 6974 6c79 2e20 5468 6520 626f 6f6c 2069  itly. The bool i
-0000ae70: 6e64 6963 6174 6573 2077 6865 7468 6572  ndicates whether
-0000ae80: 2074 6865 204a 6f69 6e74 2053 7461 7465   the Joint State
-0000ae90: 0a20 2020 2020 2020 2077 696c 6c20 6265  .        will be
-0000aea0: 206c 6566 7420 6175 746f 6d61 7469 6361   left automatica
-0000aeb0: 6c6c 792e 0a20 2020 2020 2020 2022 2222  lly..        """
-0000aec0: 0a20 2020 2064 6566 206d 6572 6765 5f66  .    def merge_f
-0000aed0: 726f 6d5f 6279 7465 7328 7365 6c66 2c20  rom_bytes(self, 
-0000aee0: 623a 2062 7974 6573 2920 2d3e 204e 6f6e  b: bytes) -> Non
-0000aef0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-0000af00: 2020 2020 2020 2055 7064 6174 6520 7468         Update th
-0000af10: 6973 206d 6573 7361 6765 206f 626a 6563  is message objec
-0000af20: 7420 7769 7468 2066 6965 6c64 7320 7265  t with fields re
-0000af30: 6164 2066 726f 6d20 6769 7665 6e20 7374  ad from given st
-0000af40: 7265 616d 2e0a 2020 2020 2020 2020 2222  ream..        ""
-0000af50: 220a 2020 2020 6465 6620 6c65 6176 655f  ".    def leave_
-0000af60: 6a6f 696e 7428 7365 6c66 2920 2d3e 2062  joint(self) -> b
-0000af70: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-0000af80: 0a20 2020 2020 2020 2043 6865 636b 7320  .        Checks 
-0000af90: 6966 2074 6865 2063 6f6e 6669 6775 7261  if the configura
-0000afa0: 7469 6f6e 2063 6861 6e67 6520 6c65 6176  tion change leav
-0000afb0: 6573 2061 206a 6f69 6e74 2063 6f6e 6669  es a joint confi
-0000afc0: 6775 7261 7469 6f6e 2e0a 0a20 2020 2020  guration...     
-0000afd0: 2020 2054 6869 7320 6973 2074 6865 2063     This is the c
-0000afe0: 6173 6520 6966 2074 6865 2043 6f6e 6643  ase if the ConfC
-0000aff0: 6861 6e67 6556 3220 6973 207a 6572 6f2c  hangeV2 is zero,
-0000b000: 2077 6974 6820 7468 6520 706f 7373 6962   with the possib
-0000b010: 6c65 2065 7863 6570 7469 6f6e 206f 660a  le exception of.
-0000b020: 2020 2020 2020 2020 7468 6520 436f 6e74          the Cont
-0000b030: 6578 7420 6669 656c 642e 0a20 2020 2020  ext field..     
-0000b040: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
-0000b050: 735f 7631 2873 656c 6629 202d 3e20 4f70  s_v1(self) -> Op
-0000b060: 7469 6f6e 616c 5b22 436f 6e66 4368 616e  tional["ConfChan
-0000b070: 6765 5265 6622 5d3a 0a20 2020 2020 2020  geRef"]:.       
-0000b080: 2022 2222 0a20 2020 2020 2020 2043 6f6e   """.        Con
-0000b090: 7665 7274 7320 636f 6e66 2063 6861 6e67  verts conf chang
-0000b0a0: 6520 746f 2060 436f 6e66 4368 616e 6765  e to `ConfChange
-0000b0b0: 602e 0a0a 2020 2020 2020 2020 6043 6f6e  `...        `Con
-0000b0c0: 6643 6861 6e67 6556 3260 2063 616e 2774  fChangeV2` can't
-0000b0d0: 2062 6520 6368 616e 6765 6420 6261 636b   be changed back
-0000b0e0: 2074 6f20 6043 6f6e 6643 6861 6e67 6560   to `ConfChange`
-0000b0f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000b100: 2020 6465 6620 6173 5f76 3228 7365 6c66    def as_v2(self
-0000b110: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000b120: 5632 223a 0a20 2020 2020 2020 2022 2222  V2":.        """
-0000b130: 0a20 2020 2020 2020 2047 6574 7320 636f  .        Gets co
-0000b140: 6e66 2063 6861 6e67 6520 6173 2060 436f  nf change as `Co
-0000b150: 6e66 4368 616e 6765 5632 602e 0a20 2020  nfChangeV2`..   
-0000b160: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000b170: 2069 6e74 6f5f 7632 2873 656c 6629 202d   into_v2(self) -
-0000b180: 3e20 2243 6f6e 6643 6861 6e67 6556 3222  > "ConfChangeV2"
-0000b190: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000b1a0: 2020 2020 2020 436f 6e76 6572 7473 2063        Converts c
-0000b1b0: 6f6e 6620 6368 616e 6765 2074 6f20 6043  onf change to `C
-0000b1c0: 6f6e 6643 6861 6e67 6556 3260 2e0a 2020  onfChangeV2`..  
-0000b1d0: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
-0000b1e0: 2043 6f6e 6643 6861 6e67 6556 3228 5f5f   ConfChangeV2(__
-0000b1f0: 4150 495f 436f 6e66 4368 616e 6765 5632  API_ConfChangeV2
-0000b200: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
-0000b210: 6f6e 6643 6861 6e67 6556 3220 6d65 7373  onfChangeV2 mess
-0000b220: 6167 6573 2069 6e69 7469 6174 6520 636f  ages initiate co
-0000b230: 6e66 6967 7572 6174 696f 6e20 6368 616e  nfiguration chan
-0000b240: 6765 732e 2054 6865 7920 7375 7070 6f72  ges. They suppor
-0000b250: 7420 626f 7468 2074 6865 0a20 2020 2073  t both the.    s
-0000b260: 696d 706c 6520 226f 6e65 2061 7420 6120  imple "one at a 
-0000b270: 7469 6d65 2220 6d65 6d62 6572 7368 6970  time" membership
-0000b280: 2063 6861 6e67 6520 7072 6f74 6f63 6f6c   change protocol
-0000b290: 2061 6e64 2066 756c 6c20 4a6f 696e 7420   and full Joint 
-0000b2a0: 436f 6e73 656e 7375 730a 2020 2020 616c  Consensus.    al
-0000b2b0: 6c6f 7769 6e67 2066 6f72 2061 7262 6974  lowing for arbit
-0000b2c0: 7261 7279 2063 6861 6e67 6573 2069 6e20  rary changes in 
-0000b2d0: 6d65 6d62 6572 7368 6970 2e0a 0a20 2020  membership...   
-0000b2e0: 2054 6865 2073 7570 706c 6965 6420 636f   The supplied co
-0000b2f0: 6e74 6578 7420 6973 2074 7265 6174 6564  ntext is treated
-0000b300: 2061 7320 616e 206f 7061 7175 6520 7061   as an opaque pa
-0000b310: 796c 6f61 6420 616e 6420 6361 6e20 6265  yload and can be
-0000b320: 2075 7365 6420 746f 0a20 2020 2061 7474   used to.    att
-0000b330: 6163 6820 616e 2061 6374 696f 6e20 6f6e  ach an action on
-0000b340: 2074 6865 2073 7461 7465 206d 6163 6869   the state machi
-0000b350: 6e65 2074 6f20 7468 6520 6170 706c 6963  ne to the applic
-0000b360: 6174 696f 6e20 6f66 2074 6865 2063 6f6e  ation of the con
-0000b370: 6669 6720 6368 616e 6765 0a20 2020 2070  fig change.    p
-0000b380: 726f 706f 7361 6c2e 204e 6f74 6520 7468  roposal. Note th
-0000b390: 6174 2063 6f6e 7472 6172 7920 746f 204a  at contrary to J
-0000b3a0: 6f69 6e74 2043 6f6e 7365 6e73 7573 2061  oint Consensus a
-0000b3b0: 7320 6f75 746c 696e 6564 2069 6e20 7468  s outlined in th
-0000b3c0: 6520 5261 6674 0a20 2020 2070 6170 6572  e Raft.    paper
-0000b3d0: 5b31 5d2c 2063 6f6e 6669 6775 7261 7469  [1], configurati
-0000b3e0: 6f6e 2063 6861 6e67 6573 2062 6563 6f6d  on changes becom
-0000b3f0: 6520 6163 7469 7665 2077 6865 6e20 7468  e active when th
-0000b400: 6579 2061 7265 202a 6170 706c 6965 642a  ey are *applied*
-0000b410: 2074 6f20 7468 650a 2020 2020 7374 6174   to the.    stat
-0000b420: 6520 6d61 6368 696e 6520 286e 6f74 2077  e machine (not w
-0000b430: 6865 6e20 7468 6579 2061 7265 2061 7070  hen they are app
-0000b440: 656e 6465 6420 746f 2074 6865 206c 6f67  ended to the log
-0000b450: 292e 0a0a 2020 2020 5468 6520 7369 6d70  )...    The simp
-0000b460: 6c65 2070 726f 746f 636f 6c20 6361 6e20  le protocol can 
-0000b470: 6265 2075 7365 6420 7768 656e 6576 6572  be used whenever
-0000b480: 206f 6e6c 7920 6120 7369 6e67 6c65 2063   only a single c
-0000b490: 6861 6e67 6520 6973 206d 6164 652e 0a0a  hange is made...
-0000b4a0: 2020 2020 4e6f 6e2d 7369 6d70 6c65 2063      Non-simple c
-0000b4b0: 6861 6e67 6573 2072 6571 7569 7265 2074  hanges require t
-0000b4c0: 6865 2075 7365 206f 6620 4a6f 696e 7420  he use of Joint 
-0000b4d0: 436f 6e73 656e 7375 732c 2066 6f72 2077  Consensus, for w
-0000b4e0: 6869 6368 2074 776f 0a20 2020 2063 6f6e  hich two.    con
-0000b4f0: 6669 6775 7261 7469 6f6e 2063 6861 6e67  figuration chang
-0000b500: 6573 2061 7265 2072 756e 2e20 5468 6520  es are run. The 
-0000b510: 6669 7273 7420 636f 6e66 6967 7572 6174  first configurat
-0000b520: 696f 6e20 6368 616e 6765 2073 7065 6369  ion change speci
-0000b530: 6669 6573 2074 6865 0a20 2020 2064 6573  fies the.    des
-0000b540: 6972 6564 2063 6861 6e67 6573 2061 6e64  ired changes and
-0000b550: 2074 7261 6e73 6974 696f 6e73 2074 6865   transitions the
-0000b560: 2052 6166 7420 6772 6f75 7020 696e 746f   Raft group into
-0000b570: 2074 6865 206a 6f69 6e74 2063 6f6e 6669   the joint confi
-0000b580: 6775 7261 7469 6f6e 2c0a 2020 2020 696e  guration,.    in
-0000b590: 2077 6869 6368 2071 756f 7275 6d20 7265   which quorum re
-0000b5a0: 7175 6972 6573 2061 206d 616a 6f72 6974  quires a majorit
-0000b5b0: 7920 6f66 2062 6f74 6820 7468 6520 7072  y of both the pr
-0000b5c0: 652d 6368 616e 6765 7320 616e 6420 706f  e-changes and po
-0000b5d0: 7374 2d63 6861 6e67 6573 0a20 2020 2063  st-changes.    c
-0000b5e0: 6f6e 6669 6775 7261 7469 6f6e 2e20 4a6f  onfiguration. Jo
-0000b5f0: 696e 7420 436f 6e73 656e 7375 7320 6176  int Consensus av
-0000b600: 6f69 6473 2065 6e74 6572 696e 6720 6672  oids entering fr
-0000b610: 6167 696c 6520 696e 7465 726d 6564 6961  agile intermedia
-0000b620: 7465 0a20 2020 2063 6f6e 6669 6775 7261  te.    configura
-0000b630: 7469 6f6e 7320 7468 6174 2063 6f75 6c64  tions that could
-0000b640: 2063 6f6d 7072 6f6d 6973 6520 7375 7276   compromise surv
-0000b650: 6976 6162 696c 6974 792e 2046 6f72 2065  ivability. For e
-0000b660: 7861 6d70 6c65 2c20 7769 7468 6f75 7420  xample, without 
-0000b670: 7468 650a 2020 2020 7573 6520 6f66 204a  the.    use of J
-0000b680: 6f69 6e74 2043 6f6e 7365 6e73 7573 2061  oint Consensus a
-0000b690: 6e64 2072 756e 6e69 6e67 2061 6372 6f73  nd running acros
-0000b6a0: 7320 7468 7265 6520 6176 6169 6c61 6269  s three availabi
-0000b6b0: 6c69 7479 207a 6f6e 6573 2077 6974 6820  lity zones with 
-0000b6c0: 610a 2020 2020 7265 706c 6963 6174 696f  a.    replicatio
-0000b6d0: 6e20 6661 6374 6f72 206f 6620 7468 7265  n factor of thre
-0000b6e0: 652c 2069 7420 6973 206e 6f74 2070 6f73  e, it is not pos
-0000b6f0: 7369 626c 6520 746f 2072 6570 6c61 6365  sible to replace
-0000b700: 2061 2076 6f74 6572 2077 6974 686f 7574   a voter without
-0000b710: 0a20 2020 2065 6e74 6572 696e 6720 616e  .    entering an
-0000b720: 2069 6e74 6572 6d65 6469 6174 6520 636f   intermediate co
-0000b730: 6e66 6967 7572 6174 696f 6e20 7468 6174  nfiguration that
-0000b740: 2064 6f65 7320 6e6f 7420 7375 7276 6976   does not surviv
-0000b750: 6520 7468 6520 6f75 7461 6765 206f 660a  e the outage of.
-0000b760: 2020 2020 6f6e 6520 6176 6169 6c61 6269      one availabi
-0000b770: 6c69 7479 207a 6f6e 652e 0a0a 2020 2020  lity zone...    
-0000b780: 5468 6520 7072 6f76 6964 6564 2043 6f6e  The provided Con
-0000b790: 6643 6861 6e67 6554 7261 6e73 6974 696f  fChangeTransitio
-0000b7a0: 6e20 7370 6563 6966 6965 7320 686f 7720  n specifies how 
-0000b7b0: 2861 6e64 2077 6865 7468 6572 2920 4a6f  (and whether) Jo
-0000b7c0: 696e 7420 436f 6e73 656e 7375 730a 2020  int Consensus.  
-0000b7d0: 2020 6973 2075 7365 642c 2061 6e64 2061    is used, and a
-0000b7e0: 7373 6967 6e73 2074 6865 2074 6173 6b20  ssigns the task 
-0000b7f0: 6f66 206c 6561 7669 6e67 2074 6865 206a  of leaving the j
-0000b800: 6f69 6e74 2063 6f6e 6669 6775 7261 7469  oint configurati
-0000b810: 6f6e 2065 6974 6865 7220 746f 0a20 2020  on either to.   
-0000b820: 2052 6166 7420 6f72 2074 6865 2061 7070   Raft or the app
-0000b830: 6c69 6361 7469 6f6e 2e20 4c65 6176 696e  lication. Leavin
-0000b840: 6720 7468 6520 6a6f 696e 7420 636f 6e66  g the joint conf
-0000b850: 6967 7572 6174 696f 6e20 6973 2061 6363  iguration is acc
-0000b860: 6f6d 706c 6973 6865 6420 6279 0a20 2020  omplished by.   
-0000b870: 2070 726f 706f 7369 6e67 2061 2043 6f6e   proposing a Con
-0000b880: 6643 6861 6e67 6556 3220 7769 7468 206f  fChangeV2 with o
-0000b890: 6e6c 7920 616e 6420 6f70 7469 6f6e 616c  nly and optional
-0000b8a0: 6c79 2074 6865 2043 6f6e 7465 7874 2066  ly the Context f
-0000b8b0: 6965 6c64 0a20 2020 2070 6f70 756c 6174  ield.    populat
-0000b8c0: 6564 2e0a 0a20 2020 2046 6f72 2064 6574  ed...    For det
-0000b8d0: 6169 6c73 206f 6e20 5261 6674 206d 656d  ails on Raft mem
-0000b8e0: 6265 7273 6869 7020 6368 616e 6765 732c  bership changes,
-0000b8f0: 2073 6565 3a0a 0a20 2020 205b 315d 3a20   see:..    [1]: 
-0000b900: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000b910: 6f6d 2f6f 6e67 6172 6469 652f 6469 7373  om/ongardie/diss
-0000b920: 6572 7461 7469 6f6e 2f62 6c6f 622f 6d61  ertation/blob/ma
-0000b930: 7374 6572 2f6f 6e6c 696e 652d 7472 696d  ster/online-trim
-0000b940: 2e70 6466 0a20 2020 2022 2222 0a0a 2020  .pdf.    """..  
-0000b950: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000b960: 656c 6629 202d 3e20 4e6f 6e65 3a20 2e2e  elf) -> None: ..
-0000b970: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000b980: 686f 640a 2020 2020 6465 6620 6465 6661  hod.    def defa
-0000b990: 756c 7428 2920 2d3e 2022 436f 6e66 4368  ult() -> "ConfCh
-0000b9a0: 616e 6765 5632 223a 202e 2e2e 0a20 2020  angeV2": ....   
-0000b9b0: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
-0000b9c0: 6c66 2920 2d3e 2022 436f 6e66 4368 616e  lf) -> "ConfChan
-0000b9d0: 6765 5632 5265 6622 3a20 2e2e 2e0a 2020  geV2Ref": ....  
-0000b9e0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-0000b9f0: 2020 2020 6465 6620 6465 636f 6465 2876      def decode(v
-0000ba00: 3a20 6279 7465 7329 202d 3e20 2243 6f6e  : bytes) -> "Con
-0000ba10: 6643 6861 6e67 6556 3222 3a20 2e2e 2e0a  fChangeV2": ....
-0000ba20: 0a63 6c61 7373 2043 6f6e 6643 6861 6e67  .class ConfChang
-0000ba30: 6556 3252 6566 285f 5f41 5049 5f43 6f6e  eV2Ref(__API_Con
-0000ba40: 6643 6861 6e67 6556 3229 3a0a 2020 2020  fChangeV2):.    
-0000ba50: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
-0000ba60: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
-0000ba70: 3a60 436f 6e66 4368 616e 6765 5632 602e  :`ConfChangeV2`.
-0000ba80: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-0000ba90: 5f5f 4150 495f 436f 6e66 4368 616e 6765  __API_ConfChange
-0000baa0: 5369 6e67 6c65 285f 5f43 6c6f 6e65 6162  Single(__Cloneab
-0000bab0: 6c65 2c20 5f5f 456e 636f 6465 722c 205f  le, __Encoder, _
-0000bac0: 5f44 6563 6f64 6572 293a 0a20 2020 2064  _Decoder):.    d
-0000bad0: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-0000bae0: 3e20 2243 6f6e 6643 6861 6e67 6553 696e  > "ConfChangeSin
-0000baf0: 676c 6522 3a20 2e2e 2e0a 2020 2020 6465  gle": ....    de
-0000bb00: 6620 6765 745f 6e6f 6465 5f69 6428 7365  f get_node_id(se
-0000bb10: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-0000bb20: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-0000bb30: 6465 6620 7365 745f 6e6f 6465 5f69 6428  def set_node_id(
-0000bb40: 7365 6c66 2c20 6e6f 6465 5f69 643a 2069  self, node_id: i
-0000bb50: 6e74 293a 0a20 2020 2020 2020 2022 2222  nt):.        """
-0000bb60: 2022 2222 0a20 2020 2064 6566 2063 6c65   """.    def cle
-0000bb70: 6172 5f6e 6f64 655f 6964 2873 656c 6629  ar_node_id(self)
-0000bb80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000bb90: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-0000bba0: 6620 6765 745f 6368 616e 6765 5f74 7970  f get_change_typ
-0000bbb0: 6528 7365 6c66 2920 2d3e 2022 436f 6e66  e(self) -> "Conf
-0000bbc0: 4368 616e 6765 5479 7065 223a 0a20 2020  ChangeType":.   
-0000bbd0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000bbe0: 2064 6566 2073 6574 5f63 6861 6e67 655f   def set_change_
-0000bbf0: 7479 7065 2873 656c 662c 2074 7970 3a20  type(self, typ: 
-0000bc00: 2243 6f6e 6643 6861 6e67 6554 7970 6522  "ConfChangeType"
-0000bc10: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000bc20: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-0000bc30: 6566 2063 6c65 6172 5f63 6861 6e67 655f  ef clear_change_
-0000bc40: 7479 7065 2873 656c 6629 202d 3e20 4e6f  type(self) -> No
-0000bc50: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000bc60: 2222 220a 0a63 6c61 7373 2043 6f6e 6643  """..class ConfC
-0000bc70: 6861 6e67 6553 696e 676c 6528 5f5f 4150  hangeSingle(__AP
-0000bc80: 495f 436f 6e66 4368 616e 6765 5369 6e67  I_ConfChangeSing
-0000bc90: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
-0000bca0: 2043 6f6e 6643 6861 6e67 6553 696e 676c   ConfChangeSingl
-0000bcb0: 6520 6973 2061 6e20 696e 6469 7669 6475  e is an individu
-0000bcc0: 616c 2063 6f6e 6669 6775 7261 7469 6f6e  al configuration
-0000bcd0: 2063 6861 6e67 6520 6f70 6572 6174 696f   change operatio
-0000bce0: 6e2e 204d 756c 7469 706c 650a 2020 2020  n. Multiple.    
-0000bcf0: 7375 6368 206f 7065 7261 7469 6f6e 7320  such operations 
-0000bd00: 6361 6e20 6265 2063 6172 7269 6564 206f  can be carried o
-0000bd10: 7574 2061 746f 6d69 6361 6c6c 7920 7669  ut atomically vi
-0000bd20: 6120 6120 436f 6e66 4368 616e 6765 5632  a a ConfChangeV2
-0000bd30: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-0000bd40: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000bd50: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-0000bd60: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
-0000bd70: 7365 6c66 2920 2d3e 2022 436f 6e66 4368  self) -> "ConfCh
-0000bd80: 616e 6765 5369 6e67 6c65 5265 6622 3a20  angeSingleRef": 
-0000bd90: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-0000bda0: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
-0000bdb0: 6661 756c 7428 2920 2d3e 2022 436f 6e66  fault() -> "Conf
-0000bdc0: 4368 616e 6765 5369 6e67 6c65 223a 202e  ChangeSingle": .
-0000bdd0: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-0000bde0: 7468 6f64 0a20 2020 2064 6566 2064 6563  thod.    def dec
-0000bdf0: 6f64 6528 763a 2062 7974 6573 2920 2d3e  ode(v: bytes) ->
-0000be00: 2022 436f 6e66 4368 616e 6765 5369 6e67   "ConfChangeSing
-0000be10: 6c65 223a 202e 2e2e 0a0a 636c 6173 7320  le": .....class 
-0000be20: 436f 6e66 4368 616e 6765 5369 6e67 6c65  ConfChangeSingle
-0000be30: 5265 6628 5f5f 4150 495f 436f 6e66 4368  Ref(__API_ConfCh
-0000be40: 616e 6765 5369 6e67 6c65 293a 0a20 2020  angeSingle):.   
-0000be50: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
-0000be60: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
-0000be70: 733a 6043 6f6e 6643 6861 6e67 6553 696e  s:`ConfChangeSin
-0000be80: 676c 6560 2e0a 2020 2020 2222 220a 0a63  gle`..    """..c
-0000be90: 6c61 7373 205f 5f41 5049 5f43 6f6e 6643  lass __API_ConfC
-0000bea0: 6861 6e67 6528 5f5f 436c 6f6e 6561 626c  hange(__Cloneabl
-0000beb0: 652c 205f 5f45 6e63 6f64 6572 2c20 5f5f  e, __Encoder, __
-0000bec0: 4465 636f 6465 7229 3a0a 2020 2020 6465  Decoder):.    de
-0000bed0: 6620 636c 6f6e 6528 7365 6c66 2920 2d3e  f clone(self) ->
-0000bee0: 2022 436f 6e66 4368 616e 6765 223a 202e   "ConfChange": .
-0000bef0: 2e2e 0a20 2020 2064 6566 2067 6574 5f69  ...    def get_i
-0000bf00: 6428 7365 6c66 2920 2d3e 2069 6e74 3a0a  d(self) -> int:.
-0000bf10: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000bf20: 2020 2020 6465 6620 7365 745f 6964 2873      def set_id(s
-0000bf30: 656c 662c 2069 643a 2069 6e74 2920 2d3e  elf, id: int) ->
-0000bf40: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000bf50: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-0000bf60: 6c65 6172 5f69 6428 7365 6c66 2920 2d3e  lear_id(self) ->
-0000bf70: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000bf80: 2222 2022 2222 0a20 2020 2064 6566 2067  "" """.    def g
-0000bf90: 6574 5f6e 6f64 655f 6964 2873 656c 6629  et_node_id(self)
-0000bfa0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-0000bfb0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000bfc0: 2073 6574 5f6e 6f64 655f 6964 2873 656c   set_node_id(sel
-0000bfd0: 662c 206e 6f64 655f 6964 3a20 696e 7429  f, node_id: int)
-0000bfe0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000bff0: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-0000c000: 6620 636c 6561 725f 6e6f 6465 5f69 6428  f clear_node_id(
-0000c010: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000c020: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-0000c030: 2020 2064 6566 2067 6574 5f63 6861 6e67     def get_chang
-0000c040: 655f 7479 7065 2873 656c 6629 202d 3e20  e_type(self) -> 
-0000c050: 2243 6f6e 6643 6861 6e67 6554 7970 6522  "ConfChangeType"
-0000c060: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-0000c070: 220a 2020 2020 6465 6620 7365 745f 6368  ".    def set_ch
-0000c080: 616e 6765 5f74 7970 6528 7365 6c66 2c20  ange_type(self, 
-0000c090: 7479 703a 2022 436f 6e66 4368 616e 6765  typ: "ConfChange
-0000c0a0: 5479 7065 2229 202d 3e20 4e6f 6e65 3a0a  Type") -> None:.
-0000c0b0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000c0c0: 2020 2020 6465 6620 636c 6561 725f 6368      def clear_ch
-0000c0d0: 616e 6765 5f74 7970 6528 7365 6c66 2920  ange_type(self) 
-0000c0e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000c0f0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000c100: 2067 6574 5f63 6f6e 7465 7874 2873 656c   get_context(sel
-0000c110: 6629 202d 3e20 6279 7465 733a 0a20 2020  f) -> bytes:.   
-0000c120: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000c130: 2064 6566 2073 6574 5f63 6f6e 7465 7874   def set_context
-0000c140: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
-0000c150: 6279 7465 7329 202d 3e20 4e6f 6e65 3a0a  bytes) -> None:.
-0000c160: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000c170: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
-0000c180: 6e74 6578 7428 7365 6c66 2920 2d3e 204e  ntext(self) -> N
-0000c190: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000c1a0: 2022 2222 0a20 2020 2064 6566 206d 6572   """.    def mer
-0000c1b0: 6765 5f66 726f 6d5f 6279 7465 7328 7365  ge_from_bytes(se
-0000c1c0: 6c66 2c20 623a 2062 7974 6573 2920 2d3e  lf, b: bytes) ->
-0000c1d0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000c1e0: 2222 0a20 2020 2020 2020 2055 7064 6174  "".        Updat
-0000c1f0: 6520 7468 6973 206d 6573 7361 6765 206f  e this message o
-0000c200: 626a 6563 7420 7769 7468 2066 6965 6c64  bject with field
-0000c210: 7320 7265 6164 2066 726f 6d20 6769 7665  s read from give
-0000c220: 6e20 7374 7265 616d 2e0a 2020 2020 2020  n stream..      
-0000c230: 2020 2222 220a 2020 2020 6465 6620 6173    """.    def as
-0000c240: 5f76 3128 7365 6c66 2920 2d3e 204f 7074  _v1(self) -> Opt
-0000c250: 696f 6e61 6c5b 2243 6f6e 6643 6861 6e67  ional["ConfChang
-0000c260: 6552 6566 225d 3a0a 2020 2020 2020 2020  eRef"]:.        
-0000c270: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
-0000c280: 6572 7473 2063 6f6e 6620 6368 616e 6765  erts conf change
-0000c290: 2074 6f20 6043 6f6e 6643 6861 6e67 6560   to `ConfChange`
-0000c2a0: 2e0a 0a20 2020 2020 2020 2060 436f 6e66  ...        `Conf
-0000c2b0: 4368 616e 6765 5632 6020 6361 6e27 7420  ChangeV2` can't 
-0000c2c0: 6265 2063 6861 6e67 6564 2062 6163 6b20  be changed back 
-0000c2d0: 746f 2060 436f 6e66 4368 616e 6765 602e  to `ConfChange`.
-0000c2e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c2f0: 2064 6566 2061 735f 7632 2873 656c 6629   def as_v2(self)
-0000c300: 202d 3e20 2243 6f6e 6643 6861 6e67 6556   -> "ConfChangeV
-0000c310: 3222 3a0a 2020 2020 2020 2020 2222 220a  2":.        """.
-0000c320: 2020 2020 2020 2020 4765 7473 2063 6f6e          Gets con
-0000c330: 6620 6368 616e 6765 2061 7320 6043 6f6e  f change as `Con
-0000c340: 6643 6861 6e67 6556 3260 2e0a 2020 2020  fChangeV2`..    
-0000c350: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000c360: 696e 746f 5f76 3228 7365 6c66 2920 2d3e  into_v2(self) ->
-0000c370: 2022 436f 6e66 4368 616e 6765 5632 223a   "ConfChangeV2":
-0000c380: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c390: 2020 2020 2043 6f6e 7665 7274 7320 636f       Converts co
-0000c3a0: 6e66 2063 6861 6e67 6520 746f 2060 436f  nf change to `Co
-0000c3b0: 6e66 4368 616e 6765 5632 602e 0a20 2020  nfChangeV2`..   
-0000c3c0: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-0000c3d0: 436f 6e66 4368 616e 6765 285f 5f41 5049  ConfChange(__API
-0000c3e0: 5f43 6f6e 6643 6861 6e67 6529 3a0a 2020  _ConfChange):.  
-0000c3f0: 2020 2222 2220 2222 220a 0a20 2020 2064    """ """..    d
-0000c400: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000c410: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-0000c420: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
-0000c430: 7365 6c66 2920 2d3e 2022 436f 6e66 4368  self) -> "ConfCh
-0000c440: 616e 6765 5265 6622 3a20 2e2e 2e0a 2020  angeRef": ....  
-0000c450: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-0000c460: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
-0000c470: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000c480: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
-0000c490: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-0000c4a0: 2064 6563 6f64 6528 763a 2062 7974 6573   decode(v: bytes
-0000c4b0: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000c4c0: 223a 202e 2e2e 0a0a 636c 6173 7320 436f  ": .....class Co
-0000c4d0: 6e66 4368 616e 6765 5265 6628 5f5f 4150  nfChangeRef(__AP
-0000c4e0: 495f 436f 6e66 4368 616e 6765 293a 0a20  I_ConfChange):. 
-0000c4f0: 2020 2022 2222 0a20 2020 2052 6566 6572     """.    Refer
-0000c500: 656e 6365 2074 7970 6520 6f66 203a 636c  ence type of :cl
-0000c510: 6173 733a 6043 6f6e 6643 6861 6e67 6560  ass:`ConfChange`
-0000c520: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
-0000c530: 205f 5f41 5049 5f55 6e73 7461 626c 653a   __API_Unstable:
-0000c540: 0a20 2020 2064 6566 206d 6179 6265 5f66  .    def maybe_f
-0000c550: 6972 7374 5f69 6e64 6578 2873 656c 6629  irst_index(self)
-0000c560: 202d 3e20 4f70 7469 6f6e 616c 5b69 6e74   -> Optional[int
-0000c570: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-0000c580: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
-0000c590: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
-0000c5a0: 6669 7273 7420 706f 7373 6962 6c65 2065  first possible e
-0000c5b0: 6e74 7279 2069 6e20 656e 7472 6965 730a  ntry in entries.
-0000c5c0: 2020 2020 2020 2020 6966 2069 7420 6861          if it ha
-0000c5d0: 7320 6120 736e 6170 7368 6f74 2e0a 2020  s a snapshot..  
-0000c5e0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000c5f0: 6620 6d61 7962 655f 6c61 7374 5f69 6e64  f maybe_last_ind
-0000c600: 6578 2873 656c 6629 202d 3e20 4f70 7469  ex(self) -> Opti
-0000c610: 6f6e 616c 5b69 6e74 5d3a 0a20 2020 2020  onal[int]:.     
-0000c620: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000c630: 6574 7572 6e73 2074 6865 206c 6173 7420  eturns the last 
-0000c640: 696e 6465 7820 6966 2069 7420 6861 7320  index if it has 
-0000c650: 6174 206c 6561 7374 206f 6e65 2075 6e73  at least one uns
-0000c660: 7461 626c 6520 656e 7472 7920 6f72 2073  table entry or s
-0000c670: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
-0000c680: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
-0000c690: 6265 5f74 6572 6d28 7365 6c66 2920 2d3e  be_term(self) ->
-0000c6a0: 204f 7074 696f 6e61 6c5b 696e 745d 3a0a   Optional[int]:.
-0000c6b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c6c0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
-0000c6d0: 7465 726d 206f 6620 7468 6520 656e 7472  term of the entr
-0000c6e0: 7920 6174 2069 6e64 6578 2069 6478 2c20  y at index idx, 
-0000c6f0: 6966 2074 6865 7265 2069 7320 616e 792e  if there is any.
-0000c700: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c710: 2064 6566 206d 7573 745f 6368 6563 6b5f   def must_check_
-0000c720: 6f75 746f 6662 6f75 6e64 7328 7365 6c66  outofbounds(self
-0000c730: 2c20 6c6f 3a20 696e 742c 2068 693a 2069  , lo: int, hi: i
-0000c740: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-0000c750: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c760: 2041 7373 6572 7473 2074 6865 2060 6869   Asserts the `hi
-0000c770: 6020 616e 6420 606c 6f60 2076 616c 7565  ` and `lo` value
-0000c780: 7320 6167 6169 6e73 7420 6561 6368 206f  s against each o
-0000c790: 7468 6572 2061 6e64 2061 6761 696e 7374  ther and against
-0000c7a0: 2074 6865 0a20 2020 2020 2020 2065 6e74   the.        ent
-0000c7b0: 7269 6573 2074 6865 6d73 656c 7665 732e  ries themselves.
-0000c7c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c7d0: 2064 6566 2073 6c69 6365 2873 656c 662c   def slice(self,
-0000c7e0: 206c 6f3a 2069 6e74 2c20 6869 3a20 696e   lo: int, hi: in
-0000c7f0: 7429 202d 3e20 4c69 7374 5b22 456e 7472  t) -> List["Entr
-0000c800: 7952 6566 225d 3a0a 2020 2020 2020 2020  yRef"]:.        
-0000c810: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-0000c820: 726e 7320 6120 736c 6963 6520 6f66 2065  rns a slice of e
-0000c830: 6e74 7269 6573 2062 6574 7765 656e 2074  ntries between t
-0000c840: 6865 2068 6967 6820 616e 6420 6c6f 772e  he high and low.
-0000c850: 0a0a 2020 2020 2020 2020 2320 5061 6e69  ..        # Pani
-0000c860: 6373 0a0a 2020 2020 2020 2020 5061 6e69  cs..        Pani
-0000c870: 6373 2069 6620 7468 6520 606c 6f60 206f  cs if the `lo` o
-0000c880: 7220 6068 6960 2061 7265 206f 7574 206f  r `hi` are out o
-0000c890: 6620 626f 756e 6473 2e0a 2020 2020 2020  f bounds..      
-0000c8a0: 2020 5061 6e69 6373 2069 6620 606c 6f20    Panics if `lo 
-0000c8b0: 3e20 6869 602e 0a20 2020 2020 2020 2022  > hi`..        "
-0000c8c0: 2222 0a20 2020 2064 6566 2073 7461 626c  "".    def stabl
-0000c8d0: 655f 736e 6170 2873 656c 662c 2069 6e64  e_snap(self, ind
-0000c8e0: 6578 3a20 696e 7429 202d 3e20 4e6f 6e65  ex: int) -> None
-0000c8f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000c900: 2020 2020 2020 436c 6561 7273 2074 6865        Clears the
-0000c910: 2075 6e73 7461 626c 6520 736e 6170 7368   unstable snapsh
-0000c920: 6f74 2e0a 2020 2020 2020 2020 2222 220a  ot..        """.
-0000c930: 2020 2020 6465 6620 7374 6162 6c65 5f65      def stable_e
-0000c940: 6e74 7269 6573 2873 656c 662c 2069 6e64  ntries(self, ind
-0000c950: 6578 3a20 696e 742c 2074 6572 6d3a 2069  ex: int, term: i
-0000c960: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-0000c970: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c980: 2043 6c65 6172 7320 7468 6520 756e 7374   Clears the unst
-0000c990: 6162 6c65 2065 6e74 7269 6573 2061 6e64  able entries and
-0000c9a0: 206d 6f76 6573 2074 6865 2073 7461 626c   moves the stabl
-0000c9b0: 6520 6f66 6673 6574 2075 7020 746f 2074  e offset up to t
-0000c9c0: 6865 0a20 2020 2020 2020 206c 6173 7420  he.        last 
-0000c9d0: 696e 6465 782c 2069 6620 7468 6572 6520  index, if there 
-0000c9e0: 6973 2061 6e79 2e0a 2020 2020 2020 2020  is any..        
-0000c9f0: 2222 220a 2020 2020 6465 6620 7265 7374  """.    def rest
-0000ca00: 6f72 6528 7365 6c66 2c20 736e 6170 3a20  ore(self, snap: 
-0000ca10: 2253 6e61 7073 686f 7452 6566 2229 202d  "SnapshotRef") -
-0000ca20: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000ca30: 2222 220a 2020 2020 2020 2020 4672 6f6d  """.        From
-0000ca40: 2061 2067 6976 656e 2073 6e61 7073 686f   a given snapsho
-0000ca50: 742c 2072 6573 746f 7265 7320 7468 6520  t, restores the 
-0000ca60: 736e 6170 7368 6f74 2074 6f20 7365 6c66  snapshot to self
-0000ca70: 2c20 6275 7420 646f 6573 6e27 7420 756e  , but doesn't un
-0000ca80: 7061 636b 2e0a 2020 2020 2020 2020 2222  pack..        ""
-0000ca90: 220a 2020 2020 6465 6620 7472 756e 6361  ".    def trunca
-0000caa0: 7465 5f61 6e64 5f61 7070 656e 6428 7365  te_and_append(se
-0000cab0: 6c66 2c20 656e 7473 3a20 4c69 7374 5b22  lf, ents: List["
-0000cac0: 456e 7472 7922 5d20 7c20 4c69 7374 5b22  Entry"] | List["
-0000cad0: 456e 7472 7952 6566 225d 2920 2d3e 204e  EntryRef"]) -> N
-0000cae0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000caf0: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
-0000cb00: 656e 7472 6965 7320 746f 2075 6e73 7461  entries to unsta
-0000cb10: 626c 652c 2074 7275 6e63 6174 6520 6c6f  ble, truncate lo
-0000cb20: 6361 6c20 626c 6f63 6b20 6669 7273 7420  cal block first 
-0000cb30: 6966 206f 7665 726c 6170 7065 642e 0a0a  if overlapped...
-0000cb40: 2020 2020 2020 2020 2320 5061 6e69 6373          # Panics
-0000cb50: 0a0a 2020 2020 2020 2020 5061 6e69 6373  ..        Panics
-0000cb60: 2069 6620 7472 756e 6361 7465 206c 6f67   if truncate log
-0000cb70: 7320 746f 2074 6865 2065 6e74 7279 2062  s to the entry b
-0000cb80: 6566 6f72 6520 736e 6170 7368 6f74 0a20  efore snapshot. 
-0000cb90: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000cba0: 6566 2067 6574 5f65 6e74 7269 6573 5f73  ef get_entries_s
-0000cbb0: 697a 6528 7365 6c66 2920 2d3e 2069 6e74  ize(self) -> int
-0000cbc0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000cbd0: 2020 2020 2020 6065 6e74 7269 6573 5f73        `entries_s
-0000cbe0: 697a 6560 3a20 5468 6520 7369 7a65 206f  ize`: The size o
-0000cbf0: 6620 656e 7472 6965 730a 2020 2020 2020  f entries.      
-0000cc00: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-0000cc10: 745f 656e 7472 6965 735f 7369 7a65 2873  t_entries_size(s
-0000cc20: 656c 662c 2065 6e74 7269 6573 5f73 697a  elf, entries_siz
-0000cc30: 653a 2069 6e74 2920 2d3e 204e 6f6e 653a  e: int) -> None:
-0000cc40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000cc50: 2020 2020 2060 656e 7472 6965 735f 7369       `entries_si
-0000cc60: 7a65 603a 2054 6865 2073 697a 6520 6f66  ze`: The size of
-0000cc70: 2065 6e74 7269 6573 0a20 2020 2020 2020   entries.       
-0000cc80: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-0000cc90: 5f6f 6666 7365 7428 7365 6c66 2920 2d3e  _offset(self) ->
-0000cca0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000ccb0: 220a 2020 2020 2020 2020 606f 6666 7365  ".        `offse
-0000ccc0: 7460 3a20 5468 6520 6f66 6673 6574 2066  t`: The offset f
-0000ccd0: 726f 6d20 7468 6520 7665 6374 6f72 2069  rom the vector i
-0000cce0: 6e64 6578 2e0a 2020 2020 2020 2020 2222  ndex..        ""
-0000ccf0: 220a 2020 2020 6465 6620 7365 745f 6f66  ".    def set_of
-0000cd00: 6673 6574 2873 656c 662c 206f 6666 7365  fset(self, offse
-0000cd10: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-0000cd20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000cd30: 2020 2020 2060 6f66 6673 6574 603a 2054       `offset`: T
-0000cd40: 6865 206f 6666 7365 7420 6672 6f6d 2074  he offset from t
-0000cd50: 6865 2076 6563 746f 7220 696e 6465 782e  he vector index.
-0000cd60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000cd70: 2064 6566 2067 6574 5f65 6e74 7269 6573   def get_entries
-0000cd80: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
-0000cd90: 456e 7472 7952 6566 225d 3a0a 2020 2020  EntryRef"]:.    
-0000cda0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000cdb0: 6065 6e74 7269 6573 603a 2041 6c6c 2065  `entries`: All e
-0000cdc0: 6e74 7269 6573 2074 6861 7420 6861 7665  ntries that have
-0000cdd0: 206e 6f74 2079 6574 2062 6565 6e20 7772   not yet been wr
-0000cde0: 6974 7465 6e20 746f 2073 746f 7261 6765  itten to storage
-0000cdf0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000ce00: 2020 6465 6620 7365 745f 656e 7472 6965    def set_entrie
-0000ce10: 7328 7365 6c66 2c20 656e 7473 3a20 4c69  s(self, ents: Li
-0000ce20: 7374 5b22 456e 7472 7922 5d20 7c20 4c69  st["Entry"] | Li
-0000ce30: 7374 5b22 456e 7472 7952 6566 225d 2920  st["EntryRef"]) 
-0000ce40: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000ce50: 2022 2222 0a20 2020 2020 2020 2060 656e   """.        `en
-0000ce60: 7472 6965 7360 3a20 416c 6c20 656e 7472  tries`: All entr
-0000ce70: 6965 7320 7468 6174 2068 6176 6520 6e6f  ies that have no
-0000ce80: 7420 7965 7420 6265 656e 2077 7269 7474  t yet been writt
-0000ce90: 656e 2074 6f20 7374 6f72 6167 652e 0a20  en to storage.. 
-0000cea0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000ceb0: 6566 2067 6574 5f6c 6f67 6765 7228 7365  ef get_logger(se
-0000cec0: 6c66 2920 2d3e 2022 4c6f 6767 6572 5265  lf) -> "LoggerRe
-0000ced0: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
-0000cee0: 2020 2020 2020 2020 606c 6f67 6765 7260          `logger`
-0000cef0: 3a20 5468 6520 7461 6720 746f 2075 7365  : The tag to use
-0000cf00: 2077 6865 6e20 6c6f 6767 696e 672e 0a20   when logging.. 
-0000cf10: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000cf20: 6566 2073 6574 5f6c 6f67 6765 7228 7365  ef set_logger(se
-0000cf30: 6c66 2c20 6c6f 6767 6572 3a20 224c 6f67  lf, logger: "Log
-0000cf40: 6765 7222 207c 2022 4c6f 6767 6572 5265  ger" | "LoggerRe
-0000cf50: 6622 2920 2d3e 204e 6f6e 653a 0a20 2020  f") -> None:.   
-0000cf60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000cf70: 2060 6c6f 6767 6572 603a 2054 6865 2074   `logger`: The t
-0000cf80: 6167 2074 6f20 7573 6520 7768 656e 206c  ag to use when l
-0000cf90: 6f67 6769 6e67 2e0a 2020 2020 2020 2020  ogging..        
-0000cfa0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-0000cfb0: 736e 6170 7368 6f74 2873 656c 6629 202d  snapshot(self) -
-0000cfc0: 3e20 4f70 7469 6f6e 616c 5b22 536e 6170  > Optional["Snap
-0000cfd0: 7368 6f74 5265 6622 5d3a 0a20 2020 2020  shotRef"]:.     
-0000cfe0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-0000cff0: 736e 6170 7368 6f74 603a 2054 6865 2069  snapshot`: The i
-0000d000: 6e63 6f6d 696e 6720 756e 7374 6162 6c65  ncoming unstable
-0000d010: 2073 6e61 7073 686f 742c 2069 6620 616e   snapshot, if an
-0000d020: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
-0000d030: 2020 2064 6566 2073 6574 5f73 6e61 7073     def set_snaps
-0000d040: 686f 7428 7365 6c66 2c20 736e 6170 7368  hot(self, snapsh
-0000d050: 6f74 3a20 2253 6e61 7073 686f 7422 207c  ot: "Snapshot" |
-0000d060: 2022 536e 6170 7368 6f74 5265 6622 2920   "SnapshotRef") 
-0000d070: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000d080: 2022 2222 0a20 2020 2020 2020 2060 736e   """.        `sn
-0000d090: 6170 7368 6f74 603a 2054 6865 2069 6e63  apshot`: The inc
-0000d0a0: 6f6d 696e 6720 756e 7374 6162 6c65 2073  oming unstable s
-0000d0b0: 6e61 7073 686f 742c 2069 6620 616e 792e  napshot, if any.
-0000d0c0: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
-0000d0d0: 6173 7320 556e 7374 6162 6c65 285f 5f41  ass Unstable(__A
-0000d0e0: 5049 5f55 6e73 7461 626c 6529 3a0a 2020  PI_Unstable):.  
-0000d0f0: 2020 2222 220a 2020 2020 5468 6520 6075    """.    The `u
-0000d100: 6e73 7461 626c 652e 656e 7472 6965 735b  nstable.entries[
-0000d110: 695d 6020 6861 7320 7261 6674 206c 6f67  i]` has raft log
-0000d120: 2070 6f73 6974 696f 6e20 6069 2b75 6e73   position `i+uns
-0000d130: 7461 626c 652e 6f66 6673 6574 602e 0a20  table.offset`.. 
-0000d140: 2020 204e 6f74 6520 7468 6174 2060 756e     Note that `un
-0000d150: 7374 6162 6c65 2e6f 6666 7365 7460 206d  stable.offset` m
-0000d160: 6179 2062 6520 6c65 7373 2074 6861 6e20  ay be less than 
-0000d170: 7468 6520 6869 6768 6573 7420 6c6f 670a  the highest log.
-0000d180: 2020 2020 706f 7369 7469 6f6e 2069 6e20      position in 
-0000d190: 7374 6f72 6167 653b 2074 6869 7320 6d65  storage; this me
-0000d1a0: 616e 7320 7468 6174 2074 6865 206e 6578  ans that the nex
-0000d1b0: 7420 7772 6974 6520 746f 2073 746f 7261  t write to stora
-0000d1c0: 6765 0a20 2020 206d 6967 6874 206e 6565  ge.    might nee
-0000d1d0: 6420 746f 2074 7275 6e63 6174 6520 7468  d to truncate th
-0000d1e0: 6520 6c6f 6720 6265 666f 7265 2070 6572  e log before per
-0000d1f0: 7369 7374 696e 6720 756e 7374 6162 6c65  sisting unstable
-0000d200: 2e65 6e74 7269 6573 2e0a 2020 2020 2222  .entries..    ""
-0000d210: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-0000d220: 745f 5f28 7365 6c66 2c20 6f66 6673 6574  t__(self, offset
-0000d230: 3a20 696e 742c 206c 6f67 6765 723a 2022  : int, logger: "
-0000d240: 4c6f 6767 6572 2220 7c20 224c 6f67 6765  Logger" | "Logge
-0000d250: 7252 6566 2229 202d 3e20 4e6f 6e65 3a20  rRef") -> None: 
-0000d260: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-0000d270: 5f72 6566 2873 656c 6629 202d 3e20 2255  _ref(self) -> "U
-0000d280: 6e73 7461 626c 6552 6566 223a 202e 2e2e  nstableRef": ...
-0000d290: 0a0a 636c 6173 7320 556e 7374 6162 6c65  ..class Unstable
-0000d2a0: 5265 6628 5f5f 4150 495f 556e 7374 6162  Ref(__API_Unstab
-0000d2b0: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
-0000d2c0: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-0000d2d0: 6f66 203a 636c 6173 733a 6055 6e73 7461  of :class:`Unsta
-0000d2e0: 626c 6560 2e0a 2020 2020 2222 220a 0a63  ble`..    """..c
-0000d2f0: 6c61 7373 205f 5f41 5049 5f53 6f66 7453  lass __API_SoftS
-0000d300: 7461 7465 3a0a 2020 2020 6465 6620 6765  tate:.    def ge
-0000d310: 745f 6c65 6164 6572 5f69 6428 7365 6c66  t_leader_id(self
-0000d320: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-0000d330: 2020 2222 220a 2020 2020 2020 2020 606c    """.        `l
-0000d340: 6561 6465 725f 6964 603a 2054 6865 2070  eader_id`: The p
-0000d350: 6f74 656e 7469 616c 206c 6561 6465 7220  otential leader 
-0000d360: 6f66 2074 6865 2063 6c75 7374 6572 2e0a  of the cluster..
-0000d370: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d380: 6465 6620 7365 745f 6c65 6164 6572 5f69  def set_leader_i
-0000d390: 6428 7365 6c66 2c20 6c65 6164 6572 5f69  d(self, leader_i
-0000d3a0: 643a 2069 6e74 2920 2d3e 204e 6f6e 653a  d: int) -> None:
-0000d3b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d3c0: 2020 2020 2060 6c65 6164 6572 5f69 6460       `leader_id`
-0000d3d0: 3a20 5468 6520 706f 7465 6e74 6961 6c20  : The potential 
-0000d3e0: 6c65 6164 6572 206f 6620 7468 6520 636c  leader of the cl
-0000d3f0: 7573 7465 722e 0a20 2020 2020 2020 2022  uster..        "
-0000d400: 2222 0a20 2020 2064 6566 2067 6574 5f72  "".    def get_r
-0000d410: 6166 745f 7374 6174 6528 7365 6c66 2920  aft_state(self) 
-0000d420: 2d3e 2022 5374 6174 6552 6f6c 6522 3a0a  -> "StateRole":.
-0000d430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d440: 2020 2020 6072 6166 745f 7374 6174 6560      `raft_state`
-0000d450: 3a20 5468 6520 736f 6674 2072 6f6c 6520  : The soft role 
-0000d460: 7468 6973 206e 6f64 6520 6d61 7920 7461  this node may ta
-0000d470: 6b65 2e0a 2020 2020 2020 2020 2222 220a  ke..        """.
-0000d480: 2020 2020 6465 6620 7365 745f 7261 6674      def set_raft
-0000d490: 5f73 7461 7465 2873 656c 662c 2072 6f6c  _state(self, rol
-0000d4a0: 653a 2022 5374 6174 6552 6f6c 6522 2920  e: "StateRole") 
-0000d4b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000d4c0: 2022 2222 0a20 2020 2020 2020 2060 7261   """.        `ra
-0000d4d0: 6674 5f73 7461 7465 603a 2054 6865 2073  ft_state`: The s
-0000d4e0: 6f66 7420 726f 6c65 2074 6869 7320 6e6f  oft role this no
-0000d4f0: 6465 206d 6179 2074 616b 652e 0a20 2020  de may take..   
-0000d500: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-0000d510: 536f 6674 5374 6174 6528 5f5f 4150 495f  SoftState(__API_
-0000d520: 536f 6674 5374 6174 6529 3a0a 2020 2020  SoftState):.    
-0000d530: 2222 220a 2020 2020 536f 6674 5374 6174  """.    SoftStat
-0000d540: 6520 7072 6f76 6964 6573 2073 7461 7465  e provides state
-0000d550: 2074 6861 7420 6973 2075 7365 6675 6c20   that is useful 
-0000d560: 666f 7220 6c6f 6767 696e 6720 616e 6420  for logging and 
-0000d570: 6465 6275 6767 696e 672e 0a20 2020 2054  debugging..    T
-0000d580: 6865 2073 7461 7465 2069 7320 766f 6c61  he state is vola
-0000d590: 7469 6c65 2061 6e64 2064 6f65 7320 6e6f  tile and does no
-0000d5a0: 7420 6e65 6564 2074 6f20 6265 2070 6572  t need to be per
-0000d5b0: 7369 7374 6564 2074 6f20 7468 6520 5741  sisted to the WA
-0000d5c0: 4c2e 0a20 2020 2022 2222 0a0a 2020 2020  L..    """..    
-0000d5d0: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
-0000d5e0: 6629 202d 3e20 2253 6f66 7453 7461 7465  f) -> "SoftState
-0000d5f0: 5265 6622 3a20 2e2e 2e0a 2020 2020 4073  Ref": ....    @s
-0000d600: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-0000d610: 6465 6620 6465 6661 756c 7428 2920 2d3e  def default() ->
-0000d620: 2022 536f 6674 5374 6174 6522 3a20 2e2e   "SoftState": ..
-0000d630: 2e0a 0a63 6c61 7373 2053 6f66 7453 7461  ...class SoftSta
-0000d640: 7465 5265 6628 5f5f 4150 495f 536f 6674  teRef(__API_Soft
-0000d650: 5374 6174 6529 3a0a 2020 2020 2222 220a  State):.    """.
-0000d660: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
-0000d670: 7065 206f 6620 3a63 6c61 7373 3a60 536f  pe of :class:`So
-0000d680: 6674 5374 6174 6560 2e0a 2020 2020 2222  ftState`..    ""
-0000d690: 220a 0a63 6c61 7373 205f 5f41 5049 5f52  "..class __API_R
-0000d6a0: 6561 6453 7461 7465 285f 5f43 6c6f 6e65  eadState(__Clone
-0000d6b0: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
-0000d6c0: 6c6f 6e65 2873 656c 6629 202d 3e20 2252  lone(self) -> "R
-0000d6d0: 6561 6453 7461 7465 223a 202e 2e2e 0a20  eadState": .... 
-0000d6e0: 2020 2064 6566 2067 6574 5f69 6e64 6578     def get_index
-0000d6f0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-0000d700: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d710: 2020 2060 696e 6465 7860 3a20 5468 6520     `index`: The 
-0000d720: 696e 6465 7820 6f66 2074 6865 2072 6561  index of the rea
-0000d730: 6420 7374 6174 652e 0a20 2020 2020 2020  d state..       
-0000d740: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-0000d750: 5f69 6e64 6578 2873 656c 662c 2069 6478  _index(self, idx
-0000d760: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-0000d770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d780: 2020 2020 6069 6e64 6578 603a 2054 6865      `index`: The
-0000d790: 2069 6e64 6578 206f 6620 7468 6520 7265   index of the re
-0000d7a0: 6164 2073 7461 7465 2e0a 2020 2020 2020  ad state..      
-0000d7b0: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-0000d7c0: 745f 7265 7175 6573 745f 6374 7828 7365  t_request_ctx(se
-0000d7d0: 6c66 2920 2d3e 2062 7974 6573 3a0a 2020  lf) -> bytes:.  
-0000d7e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d7f0: 2020 6072 6571 7565 7374 5f63 7478 603a    `request_ctx`:
-0000d800: 2041 2064 6174 6167 7261 6d20 636f 6e73   A datagram cons
-0000d810: 6973 7469 6e67 206f 6620 636f 6e74 6578  isting of contex
-0000d820: 7420 6162 6f75 7420 7468 6520 7265 7175  t about the requ
-0000d830: 6573 742e 0a20 2020 2020 2020 2022 2222  est..        """
-0000d840: 0a20 2020 2064 6566 2073 6574 5f72 6571  .    def set_req
-0000d850: 7565 7374 5f63 7478 2873 656c 662c 2072  uest_ctx(self, r
-0000d860: 6571 7565 7374 5f63 7478 3a20 6279 7465  equest_ctx: byte
-0000d870: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
-0000d880: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000d890: 6072 6571 7565 7374 5f63 7478 603a 2041  `request_ctx`: A
-0000d8a0: 2064 6174 6167 7261 6d20 636f 6e73 6973   datagram consis
-0000d8b0: 7469 6e67 206f 6620 636f 6e74 6578 7420  ting of context 
-0000d8c0: 6162 6f75 7420 7468 6520 7265 7175 6573  about the reques
-0000d8d0: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
-0000d8e0: 636c 6173 7320 5265 6164 5374 6174 6528  class ReadState(
-0000d8f0: 5f5f 4150 495f 5265 6164 5374 6174 6529  __API_ReadState)
-0000d900: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-0000d910: 6164 5374 6174 6520 7072 6f76 6964 6573  adState provides
-0000d920: 2073 7461 7465 2066 6f72 2072 6561 6420   state for read 
-0000d930: 6f6e 6c79 2071 7565 7279 2e0a 2020 2020  only query..    
-0000d940: 4974 2773 2063 616c 6c65 7227 7320 7265  It's caller's re
-0000d950: 7370 6f6e 7369 6269 6c69 7479 2074 6f20  sponsibility to 
-0000d960: 7365 6e64 204d 7367 5265 6164 496e 6465  send MsgReadInde
-0000d970: 7820 6669 7273 7420 6265 666f 7265 2067  x first before g
-0000d980: 6574 7469 6e67 0a20 2020 2074 6869 7320  etting.    this 
-0000d990: 7374 6174 6520 6672 6f6d 2072 6561 6479  state from ready
-0000d9a0: 2e20 4974 2773 2061 6c73 6f20 6361 6c6c  . It's also call
-0000d9b0: 6572 2773 2064 7574 7920 746f 2064 6966  er's duty to dif
-0000d9c0: 6665 7265 6e74 6961 7465 2069 6620 7468  ferentiate if th
-0000d9d0: 6973 0a20 2020 2073 7461 7465 2069 7320  is.    state is 
-0000d9e0: 7768 6174 2069 7420 7265 7175 6573 7473  what it requests
-0000d9f0: 2074 6872 6f75 6768 2072 6571 7565 7374   through request
-0000da00: 5f63 7478 2c20 652e 672e 2067 6976 656e  _ctx, e.g. given
-0000da10: 2061 2075 6e69 7175 6520 6964 2061 730a   a unique id as.
-0000da20: 2020 2020 7265 7175 6573 745f 6374 782e      request_ctx.
-0000da30: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-0000da40: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-0000da50: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-0000da60: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
-0000da70: 656c 6629 202d 3e20 2252 6561 6453 7461  elf) -> "ReadSta
-0000da80: 7465 5265 6622 3a20 2e2e 2e0a 0a63 6c61  teRef": .....cla
-0000da90: 7373 2052 6561 6453 7461 7465 5265 6628  ss ReadStateRef(
-0000daa0: 5f5f 4150 495f 5265 6164 5374 6174 6529  __API_ReadState)
-0000dab0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-0000dac0: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
-0000dad0: 3a63 6c61 7373 3a60 5265 6164 5374 6174  :class:`ReadStat
-0000dae0: 6560 2e0a 2020 2020 2222 220a 0a63 6c61  e`..    """..cla
-0000daf0: 7373 205f 5f41 5049 5f52 6166 744c 6f67  ss __API_RaftLog
-0000db00: 3a0a 2020 2020 6465 6620 656e 7472 6965  :.    def entrie
-0000db10: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-0000db20: 2069 6478 3a20 696e 742c 2063 6f6e 7465   idx: int, conte
-0000db30: 7874 3a20 2247 6574 456e 7472 6965 7343  xt: "GetEntriesC
-0000db40: 6f6e 7465 7874 5265 6622 2c20 6d61 785f  ontextRef", max_
-0000db50: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
-0000db60: 6e74 5d0a 2020 2020 2920 2d3e 204c 6973  nt].    ) -> Lis
-0000db70: 745b 2245 6e74 7279 225d 3a0a 2020 2020  t["Entry"]:.    
-0000db80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000db90: 5265 7475 726e 7320 656e 7472 6965 7320  Returns entries 
-0000dba0: 7374 6172 7469 6e67 2066 726f 6d20 6120  starting from a 
-0000dbb0: 7061 7274 6963 756c 6172 2069 6e64 6578  particular index
-0000dbc0: 2061 6e64 206e 6f74 2065 7863 6565 6469   and not exceedi
-0000dbd0: 6e67 2061 2062 7974 6573 697a 652e 0a20  ng a bytesize.. 
-0000dbe0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000dbf0: 6566 2061 6c6c 5f65 6e74 7269 6573 2873  ef all_entries(s
-0000dc00: 656c 6629 202d 3e20 4c69 7374 5b22 456e  elf) -> List["En
-0000dc10: 7472 7922 5d3a 0a20 2020 2020 2020 2022  try"]:.        "
-0000dc20: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-0000dc30: 6e73 2061 6c6c 2074 6865 2065 6e74 7269  ns all the entri
-0000dc40: 6573 2e20 4f6e 6c79 2075 7365 6420 6279  es. Only used by
-0000dc50: 2074 6573 7473 2e0a 2020 2020 2020 2020   tests..        
-0000dc60: 2222 220a 2020 2020 6465 6620 6170 7065  """.    def appe
-0000dc70: 6e64 2873 656c 662c 2065 6e74 733a 204c  nd(self, ents: L
-0000dc80: 6973 745b 2245 6e74 7279 225d 207c 204c  ist["Entry"] | L
-0000dc90: 6973 745b 2245 6e74 7279 5265 6622 5d29  ist["EntryRef"])
-0000dca0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-0000dcb0: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
-0000dcc0: 656e 6473 2061 2073 6574 206f 6620 656e  ends a set of en
-0000dcd0: 7472 6965 7320 746f 2074 6865 2075 6e73  tries to the uns
-0000dce0: 7461 626c 6520 6c69 7374 2e0a 2020 2020  table list..    
-0000dcf0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000dd00: 6170 706c 6965 6428 7365 6c66 2920 2d3e  applied(self) ->
-0000dd10: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000dd20: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-0000dd30: 7320 7468 6520 6c61 7374 2061 7070 6c69  s the last appli
-0000dd40: 6564 2069 6e64 6578 2e0a 2020 2020 2020  ed index..      
-0000dd50: 2020 2222 220a 2020 2020 6465 6620 6669    """.    def fi
-0000dd60: 6e64 5f63 6f6e 666c 6963 7428 7365 6c66  nd_conflict(self
-0000dd70: 2c20 656e 7473 3a20 4c69 7374 5b22 456e  , ents: List["En
-0000dd80: 7472 7922 5d20 7c20 4c69 7374 5b22 456e  try"] | List["En
-0000dd90: 7472 7952 6566 225d 2920 2d3e 2069 6e74  tryRef"]) -> int
-0000dda0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000ddb0: 2020 2020 2020 4669 6e64 7320 7468 6520        Finds the 
-0000ddc0: 696e 6465 7820 6f66 2074 6865 2063 6f6e  index of the con
-0000ddd0: 666c 6963 742e 0a0a 2020 2020 2020 2020  flict...        
-0000dde0: 4974 2072 6574 7572 6e73 2074 6865 2066  It returns the f
-0000ddf0: 6972 7374 2069 6e64 6578 206f 6620 636f  irst index of co
-0000de00: 6e66 6c69 6374 696e 6720 656e 7472 6965  nflicting entrie
-0000de10: 7320 6265 7477 6565 6e20 7468 6520 6578  s between the ex
-0000de20: 6973 7469 6e67 0a20 2020 2020 2020 2065  isting.        e
-0000de30: 6e74 7269 6573 2061 6e64 2074 6865 2067  ntries and the g
-0000de40: 6976 656e 2065 6e74 7269 6573 2c20 6966  iven entries, if
-0000de50: 2074 6865 7265 2061 7265 2061 6e79 2e0a   there are any..
-0000de60: 0a20 2020 2020 2020 2049 6620 7468 6572  .        If ther
-0000de70: 6520 6172 6520 6e6f 2063 6f6e 666c 6963  e are no conflic
-0000de80: 7469 6e67 2065 6e74 7269 6573 2c20 616e  ting entries, an
-0000de90: 6420 7468 6520 6578 6973 7469 6e67 2065  d the existing e
-0000dea0: 6e74 7269 6573 2063 6f6e 7461 696e 0a20  ntries contain. 
-0000deb0: 2020 2020 2020 2061 6c6c 2074 6865 2067         all the g
-0000dec0: 6976 656e 2065 6e74 7269 6573 2c20 7a65  iven entries, ze
-0000ded0: 726f 2077 696c 6c20 6265 2072 6574 7572  ro will be retur
-0000dee0: 6e65 642e 0a0a 2020 2020 2020 2020 4966  ned...        If
-0000def0: 2074 6865 7265 2061 7265 206e 6f20 636f   there are no co
-0000df00: 6e66 6c69 6374 696e 6720 656e 7472 6965  nflicting entrie
-0000df10: 732c 2062 7574 2074 6865 2067 6976 656e  s, but the given
-0000df20: 2065 6e74 7269 6573 2063 6f6e 7461 696e   entries contain
-0000df30: 7320 6e65 770a 2020 2020 2020 2020 656e  s new.        en
-0000df40: 7472 6965 732c 2074 6865 2069 6e64 6578  tries, the index
-0000df50: 206f 6620 7468 6520 6669 7273 7420 6e65   of the first ne
-0000df60: 7720 656e 7472 7920 7769 6c6c 2062 6520  w entry will be 
-0000df70: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
-0000df80: 2020 2041 6e20 656e 7472 7920 6973 2063     An entry is c
-0000df90: 6f6e 7369 6465 7265 6420 746f 2062 6520  onsidered to be 
-0000dfa0: 636f 6e66 6c69 6374 696e 6720 6966 2069  conflicting if i
-0000dfb0: 7420 6861 7320 7468 6520 7361 6d65 2069  t has the same i
-0000dfc0: 6e64 6578 2062 7574 0a20 2020 2020 2020  ndex but.       
-0000dfd0: 2061 2064 6966 6665 7265 6e74 2074 6572   a different ter
-0000dfe0: 6d2e 0a0a 2020 2020 2020 2020 5468 6520  m...        The 
-0000dff0: 6669 7273 7420 656e 7472 7920 4d55 5354  first entry MUST
-0000e000: 2068 6176 6520 616e 2069 6e64 6578 2065   have an index e
-0000e010: 7175 616c 2074 6f20 7468 6520 6172 6775  qual to the argu
-0000e020: 6d65 6e74 2027 6672 6f6d 272e 0a20 2020  ment 'from'..   
-0000e030: 2020 2020 2054 6865 2069 6e64 6578 206f       The index o
-0000e040: 6620 7468 6520 6769 7665 6e20 656e 7472  f the given entr
-0000e050: 6965 7320 4d55 5354 2062 6520 636f 6e74  ies MUST be cont
-0000e060: 696e 756f 7573 6c79 2069 6e63 7265 6173  inuously increas
-0000e070: 696e 672e 0a20 2020 2020 2020 2022 2222  ing..        """
-0000e080: 0a20 2020 2064 6566 2066 696e 645f 636f  .    def find_co
-0000e090: 6e66 6c69 6374 5f62 795f 7465 726d 2873  nflict_by_term(s
-0000e0a0: 656c 662c 2069 6e64 6578 3a20 696e 742c  elf, index: int,
-0000e0b0: 2074 6572 6d3a 2069 6e74 2920 2d3e 2054   term: int) -> T
-0000e0c0: 7570 6c65 5b69 6e74 2c20 4f70 7469 6f6e  uple[int, Option
-0000e0d0: 616c 5b69 6e74 5d5d 3a0a 2020 2020 2020  al[int]]:.      
-0000e0e0: 2020 2222 220a 2020 2020 2020 2020 6669    """.        fi
-0000e0f0: 6e64 5f63 6f6e 666c 6963 745f 6279 5f74  nd_conflict_by_t
-0000e100: 6572 6d20 7461 6b65 7320 616e 2028 6069  erm takes an (`i
-0000e110: 6e64 6578 602c 2060 7465 726d 6029 2070  ndex`, `term`) p
-0000e120: 6169 7220 2869 6e64 6963 6174 696e 6720  air (indicating 
-0000e130: 6120 636f 6e66 6c69 6374 696e 6720 6c6f  a conflicting lo
-0000e140: 670a 2020 2020 2020 2020 656e 7472 7920  g.        entry 
-0000e150: 6f6e 2061 206c 6561 6465 722f 666f 6c6c  on a leader/foll
-0000e160: 6f77 6572 2064 7572 696e 6720 616e 2061  ower during an a
-0000e170: 7070 656e 6429 2061 6e64 2066 696e 6473  ppend) and finds
-0000e180: 2074 6865 206c 6172 6765 7374 2069 6e64   the largest ind
-0000e190: 6578 2069 6e0a 2020 2020 2020 2020 6c6f  ex in.        lo
-0000e1a0: 6720 7769 7468 206c 6f67 2e74 6572 6d20  g with log.term 
-0000e1b0: 3c3d 2060 7465 726d 6020 616e 6420 6c6f  <= `term` and lo
-0000e1c0: 672e 696e 6465 7820 3c3d 2060 696e 6465  g.index <= `inde
-0000e1d0: 7860 2e20 4966 206e 6f20 7375 6368 2069  x`. If no such i
-0000e1e0: 6e64 6578 2065 7869 7374 730a 2020 2020  ndex exists.    
-0000e1f0: 2020 2020 696e 2074 6865 206c 6f67 2c20      in the log, 
-0000e200: 7468 6520 6c6f 6727 7320 6669 7273 7420  the log's first 
-0000e210: 696e 6465 7820 6973 2072 6574 7572 6e65  index is returne
-0000e220: 642e 0a0a 2020 2020 2020 2020 5468 6520  d...        The 
-0000e230: 696e 6465 7820 7072 6f76 6964 6564 204d  index provided M
-0000e240: 5553 5420 6265 2065 7175 616c 2074 6f20  UST be equal to 
-0000e250: 6f72 206c 6573 7320 7468 616e 2073 656c  or less than sel
-0000e260: 662e 6c61 7374 5f69 6e64 6578 2829 2e20  f.last_index(). 
-0000e270: 496e 7661 6c69 640a 2020 2020 2020 2020  Invalid.        
-0000e280: 696e 7075 7473 206c 6f67 2061 2077 6172  inputs log a war
-0000e290: 6e69 6e67 2061 6e64 2074 6865 2069 6e70  ning and the inp
-0000e2a0: 7574 2069 6e64 6578 2069 7320 7265 7475  ut index is retu
-0000e2b0: 726e 6564 2e0a 0a20 2020 2020 2020 2052  rned...        R
-0000e2c0: 6574 7572 6e20 2869 6e64 6578 2c20 7465  eturn (index, te
-0000e2d0: 726d 290a 2020 2020 2020 2020 2222 220a  rm).        """.
-0000e2e0: 2020 2020 6465 6620 636f 6d6d 6974 5f74      def commit_t
-0000e2f0: 6f28 7365 6c66 2c20 746f 5f63 6f6d 6d69  o(self, to_commi
-0000e300: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-0000e310: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000e320: 2020 2020 2053 6574 7320 7468 6520 6c61       Sets the la
-0000e330: 7374 2063 6f6d 6d69 7474 6564 2076 616c  st committed val
-0000e340: 7565 2074 6f20 7468 6520 7061 7373 6564  ue to the passed
-0000e350: 2069 6e20 7661 6c75 652e 0a0a 2020 2020   in value...    
-0000e360: 2020 2020 2320 5061 6e69 6373 0a0a 2020      # Panics..  
-0000e370: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
-0000e380: 7468 6520 696e 6465 7820 676f 6573 2070  the index goes p
-0000e390: 6173 7420 7468 6520 6c61 7374 2069 6e64  ast the last ind
-0000e3a0: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
-0000e3b0: 2020 2020 6465 6620 636f 6d6d 6974 5f69      def commit_i
-0000e3c0: 6e66 6f28 7365 6c66 2920 2d3e 2054 7570  nfo(self) -> Tup
-0000e3d0: 6c65 5b69 6e74 2c20 696e 745d 3a0a 2020  le[int, int]:.  
-0000e3e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e3f0: 2020 5265 7475 726e 7320 7468 6520 636f    Returns the co
-0000e400: 6d6d 6974 7465 6420 696e 6465 7820 616e  mmitted index an
-0000e410: 6420 6974 7320 7465 726d 2e0a 2020 2020  d its term..    
-0000e420: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000e430: 7374 6f72 6528 7365 6c66 2920 2d3e 2022  store(self) -> "
-0000e440: 4d65 6d53 746f 7261 6765 5265 6622 3a0a  MemStorageRef":.
-0000e450: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000e460: 2020 2020 6465 6620 6e65 7874 5f65 6e74      def next_ent
-0000e470: 7269 6573 2873 656c 662c 206d 6178 5f73  ries(self, max_s
-0000e480: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
-0000e490: 745d 2920 2d3e 204f 7074 696f 6e61 6c5b  t]) -> Optional[
-0000e4a0: 4c69 7374 5b22 456e 7472 7922 5d5d 3a0a  List["Entry"]]:.
-0000e4b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e4c0: 2020 2020 5265 7475 726e 7320 616c 6c20      Returns all 
-0000e4d0: 7468 6520 6176 6169 6c61 626c 6520 656e  the available en
-0000e4e0: 7472 6965 7320 666f 7220 6578 6563 7574  tries for execut
-0000e4f0: 696f 6e2e 0a20 2020 2020 2020 2049 6620  ion..        If 
-0000e500: 6170 706c 6965 6420 6973 2073 6d61 6c6c  applied is small
-0000e510: 6572 2074 6861 6e20 7468 6520 696e 6465  er than the inde
-0000e520: 7820 6f66 2073 6e61 7073 686f 742c 2069  x of snapshot, i
-0000e530: 7420 7265 7475 726e 7320 616c 6c20 636f  t returns all co
-0000e540: 6d6d 6974 7465 640a 2020 2020 2020 2020  mmitted.        
-0000e550: 656e 7472 6965 7320 6166 7465 7220 7468  entries after th
-0000e560: 6520 696e 6465 7820 6f66 2073 6e61 7073  e index of snaps
-0000e570: 686f 742e 0a20 2020 2020 2020 2022 2222  hot..        """
-0000e580: 0a20 2020 2064 6566 206e 6578 745f 656e  .    def next_en
-0000e590: 7472 6965 735f 7369 6e63 6528 0a20 2020  tries_since(.   
-0000e5a0: 2020 2020 2073 656c 662c 2073 696e 6365       self, since
-0000e5b0: 5f69 6478 3a20 696e 742c 206d 6178 5f73  _idx: int, max_s
-0000e5c0: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
-0000e5d0: 745d 0a20 2020 2029 202d 3e20 4f70 7469  t].    ) -> Opti
-0000e5e0: 6f6e 616c 5b4c 6973 745b 2245 6e74 7279  onal[List["Entry
-0000e5f0: 225d 5d3a 0a20 2020 2020 2020 2022 2222  "]]:.        """
-0000e600: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000e610: 2063 6f6d 6d69 7474 6564 2061 6e64 2070   committed and p
-0000e620: 6572 7369 7374 6564 2065 6e74 7269 6573  ersisted entries
-0000e630: 2073 696e 6365 206d 6178 2860 7369 6e63   since max(`sinc
-0000e640: 655f 6964 7860 202b 2031 2c20 6669 7273  e_idx` + 1, firs
-0000e650: 745f 696e 6465 7829 2e0a 2020 2020 2020  t_index)..      
-0000e660: 2020 2222 220a 2020 2020 6465 6620 6861    """.    def ha
-0000e670: 735f 6e65 7874 5f65 6e74 7269 6573 2873  s_next_entries(s
-0000e680: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-0000e690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e6a0: 2020 5265 7475 726e 7320 7768 6574 6865    Returns whethe
-0000e6b0: 7220 7468 6572 6520 6172 6520 6e65 7720  r there are new 
-0000e6c0: 656e 7472 6965 732e 0a20 2020 2020 2020  entries..       
-0000e6d0: 2022 2222 0a20 2020 2064 6566 2068 6173   """.    def has
-0000e6e0: 5f6e 6578 745f 656e 7472 6965 735f 7369  _next_entries_si
-0000e6f0: 6e63 6528 7365 6c66 2c20 7369 6e63 655f  nce(self, since_
-0000e700: 6964 783a 2069 6e74 2920 2d3e 2062 6f6f  idx: int) -> boo
-0000e710: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-0000e720: 2020 2020 2020 2052 6574 7572 6e73 2077         Returns w
-0000e730: 6865 7468 6572 2074 6865 7265 2061 7265  hether there are
-0000e740: 2063 6f6d 6d69 7474 6564 2061 6e64 2070   committed and p
-0000e750: 6572 7369 7374 6564 2065 6e74 7269 6573  ersisted entries
-0000e760: 2073 696e 6365 0a20 2020 2020 2020 206d   since.        m
-0000e770: 6178 2860 7369 6e63 655f 6964 7860 202b  ax(`since_idx` +
-0000e780: 2031 2c20 6669 7273 745f 696e 6465 7829   1, first_index)
-0000e790: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000e7a0: 2020 6465 6620 6973 5f75 705f 746f 5f64    def is_up_to_d
-0000e7b0: 6174 6528 7365 6c66 2c20 6c61 7374 5f69  ate(self, last_i
-0000e7c0: 6e64 6578 3a20 696e 742c 2074 6572 6d3a  ndex: int, term:
-0000e7d0: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
-0000e7e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e7f0: 2020 2044 6574 6572 6d69 6e65 7320 6966     Determines if
-0000e800: 2074 6865 2067 6976 656e 2028 6c61 7374   the given (last
-0000e810: 496e 6465 782c 7465 726d 2920 6c6f 6720  Index,term) log 
-0000e820: 6973 206d 6f72 6520 7570 2d74 6f2d 6461  is more up-to-da
-0000e830: 7465 0a20 2020 2020 2020 2062 7920 636f  te.        by co
-0000e840: 6d70 6172 696e 6720 7468 6520 696e 6465  mparing the inde
-0000e850: 7820 616e 6420 7465 726d 206f 6620 7468  x and term of th
-0000e860: 6520 6c61 7374 2065 6e74 7279 2069 6e20  e last entry in 
-0000e870: 7468 6520 6578 6973 7469 6e67 206c 6f67  the existing log
-0000e880: 732e 0a20 2020 2020 2020 2049 6620 7468  s..        If th
-0000e890: 6520 6c6f 6773 2068 6176 6520 6c61 7374  e logs have last
-0000e8a0: 2065 6e74 7279 2077 6974 6820 6469 6666   entry with diff
-0000e8b0: 6572 656e 7420 7465 726d 732c 2074 6865  erent terms, the
-0000e8c0: 6e20 7468 6520 6c6f 6720 7769 7468 2074  n the log with t
-0000e8d0: 6865 0a20 2020 2020 2020 206c 6174 6572  he.        later
-0000e8e0: 2074 6572 6d20 6973 206d 6f72 6520 7570   term is more up
-0000e8f0: 2d74 6f2d 6461 7465 2e20 4966 2074 6865  -to-date. If the
-0000e900: 206c 6f67 7320 656e 6420 7769 7468 2074   logs end with t
-0000e910: 6865 2073 616d 6520 7465 726d 2c20 7468  he same term, th
-0000e920: 656e 0a20 2020 2020 2020 2077 6869 6368  en.        which
-0000e930: 6576 6572 206c 6f67 2068 6173 2074 6865  ever log has the
-0000e940: 206c 6172 6765 7220 6c61 7374 5f69 6e64   larger last_ind
-0000e950: 6578 2069 7320 6d6f 7265 2075 702d 746f  ex is more up-to
-0000e960: 2d64 6174 652e 2049 6620 7468 6520 6c6f  -date. If the lo
-0000e970: 6773 2061 7265 0a20 2020 2020 2020 2074  gs are.        t
-0000e980: 6865 2073 616d 652c 2074 6865 2067 6976  he same, the giv
-0000e990: 656e 206c 6f67 2069 7320 7570 2d74 6f2d  en log is up-to-
-0000e9a0: 6461 7465 2e0a 2020 2020 2020 2020 2222  date..        ""
-0000e9b0: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
-0000e9c0: 636f 6d6d 6974 2873 656c 662c 206d 6178  commit(self, max
-0000e9d0: 5f69 6e64 6578 3a20 696e 742c 2074 6572  _index: int, ter
-0000e9e0: 6d3a 2069 6e74 2920 2d3e 2062 6f6f 6c3a  m: int) -> bool:
-0000e9f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ea00: 2020 2020 2041 7474 656d 7074 7320 746f       Attempts to
-0000ea10: 2063 6f6d 6d69 7420 7468 6520 696e 6465   commit the inde
-0000ea20: 7820 616e 6420 7465 726d 2061 6e64 2072  x and term and r
-0000ea30: 6574 7572 6e73 2077 6865 7468 6572 2069  eturns whether i
-0000ea40: 7420 6469 642e 0a20 2020 2020 2020 2022  t did..        "
-0000ea50: 2222 0a20 2020 2064 6566 206d 6179 6265  "".    def maybe
-0000ea60: 5f70 6572 7369 7374 2873 656c 662c 2069  _persist(self, i
-0000ea70: 6e64 6578 3a20 696e 742c 2074 6572 6d3a  ndex: int, term:
-0000ea80: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
-0000ea90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000eaa0: 2020 2041 7474 656d 7074 7320 746f 2070     Attempts to p
-0000eab0: 6572 7369 7374 2074 6865 2069 6e64 6578  ersist the index
-0000eac0: 2061 6e64 2074 6572 6d20 616e 6420 7265   and term and re
-0000ead0: 7475 726e 7320 7768 6574 6865 7220 6974  turns whether it
-0000eae0: 2064 6964 2e0a 2020 2020 2020 2020 2222   did..        ""
-0000eaf0: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
-0000eb00: 7065 7273 6973 745f 736e 6170 2873 656c  persist_snap(sel
-0000eb10: 662c 2069 6e64 6578 3a20 696e 7429 202d  f, index: int) -
-0000eb20: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-0000eb30: 2222 220a 2020 2020 2020 2020 4174 7465  """.        Atte
-0000eb40: 6d70 7473 2074 6f20 7065 7273 6973 7420  mpts to persist 
-0000eb50: 7468 6520 736e 6170 7368 6f74 2061 6e64  the snapshot and
-0000eb60: 2072 6574 7572 6e73 2077 6865 7468 6572   returns whether
-0000eb70: 2069 7420 6469 642e 0a20 2020 2020 2020   it did..       
-0000eb80: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
-0000eb90: 6265 5f61 7070 656e 6428 0a20 2020 2020  be_append(.     
-0000eba0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000ebb0: 2069 6478 3a20 696e 742c 0a20 2020 2020   idx: int,.     
-0000ebc0: 2020 2074 6572 6d3a 2069 6e74 2c0a 2020     term: int,.  
-0000ebd0: 2020 2020 2020 636f 6d6d 6974 7465 643a        committed:
-0000ebe0: 2069 6e74 2c0a 2020 2020 2020 2020 656e   int,.        en
-0000ebf0: 7473 3a20 4c69 7374 5b22 456e 7472 7922  ts: List["Entry"
-0000ec00: 5d20 7c20 4c69 7374 5b22 456e 7472 7952  ] | List["EntryR
-0000ec10: 6566 225d 2c0a 2020 2020 2920 2d3e 204f  ef"],.    ) -> O
-0000ec20: 7074 696f 6e61 6c5b 5475 706c 655b 696e  ptional[Tuple[in
-0000ec30: 742c 2069 6e74 5d5d 3a0a 2020 2020 2020  t, int]]:.      
-0000ec40: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0000ec50: 7475 726e 7320 4e6f 6e65 2069 6620 7468  turns None if th
-0000ec60: 6520 656e 7472 6965 7320 6361 6e6e 6f74  e entries cannot
-0000ec70: 2062 6520 6170 7065 6e64 6564 2e20 4f74   be appended. Ot
-0000ec80: 6865 7277 6973 652c 0a20 2020 2020 2020  herwise,.       
-0000ec90: 2069 7420 7265 7475 726e 7320 536f 6d65   it returns Some
-0000eca0: 2828 636f 6e66 6c69 6374 5f69 6e64 6578  ((conflict_index
-0000ecb0: 2c20 6c61 7374 5f69 6e64 6578 2929 2e0a  , last_index))..
-0000ecc0: 0a20 2020 2020 2020 2023 2050 616e 6963  .        # Panic
-0000ecd0: 730a 0a20 2020 2020 2020 2050 616e 6963  s..        Panic
-0000ece0: 7320 6966 2069 7420 6669 6e64 7320 6120  s if it finds a 
-0000ecf0: 636f 6e66 6c69 6374 696e 6720 696e 6465  conflicting inde
-0000ed00: 7820 6c65 7373 2074 6861 6e20 636f 6d6d  x less than comm
-0000ed10: 6974 7465 6420 696e 6465 782e 0a20 2020  itted index..   
-0000ed20: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000ed30: 2073 6e61 7073 686f 7428 7365 6c66 2c20   snapshot(self, 
-0000ed40: 7265 7175 6573 745f 696e 6465 783a 2069  request_index: i
-0000ed50: 6e74 2c20 746f 3a20 696e 7429 202d 3e20  nt, to: int) -> 
-0000ed60: 2253 6e61 7073 686f 7452 6566 223a 0a20  "SnapshotRef":. 
-0000ed70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ed80: 2020 2052 6574 7572 6e73 2074 6865 2063     Returns the c
-0000ed90: 7572 7265 6e74 2073 6e61 7073 686f 740a  urrent snapshot.
-0000eda0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000edb0: 6465 6620 7374 6162 6c65 5f65 6e74 7269  def stable_entri
-0000edc0: 6573 2873 656c 662c 2069 6e64 6578 3a20  es(self, index: 
-0000edd0: 696e 742c 2074 6572 6d3a 2069 6e74 2920  int, term: int) 
-0000ede0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000edf0: 2022 2222 0a20 2020 2020 2020 2043 6c65   """.        Cle
-0000ee00: 6172 7320 7468 6520 756e 7374 6162 6c65  ars the unstable
-0000ee10: 2065 6e74 7269 6573 2061 6e64 206d 6f76   entries and mov
-0000ee20: 6573 2074 6865 2073 7461 626c 6520 6f66  es the stable of
-0000ee30: 6673 6574 2075 7020 746f 2074 6865 0a20  fset up to the. 
-0000ee40: 2020 2020 2020 206c 6173 7420 696e 6465         last inde
-0000ee50: 782c 2069 6620 7468 6572 6520 6973 2061  x, if there is a
-0000ee60: 6e79 2e0a 2020 2020 2020 2020 2222 220a  ny..        """.
-0000ee70: 2020 2020 6465 6620 7374 6162 6c65 5f73      def stable_s
-0000ee80: 6e61 7028 7365 6c66 2c20 696e 6465 783a  nap(self, index:
-0000ee90: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-0000eea0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000eeb0: 2020 2043 6c65 6172 7320 7468 6520 756e     Clears the un
-0000eec0: 7374 6162 6c65 2073 6e61 7073 686f 742e  stable snapshot.
-0000eed0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000eee0: 2064 6566 2074 6572 6d28 7365 6c66 2c20   def term(self, 
-0000eef0: 6964 783a 2069 6e74 2920 2d3e 2069 6e74  idx: int) -> int
+00001840: 2022 2222 2022 2222 0a0a 2020 2020 6465   """ """..    de
+00001850: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00001860: 2020 2020 7365 6c66 2c20 6368 616e 5f73      self, chan_s
+00001870: 697a 653a 2069 6e74 2c20 6f76 6572 666c  ize: int, overfl
+00001880: 6f77 5f73 7472 6174 6567 793a 2022 4f76  ow_strategy: "Ov
+00001890: 6572 666c 6f77 5374 7261 7465 6779 220a  erflowStrategy".
+000018a0: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
+000018b0: 2e2e 0a0a 636c 6173 7320 5f5f 4150 495f  ....class __API_
+000018c0: 5261 6674 5374 6174 6528 5f5f 436c 6f6e  RaftState(__Clon
+000018d0: 6561 626c 6529 3a0a 2020 2020 6465 6620  eable):.    def 
+000018e0: 636c 6f6e 6528 7365 6c66 2920 2d3e 2022  clone(self) -> "
+000018f0: 5261 6674 5374 6174 6522 3a20 2e2e 2e0a  RaftState": ....
+00001900: 2020 2020 6465 6620 696e 6974 6961 6c69      def initiali
+00001910: 7a65 6428 7365 6c66 2920 2d3e 2062 6f6f  zed(self) -> boo
+00001920: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00001930: 2020 2020 2020 2049 6e64 6963 6174 6573         Indicates
+00001940: 2074 6865 2060 5261 6674 5374 6174 6560   the `RaftState`
+00001950: 2069 7320 696e 6974 6961 6c69 7a65 6420   is initialized 
+00001960: 6f72 206e 6f74 2e0a 2020 2020 2020 2020  or not..        
+00001970: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00001980: 636f 6e66 5f73 7461 7465 2873 656c 6629  conf_state(self)
+00001990: 202d 3e20 2243 6f6e 6653 7461 7465 5265   -> "ConfStateRe
+000019a0: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
+000019b0: 2020 2020 2020 2020 6063 6f6e 665f 7374          `conf_st
+000019c0: 6174 6560 3a20 5265 636f 7264 7320 7468  ate`: Records th
+000019d0: 6520 6375 7272 656e 7420 6e6f 6465 2049  e current node I
+000019e0: 4473 206c 696b 6520 605b 312c 2032 2c20  Ds like `[1, 2, 
+000019f0: 335d 6020 696e 2074 6865 2063 6c75 7374  3]` in the clust
+00001a00: 6572 2e20 4576 6572 7920 5261 6674 206e  er. Every Raft n
+00001a10: 6f64 6520 6d75 7374 2068 6176 6520 610a  ode must have a.
+00001a20: 2020 2020 2020 2020 756e 6971 7565 2049          unique I
+00001a30: 4420 696e 2074 6865 2063 6c75 7374 6572  D in the cluster
+00001a40: 3b0a 2020 2020 2020 2020 2222 220a 2020  ;.        """.  
+00001a50: 2020 6465 6620 7365 745f 636f 6e66 5f73    def set_conf_s
+00001a60: 7461 7465 2873 656c 662c 2063 733a 2022  tate(self, cs: "
+00001a70: 436f 6e66 5374 6174 6552 6566 2229 202d  ConfStateRef") -
+00001a80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001a90: 2222 220a 2020 2020 2020 2020 6063 6f6e  """.        `con
+00001aa0: 665f 7374 6174 6560 3a20 5265 636f 7264  f_state`: Record
+00001ab0: 7320 7468 6520 6375 7272 656e 7420 6e6f  s the current no
+00001ac0: 6465 2049 4473 206c 696b 6520 605b 312c  de IDs like `[1,
+00001ad0: 2032 2c20 335d 6020 696e 2074 6865 2063   2, 3]` in the c
+00001ae0: 6c75 7374 6572 2e20 4576 6572 7920 5261  luster. Every Ra
+00001af0: 6674 206e 6f64 6520 6d75 7374 2068 6176  ft node must hav
+00001b00: 6520 610a 2020 2020 2020 2020 756e 6971  e a.        uniq
+00001b10: 7565 2049 4420 696e 2074 6865 2063 6c75  ue ID in the clu
+00001b20: 7374 6572 3b0a 2020 2020 2020 2020 2222  ster;.        ""
+00001b30: 220a 2020 2020 6465 6620 6765 745f 6861  ".    def get_ha
+00001b40: 7264 5f73 7461 7465 2873 656c 6629 202d  rd_state(self) -
+00001b50: 3e20 2248 6172 6453 7461 7465 5265 6622  > "HardStateRef"
+00001b60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00001b70: 2020 2020 2020 6068 6172 645f 7374 6174        `hard_stat
+00001b80: 6560 3a20 436f 6e74 6169 6e73 2074 6865  e`: Contains the
+00001b90: 206c 6173 7420 6d65 7461 2069 6e66 6f72   last meta infor
+00001ba0: 6d61 7469 6f6e 2069 6e63 6c75 6469 6e67  mation including
+00001bb0: 2063 6f6d 6d69 7420 696e 6465 782c 2074   commit index, t
+00001bc0: 6865 2076 6f74 6520 6c65 6164 6572 2c20  he vote leader, 
+00001bd0: 616e 6420 7468 6520 766f 7465 2074 6572  and the vote ter
+00001be0: 6d2e 0a20 2020 2020 2020 2022 2222 0a20  m..        """. 
+00001bf0: 2020 2064 6566 2073 6574 5f68 6172 645f     def set_hard_
+00001c00: 7374 6174 6528 7365 6c66 2c20 6873 3a20  state(self, hs: 
+00001c10: 2248 6172 6453 7461 7465 5265 6622 2920  "HardStateRef") 
+00001c20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00001c30: 2022 2222 0a20 2020 2020 2020 2060 6861   """.        `ha
+00001c40: 7264 5f73 7461 7465 603a 2043 6f6e 7461  rd_state`: Conta
+00001c50: 696e 7320 7468 6520 6c61 7374 206d 6574  ins the last met
+00001c60: 6120 696e 666f 726d 6174 696f 6e20 696e  a information in
+00001c70: 636c 7564 696e 6720 636f 6d6d 6974 2069  cluding commit i
+00001c80: 6e64 6578 2c20 7468 6520 766f 7465 206c  ndex, the vote l
+00001c90: 6561 6465 722c 2061 6e64 2074 6865 2076  eader, and the v
+00001ca0: 6f74 6520 7465 726d 2e0a 2020 2020 2020  ote term..      
+00001cb0: 2020 2222 220a 0a63 6c61 7373 2052 6166    """..class Raf
+00001cc0: 7453 7461 7465 285f 5f41 5049 5f52 6166  tState(__API_Raf
+00001cd0: 7453 7461 7465 293a 0a20 2020 2022 2222  tState):.    """
+00001ce0: 0a20 2020 2048 6f6c 6473 2062 6f74 6820  .    Holds both 
+00001cf0: 7468 6520 6861 7264 2073 7461 7465 2028  the hard state (
+00001d00: 636f 6d6d 6974 2069 6e64 6578 2c20 766f  commit index, vo
+00001d10: 7465 206c 6561 6465 722c 2074 6572 6d29  te leader, term)
+00001d20: 2061 6e64 2074 6865 2063 6f6e 6669 6775   and the configu
+00001d30: 7261 7469 6f6e 2073 7461 7465 0a20 2020  ration state.   
+00001d40: 2028 4375 7272 656e 7420 6e6f 6465 2049   (Current node I
+00001d50: 4473 290a 2020 2020 2222 220a 0a20 2020  Ds).    """..   
+00001d60: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00001d70: 6c66 2920 2d3e 204e 6f6e 653a 202e 2e2e  lf) -> None: ...
+00001d80: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
+00001d90: 6628 7365 6c66 2920 2d3e 2022 5261 6674  f(self) -> "Raft
+00001da0: 5374 6174 6552 6566 223a 202e 2e2e 0a20  StateRef": .... 
+00001db0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00001dc0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
+00001dd0: 2829 202d 3e20 2252 6166 7453 7461 7465  () -> "RaftState
+00001de0: 223a 202e 2e2e 0a0a 636c 6173 7320 5261  ": .....class Ra
+00001df0: 6674 5374 6174 6552 6566 285f 5f41 5049  ftStateRef(__API
+00001e00: 5f52 6166 7453 7461 7465 293a 0a20 2020  _RaftState):.   
+00001e10: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
+00001e20: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
+00001e30: 733a 6052 6166 7453 7461 7465 602e 0a20  s:`RaftState`.. 
+00001e40: 2020 2022 2222 0a0a 636c 6173 7320 5f5f     """..class __
+00001e50: 4150 495f 5374 6f72 6167 6543 6f72 653a  API_StorageCore:
+00001e60: 0a20 2020 2064 6566 2061 7070 656e 6428  .    def append(
+00001e70: 7365 6c66 2c20 656e 7473 3a20 4c69 7374  self, ents: List
+00001e80: 5b22 456e 7472 7922 5d20 7c20 4c69 7374  ["Entry"] | List
+00001e90: 5b22 456e 7472 7952 6566 225d 2920 2d3e  ["EntryRef"]) ->
+00001ea0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00001eb0: 2222 0a20 2020 2020 2020 2041 7070 656e  "".        Appen
+00001ec0: 6420 7468 6520 6e65 7720 656e 7472 6965  d the new entrie
+00001ed0: 7320 746f 2073 746f 7261 6765 2e0a 0a20  s to storage... 
+00001ee0: 2020 2020 2020 2023 2050 616e 6963 730a         # Panics.
+00001ef0: 0a20 2020 2020 2020 2050 616e 6963 7320  .        Panics 
+00001f00: 6966 2060 656e 7473 6020 636f 6e74 6169  if `ents` contai
+00001f10: 6e73 2063 6f6d 7061 6374 6564 2065 6e74  ns compacted ent
+00001f20: 7269 6573 2c20 6f72 2074 6865 7265 2773  ries, or there's
+00001f30: 2061 2067 6170 2062 6574 7765 656e 2060   a gap between `
+00001f40: 656e 7473 6020 616e 6420 7468 6520 6c61  ents` and the la
+00001f50: 7374 0a20 2020 2020 2020 2072 6563 6569  st.        recei
+00001f60: 7665 6420 656e 7472 7920 696e 2074 6865  ved entry in the
+00001f70: 2073 746f 7261 6765 2e0a 2020 2020 2020   storage..      
+00001f80: 2020 2222 220a 2020 2020 6465 6620 6170    """.    def ap
+00001f90: 706c 795f 736e 6170 7368 6f74 2873 656c  ply_snapshot(sel
+00001fa0: 662c 2073 6e61 7073 686f 743a 2022 536e  f, snapshot: "Sn
+00001fb0: 6170 7368 6f74 2220 7c20 2253 6e61 7073  apshot" | "Snaps
+00001fc0: 686f 7452 6566 2229 202d 3e20 4e6f 6e65  hotRef") -> None
+00001fd0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00001fe0: 2020 2020 2020 4f76 6572 7772 6974 6573        Overwrites
+00001ff0: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
+00002000: 2074 6869 7320 5374 6f72 6167 6520 6f62   this Storage ob
+00002010: 6a65 6374 2077 6974 6820 7468 6f73 6520  ject with those 
+00002020: 6f66 2074 6865 2067 6976 656e 2073 6e61  of the given sna
+00002030: 7073 686f 742e 0a0a 2020 2020 2020 2020  pshot...        
+00002040: 2320 5061 6e69 6373 0a0a 2020 2020 2020  # Panics..      
+00002050: 2020 5061 6e69 6373 2069 6620 7468 6520    Panics if the 
+00002060: 736e 6170 7368 6f74 2069 6e64 6578 2069  snapshot index i
+00002070: 7320 6c65 7373 2074 6861 6e20 7468 6520  s less than the 
+00002080: 7374 6f72 6167 6527 7320 6669 7273 7420  storage's first 
+00002090: 696e 6465 782e 0a20 2020 2020 2020 2022  index..        "
+000020a0: 2222 0a20 2020 2064 6566 2063 6f6d 7061  "".    def compa
+000020b0: 6374 2873 656c 662c 2063 6f6d 7061 6374  ct(self, compact
+000020c0: 5f69 6e64 6578 3a20 696e 7429 202d 3e20  _index: int) -> 
+000020d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000020e0: 220a 2020 2020 2020 2020 4469 7363 6172  ".        Discar
+000020f0: 6473 2061 6c6c 206c 6f67 2065 6e74 7269  ds all log entri
+00002100: 6573 2070 7269 6f72 2074 6f20 636f 6d70  es prior to comp
+00002110: 6163 745f 696e 6465 782e 0a20 2020 2020  act_index..     
+00002120: 2020 2049 7420 6973 2074 6865 2061 7070     It is the app
+00002130: 6c69 6361 7469 6f6e 2773 2072 6573 706f  lication's respo
+00002140: 6e73 6962 696c 6974 7920 746f 206e 6f74  nsibility to not
+00002150: 2061 7474 656d 7074 2074 6f20 636f 6d70   attempt to comp
+00002160: 6163 7420 616e 2069 6e64 6578 0a20 2020  act an index.   
+00002170: 2020 2020 2067 7265 6174 6572 2074 6861       greater tha
+00002180: 6e20 5261 6674 4c6f 672e 6170 706c 6965  n RaftLog.applie
+00002190: 642e 0a0a 2020 2020 2020 2020 2320 5061  d...        # Pa
+000021a0: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
+000021b0: 6e69 6373 2069 6620 6063 6f6d 7061 6374  nics if `compact
+000021c0: 5f69 6e64 6578 6020 6973 2068 6967 6865  _index` is highe
+000021d0: 7220 7468 616e 2060 5374 6f72 6167 653a  r than `Storage:
+000021e0: 3a6c 6173 745f 696e 6465 7828 2673 656c  :last_index(&sel
+000021f0: 6629 202b 2031 602e 0a20 2020 2020 2020  f) + 1`..       
+00002200: 2022 2222 0a20 2020 2064 6566 2063 6f6d   """.    def com
+00002210: 6d69 745f 746f 2873 656c 662c 2069 6e64  mit_to(self, ind
+00002220: 6578 3a20 696e 7429 202d 3e20 4e6f 6e65  ex: int) -> None
+00002230: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00002240: 2020 2020 2020 436f 6d6d 6974 2074 6f20        Commit to 
+00002250: 616e 2069 6e64 6578 2e0a 0a20 2020 2020  an index...     
+00002260: 2020 2023 2050 616e 6963 730a 0a20 2020     # Panics..   
+00002270: 2020 2020 2050 616e 6963 7320 6966 2074       Panics if t
+00002280: 6865 7265 2069 7320 6e6f 2073 7563 6820  here is no such 
+00002290: 656e 7472 7920 696e 2072 6166 7420 6c6f  entry in raft lo
+000022a0: 6773 2e0a 2020 2020 2020 2020 2222 220a  gs..        """.
+000022b0: 2020 2020 6465 6620 636f 6d6d 6974 5f74      def commit_t
+000022c0: 6f5f 616e 645f 7365 745f 636f 6e66 5f73  o_and_set_conf_s
+000022d0: 7461 7465 7328 0a20 2020 2020 2020 2073  tates(.        s
+000022e0: 656c 662c 2069 6478 3a20 696e 742c 2063  elf, idx: int, c
+000022f0: 733a 204f 7074 696f 6e61 6c5b 2243 6f6e  s: Optional["Con
+00002300: 6653 7461 7465 225d 207c 204f 7074 696f  fState"] | Optio
+00002310: 6e61 6c5b 2243 6f6e 6653 7461 7465 5265  nal["ConfStateRe
+00002320: 6622 5d0a 2020 2020 2920 2d3e 204e 6f6e  f"].    ) -> Non
+00002330: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00002340: 2020 2020 2020 2043 6f6d 6d69 7420 746f         Commit to
+00002350: 2060 6964 7860 2061 6e64 2073 6574 2063   `idx` and set c
+00002360: 6f6e 6669 6775 7261 7469 6f6e 2074 6f20  onfiguration to 
+00002370: 7468 6520 6769 7665 6e20 7374 6174 6573  the given states
+00002380: 2e20 4f6e 6c79 2075 7365 6420 666f 7220  . Only used for 
+00002390: 7465 7374 732e 0a20 2020 2020 2020 2022  tests..        "
+000023a0: 2222 0a20 2020 2064 6566 2073 6574 5f63  "".    def set_c
+000023b0: 6f6e 665f 7374 6174 6528 7365 6c66 2c20  onf_state(self, 
+000023c0: 6373 3a20 2243 6f6e 6653 7461 7465 2220  cs: "ConfState" 
+000023d0: 7c20 2243 6f6e 6653 7461 7465 5265 6622  | "ConfStateRef"
+000023e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000023f0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00002400: 6176 6573 2074 6865 2063 7572 7265 6e74  aves the current
+00002410: 2063 6f6e 6620 7374 6174 652e 0a20 2020   conf state..   
+00002420: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00002430: 2068 6172 645f 7374 6174 6528 7365 6c66   hard_state(self
+00002440: 2920 2d3e 2022 4861 7264 5374 6174 6552  ) -> "HardStateR
+00002450: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
+00002460: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+00002470: 2068 6172 6420 7374 6174 652e 0a20 2020   hard state..   
+00002480: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00002490: 2073 6574 5f68 6172 6473 7461 7465 2873   set_hardstate(s
+000024a0: 656c 662c 2068 733a 2022 4861 7264 5374  elf, hs: "HardSt
+000024b0: 6174 6522 207c 2022 4861 7264 5374 6174  ate" | "HardStat
+000024c0: 6552 6566 2229 202d 3e20 4e6f 6e65 3a0a  eRef") -> None:.
+000024d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000024e0: 2020 2020 5361 7665 7320 7468 6520 6375      Saves the cu
+000024f0: 7272 656e 7420 4861 7264 5374 6174 652e  rrent HardState.
+00002500: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002510: 2064 6566 2074 7269 6767 6572 5f73 6e61   def trigger_sna
+00002520: 705f 756e 6176 6169 6c61 626c 6528 7365  p_unavailable(se
+00002530: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00002540: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002550: 2054 7269 6767 6572 2061 2053 6e61 7073   Trigger a Snaps
+00002560: 686f 7454 656d 706f 7261 7269 6c79 556e  hotTemporarilyUn
+00002570: 6176 6169 6c61 626c 6520 6572 726f 722e  available error.
+00002580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002590: 2064 6566 2074 7269 6767 6572 5f6c 6f67   def trigger_log
+000025a0: 5f75 6e61 7661 696c 6162 6c65 2873 656c  _unavailable(sel
+000025b0: 662c 2076 3a20 626f 6f6c 2920 2d3e 204e  f, v: bool) -> N
+000025c0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000025d0: 0a20 2020 2020 2020 2053 6574 2061 204c  .        Set a L
+000025e0: 6f67 5465 6d70 6f72 6172 696c 7955 6e61  ogTemporarilyUna
+000025f0: 7661 696c 6162 6c65 2065 7272 6f72 2e0a  vailable error..
+00002600: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002610: 6465 6620 7461 6b65 5f67 6574 5f65 6e74  def take_get_ent
+00002620: 7269 6573 5f63 6f6e 7465 7874 2873 656c  ries_context(sel
+00002630: 6629 202d 3e20 4f70 7469 6f6e 616c 5b22  f) -> Optional["
+00002640: 4765 7445 6e74 7269 6573 436f 6e74 6578  GetEntriesContex
+00002650: 7422 5d3a 0a20 2020 2020 2020 2022 2222  t"]:.        """
+00002660: 0a20 2020 2020 2020 2054 616b 6520 6765  .        Take ge
+00002670: 7420 656e 7472 6965 7320 636f 6e74 6578  t entries contex
+00002680: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
+00002690: 636c 6173 7320 4d65 6d53 746f 7261 6765  class MemStorage
+000026a0: 436f 7265 285f 5f41 5049 5f53 746f 7261  Core(__API_Stora
+000026b0: 6765 436f 7265 293a 0a20 2020 2022 2222  geCore):.    """
+000026c0: 0a20 2020 2054 6865 204d 656d 6f72 7920  .    The Memory 
+000026d0: 5374 6f72 6167 6520 436f 7265 2069 6e73  Storage Core ins
+000026e0: 7461 6e63 6520 686f 6c64 7320 7468 6520  tance holds the 
+000026f0: 6163 7475 616c 2073 7461 7465 206f 6620  actual state of 
+00002700: 7468 6520 7374 6f72 6167 6520 7374 7275  the storage stru
+00002710: 6374 2e20 546f 2061 6363 6573 7320 7468  ct. To access th
+00002720: 6973 0a20 2020 2076 616c 7565 2c20 7573  is.    value, us
+00002730: 6520 7468 6520 6072 6c60 2061 6e64 2060  e the `rl` and `
+00002740: 776c 6020 6675 6e63 7469 6f6e 7320 6f6e  wl` functions on
+00002750: 2074 6865 206d 6169 6e20 4d65 6d53 746f   the main MemSto
+00002760: 7261 6765 2069 6d70 6c65 6d65 6e74 6174  rage implementat
+00002770: 696f 6e2e 0a20 2020 2022 2222 0a0a 2020  ion..    """..  
+00002780: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
+00002790: 656c 6629 202d 3e20 224d 656d 5374 6f72  elf) -> "MemStor
+000027a0: 6167 6543 6f72 6552 6566 223a 202e 2e2e  ageCoreRef": ...
+000027b0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+000027c0: 6f64 0a20 2020 2064 6566 2064 6566 6175  od.    def defau
+000027d0: 6c74 2829 202d 3e20 224d 656d 5374 6f72  lt() -> "MemStor
+000027e0: 6167 6543 6f72 6522 3a20 2e2e 2e0a 0a63  ageCore": .....c
+000027f0: 6c61 7373 204d 656d 5374 6f72 6167 6543  lass MemStorageC
+00002800: 6f72 6552 6566 285f 5f41 5049 5f53 746f  oreRef(__API_Sto
+00002810: 7261 6765 436f 7265 293a 0a20 2020 2022  rageCore):.    "
+00002820: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+00002830: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+00002840: 604d 656d 5374 6f72 6167 6560 2e0a 2020  `MemStorage`..  
+00002850: 2020 2222 220a 0a63 6c61 7373 2053 746f    """..class Sto
+00002860: 7261 6765 436f 7265 285f 5f41 5049 5f53  rageCore(__API_S
+00002870: 746f 7261 6765 436f 7265 293a 0a20 2020  torageCore):.   
+00002880: 2022 2222 2022 2222 0a0a 2020 2020 6465   """ """..    de
+00002890: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+000028a0: 202d 3e20 2253 746f 7261 6765 436f 7265   -> "StorageCore
+000028b0: 5265 6622 3a20 2e2e 2e0a 2020 2020 4073  Ref": ....    @s
+000028c0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+000028d0: 6465 6620 6465 6661 756c 7428 2920 2d3e  def default() ->
+000028e0: 2022 5374 6f72 6167 6543 6f72 6522 3a20   "StorageCore": 
+000028f0: 2e2e 2e0a 0a63 6c61 7373 2053 746f 7261  .....class Stora
+00002900: 6765 436f 7265 5265 6628 5f5f 4150 495f  geCoreRef(__API_
+00002910: 5374 6f72 6167 6543 6f72 6529 3a0a 2020  StorageCore):.  
+00002920: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
+00002930: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
+00002940: 7373 3a60 5374 6f72 6167 6543 6f72 6560  ss:`StorageCore`
+00002950: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
+00002960: 205f 5f41 5049 5f53 746f 7261 6765 285f   __API_Storage(_
+00002970: 5f43 6c6f 6e65 6162 6c65 293a 0a20 2020  _Cloneable):.   
+00002980: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
+00002990: 202d 3e20 416e 793a 202e 2e2e 0a20 2020   -> Any: ....   
+000029a0: 2064 6566 2069 6e69 7469 616c 697a 655f   def initialize_
+000029b0: 7769 7468 5f63 6f6e 665f 7374 6174 6528  with_conf_state(
+000029c0: 0a20 2020 2020 2020 2073 656c 662c 2063  .        self, c
+000029d0: 6f6e 665f 7374 6174 653a 2022 436f 6e66  onf_state: "Conf
+000029e0: 5374 6174 6522 207c 2022 436f 6e66 5374  State" | "ConfSt
+000029f0: 6174 6552 6566 220a 2020 2020 2920 2d3e  ateRef".    ) ->
+00002a00: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00002a10: 2222 0a20 2020 2020 2020 2049 6e69 7469  "".        Initi
+00002a20: 616c 697a 6520 6120 604d 656d 5374 6f72  alize a `MemStor
+00002a30: 6167 6560 2077 6974 6820 6120 6769 7665  age` with a give
+00002a40: 6e20 6043 6f6e 6669 6760 2e0a 0a20 2020  n `Config`...   
+00002a50: 2020 2020 2059 6f75 2073 686f 756c 6420       You should 
+00002a60: 7573 6520 7468 6520 7361 6d65 2069 6e70  use the same inp
+00002a70: 7574 2074 6f20 696e 6974 6961 6c69 7a65  ut to initialize
+00002a80: 2061 6c6c 206e 6f64 6573 2e0a 2020 2020   all nodes..    
+00002a90: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00002aa0: 696e 6974 6961 6c5f 7374 6174 6528 7365  initial_state(se
+00002ab0: 6c66 2920 2d3e 2052 6166 7453 7461 7465  lf) -> RaftState
+00002ac0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00002ad0: 2020 2020 2020 496d 706c 656d 656e 7473        Implements
+00002ae0: 2074 6865 2053 746f 7261 6765 2074 7261   the Storage tra
+00002af0: 6974 2e0a 2020 2020 2020 2020 2222 220a  it..        """.
+00002b00: 2020 2020 6465 6620 656e 7472 6965 7328      def entries(
+00002b10: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00002b20: 2020 2020 2020 206c 6f77 3a20 696e 742c         low: int,
+00002b30: 0a20 2020 2020 2020 2068 6967 683a 2069  .        high: i
+00002b40: 6e74 2c0a 2020 2020 2020 2020 636f 6e74  nt,.        cont
+00002b50: 6578 743a 2022 4765 7445 6e74 7269 6573  ext: "GetEntries
+00002b60: 436f 6e74 6578 7452 6566 222c 0a20 2020  ContextRef",.   
+00002b70: 2020 2020 206d 6178 5f73 697a 653a 204f       max_size: O
+00002b80: 7074 696f 6e61 6c5b 696e 745d 2c0a 2020  ptional[int],.  
+00002b90: 2020 2920 2d3e 204c 6973 745b 2245 6e74    ) -> List["Ent
+00002ba0: 7279 225d 3a0a 2020 2020 2020 2020 2222  ry"]:.        ""
+00002bb0: 220a 2020 2020 2020 2020 496d 706c 656d  ".        Implem
+00002bc0: 656e 7473 2074 6865 2053 746f 7261 6765  ents the Storage
+00002bd0: 2074 7261 6974 2e0a 2020 2020 2020 2020   trait..        
+00002be0: 2222 220a 2020 2020 6465 6620 7465 726d  """.    def term
+00002bf0: 2873 656c 662c 2069 6478 3a20 696e 7429  (self, idx: int)
+00002c00: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00002c10: 2022 2222 0a20 2020 2020 2020 2049 6d70   """.        Imp
+00002c20: 6c65 6d65 6e74 7320 7468 6520 5374 6f72  lements the Stor
+00002c30: 6167 6520 7472 6169 742e 0a20 2020 2020  age trait..     
+00002c40: 2020 2022 2222 0a20 2020 2064 6566 2066     """.    def f
+00002c50: 6972 7374 5f69 6e64 6578 2873 656c 6629  irst_index(self)
+00002c60: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00002c70: 2022 2222 0a20 2020 2020 2020 2049 6d70   """.        Imp
+00002c80: 6c65 6d65 6e74 7320 7468 6520 5374 6f72  lements the Stor
+00002c90: 6167 6520 7472 6169 742e 0a20 2020 2020  age trait..     
+00002ca0: 2020 2022 2222 0a20 2020 2064 6566 206c     """.    def l
+00002cb0: 6173 745f 696e 6465 7828 7365 6c66 2920  ast_index(self) 
+00002cc0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00002cd0: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
+00002ce0: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
+00002cf0: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
+00002d00: 2020 2222 220a 2020 2020 6465 6620 736e    """.    def sn
+00002d10: 6170 7368 6f74 2873 656c 662c 2072 6571  apshot(self, req
+00002d20: 7565 7374 5f69 6e64 6578 3a20 696e 742c  uest_index: int,
+00002d30: 2074 6f3a 2069 6e74 2920 2d3e 2022 536e   to: int) -> "Sn
+00002d40: 6170 7368 6f74 223a 0a20 2020 2020 2020  apshot":.       
+00002d50: 2022 2222 0a20 2020 2020 2020 2049 6d70   """.        Imp
+00002d60: 6c65 6d65 6e74 7320 7468 6520 5374 6f72  lements the Stor
+00002d70: 6167 6520 7472 6169 742e 0a20 2020 2020  age trait..     
+00002d80: 2020 2022 2222 0a0a 636c 6173 7320 4d65     """..class Me
+00002d90: 6d53 746f 7261 6765 285f 5f41 5049 5f53  mStorage(__API_S
+00002da0: 746f 7261 6765 293a 0a20 2020 2022 2222  torage):.    """
+00002db0: 0a20 2020 2060 4d65 6d53 746f 7261 6765  .    `MemStorage
+00002dc0: 6020 6973 2061 2074 6872 6561 642d 7361  ` is a thread-sa
+00002dd0: 6665 2062 7574 2069 6e63 6f6d 706c 6574  fe but incomplet
+00002de0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00002df0: 206f 6620 6053 746f 7261 6765 602c 206d   of `Storage`, m
+00002e00: 6169 6e6c 7920 666f 7220 7465 7374 732e  ainly for tests.
+00002e10: 0a0a 2020 2020 4120 7265 616c 2060 5374  ..    A real `St
+00002e20: 6f72 6167 6560 2073 686f 756c 6420 7361  orage` should sa
+00002e30: 7665 2062 6f74 6820 7261 6674 206c 6f67  ve both raft log
+00002e40: 7320 616e 6420 6170 706c 6965 6420 6461  s and applied da
+00002e50: 7461 2e20 486f 7765 7665 7220 604d 656d  ta. However `Mem
+00002e60: 5374 6f72 6167 6560 206f 6e6c 790a 2020  Storage` only.  
+00002e70: 2020 636f 6e74 6169 6e73 2072 6166 7420    contains raft 
+00002e80: 6c6f 6773 2e20 536f 2079 6f75 2063 616e  logs. So you can
+00002e90: 2063 616c 6c20 604d 656d 5374 6f72 6167   call `MemStorag
+00002ea0: 653a 3a61 7070 656e 6460 2074 6f20 7065  e::append` to pe
+00002eb0: 7273 6973 7420 6e65 7720 7265 6365 6976  rsist new receiv
+00002ec0: 6564 2075 6e73 7461 626c 6520 7261 6674  ed unstable raft
+00002ed0: 0a20 2020 206c 6f67 7320 616e 6420 7468  .    logs and th
+00002ee0: 656e 2061 6363 6573 7320 7468 656d 2077  en access them w
+00002ef0: 6974 6820 6053 746f 7261 6765 6020 4150  ith `Storage` AP
+00002f00: 4973 2e20 5468 6520 6f6e 6c79 2065 7863  Is. The only exc
+00002f10: 6570 7469 6f6e 2069 7320 6053 746f 7261  eption is `Stora
+00002f20: 6765 3a3a 736e 6170 7368 6f74 602e 2054  ge::snapshot`. T
+00002f30: 6865 7265 0a20 2020 2069 7320 6e6f 2064  here.    is no d
+00002f40: 6174 6120 696e 2060 536e 6170 7368 6f74  ata in `Snapshot
+00002f50: 6020 7265 7475 726e 6564 2062 7920 604d  ` returned by `M
+00002f60: 656d 5374 6f72 6167 653a 3a73 6e61 7073  emStorage::snaps
+00002f70: 686f 7460 2062 6563 6175 7365 2061 7070  hot` because app
+00002f80: 6c69 6564 2064 6174 6120 6973 206e 6f74  lied data is not
+00002f90: 2073 746f 7265 640a 2020 2020 696e 2060   stored.    in `
+00002fa0: 4d65 6d53 746f 7261 6765 602e 0a20 2020  MemStorage`..   
+00002fb0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00002fc0: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+00002fd0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+00002fe0: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+00002ff0: 202d 3e20 224d 656d 5374 6f72 6167 6552   -> "MemStorageR
+00003000: 6566 223a 202e 2e2e 0a20 2020 2064 6566  ef": ....    def
+00003010: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
+00003020: 224d 656d 5374 6f72 6167 6522 3a20 2e2e  "MemStorage": ..
+00003030: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00003040: 686f 640a 2020 2020 6465 6620 6465 6661  hod.    def defa
+00003050: 756c 7428 2920 2d3e 2022 4d65 6d53 746f  ult() -> "MemSto
+00003060: 7261 6765 223a 202e 2e2e 0a20 2020 2040  rage": ....    @
+00003070: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+00003080: 2064 6566 206e 6577 5f77 6974 685f 636f   def new_with_co
+00003090: 6e66 5f73 7461 7465 280a 2020 2020 2020  nf_state(.      
+000030a0: 2020 636f 6e66 5f73 7461 7465 3a20 2243    conf_state: "C
+000030b0: 6f6e 6653 7461 7465 2220 7c20 2243 6f6e  onfState" | "Con
+000030c0: 6653 7461 7465 5265 6622 2c0a 2020 2020  fStateRef",.    
+000030d0: 2920 2d3e 2022 4d65 6d53 746f 7261 6765  ) -> "MemStorage
+000030e0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+000030f0: 2020 2020 2020 2043 7265 6174 6520 6120         Create a 
+00003100: 6e65 7720 604d 656d 5374 6f72 6167 6560  new `MemStorage`
+00003110: 2077 6974 6820 6120 6769 7665 6e20 6043   with a given `C
+00003120: 6f6e 6669 6760 2e20 5468 6520 6769 7665  onfig`. The give
+00003130: 6e20 6043 6f6e 6669 6760 2077 696c 6c20  n `Config` will 
+00003140: 6265 2075 7365 6420 746f 0a20 2020 2020  be used to.     
+00003150: 2020 2069 6e69 7469 616c 697a 6520 7468     initialize th
+00003160: 6520 7374 6f72 6167 652e 0a0a 2020 2020  e storage...    
+00003170: 2020 2020 596f 7520 7368 6f75 6c64 2075      You should u
+00003180: 7365 2074 6865 2073 616d 6520 696e 7075  se the same inpu
+00003190: 7420 746f 2069 6e69 7469 616c 697a 6520  t to initialize 
+000031a0: 616c 6c20 6e6f 6465 732e 0a20 2020 2020  all nodes..     
+000031b0: 2020 2022 2222 0a20 2020 2064 6566 2077     """.    def w
+000031c0: 6c28 7365 6c66 2920 2d3e 2022 4d65 6d53  l(self) -> "MemS
+000031d0: 746f 7261 6765 436f 7265 5265 6622 3a0a  torageCoreRef":.
+000031e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000031f0: 2020 2020 4f70 656e 7320 7570 2061 2077      Opens up a w
+00003200: 7269 7465 206c 6f63 6b20 6f6e 2074 6865  rite lock on the
+00003210: 2073 746f 7261 6765 2061 6e64 2072 6574   storage and ret
+00003220: 7572 6e73 2067 7561 7264 2068 616e 646c  urns guard handl
+00003230: 652e 2055 7365 2074 6869 730a 2020 2020  e. Use this.    
+00003240: 2020 2020 7769 7468 2066 756e 6374 696f      with functio
+00003250: 6e73 2074 6861 7420 7461 6b65 2061 206d  ns that take a m
+00003260: 7574 6162 6c65 2072 6566 6572 656e 6365  utable reference
+00003270: 2074 6f20 7365 6c66 2e0a 2020 2020 2020   to self..      
+00003280: 2020 2222 220a 2020 2020 6465 6620 726c    """.    def rl
+00003290: 2873 656c 6629 202d 3e20 224d 656d 5374  (self) -> "MemSt
+000032a0: 6f72 6167 6543 6f72 6552 6566 223a 0a20  orageCoreRef":. 
+000032b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000032c0: 2020 204f 7065 6e73 2075 7020 6120 7265     Opens up a re
+000032d0: 6164 206c 6f63 6b20 6f6e 2074 6865 2073  ad lock on the s
+000032e0: 746f 7261 6765 2061 6e64 2072 6574 7572  torage and retur
+000032f0: 6e73 2061 2067 7561 7264 2068 616e 646c  ns a guard handl
+00003300: 652e 2055 7365 2074 6869 730a 2020 2020  e. Use this.    
+00003310: 2020 2020 7769 7468 2066 756e 6374 696f      with functio
+00003320: 6e73 2074 6861 7420 646f 6e27 7420 7265  ns that don't re
+00003330: 7175 6972 6520 6d75 7461 7469 6f6e 2e0a  quire mutation..
+00003340: 2020 2020 2020 2020 2222 220a 0a63 6c61          """..cla
+00003350: 7373 204d 656d 5374 6f72 6167 6552 6566  ss MemStorageRef
+00003360: 285f 5f41 5049 5f53 746f 7261 6765 293a  (__API_Storage):
+00003370: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
+00003380: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
+00003390: 636c 6173 733a 604d 656d 5374 6f72 6167  class:`MemStorag
+000033a0: 6560 2e0a 2020 2020 2222 220a 0a20 2020  e`..    """..   
+000033b0: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
+000033c0: 202d 3e20 224d 656d 5374 6f72 6167 6522   -> "MemStorage"
+000033d0: 3a20 2e2e 2e0a 2020 2020 6465 6620 776c  : ....    def wl
+000033e0: 2873 656c 6629 202d 3e20 224d 656d 5374  (self) -> "MemSt
+000033f0: 6f72 6167 6543 6f72 6552 6566 223a 0a20  orageCoreRef":. 
+00003400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003410: 2020 204f 7065 6e73 2075 7020 6120 7772     Opens up a wr
+00003420: 6974 6520 6c6f 636b 206f 6e20 7468 6520  ite lock on the 
+00003430: 7374 6f72 6167 6520 616e 6420 7265 7475  storage and retu
+00003440: 726e 7320 6775 6172 6420 6861 6e64 6c65  rns guard handle
+00003450: 2e20 5573 6520 7468 6973 0a20 2020 2020  . Use this.     
+00003460: 2020 2077 6974 6820 6675 6e63 7469 6f6e     with function
+00003470: 7320 7468 6174 2074 616b 6520 6120 6d75  s that take a mu
+00003480: 7461 626c 6520 7265 6665 7265 6e63 6520  table reference 
+00003490: 746f 2073 656c 662e 0a20 2020 2020 2020  to self..       
+000034a0: 2022 2222 0a20 2020 2064 6566 2072 6c28   """.    def rl(
+000034b0: 7365 6c66 2920 2d3e 2022 4d65 6d53 746f  self) -> "MemSto
+000034c0: 7261 6765 436f 7265 5265 6622 3a0a 2020  rageCoreRef":.  
+000034d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000034e0: 2020 4f70 656e 7320 7570 2061 2072 6561    Opens up a rea
+000034f0: 6420 6c6f 636b 206f 6e20 7468 6520 7374  d lock on the st
+00003500: 6f72 6167 6520 616e 6420 7265 7475 726e  orage and return
+00003510: 7320 6120 6775 6172 6420 6861 6e64 6c65  s a guard handle
+00003520: 2e20 5573 6520 7468 6973 0a20 2020 2020  . Use this.     
+00003530: 2020 2077 6974 6820 6675 6e63 7469 6f6e     with function
+00003540: 7320 7468 6174 2064 6f6e 2774 2072 6571  s that don't req
+00003550: 7569 7265 206d 7574 6174 696f 6e2e 0a20  uire mutation.. 
+00003560: 2020 2020 2020 2022 2222 0a0a 636c 6173         """..clas
+00003570: 7320 5374 6f72 6167 6528 5f5f 4150 495f  s Storage(__API_
+00003580: 5374 6f72 6167 6529 3a0a 2020 2020 2222  Storage):.    ""
+00003590: 220a 2020 2020 5374 6f72 6167 6520 7361  ".    Storage sa
+000035a0: 7665 7320 616c 6c20 7468 6520 696e 666f  ves all the info
+000035b0: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
+000035c0: 6520 6375 7272 656e 7420 5261 6674 2069  e current Raft i
+000035d0: 6d70 6c65 6d65 6e74 6174 696f 6e2c 2069  mplementation, i
+000035e0: 6e63 6c75 6469 6e67 2052 6166 7420 4c6f  ncluding Raft Lo
+000035f0: 672c 0a20 2020 2063 6f6d 6d69 7420 696e  g,.    commit in
+00003600: 6465 782c 2074 6865 206c 6561 6465 7220  dex, the leader 
+00003610: 746f 2076 6f74 6520 666f 722c 2065 7463  to vote for, etc
+00003620: 2e0a 0a20 2020 2049 6620 616e 7920 5374  ...    If any St
+00003630: 6f72 6167 6520 6d65 7468 6f64 2072 6574  orage method ret
+00003640: 7572 6e73 2061 6e20 6572 726f 722c 2074  urns an error, t
+00003650: 6865 2072 6166 7420 696e 7374 616e 6365  he raft instance
+00003660: 2077 696c 6c0a 2020 2020 6265 636f 6d65   will.    become
+00003670: 2069 6e6f 7065 7261 626c 6520 616e 6420   inoperable and 
+00003680: 7265 6675 7365 2074 6f20 7061 7274 6963  refuse to partic
+00003690: 6970 6174 6520 696e 2065 6c65 6374 696f  ipate in electio
+000036a0: 6e73 3b20 7468 650a 2020 2020 6170 706c  ns; the.    appl
+000036b0: 6963 6174 696f 6e20 6973 2072 6573 706f  ication is respo
+000036c0: 6e73 6962 6c65 2066 6f72 2063 6c65 616e  nsible for clean
+000036d0: 7570 2061 6e64 2072 6563 6f76 6572 7920  up and recovery 
+000036e0: 696e 2074 6869 7320 6361 7365 2e0a 2020  in this case..  
+000036f0: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+00003700: 5f69 6e69 745f 5f28 7365 6c66 2920 2d3e  _init__(self) ->
+00003710: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
+00003720: 6566 206d 616b 655f 7265 6628 7365 6c66  ef make_ref(self
+00003730: 2920 2d3e 2022 5374 6f72 6167 6552 6566  ) -> "StorageRef
+00003740: 223a 202e 2e2e 0a20 2020 2064 6566 2063  ": ....    def c
+00003750: 6c6f 6e65 2873 656c 6629 202d 3e20 2253  lone(self) -> "S
+00003760: 746f 7261 6765 223a 202e 2e2e 0a20 2020  torage": ....   
+00003770: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00003780: 2020 2064 6566 2064 6566 6175 6c74 2829     def default()
+00003790: 202d 3e20 2253 746f 7261 6765 223a 202e   -> "Storage": .
+000037a0: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+000037b0: 7468 6f64 0a20 2020 2064 6566 206e 6577  thod.    def new
+000037c0: 5f77 6974 685f 636f 6e66 5f73 7461 7465  _with_conf_state
+000037d0: 280a 2020 2020 2020 2020 636f 6e66 5f73  (.        conf_s
+000037e0: 7461 7465 3a20 2243 6f6e 6653 7461 7465  tate: "ConfState
+000037f0: 2220 7c20 2243 6f6e 6653 7461 7465 5265  " | "ConfStateRe
+00003800: 6622 2c0a 2020 2020 2920 2d3e 2022 5374  f",.    ) -> "St
+00003810: 6f72 6167 6522 3a0a 2020 2020 2020 2020  orage":.        
+00003820: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00003830: 776c 2873 656c 6629 202d 3e20 416e 793a  wl(self) -> Any:
+00003840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00003850: 2020 2020 204f 7065 6e73 2075 7020 6120       Opens up a 
+00003860: 7772 6974 6520 6c6f 636b 206f 6e20 7468  write lock on th
+00003870: 6520 7374 6f72 6167 6520 616e 6420 7265  e storage and re
+00003880: 7475 726e 7320 6775 6172 6420 6861 6e64  turns guard hand
+00003890: 6c65 2e20 5573 6520 7468 6973 0a20 2020  le. Use this.   
+000038a0: 2020 2020 2077 6974 6820 6675 6e63 7469       with functi
+000038b0: 6f6e 7320 7468 6174 2074 616b 6520 6120  ons that take a 
+000038c0: 6d75 7461 626c 6520 7265 6665 7265 6e63  mutable referenc
+000038d0: 6520 746f 2073 656c 662e 0a20 2020 2020  e to self..     
+000038e0: 2020 2022 2222 0a20 2020 2064 6566 2072     """.    def r
+000038f0: 6c28 7365 6c66 2920 2d3e 2041 6e79 3a0a  l(self) -> Any:.
+00003900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003910: 2020 2020 4f70 656e 7320 7570 2061 2072      Opens up a r
+00003920: 6561 6420 6c6f 636b 206f 6e20 7468 6520  ead lock on the 
+00003930: 7374 6f72 6167 6520 616e 6420 7265 7475  storage and retu
+00003940: 726e 7320 6120 6775 6172 6420 6861 6e64  rns a guard hand
+00003950: 6c65 2e20 5573 6520 7468 6973 0a20 2020  le. Use this.   
+00003960: 2020 2020 2077 6974 6820 6675 6e63 7469       with functi
+00003970: 6f6e 7320 7468 6174 2064 6f6e 2774 2072  ons that don't r
+00003980: 6571 7569 7265 206d 7574 6174 696f 6e2e  equire mutation.
+00003990: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+000039a0: 6173 7320 5374 6f72 6167 6552 6566 285f  ass StorageRef(_
+000039b0: 5f41 5049 5f53 746f 7261 6765 293a 0a20  _API_Storage):. 
+000039c0: 2020 2022 2222 0a20 2020 2052 6566 6572     """.    Refer
+000039d0: 656e 6365 2074 7970 6520 6f66 203a 636c  ence type of :cl
+000039e0: 6173 733a 6053 746f 7261 6765 602e 0a20  ass:`Storage`.. 
+000039f0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+00003a00: 636c 6f6e 6528 7365 6c66 2920 2d3e 2022  clone(self) -> "
+00003a10: 5374 6f72 6167 6522 3a20 2e2e 2e0a 2020  Storage": ....  
+00003a20: 2020 6465 6620 776c 2873 656c 6629 202d    def wl(self) -
+00003a30: 3e20 416e 793a 0a20 2020 2020 2020 2022  > Any:.        "
+00003a40: 2222 0a20 2020 2020 2020 204f 7065 6e73  "".        Opens
+00003a50: 2075 7020 6120 7772 6974 6520 6c6f 636b   up a write lock
+00003a60: 206f 6e20 7468 6520 7374 6f72 6167 6520   on the storage 
+00003a70: 616e 6420 7265 7475 726e 7320 6775 6172  and returns guar
+00003a80: 6420 6861 6e64 6c65 2e20 5573 6520 7468  d handle. Use th
+00003a90: 6973 0a20 2020 2020 2020 2077 6974 6820  is.        with 
+00003aa0: 6675 6e63 7469 6f6e 7320 7468 6174 2074  functions that t
+00003ab0: 616b 6520 6120 6d75 7461 626c 6520 7265  ake a mutable re
+00003ac0: 6665 7265 6e63 6520 746f 2073 656c 662e  ference to self.
+00003ad0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00003ae0: 2064 6566 2072 6c28 7365 6c66 2920 2d3e   def rl(self) ->
+00003af0: 2041 6e79 3a0a 2020 2020 2020 2020 2222   Any:.        ""
+00003b00: 220a 2020 2020 2020 2020 4f70 656e 7320  ".        Opens 
+00003b10: 7570 2061 2072 6561 6420 6c6f 636b 206f  up a read lock o
+00003b20: 6e20 7468 6520 7374 6f72 6167 6520 616e  n the storage an
+00003b30: 6420 7265 7475 726e 7320 6120 6775 6172  d returns a guar
+00003b40: 6420 6861 6e64 6c65 2e20 5573 6520 7468  d handle. Use th
+00003b50: 6973 0a20 2020 2020 2020 2077 6974 6820  is.        with 
+00003b60: 6675 6e63 7469 6f6e 7320 7468 6174 2064  functions that d
+00003b70: 6f6e 2774 2072 6571 7569 7265 206d 7574  on't require mut
+00003b80: 6174 696f 6e2e 0a20 2020 2020 2020 2022  ation..        "
+00003b90: 2222 0a0a 636c 6173 7320 5f5f 4150 495f  ""..class __API_
+00003ba0: 5265 6164 793a 0a20 2020 2064 6566 2068  Ready:.    def h
+00003bb0: 7328 7365 6c66 2920 2d3e 204f 7074 696f  s(self) -> Optio
+00003bc0: 6e61 6c5b 2248 6172 6453 7461 7465 5265  nal["HardStateRe
+00003bd0: 6622 5d3a 0a20 2020 2020 2020 2022 2222  f"]:.        """
+00003be0: 0a20 2020 2020 2020 2054 6865 2063 7572  .        The cur
+00003bf0: 7265 6e74 2073 7461 7465 206f 6620 6120  rent state of a 
+00003c00: 4e6f 6465 2074 6f20 6265 2073 6176 6564  Node to be saved
+00003c10: 2074 6f20 7374 6162 6c65 2073 746f 7261   to stable stora
+00003c20: 6765 2e0a 2020 2020 2020 2020 4861 7264  ge..        Hard
+00003c30: 5374 6174 6520 7769 6c6c 2062 6520 4e6f  State will be No
+00003c40: 6e65 2073 7461 7465 2069 6620 7468 6572  ne state if ther
+00003c50: 6520 6973 206e 6f20 7570 6461 7465 2e0a  e is no update..
+00003c60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003c70: 6465 6620 7373 2873 656c 6629 202d 3e20  def ss(self) -> 
+00003c80: 4f70 7469 6f6e 616c 5b22 536f 6674 5374  Optional["SoftSt
+00003c90: 6174 6552 6566 225d 3a0a 2020 2020 2020  ateRef"]:.      
+00003ca0: 2020 2222 220a 2020 2020 2020 2020 5468    """.        Th
+00003cb0: 6520 6375 7272 656e 7420 766f 6c61 7469  e current volati
+00003cc0: 6c65 2073 7461 7465 206f 6620 6120 4e6f  le state of a No
+00003cd0: 6465 2e0a 2020 2020 2020 2020 536f 6674  de..        Soft
+00003ce0: 5374 6174 6520 7769 6c6c 2062 6520 4e6f  State will be No
+00003cf0: 6e65 2069 6620 7468 6572 6520 6973 206e  ne if there is n
+00003d00: 6f20 7570 6461 7465 2e0a 2020 2020 2020  o update..      
+00003d10: 2020 4974 2069 7320 6e6f 7420 7265 7175    It is not requ
+00003d20: 6972 6564 2074 6f20 636f 6e73 756d 6520  ired to consume 
+00003d30: 6f72 2073 746f 7265 2053 6f66 7453 7461  or store SoftSta
+00003d40: 7465 2e0a 2020 2020 2020 2020 2222 220a  te..        """.
+00003d50: 2020 2020 6465 6620 6d75 7374 5f73 796e      def must_syn
+00003d60: 6328 7365 6c66 2920 2d3e 2062 6f6f 6c3a  c(self) -> bool:
+00003d70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00003d80: 2020 2020 204d 7573 7453 796e 6320 6973       MustSync is
+00003d90: 2066 616c 7365 2069 6620 616e 6420 6f6e   false if and on
+00003da0: 6c79 2069 660a 2020 2020 2020 2020 312e  ly if.        1.
+00003db0: 206e 6f20 4861 7264 5374 6174 6520 6f72   no HardState or
+00003dc0: 206f 6e6c 7920 6974 7320 636f 6d6d 6974   only its commit
+00003dd0: 2069 7320 6469 6666 6572 656e 7420 6672   is different fr
+00003de0: 6f6d 2062 6566 6f72 650a 2020 2020 2020  om before.      
+00003df0: 2020 322e 206e 6f20 456e 7472 6965 7320    2. no Entries 
+00003e00: 616e 6420 536e 6170 7368 6f74 0a20 2020  and Snapshot.   
+00003e10: 2020 2020 2049 6620 6974 2773 2066 616c       If it's fal
+00003e20: 7365 2c20 616e 2061 7379 6e63 6872 6f6e  se, an asynchron
+00003e30: 6f75 7320 7772 6974 6520 6f66 2048 6172  ous write of Har
+00003e40: 6453 7461 7465 2069 7320 7065 726d 6973  dState is permis
+00003e50: 7369 626c 6520 6265 666f 7265 2063 616c  sible before cal
+00003e60: 6c69 6e67 0a20 2020 2020 2020 205b 6052  ling.        [`R
+00003e70: 6177 4e6f 6465 3a3a 6f6e 5f70 6572 7369  awNode::on_persi
+00003e80: 7374 5f72 6561 6479 605d 206f 7220 5b60  st_ready`] or [`
+00003e90: 5261 774e 6f64 653a 3a61 6476 616e 6365  RawNode::advance
+00003ea0: 605d 206f 7220 6974 7320 6661 6d69 6c69  `] or its famili
+00003eb0: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00003ec0: 2020 2020 6465 6620 6e75 6d62 6572 2873      def number(s
+00003ed0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+00003ee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003ef0: 2054 6865 206e 756d 6265 7220 6f66 2063   The number of c
+00003f00: 7572 7265 6e74 2052 6561 6479 2e0a 2020  urrent Ready..  
+00003f10: 2020 2020 2020 4974 2069 7320 7573 6564        It is used
+00003f20: 2066 6f72 2069 6465 6e74 6966 7969 6e67   for identifying
+00003f30: 2074 6865 2064 6966 6665 7265 6e74 2052   the different R
+00003f40: 6561 6479 2061 6e64 2052 6561 6479 5265  eady and ReadyRe
+00003f50: 636f 7264 2e0a 2020 2020 2020 2020 2222  cord..        ""
+00003f60: 220a 2020 2020 6465 6620 736e 6170 7368  ".    def snapsh
+00003f70: 6f74 2873 656c 6629 202d 3e20 2253 6e61  ot(self) -> "Sna
+00003f80: 7073 686f 7452 6566 223a 0a20 2020 2020  pshotRef":.     
+00003f90: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00003fa0: 6e61 7073 686f 7420 7370 6563 6966 6965  napshot specifie
+00003fb0: 7320 7468 6520 736e 6170 7368 6f74 2074  s the snapshot t
+00003fc0: 6f20 6265 2073 6176 6564 2074 6f20 7374  o be saved to st
+00003fd0: 6162 6c65 2073 746f 7261 6765 2e0a 2020  able storage..  
+00003fe0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00003ff0: 6620 636f 6d6d 6974 7465 645f 656e 7472  f committed_entr
+00004000: 6965 7328 7365 6c66 2920 2d3e 204c 6973  ies(self) -> Lis
+00004010: 745b 2245 6e74 7279 5265 6622 5d3a 0a20  t["EntryRef"]:. 
+00004020: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004030: 2020 2043 6f6d 6d69 7474 6564 456e 7472     CommittedEntr
+00004040: 6965 7320 7370 6563 6966 6965 7320 656e  ies specifies en
+00004050: 7472 6965 7320 746f 2062 6520 636f 6d6d  tries to be comm
+00004060: 6974 7465 6420 746f 2061 0a20 2020 2020  itted to a.     
+00004070: 2020 2073 746f 7265 2f73 7461 7465 2d6d     store/state-m
+00004080: 6163 6869 6e65 2e20 5468 6573 6520 6861  achine. These ha
+00004090: 7665 2070 7265 7669 6f75 736c 7920 6265  ve previously be
+000040a0: 656e 2063 6f6d 6d69 7474 6564 2074 6f20  en committed to 
+000040b0: 7374 6162 6c65 0a20 2020 2020 2020 2073  stable.        s
+000040c0: 746f 7265 2e0a 2020 2020 2020 2020 2222  tore..        ""
+000040d0: 220a 2020 2020 6465 6620 7461 6b65 5f63  ".    def take_c
+000040e0: 6f6d 6d69 7474 6564 5f65 6e74 7269 6573  ommitted_entries
+000040f0: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
+00004100: 456e 7472 7922 5d3a 0a20 2020 2020 2020  Entry"]:.       
+00004110: 2022 2222 0a20 2020 2020 2020 2054 616b   """.        Tak
+00004120: 6520 7468 6520 436f 6d6d 6974 456e 7472  e the CommitEntr
+00004130: 6965 732e 0a20 2020 2020 2020 2022 2222  ies..        """
+00004140: 0a20 2020 2064 6566 2065 6e74 7269 6573  .    def entries
+00004150: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
+00004160: 456e 7472 7952 6566 225d 3a0a 2020 2020  EntryRef"]:.    
+00004170: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004180: 456e 7472 6965 7320 7370 6563 6966 6965  Entries specifie
+00004190: 7320 656e 7472 6965 7320 746f 2062 6520  s entries to be 
+000041a0: 7361 7665 6420 746f 2073 7461 626c 6520  saved to stable 
+000041b0: 7374 6f72 6167 652e 0a20 2020 2020 2020  storage..       
+000041c0: 2022 2222 0a20 2020 2064 6566 2074 616b   """.    def tak
+000041d0: 655f 656e 7472 6965 7328 7365 6c66 2920  e_entries(self) 
+000041e0: 2d3e 204c 6973 745b 2245 6e74 7279 225d  -> List["Entry"]
+000041f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00004200: 2020 2020 2020 5461 6b65 2074 6865 2045        Take the E
+00004210: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
+00004220: 2222 220a 2020 2020 6465 6620 6d65 7373  """.    def mess
+00004230: 6167 6573 2873 656c 6629 202d 3e20 4c69  ages(self) -> Li
+00004240: 7374 5b22 4d65 7373 6167 6552 6566 225d  st["MessageRef"]
+00004250: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00004260: 2020 2020 2020 4d65 7373 6167 6573 2073        Messages s
+00004270: 7065 6369 6669 6573 206f 7574 626f 756e  pecifies outboun
+00004280: 6420 6d65 7373 6167 6573 2074 6f20 6265  d messages to be
+00004290: 2073 656e 742e 0a20 2020 2020 2020 2049   sent..        I
+000042a0: 6620 6974 2063 6f6e 7461 696e 7320 6120  f it contains a 
+000042b0: 4d73 6753 6e61 7020 6d65 7373 6167 652c  MsgSnap message,
+000042c0: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+000042d0: 204d 5553 5420 7265 706f 7274 2062 6163   MUST report bac
+000042e0: 6b20 746f 2072 6166 740a 2020 2020 2020  k to raft.      
+000042f0: 2020 7768 656e 2074 6865 2073 6e61 7073    when the snaps
+00004300: 686f 7420 6861 7320 6265 656e 2072 6563  hot has been rec
+00004310: 6569 7665 6420 6f72 2068 6173 2066 6169  eived or has fai
+00004320: 6c65 6420 6279 2063 616c 6c69 6e67 2052  led by calling R
+00004330: 6570 6f72 7453 6e61 7073 686f 742e 0a20  eportSnapshot.. 
+00004340: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00004350: 6566 2074 616b 655f 6d65 7373 6167 6573  ef take_messages
+00004360: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
+00004370: 4d65 7373 6167 6522 5d3a 0a20 2020 2020  Message"]:.     
+00004380: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
+00004390: 616b 6520 7468 6520 4d65 7373 6167 6573  ake the Messages
+000043a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000043b0: 2020 6465 6620 7065 7273 6973 7465 645f    def persisted_
+000043c0: 6d65 7373 6167 6573 2873 656c 6629 202d  messages(self) -
+000043d0: 3e20 4c69 7374 5b22 4d65 7373 6167 6552  > List["MessageR
+000043e0: 6566 225d 3a0a 2020 2020 2020 2020 2222  ef"]:.        ""
+000043f0: 220a 2020 2020 2020 2020 5065 7273 6973  ".        Persis
+00004400: 7465 6420 4d65 7373 6167 6573 2073 7065  ted Messages spe
+00004410: 6369 6669 6573 206f 7574 626f 756e 6420  cifies outbound 
+00004420: 6d65 7373 6167 6573 2074 6f20 6265 2073  messages to be s
+00004430: 656e 7420 4146 5445 5220 7468 6520 4861  ent AFTER the Ha
+00004440: 7264 5374 6174 652c 0a20 2020 2020 2020  rdState,.       
+00004450: 2045 6e74 7269 6573 2061 6e64 2053 6e61   Entries and Sna
+00004460: 7073 686f 7420 6172 6520 7065 7273 6973  pshot are persis
+00004470: 7465 6420 746f 2073 7461 626c 6520 7374  ted to stable st
+00004480: 6f72 6167 652e 0a20 2020 2020 2020 2022  orage..        "
+00004490: 2222 0a20 2020 2064 6566 2074 616b 655f  "".    def take_
+000044a0: 7065 7273 6973 7465 645f 6d65 7373 6167  persisted_messag
+000044b0: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
+000044c0: 5b22 4d65 7373 6167 6522 5d3a 0a20 2020  ["Message"]:.   
+000044d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000044e0: 2054 616b 6520 7468 6520 5065 7273 6973   Take the Persis
+000044f0: 7465 6420 4d65 7373 6167 6573 2e0a 2020  ted Messages..  
+00004500: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00004510: 6620 7265 6164 5f73 7461 7465 7328 7365  f read_states(se
+00004520: 6c66 2920 2d3e 204c 6973 745b 2252 6561  lf) -> List["Rea
+00004530: 6453 7461 7465 5265 6622 5d3a 0a20 2020  dStateRef"]:.   
+00004540: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004550: 2052 6561 6453 7461 7465 7320 7370 6563   ReadStates spec
+00004560: 6966 6965 7320 7468 6520 7374 6174 6520  ifies the state 
+00004570: 666f 7220 7265 6164 206f 6e6c 7920 7175  for read only qu
+00004580: 6572 792e 0a20 2020 2020 2020 2022 2222  ery..        """
+00004590: 0a20 2020 2064 6566 2074 616b 655f 7265  .    def take_re
+000045a0: 6164 5f73 7461 7465 7328 7365 6c66 2920  ad_states(self) 
+000045b0: 2d3e 204c 6973 745b 2252 6561 6453 7461  -> List["ReadSta
+000045c0: 7465 225d 3a0a 2020 2020 2020 2020 2222  te"]:.        ""
+000045d0: 220a 2020 2020 2020 2020 5265 6164 5374  ".        ReadSt
+000045e0: 6174 6573 2073 7065 6369 6669 6573 2074  ates specifies t
+000045f0: 6865 2073 7461 7465 2066 6f72 2072 6561  he state for rea
+00004600: 6420 6f6e 6c79 2071 7565 7279 2e0a 2020  d only query..  
+00004610: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
+00004620: 2052 6561 6479 285f 5f41 5049 5f52 6561   Ready(__API_Rea
+00004630: 6479 293a 0a20 2020 2022 2222 0a20 2020  dy):.    """.   
+00004640: 2052 6561 6479 2065 6e63 6170 7375 6c61   Ready encapsula
+00004650: 7465 7320 7468 6520 656e 7472 6965 7320  tes the entries 
+00004660: 616e 6420 6d65 7373 6167 6573 2074 6861  and messages tha
+00004670: 7420 6172 6520 7265 6164 7920 746f 2072  t are ready to r
+00004680: 6561 642c 0a20 2020 2062 6520 7361 7665  ead,.    be save
+00004690: 6420 746f 2073 7461 626c 6520 7374 6f72  d to stable stor
+000046a0: 6167 652c 2063 6f6d 6d69 7474 6564 206f  age, committed o
+000046b0: 7220 7365 6e74 2074 6f20 6f74 6865 7220  r sent to other 
+000046c0: 7065 6572 732e 0a20 2020 2022 2222 0a0a  peers..    """..
+000046d0: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
+000046e0: 2873 656c 6629 202d 3e20 2252 6561 6479  (self) -> "Ready
+000046f0: 5265 6622 3a20 2e2e 2e0a 2020 2020 4073  Ref": ....    @s
+00004700: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00004710: 6465 6620 6465 6661 756c 7428 2920 2d3e  def default() ->
+00004720: 2022 5265 6164 7922 3a20 2e2e 2e0a 0a63   "Ready": .....c
+00004730: 6c61 7373 2052 6561 6479 5265 6628 5f5f  lass ReadyRef(__
+00004740: 4150 495f 5265 6164 7929 3a0a 2020 2020  API_Ready):.    
+00004750: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
+00004760: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
+00004770: 3a60 5265 6164 7960 2e0a 2020 2020 2222  :`Ready`..    ""
+00004780: 220a 0a63 6c61 7373 205f 5f41 5049 5f52  "..class __API_R
+00004790: 6177 4e6f 6465 3a0a 2020 2020 6465 6620  awNode:.    def 
+000047a0: 6164 7661 6e63 655f 6170 706c 7928 7365  advance_apply(se
+000047b0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+000047c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000047d0: 2041 6476 616e 6365 2061 7070 6c79 2074   Advance apply t
+000047e0: 6f20 7468 6520 696e 6465 7820 6f66 2074  o the index of t
+000047f0: 6865 206c 6173 7420 636f 6d6d 6974 7465  he last committe
+00004800: 6420 656e 7472 6965 7320 6769 7665 6e20  d entries given 
+00004810: 6265 666f 7265 2e0a 2020 2020 2020 2020  before..        
+00004820: 2222 220a 2020 2020 6465 6620 6164 7661  """.    def adva
+00004830: 6e63 655f 6170 706c 795f 746f 2873 656c  nce_apply_to(sel
+00004840: 662c 2061 7070 6c69 6564 3a20 696e 7429  f, applied: int)
+00004850: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00004860: 2020 2222 220a 2020 2020 2020 2020 4164    """.        Ad
+00004870: 7661 6e63 6520 6170 706c 7920 746f 2074  vance apply to t
+00004880: 6865 2070 6173 7365 6420 696e 6465 782e  he passed index.
+00004890: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000048a0: 2064 6566 2061 6476 616e 6365 2873 656c   def advance(sel
+000048b0: 662c 2072 643a 2022 5265 6164 7952 6566  f, rd: "ReadyRef
+000048c0: 2229 202d 3e20 224c 6967 6874 5265 6164  ") -> "LightRead
+000048d0: 7922 3a0a 2020 2020 2020 2020 2222 220a  y":.        """.
+000048e0: 2020 2020 2020 2020 4164 7661 6e63 6573          Advances
+000048f0: 2074 6865 2072 6561 6479 2061 6674 6572   the ready after
+00004900: 2066 756c 6c79 2070 726f 6365 7373 696e   fully processin
+00004910: 6720 6974 2e0a 0a20 2020 2020 2020 2046  g it...        F
+00004920: 756c 6c79 2070 726f 6365 7373 696e 6720  ully processing 
+00004930: 6120 7265 6164 7920 7265 7175 6972 6573  a ready requires
+00004940: 2074 6f20 7065 7273 6973 7420 736e 6170   to persist snap
+00004950: 7368 6f74 2c20 656e 7472 6965 7320 616e  shot, entries an
+00004960: 6420 6861 7264 2073 7461 7465 732c 2061  d hard states, a
+00004970: 7070 6c79 2061 6c6c 0a20 2020 2020 2020  pply all.       
+00004980: 2063 6f6d 6d69 7474 6564 2065 6e74 7269   committed entri
+00004990: 6573 2c20 7365 6e64 2061 6c6c 206d 6573  es, send all mes
+000049a0: 7361 6765 732e 0a0a 2020 2020 2020 2020  sages...        
+000049b0: 5265 7475 726e 7320 7468 6520 4c69 6768  Returns the Ligh
+000049c0: 7452 6561 6479 2074 6861 7420 636f 6e74  tReady that cont
+000049d0: 6169 6e73 2063 6f6d 6d69 7420 696e 6465  ains commit inde
+000049e0: 782c 2063 6f6d 6d69 7474 6564 2065 6e74  x, committed ent
+000049f0: 7269 6573 2061 6e64 206d 6573 7361 6765  ries and message
+00004a00: 732e 205b 604c 6967 6874 5265 6164 7960  s. [`LightReady`
+00004a10: 5d0a 2020 2020 2020 2020 636f 6e74 6169  ].        contai
+00004a20: 6e73 2075 7064 6174 6573 2074 6861 7420  ns updates that 
+00004a30: 6f6e 6c79 2076 616c 6964 2061 6674 6572  only valid after
+00004a40: 2070 6572 7369 7374 696e 6720 6c61 7374   persisting last
+00004a50: 2072 6561 6479 2e20 4974 2073 686f 756c   ready. It shoul
+00004a60: 6420 616c 736f 2062 6520 6675 6c6c 7920  d also be fully 
+00004a70: 7072 6f63 6573 7365 642e 0a20 2020 2020  processed..     
+00004a80: 2020 2054 6865 6e20 5b60 5365 6c66 3a3a     Then [`Self::
+00004a90: 6164 7661 6e63 655f 6170 706c 7960 5d20  advance_apply`] 
+00004aa0: 6f72 205b 6053 656c 663a 3a61 6476 616e  or [`Self::advan
+00004ab0: 6365 5f61 7070 6c79 5f74 6f60 5d20 7368  ce_apply_to`] sh
+00004ac0: 6f75 6c64 2062 6520 7573 6564 206c 6174  ould be used lat
+00004ad0: 6572 2074 6f20 7570 6461 7465 2061 7070  er to update app
+00004ae0: 6c79 696e 670a 2020 2020 2020 2020 7072  lying.        pr
+00004af0: 6f67 7265 7373 2e0a 2020 2020 2020 2020  ogress..        
+00004b00: 2222 220a 2020 2020 6465 6620 6164 7661  """.    def adva
+00004b10: 6e63 655f 6170 7065 6e64 2873 656c 662c  nce_append(self,
+00004b20: 2072 643a 2022 5265 6164 7952 6566 2229   rd: "ReadyRef")
+00004b30: 202d 3e20 224c 6967 6874 5265 6164 7922   -> "LightReady"
+00004b40: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00004b50: 2020 2020 2020 4164 7661 6e63 6573 2074        Advances t
+00004b60: 6865 2072 6561 6479 2077 6974 686f 7574  he ready without
+00004b70: 2061 7070 6c79 696e 6720 636f 6d6d 6974   applying commit
+00004b80: 7465 6420 656e 7472 6965 732e 205b 6053  ted entries. [`S
+00004b90: 656c 663a 3a61 6476 616e 6365 5f61 7070  elf::advance_app
+00004ba0: 6c79 605d 206f 720a 2020 2020 2020 2020  ly`] or.        
+00004bb0: 5b60 5365 6c66 3a3a 6164 7661 6e63 655f  [`Self::advance_
+00004bc0: 6170 706c 795f 746f 605d 2073 686f 756c  apply_to`] shoul
+00004bd0: 6420 6265 2075 7365 6420 6c61 7465 7220  d be used later 
+00004be0: 746f 2075 7064 6174 6520 6170 706c 7969  to update applyi
+00004bf0: 6e67 2070 726f 6772 6573 732e 0a0a 2020  ng progress...  
+00004c00: 2020 2020 2020 5265 7475 726e 7320 7468        Returns th
+00004c10: 6520 4c69 6768 7452 6561 6479 2074 6861  e LightReady tha
+00004c20: 7420 636f 6e74 6169 6e73 2063 6f6d 6d69  t contains commi
+00004c30: 7420 696e 6465 782c 2063 6f6d 6d69 7474  t index, committ
+00004c40: 6564 2065 6e74 7269 6573 2061 6e64 206d  ed entries and m
+00004c50: 6573 7361 6765 732e 0a0a 2020 2020 2020  essages...      
+00004c60: 2020 5369 6e63 6520 5265 6164 7920 6d75    Since Ready mu
+00004c70: 7374 2062 6520 7065 7273 6973 7465 6420  st be persisted 
+00004c80: 696e 206f 7264 6572 2c20 6361 6c6c 696e  in order, callin
+00004c90: 6720 7468 6973 2066 756e 6374 696f 6e20  g this function 
+00004ca0: 696d 706c 6963 6974 6c79 206d 6561 6e73  implicitly means
+00004cb0: 0a20 2020 2020 2020 2061 6c6c 2072 6561  .        all rea
+00004cc0: 6479 2063 6f6c 6c65 6374 6564 2062 6566  dy collected bef
+00004cd0: 6f72 6520 6861 7665 2062 6565 6e20 7065  ore have been pe
+00004ce0: 7273 6973 7465 642e 0a20 2020 2020 2020  rsisted..       
+00004cf0: 2022 2222 0a20 2020 2064 6566 2061 6476   """.    def adv
+00004d00: 616e 6365 5f61 7070 656e 645f 6173 796e  ance_append_asyn
+00004d10: 6328 7365 6c66 2c20 7264 3a20 2252 6561  c(self, rd: "Rea
+00004d20: 6479 5265 6622 2920 2d3e 204e 6f6e 653a  dyRef") -> None:
+00004d30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004d40: 2020 2020 2053 616d 6520 6173 205b 6053       Same as [`S
+00004d50: 656c 663a 3a61 6476 616e 6365 5f61 7070  elf::advance_app
+00004d60: 656e 6460 5d20 6578 6365 7074 2074 6861  end`] except tha
+00004d70: 7420 6974 2061 6c6c 6f77 7320 746f 206f  t it allows to o
+00004d80: 6e6c 7920 7374 6f72 6520 7468 6520 7570  nly store the up
+00004d90: 6461 7465 7320 696e 2063 6163 6865 2e0a  dates in cache..
+00004da0: 2020 2020 2020 2020 5b60 5365 6c66 3a3a          [`Self::
+00004db0: 6f6e 5f70 6572 7369 7374 5f72 6561 6479  on_persist_ready
+00004dc0: 605d 2073 686f 756c 6420 6265 2075 7365  `] should be use
+00004dd0: 6420 6c61 7465 7220 746f 2075 7064 6174  d later to updat
+00004de0: 6520 7468 6520 7065 7273 6973 7469 6e67  e the persisting
+00004df0: 2070 726f 6772 6573 732e 0a0a 2020 2020   progress...    
+00004e00: 2020 2020 5261 6674 2077 6f72 6b73 206f      Raft works o
+00004e10: 6e20 616e 2061 7373 756d 7074 696f 6e20  n an assumption 
+00004e20: 7065 7273 6973 7465 6420 7570 6461 7465  persisted update
+00004e30: 7320 7368 6f75 6c64 206e 6f74 2062 6520  s should not be 
+00004e40: 6c6f 7374 2c20 7768 6963 6820 7573 7561  lost, which usua
+00004e50: 6c6c 7920 7265 7175 6972 6573 2065 7870  lly requires exp
+00004e60: 656e 7369 7665 0a20 2020 2020 2020 206f  ensive.        o
+00004e70: 7065 7261 7469 6f6e 7320 6c69 6b65 2060  perations like `
+00004e80: 6673 796e 6360 2e20 6061 6476 616e 6365  fsync`. `advance
+00004e90: 5f61 7070 656e 645f 6173 796e 6360 2061  _append_async` a
+00004ea0: 6c6c 6f77 7320 796f 7520 746f 2063 6f6e  llows you to con
+00004eb0: 7472 6f6c 2074 6865 2072 6174 6520 6f66  trol the rate of
+00004ec0: 2073 7563 6820 6f70 6572 6174 696f 6e73   such operations
+00004ed0: 2061 6e64 0a20 2020 2020 2020 2067 6574   and.        get
+00004ee0: 2061 2072 6561 736f 6e61 626c 6520 6261   a reasonable ba
+00004ef0: 7463 6820 7369 7a65 2e20 486f 7765 7665  tch size. Howeve
+00004f00: 722c 2069 7427 7320 7374 696c 6c20 7265  r, it's still re
+00004f10: 7175 6972 6564 2074 6861 7420 7468 6520  quired that the 
+00004f20: 7570 6461 7465 7320 6361 6e20 6265 2072  updates can be r
+00004f30: 6561 6420 6279 2072 6166 7420 6672 6f6d  ead by raft from
+00004f40: 2074 6865 0a20 2020 2020 2020 2060 5374   the.        `St
+00004f50: 6f72 6167 6560 2074 7261 6974 2062 6566  orage` trait bef
+00004f60: 6f72 6520 6361 6c6c 696e 6720 6061 6476  ore calling `adv
+00004f70: 616e 6365 5f61 7070 656e 645f 6173 796e  ance_append_asyn
+00004f80: 6360 2e0a 2020 2020 2020 2020 2222 220a  c`..        """.
+00004f90: 2020 2020 6465 6620 6861 735f 7265 6164      def has_read
+00004fa0: 7928 7365 6c66 2920 2d3e 2062 6f6f 6c3a  y(self) -> bool:
+00004fb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004fc0: 2020 2020 2048 6173 5265 6164 7920 6361       HasReady ca
+00004fd0: 6c6c 6564 2077 6865 6e20 5261 774e 6f64  lled when RawNod
+00004fe0: 6520 7573 6572 206e 6565 6420 746f 2063  e user need to c
+00004ff0: 6865 636b 2069 6620 616e 7920 5265 6164  heck if any Read
+00005000: 7920 7065 6e64 696e 672e 0a20 2020 2020  y pending..     
+00005010: 2020 2022 2222 0a20 2020 2064 6566 2074     """.    def t
+00005020: 6963 6b28 7365 6c66 2920 2d3e 2062 6f6f  ick(self) -> boo
+00005030: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00005040: 2020 2020 2020 2054 6963 6b20 6164 7661         Tick adva
+00005050: 6e63 6573 2074 6865 2069 6e74 6572 6e61  nces the interna
+00005060: 6c20 6c6f 6769 6361 6c20 636c 6f63 6b20  l logical clock 
+00005070: 6279 2061 2073 696e 676c 6520 7469 636b  by a single tick
+00005080: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00005090: 6e73 2074 7275 6520 746f 2069 6e64 6963  ns true to indic
+000050a0: 6174 6520 7468 6174 2074 6865 7265 2077  ate that there w
+000050b0: 696c 6c20 7072 6f62 6162 6c79 2062 6520  ill probably be 
+000050c0: 736f 6d65 2072 6561 6469 6e65 7373 2077  some readiness w
+000050d0: 6869 6368 0a20 2020 2020 2020 206e 6565  hich.        nee
+000050e0: 6473 2074 6f20 6265 2068 616e 646c 6564  ds to be handled
+000050f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00005100: 2020 6465 6620 7365 745f 6261 7463 685f    def set_batch_
+00005110: 6170 7065 6e64 2873 656c 662c 2062 6174  append(self, bat
+00005120: 6368 5f61 7070 656e 643a 2062 6f6f 6c29  ch_append: bool)
+00005130: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00005140: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
+00005150: 7420 7768 6574 6865 7220 746f 2062 6174  t whether to bat
+00005160: 6368 2061 7070 656e 6420 6d73 6720 6174  ch append msg at
+00005170: 2072 756e 7469 6d65 2e0a 2020 2020 2020   runtime..      
+00005180: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00005190: 745f 7072 696f 7269 7479 2873 656c 662c  t_priority(self,
+000051a0: 2070 7269 6f72 6974 793a 2069 6e74 2920   priority: int) 
+000051b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000051c0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+000051d0: 7320 7072 696f 7269 7479 206f 6620 6e6f  s priority of no
+000051e0: 6465 2e0a 2020 2020 2020 2020 2222 220a  de..        """.
+000051f0: 2020 2020 6465 6620 7265 706f 7274 5f73      def report_s
+00005200: 6e61 7073 686f 7428 7365 6c66 2c20 6964  napshot(self, id
+00005210: 3a20 696e 742c 2073 6e61 7073 686f 743a  : int, snapshot:
+00005220: 2022 536e 6170 7368 6f74 5374 6174 7573   "SnapshotStatus
+00005230: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
+00005240: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005250: 5265 706f 7274 536e 6170 7368 6f74 2072  ReportSnapshot r
+00005260: 6570 6f72 7473 2074 6865 2073 7461 7475  eports the statu
+00005270: 7320 6f66 2074 6865 2073 656e 7420 736e  s of the sent sn
+00005280: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
+00005290: 2222 220a 2020 2020 6465 6620 7265 706f  """.    def repo
+000052a0: 7274 5f75 6e72 6561 6368 6162 6c65 2873  rt_unreachable(s
+000052b0: 656c 662c 2069 643a 2069 6e74 2920 2d3e  elf, id: int) ->
+000052c0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000052d0: 2222 0a20 2020 2020 2020 2052 6570 6f72  "".        Repor
+000052e0: 7455 6e72 6561 6368 6162 6c65 2072 6570  tUnreachable rep
+000052f0: 6f72 7473 2074 6865 2067 6976 656e 206e  orts the given n
+00005300: 6f64 6520 6973 206e 6f74 2072 6561 6368  ode is not reach
+00005310: 6162 6c65 2066 6f72 2074 6865 206c 6173  able for the las
+00005320: 7420 7365 6e64 2e0a 2020 2020 2020 2020  t send..        
+00005330: 2222 220a 2020 2020 6465 6620 7472 616e  """.    def tran
+00005340: 7366 6572 5f6c 6561 6465 7228 7365 6c66  sfer_leader(self
+00005350: 2c20 7472 616e 7366 6572 6565 3a20 696e  , transferee: in
+00005360: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+00005370: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005380: 5472 616e 7366 6572 4c65 6164 6572 2074  TransferLeader t
+00005390: 7269 6573 2074 6f20 7472 616e 7366 6572  ries to transfer
+000053a0: 206c 6561 6465 7273 6869 7020 746f 2074   leadership to t
+000053b0: 6865 2067 6976 656e 2074 7261 6e73 6665  he given transfe
+000053c0: 7265 652e 0a20 2020 2020 2020 2022 2222  ree..        """
+000053d0: 0a20 2020 2064 6566 2073 6e61 7028 7365  .    def snap(se
+000053e0: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+000053f0: 2253 6e61 7073 686f 7452 6566 225d 3a0a  "SnapshotRef"]:.
+00005400: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005410: 2020 2020 4772 6162 7320 7468 6520 736e      Grabs the sn
+00005420: 6170 7368 6f74 2066 726f 6d20 7468 6520  apshot from the 
+00005430: 7261 6674 2069 6620 6176 6169 6c61 626c  raft if availabl
+00005440: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00005450: 2020 2064 6566 2073 7465 7028 7365 6c66     def step(self
+00005460: 2c20 6d73 673a 2022 4d65 7373 6167 6522  , msg: "Message"
+00005470: 207c 2022 4d65 7373 6167 6552 6566 2229   | "MessageRef")
+00005480: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00005490: 2020 2222 220a 2020 2020 2020 2020 5374    """.        St
+000054a0: 6570 2061 6476 616e 6365 7320 7468 6520  ep advances the 
+000054b0: 7374 6174 6520 6d61 6368 696e 6520 7573  state machine us
+000054c0: 696e 6720 7468 6520 6769 7665 6e20 6d65  ing the given me
+000054d0: 7373 6167 652e 0a20 2020 2020 2020 2022  ssage..        "
+000054e0: 2222 0a20 2020 2064 6566 2073 6b69 705f  "".    def skip_
+000054f0: 6263 6173 745f 636f 6d6d 6974 2873 656c  bcast_commit(sel
+00005500: 662c 2073 6b69 703a 2062 6f6f 6c29 202d  f, skip: bool) -
+00005510: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00005520: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
+00005530: 7768 6574 6865 7220 736b 6970 2062 726f  whether skip bro
+00005540: 6164 6361 7374 2065 6d70 7479 2063 6f6d  adcast empty com
+00005550: 6d69 7420 6d65 7373 6167 6573 2061 7420  mit messages at 
+00005560: 7275 6e74 696d 652e 0a20 2020 2020 2020  runtime..       
+00005570: 2022 2222 0a20 2020 2064 6566 2063 616d   """.    def cam
+00005580: 7061 6967 6e28 7365 6c66 2920 2d3e 204e  paign(self) -> N
+00005590: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000055a0: 0a20 2020 2020 2020 2043 616d 7061 6967  .        Campaig
+000055b0: 6e20 6361 7573 6573 2074 6869 7320 5261  n causes this Ra
+000055c0: 774e 6f64 6520 746f 2074 7261 6e73 6974  wNode to transit
+000055d0: 696f 6e20 746f 2063 616e 6469 6461 7465  ion to candidate
+000055e0: 2073 7461 7465 2e0a 2020 2020 2020 2020   state..        
+000055f0: 2222 220a 2020 2020 6465 6620 7072 6f70  """.    def prop
+00005600: 6f73 6528 7365 6c66 2c20 636f 6e74 6578  ose(self, contex
+00005610: 743a 2062 7974 6573 2c20 6461 7461 3a20  t: bytes, data: 
+00005620: 6279 7465 7329 202d 3e20 4e6f 6e65 3a0a  bytes) -> None:.
+00005630: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005640: 2020 2020 5072 6f70 6f73 6520 7072 6f70      Propose prop
+00005650: 6f73 6573 2064 6174 6120 6265 2061 7070  oses data be app
+00005660: 656e 6465 6420 746f 2074 6865 2072 6166  ended to the raf
+00005670: 7420 6c6f 672e 0a20 2020 2020 2020 2022  t log..        "
+00005680: 2222 0a20 2020 2064 6566 2070 726f 706f  "".    def propo
+00005690: 7365 5f63 6f6e 665f 6368 616e 6765 280a  se_conf_change(.
+000056a0: 2020 2020 2020 2020 7365 6c66 2c20 636f          self, co
+000056b0: 6e74 6578 743a 2062 7974 6573 2c20 6363  ntext: bytes, cc
+000056c0: 3a20 2243 6f6e 6643 6861 6e67 6522 207c  : "ConfChange" |
+000056d0: 2022 436f 6e66 4368 616e 6765 5265 6622   "ConfChangeRef"
+000056e0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+000056f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005700: 2020 2020 5072 6f70 6f73 6543 6f6e 6643      ProposeConfC
+00005710: 6861 6e67 6520 7072 6f70 6f73 6573 2061  hange proposes a
+00005720: 2063 6f6e 6669 6720 6368 616e 6765 2e0a   config change..
+00005730: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
+00005740: 6e6f 6465 2065 6e74 6572 7320 6a6f 696e  node enters join
+00005750: 7420 7374 6174 6520 7769 7468 2060 6175  t state with `au
+00005760: 746f 5f6c 6561 7665 6020 7365 7420 746f  to_leave` set to
+00005770: 2074 7275 652c 2069 7427 730a 2020 2020   true, it's.    
+00005780: 2020 2020 6361 6c6c 6572 2773 2072 6573      caller's res
+00005790: 706f 6e73 6962 696c 6974 7920 746f 2070  ponsibility to p
+000057a0: 726f 706f 7365 2061 6e20 656d 7074 7920  ropose an empty 
+000057b0: 636f 6e66 2063 6861 6e67 6520 6167 6169  conf change agai
+000057c0: 6e20 746f 2066 6f72 6365 0a20 2020 2020  n to force.     
+000057d0: 2020 206c 6561 7669 6e67 206a 6f69 6e74     leaving joint
+000057e0: 2073 7461 7465 2e0a 2020 2020 2020 2020   state..        
+000057f0: 2222 220a 2020 2020 6465 6620 7072 6f70  """.    def prop
+00005800: 6f73 655f 636f 6e66 5f63 6861 6e67 655f  ose_conf_change_
+00005810: 7632 280a 2020 2020 2020 2020 7365 6c66  v2(.        self
+00005820: 2c20 636f 6e74 6578 743a 2062 7974 6573  , context: bytes
+00005830: 2c20 6363 3a20 2243 6f6e 6643 6861 6e67  , cc: "ConfChang
+00005840: 6556 3222 207c 2022 436f 6e66 4368 616e  eV2" | "ConfChan
+00005850: 6765 5632 5265 6622 0a20 2020 2029 202d  geV2Ref".    ) -
+00005860: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00005870: 2222 220a 2020 2020 2020 2020 5072 6f70  """.        Prop
+00005880: 6f73 6543 6f6e 6643 6861 6e67 6520 7072  oseConfChange pr
+00005890: 6f70 6f73 6573 2061 2063 6f6e 6669 6720  oposes a config 
+000058a0: 6368 616e 6765 2e0a 0a20 2020 2020 2020  change...       
+000058b0: 2049 6620 7468 6520 6e6f 6465 2065 6e74   If the node ent
+000058c0: 6572 7320 6a6f 696e 7420 7374 6174 6520  ers joint state 
+000058d0: 7769 7468 2060 6175 746f 5f6c 6561 7665  with `auto_leave
+000058e0: 6020 7365 7420 746f 2074 7275 652c 2069  ` set to true, i
+000058f0: 7427 730a 2020 2020 2020 2020 6361 6c6c  t's.        call
+00005900: 6572 2773 2072 6573 706f 6e73 6962 696c  er's responsibil
+00005910: 6974 7920 746f 2070 726f 706f 7365 2061  ity to propose a
+00005920: 6e20 656d 7074 7920 636f 6e66 2063 6861  n empty conf cha
+00005930: 6e67 6520 6167 6169 6e20 746f 2066 6f72  nge again to for
+00005940: 6365 0a20 2020 2020 2020 206c 6561 7669  ce.        leavi
+00005950: 6e67 206a 6f69 6e74 2073 7461 7465 2e0a  ng joint state..
+00005960: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005970: 6465 6620 6170 706c 795f 636f 6e66 5f63  def apply_conf_c
+00005980: 6861 6e67 6528 7365 6c66 2c20 6363 3a20  hange(self, cc: 
+00005990: 2243 6f6e 6643 6861 6e67 6522 207c 2022  "ConfChange" | "
+000059a0: 436f 6e66 4368 616e 6765 5265 6622 2920  ConfChangeRef") 
+000059b0: 2d3e 2043 6f6e 6653 7461 7465 3a0a 2020  -> ConfState:.  
+000059c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000059d0: 2020 4170 706c 6965 7320 6120 636f 6e66    Applies a conf
+000059e0: 6967 2063 6861 6e67 6520 746f 2074 6865  ig change to the
+000059f0: 206c 6f63 616c 206e 6f64 652e 2054 6865   local node. The
+00005a00: 2061 7070 206d 7573 7420 6361 6c6c 2074   app must call t
+00005a10: 6869 7320 7768 656e 2069 740a 2020 2020  his when it.    
+00005a20: 2020 2020 6170 706c 6965 7320 6120 636f      applies a co
+00005a30: 6e66 6967 7572 6174 696f 6e20 6368 616e  nfiguration chan
+00005a40: 6765 2c20 6578 6365 7074 2077 6865 6e20  ge, except when 
+00005a50: 6974 2064 6563 6964 6573 2074 6f20 7265  it decides to re
+00005a60: 6a65 6374 2074 6865 0a20 2020 2020 2020  ject the.       
+00005a70: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
+00005a80: 6861 6e67 652c 2069 6e20 7768 6963 6820  hange, in which 
+00005a90: 6361 7365 206e 6f20 6361 6c6c 206d 7573  case no call mus
+00005aa0: 7420 7461 6b65 2070 6c61 6365 2e0a 2020  t take place..  
+00005ab0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00005ac0: 6620 6170 706c 795f 636f 6e66 5f63 6861  f apply_conf_cha
+00005ad0: 6e67 655f 7632 280a 2020 2020 2020 2020  nge_v2(.        
+00005ae0: 7365 6c66 2c20 6363 3a20 2243 6f6e 6643  self, cc: "ConfC
+00005af0: 6861 6e67 6556 3222 207c 2022 436f 6e66  hangeV2" | "Conf
+00005b00: 4368 616e 6765 5632 5265 6622 0a20 2020  ChangeV2Ref".   
+00005b10: 2029 202d 3e20 2243 6f6e 6653 7461 7465   ) -> "ConfState
+00005b20: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+00005b30: 2020 2020 2020 2041 7070 6c69 6573 2061         Applies a
+00005b40: 2063 6f6e 6669 6720 6368 616e 6765 2074   config change t
+00005b50: 6f20 7468 6520 6c6f 6361 6c20 6e6f 6465  o the local node
+00005b60: 2e20 5468 6520 6170 7020 6d75 7374 2063  . The app must c
+00005b70: 616c 6c20 7468 6973 2077 6865 6e20 6974  all this when it
+00005b80: 0a20 2020 2020 2020 2061 7070 6c69 6573  .        applies
+00005b90: 2061 2063 6f6e 6669 6775 7261 7469 6f6e   a configuration
+00005ba0: 2063 6861 6e67 652c 2065 7863 6570 7420   change, except 
+00005bb0: 7768 656e 2069 7420 6465 6369 6465 7320  when it decides 
+00005bc0: 746f 2072 656a 6563 7420 7468 650a 2020  to reject the.  
+00005bd0: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+00005be0: 696f 6e20 6368 616e 6765 2c20 696e 2077  ion change, in w
+00005bf0: 6869 6368 2063 6173 6520 6e6f 2063 616c  hich case no cal
+00005c00: 6c20 6d75 7374 2074 616b 6520 706c 6163  l must take plac
+00005c10: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00005c20: 2020 2064 6566 2070 696e 6728 7365 6c66     def ping(self
+00005c30: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00005c40: 2020 2022 2222 0a20 2020 2020 2020 2042     """.        B
+00005c50: 726f 6164 6361 7374 2068 6561 7274 6265  roadcast heartbe
+00005c60: 6174 7320 746f 2061 6c6c 2074 6865 2066  ats to all the f
+00005c70: 6f6c 6c6f 7765 7273 2e0a 0a20 2020 2020  ollowers...     
+00005c80: 2020 2049 6620 6974 2773 206e 6f74 206c     If it's not l
+00005c90: 6561 6465 722c 206e 6f74 6869 6e67 2077  eader, nothing w
+00005ca0: 696c 6c20 6861 7070 656e 2e0a 2020 2020  ill happen..    
+00005cb0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00005cc0: 6f6e 5f70 6572 7369 7374 5f72 6561 6479  on_persist_ready
+00005cd0: 2873 656c 662c 206e 756d 6265 723a 2069  (self, number: i
+00005ce0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00005cf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005d00: 204e 6f74 6966 6965 7320 7468 6174 2074   Notifies that t
+00005d10: 6865 2072 6561 6479 206f 6620 7468 6973  he ready of this
+00005d20: 206e 756d 6265 7220 6861 7320 6265 656e   number has been
+00005d30: 2070 6572 7369 7374 6564 2e0a 0a20 2020   persisted...   
+00005d40: 2020 2020 2053 696e 6365 2052 6561 6479       Since Ready
+00005d50: 206d 7573 7420 6265 2070 6572 7369 7374   must be persist
+00005d60: 6564 2069 6e20 6f72 6465 722c 2063 616c  ed in order, cal
+00005d70: 6c69 6e67 2074 6869 7320 6675 6e63 7469  ling this functi
+00005d80: 6f6e 2069 6d70 6c69 6369 746c 7920 6d65  on implicitly me
+00005d90: 616e 730a 2020 2020 2020 2020 616c 6c20  ans.        all 
+00005da0: 7265 6164 6965 7320 7769 7468 206e 756d  readies with num
+00005db0: 6265 7273 2073 6d61 6c6c 6572 2074 6861  bers smaller tha
+00005dc0: 6e20 7468 6973 206f 6e65 2068 6176 6520  n this one have 
+00005dd0: 6265 656e 2070 6572 7369 7374 6564 2e0a  been persisted..
+00005de0: 0a20 2020 2020 2020 205b 6053 656c 663a  .        [`Self:
+00005df0: 3a68 6173 5f72 6561 6479 605d 2061 6e64  :has_ready`] and
+00005e00: 205b 6053 656c 663a 3a72 6561 6479 605d   [`Self::ready`]
+00005e10: 2073 686f 756c 6420 6265 2063 616c 6c65   should be calle
+00005e20: 6420 6c61 7465 7220 746f 2068 616e 646c  d later to handl
+00005e30: 6520 6675 7274 6865 720a 2020 2020 2020  e further.      
+00005e40: 2020 7570 6461 7465 7320 7468 6174 2062    updates that b
+00005e50: 6563 6f6d 6520 7661 6c69 6420 6166 7465  ecome valid afte
+00005e60: 7220 7265 6164 7920 6265 696e 6720 7065  r ready being pe
+00005e70: 7273 6973 7465 642e 0a20 2020 2020 2020  rsisted..       
+00005e80: 2022 2222 0a20 2020 2064 6566 2072 6561   """.    def rea
+00005e90: 645f 696e 6465 7828 7365 6c66 2c20 7263  d_index(self, rc
+00005ea0: 7478 3a20 6279 7465 7329 202d 3e20 4e6f  tx: bytes) -> No
+00005eb0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00005ec0: 2020 2020 2020 2020 5265 6164 496e 6465          ReadInde
+00005ed0: 7820 7265 7175 6573 7473 2061 2072 6561  x requests a rea
+00005ee0: 6420 7374 6174 652e 2054 6865 2072 6561  d state. The rea
+00005ef0: 6420 7374 6174 6520 7769 6c6c 2062 6520  d state will be 
+00005f00: 7365 7420 696e 2072 6561 6479 2e0a 2020  set in ready..  
+00005f10: 2020 2020 2020 5265 6164 2053 7461 7465        Read State
+00005f20: 2068 6173 2061 2072 6561 6420 696e 6465   has a read inde
+00005f30: 782e 204f 6e63 6520 7468 6520 6170 706c  x. Once the appl
+00005f40: 6963 6174 696f 6e20 6164 7661 6e63 6573  ication advances
+00005f50: 2066 7572 7468 6572 2074 6861 6e20 7468   further than th
+00005f60: 6520 7265 6164 0a20 2020 2020 2020 2069  e read.        i
+00005f70: 6e64 6578 2c20 616e 7920 6c69 6e65 6172  ndex, any linear
+00005f80: 697a 6162 6c65 2072 6561 6420 7265 7175  izable read requ
+00005f90: 6573 7473 2069 7373 7565 6420 6265 666f  ests issued befo
+00005fa0: 7265 2074 6865 2072 6561 6420 7265 7175  re the read requ
+00005fb0: 6573 7420 6361 6e20 6265 0a20 2020 2020  est can be.     
+00005fc0: 2020 2070 726f 6365 7373 6564 2073 6166     processed saf
+00005fd0: 656c 792e 2054 6865 2072 6561 6420 7374  ely. The read st
+00005fe0: 6174 6520 7769 6c6c 2068 6176 6520 7468  ate will have th
+00005ff0: 6520 7361 6d65 2072 6374 7820 6174 7461  e same rctx atta
+00006000: 6368 6564 2e0a 2020 2020 2020 2020 2222  ched..        ""
+00006010: 220a 2020 2020 6465 6620 7265 6164 7928  ".    def ready(
+00006020: 7365 6c66 2920 2d3e 2052 6561 6479 3a0a  self) -> Ready:.
+00006030: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006040: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+00006050: 6f75 7473 7461 6e64 696e 6720 776f 726b  outstanding work
+00006060: 2074 6861 7420 7468 6520 6170 706c 6963   that the applic
+00006070: 6174 696f 6e20 6e65 6564 7320 746f 2068  ation needs to h
+00006080: 616e 646c 652e 0a0a 2020 2020 2020 2020  andle...        
+00006090: 5468 6973 2069 6e63 6c75 6465 7320 6170  This includes ap
+000060a0: 7065 6e64 696e 6720 616e 6420 6170 706c  pending and appl
+000060b0: 7969 6e67 2065 6e74 7269 6573 206f 7220  ying entries or 
+000060c0: 6120 736e 6170 7368 6f74 2c20 7570 6461  a snapshot, upda
+000060d0: 7469 6e67 2074 6865 2048 6172 6453 7461  ting the HardSta
+000060e0: 7465 2c0a 2020 2020 2020 2020 616e 6420  te,.        and 
+000060f0: 7365 6e64 696e 6720 6d65 7373 6167 6573  sending messages
+00006100: 2e20 5468 6520 7265 7475 726e 6564 2060  . The returned `
+00006110: 5265 6164 7960 202a 4d55 5354 2a20 6265  Ready` *MUST* be
+00006120: 2068 616e 646c 6564 2061 6e64 2073 7562   handled and sub
+00006130: 7365 7175 656e 746c 790a 2020 2020 2020  sequently.      
+00006140: 2020 7061 7373 6564 2062 6163 6b20 7669    passed back vi
+00006150: 6120 6061 6476 616e 6365 6020 6f72 2069  a `advance` or i
+00006160: 7473 2066 616d 696c 6965 732e 2042 6566  ts families. Bef
+00006170: 6f72 6520 7468 6174 2c20 2a44 4f20 4e4f  ore that, *DO NO
+00006180: 542a 2063 616c 6c20 616e 7920 6675 6e63  T* call any func
+00006190: 7469 6f6e 206c 696b 650a 2020 2020 2020  tion like.      
+000061a0: 2020 6073 7465 7060 2c20 6070 726f 706f    `step`, `propo
+000061b0: 7365 602c 2060 6361 6d70 6169 676e 6020  se`, `campaign` 
+000061c0: 746f 2063 6861 6e67 6520 696e 7465 726e  to change intern
+000061d0: 616c 2073 7461 7465 2e0a 0a20 2020 2020  al state...     
+000061e0: 2020 205b 6053 656c 663a 3a68 6173 5f72     [`Self::has_r
+000061f0: 6561 6479 605d 2073 686f 756c 6420 6265  eady`] should be
+00006200: 2063 616c 6c65 6420 6669 7273 7420 746f   called first to
+00006210: 2063 6865 636b 2069 6620 6974 2773 206e   check if it's n
+00006220: 6563 6573 7361 7279 2074 6f20 6861 6e64  ecessary to hand
+00006230: 6c65 2074 6865 2072 6561 6479 2e0a 2020  le the ready..  
+00006240: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00006250: 6620 7265 7175 6573 745f 736e 6170 7368  f request_snapsh
+00006260: 6f74 2873 656c 6629 202d 3e20 2252 6561  ot(self) -> "Rea
+00006270: 6479 223a 0a20 2020 2020 2020 2022 2222  dy":.        """
+00006280: 0a20 2020 2020 2020 2052 6571 7565 7374  .        Request
+00006290: 2061 2073 6e61 7073 686f 7420 6672 6f6d   a snapshot from
+000062a0: 2061 206c 6561 6465 722e 0a20 2020 2020   a leader..     
+000062b0: 2020 2054 6865 2073 6e61 7073 686f 7427     The snapshot'
+000062c0: 7320 696e 6465 7820 6d75 7374 2062 6520  s index must be 
+000062d0: 6772 6561 7465 7220 6f72 2065 7175 616c  greater or equal
+000062e0: 2074 6f20 7468 6520 7265 7175 6573 745f   to the request_
+000062f0: 696e 6465 7820 286c 6173 745f 696e 6465  index (last_inde
+00006300: 7829 206f 720a 2020 2020 2020 2020 7468  x) or.        th
+00006310: 6520 6c65 6164 6572 2773 2074 6572 6d20  e leader's term 
+00006320: 6d75 7374 2062 6520 6772 6561 7465 7220  must be greater 
+00006330: 7468 616e 2074 6865 2072 6571 7565 7374  than the request
+00006340: 2074 6572 6d20 286c 6173 745f 696e 6465   term (last_inde
+00006350: 7827 7320 7465 726d 292e 0a20 2020 2020  x's term)..     
+00006360: 2020 2022 2222 0a20 2020 2064 6566 206f     """.    def o
+00006370: 6e5f 656e 7472 6965 735f 6665 7463 6865  n_entries_fetche
+00006380: 6428 7365 6c66 2920 2d3e 204e 6f6e 653a  d(self) -> None:
+00006390: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000063a0: 2020 2020 2041 2063 616c 6c62 6163 6b20       A callback 
+000063b0: 7768 656e 2065 6e74 7269 6573 2061 7265  when entries are
+000063c0: 2066 6574 6368 6564 2061 7379 6e63 6872   fetched asynchr
+000063d0: 6f6e 6f75 736c 792e 0a20 2020 2020 2020  onously..       
+000063e0: 2054 6865 2063 6f6e 7465 7874 2073 686f   The context sho
+000063f0: 756c 6420 7072 6f76 6964 6520 7468 6520  uld provide the 
+00006400: 636f 6e74 6578 7420 7061 7373 6564 2066  context passed f
+00006410: 726f 6d20 5374 6f72 6167 652e 656e 7469  rom Storage.enti
+00006420: 7265 7328 292e 0a20 2020 2020 2020 2053  res()..        S
+00006430: 6565 206d 6f72 6520 696e 2074 6865 2063  ee more in the c
+00006440: 6f6d 6d65 6e74 206f 6620 5374 6f72 6167  omment of Storag
+00006450: 652e 656e 7469 7265 7328 292e 0a0a 2020  e.entires()...  
+00006460: 2020 2020 2020 2320 5061 6e69 6373 0a0a        # Panics..
+00006470: 2020 2020 2020 2020 5061 6e69 6373 2069          Panics i
+00006480: 6620 7061 7373 6564 2077 6974 6820 7468  f passed with th
+00006490: 6520 636f 6e74 6578 7420 6f66 2063 6f6e  e context of con
+000064a0: 7465 7874 2e63 616e 5f61 7379 6e63 2829  text.can_async()
+000064b0: 203d 3d20 6661 6c73 650a 2020 2020 2020   == false.      
+000064c0: 2020 2222 220a 0a63 6c61 7373 2049 6e4d    """..class InM
+000064d0: 656d 6f72 7952 6177 4e6f 6465 285f 5f41  emoryRawNode(__A
+000064e0: 5049 5f52 6177 4e6f 6465 293a 0a20 2020  PI_RawNode):.   
+000064f0: 2022 2222 0a20 2020 2052 6177 4e6f 6465   """.    RawNode
+00006500: 2069 7320 6120 7468 7265 6164 2d75 6e73   is a thread-uns
+00006510: 6166 6520 4e6f 6465 2e0a 2020 2020 5468  afe Node..    Th
+00006520: 6520 6d65 7468 6f64 7320 6f66 2074 6869  e methods of thi
+00006530: 7320 7374 7275 6374 2063 6f72 7265 7370  s struct corresp
+00006540: 6f6e 6420 746f 2074 6865 206d 6574 686f  ond to the metho
+00006550: 6473 206f 6620 4e6f 6465 2061 6e64 2061  ds of Node and a
+00006560: 7265 2064 6573 6372 6962 6564 0a20 2020  re described.   
+00006570: 206d 6f72 6520 6675 6c6c 7920 7468 6572   more fully ther
+00006580: 652e 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
+00006590: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000065a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000065b0: 2020 2020 6366 673a 2022 436f 6e66 6967      cfg: "Config
+000065c0: 2220 7c20 2243 6f6e 6669 6752 6566 222c  " | "ConfigRef",
+000065d0: 0a20 2020 2020 2020 2073 746f 7265 3a20  .        store: 
+000065e0: 224d 656d 5374 6f72 6167 6522 207c 2022  "MemStorage" | "
+000065f0: 4d65 6d53 746f 7261 6765 5265 6622 2c0a  MemStorageRef",.
+00006600: 2020 2020 2020 2020 6c6f 6767 6572 3a20          logger: 
+00006610: 224c 6f67 6765 7222 207c 2022 4c6f 6767  "Logger" | "Logg
+00006620: 6572 5265 6622 207c 2022 5468 7265 6164  erRef" | "Thread
+00006630: 5361 6665 4c6f 6767 6572 222c 0a20 2020  SafeLogger",.   
+00006640: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+00006650: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
+00006660: 2873 656c 6629 202d 3e20 2249 6e4d 656d  (self) -> "InMem
+00006670: 6f72 7952 6177 4e6f 6465 5265 6622 3a20  oryRawNodeRef": 
+00006680: 2e2e 2e0a 2020 2020 6465 6620 6765 745f  ....    def get_
+00006690: 7261 6674 2873 656c 6629 202d 3e20 2249  raft(self) -> "I
+000066a0: 6e4d 656d 6f72 7952 6166 7452 6566 223a  nMemoryRaftRef":
+000066b0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+000066c0: 0a20 2020 2064 6566 2073 746f 7265 2873  .    def store(s
+000066d0: 656c 6629 202d 3e20 224d 656d 5374 6f72  elf) -> "MemStor
+000066e0: 6167 6552 6566 223a 0a20 2020 2020 2020  ageRef":.       
+000066f0: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
+00006700: 7374 6f72 6520 6173 2061 206d 7574 6162  store as a mutab
+00006710: 6c65 2072 6566 6572 656e 6365 2e22 2222  le reference."""
+00006720: 0a0a 636c 6173 7320 496e 4d65 6d6f 7279  ..class InMemory
+00006730: 5261 774e 6f64 6552 6566 285f 5f41 5049  RawNodeRef(__API
+00006740: 5f52 6177 4e6f 6465 293a 0a20 2020 2022  _RawNode):.    "
+00006750: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+00006760: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+00006770: 6049 6e4d 656d 6f72 7952 6177 4e6f 6465  `InMemoryRawNode
+00006780: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
+00006790: 6465 6620 6765 745f 7261 6674 2873 656c  def get_raft(sel
+000067a0: 6629 202d 3e20 2249 6e4d 656d 6f72 7952  f) -> "InMemoryR
+000067b0: 6166 7452 6566 223a 0a20 2020 2020 2020  aftRef":.       
+000067c0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+000067d0: 2073 746f 7265 2873 656c 6629 202d 3e20   store(self) -> 
+000067e0: 224d 656d 5374 6f72 6167 6552 6566 223a  "MemStorageRef":
+000067f0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00006800: 726e 7320 7468 6520 7374 6f72 6520 6173  rns the store as
+00006810: 2061 206d 7574 6162 6c65 2072 6566 6572   a mutable refer
+00006820: 656e 6365 2e22 2222 0a20 2020 2023 2064  ence.""".    # d
+00006830: 6566 2073 7461 7475 7328 7365 6c66 2920  ef status(self) 
+00006840: 2d3e 2049 6e4d 656d 6f72 7953 7461 7475  -> InMemoryStatu
+00006850: 733a 0a20 2020 2023 2020 2020 2022 2222  s:.    #     """
+00006860: 0a20 2020 2023 2020 2020 2053 7461 7475  .    #     Statu
+00006870: 7320 7265 7475 726e 7320 7468 6520 6375  s returns the cu
+00006880: 7272 656e 7420 7374 6174 7573 206f 6620  rrent status of 
+00006890: 7468 6520 6769 7665 6e20 6772 6f75 702e  the given group.
+000068a0: 0a20 2020 2023 2020 2020 2022 2222 0a0a  .    #     """..
+000068b0: 636c 6173 7320 5261 774e 6f64 6528 5f5f  class RawNode(__
+000068c0: 4150 495f 5261 774e 6f64 6529 3a0a 2020  API_RawNode):.  
+000068d0: 2020 2222 220a 2020 2020 5261 774e 6f64    """.    RawNod
+000068e0: 6520 6973 2061 2074 6872 6561 642d 756e  e is a thread-un
+000068f0: 7361 6665 204e 6f64 652e 0a20 2020 2054  safe Node..    T
+00006900: 6865 206d 6574 686f 6473 206f 6620 7468  he methods of th
+00006910: 6973 2073 7472 7563 7420 636f 7272 6573  is struct corres
+00006920: 706f 6e64 2074 6f20 7468 6520 6d65 7468  pond to the meth
+00006930: 6f64 7320 6f66 204e 6f64 6520 616e 6420  ods of Node and 
+00006940: 6172 6520 6465 7363 7269 6265 640a 2020  are described.  
+00006950: 2020 6d6f 7265 2066 756c 6c79 2074 6865    more fully the
+00006960: 7265 2e0a 2020 2020 2222 220a 0a20 2020  re..    """..   
+00006970: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00006980: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00006990: 2020 2020 2063 6667 3a20 2243 6f6e 6669       cfg: "Confi
+000069a0: 6722 207c 2022 436f 6e66 6967 5265 6622  g" | "ConfigRef"
+000069b0: 2c0a 2020 2020 2020 2020 7374 6f72 653a  ,.        store:
+000069c0: 2022 5374 6f72 6167 6522 207c 2022 5374   "Storage" | "St
+000069d0: 6f72 6167 6552 6566 222c 0a20 2020 2020  orageRef",.     
+000069e0: 2020 206c 6f67 6765 723a 2022 4c6f 6767     logger: "Logg
+000069f0: 6572 2220 7c20 224c 6f67 6765 7252 6566  er" | "LoggerRef
+00006a00: 2220 7c20 2254 6872 6561 6453 6166 654c  " | "ThreadSafeL
+00006a10: 6f67 6765 7222 2c0a 2020 2020 2920 2d3e  ogger",.    ) ->
+00006a20: 204e 6f6e 653a 202e 2e2e 0a20 2020 2064   None: ....    d
+00006a30: 6566 206d 616b 655f 7265 6628 7365 6c66  ef make_ref(self
+00006a40: 2920 2d3e 2022 5261 774e 6f64 6552 6566  ) -> "RawNodeRef
+00006a50: 223a 202e 2e2e 0a20 2020 2064 6566 2067  ": ....    def g
+00006a60: 6574 5f72 6166 7428 7365 6c66 2920 2d3e  et_raft(self) ->
+00006a70: 2022 5261 6674 5265 6622 3a0a 2020 2020   "RaftRef":.    
+00006a80: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+00006a90: 6465 6620 7374 6f72 6528 7365 6c66 2920  def store(self) 
+00006aa0: 2d3e 2022 5374 6f72 6167 6552 6566 223a  -> "StorageRef":
+00006ab0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00006ac0: 726e 7320 7468 6520 7374 6f72 6520 6173  rns the store as
+00006ad0: 2061 206d 7574 6162 6c65 2072 6566 6572   a mutable refer
+00006ae0: 656e 6365 2e22 2222 0a20 2020 2023 2064  ence.""".    # d
+00006af0: 6566 2073 7461 7475 7328 7365 6c66 2920  ef status(self) 
+00006b00: 2d3e 2053 7461 7475 733a 0a20 2020 2023  -> Status:.    #
+00006b10: 2020 2020 2022 2222 0a20 2020 2023 2020       """.    #  
+00006b20: 2020 2053 7461 7475 7320 7265 7475 726e     Status return
+00006b30: 7320 7468 6520 6375 7272 656e 7420 7374  s the current st
+00006b40: 6174 7573 206f 6620 7468 6520 6769 7665  atus of the give
+00006b50: 6e20 6772 6f75 702e 0a20 2020 2023 2020  n group..    #  
+00006b60: 2020 2022 2222 0a0a 636c 6173 7320 5261     """..class Ra
+00006b70: 774e 6f64 6552 6566 285f 5f41 5049 5f52  wNodeRef(__API_R
+00006b80: 6177 4e6f 6465 293a 0a20 2020 2022 2222  awNode):.    """
+00006b90: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
+00006ba0: 7970 6520 6f66 203a 636c 6173 733a 6052  ype of :class:`R
+00006bb0: 6177 4e6f 6465 602e 0a20 2020 2022 2222  awNode`..    """
+00006bc0: 0a0a 2020 2020 6465 6620 6765 745f 7261  ..    def get_ra
+00006bd0: 6674 2873 656c 6629 202d 3e20 2252 6166  ft(self) -> "Raf
+00006be0: 7452 6566 223a 0a20 2020 2020 2020 2022  tRef":.        "
+00006bf0: 2222 2022 2222 0a20 2020 2064 6566 2073  "" """.    def s
+00006c00: 746f 7265 2873 656c 6629 202d 3e20 2253  tore(self) -> "S
+00006c10: 746f 7261 6765 5265 6622 3a0a 2020 2020  torageRef":.    
+00006c20: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
+00006c30: 6865 2073 746f 7265 2061 7320 6120 6d75  he store as a mu
+00006c40: 7461 626c 6520 7265 6665 7265 6e63 652e  table reference.
+00006c50: 2222 220a 2020 2020 2320 6465 6620 7374  """.    # def st
+00006c60: 6174 7573 2873 656c 6629 202d 3e20 496e  atus(self) -> In
+00006c70: 4d65 6d6f 7279 5374 6174 7573 3a0a 2020  MemoryStatus:.  
+00006c80: 2020 2320 2020 2020 2222 220a 2020 2020    #     """.    
+00006c90: 2320 2020 2020 5374 6174 7573 2072 6574  #     Status ret
+00006ca0: 7572 6e73 2074 6865 2063 7572 7265 6e74  urns the current
+00006cb0: 2073 7461 7475 7320 6f66 2074 6865 2067   status of the g
+00006cc0: 6976 656e 2067 726f 7570 2e0a 2020 2020  iven group..    
+00006cd0: 2320 2020 2020 2222 220a 0a63 6c61 7373  #     """..class
+00006ce0: 205f 5f41 5049 5f50 6565 723a 0a20 2020   __API_Peer:.   
+00006cf0: 2064 6566 2067 6574 5f69 6428 7365 6c66   def get_id(self
+00006d00: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+00006d10: 2020 2222 220a 2020 2020 2020 2020 6069    """.        `i
+00006d20: 6460 3a20 5468 6520 4944 206f 6620 7468  d`: The ID of th
+00006d30: 6520 7065 6572 2e0a 2020 2020 2020 2020  e peer..        
+00006d40: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00006d50: 6964 2873 656c 662c 2069 643a 2069 6e74  id(self, id: int
+00006d60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00006d70: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00006d80: 6964 603a 2054 6865 2049 4420 6f66 2074  id`: The ID of t
+00006d90: 6865 2070 6565 722e 0a20 2020 2020 2020  he peer..       
+00006da0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00006db0: 5f63 6f6e 7465 7874 2873 656c 6629 202d  _context(self) -
+00006dc0: 3e20 6279 7465 733a 0a20 2020 2020 2020  > bytes:.       
+00006dd0: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
+00006de0: 6e74 6578 7460 3a20 4966 2074 6865 7265  ntext`: If there
+00006df0: 2069 7320 636f 6e74 6578 7420 6173 736f   is context asso
+00006e00: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
+00006e10: 7065 6572 2028 6c69 6b65 2063 6f6e 6e65  peer (like conne
+00006e20: 6374 696f 6e20 696e 666f 726d 6174 696f  ction informatio
+00006e30: 6e29 2c20 6974 2063 616e 2062 650a 2020  n), it can be.  
+00006e40: 2020 2020 2020 7365 7269 616c 697a 6564        serialized
+00006e50: 2061 6e64 2073 746f 7265 6420 6865 7265   and stored here
+00006e60: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00006e70: 2020 6465 6620 7365 745f 636f 6e74 6578    def set_contex
+00006e80: 7428 7365 6c66 2c20 636f 6e74 6578 743a  t(self, context:
+00006e90: 2062 7974 6573 2920 2d3e 204e 6f6e 653a   bytes) -> None:
+00006ea0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006eb0: 2020 2020 2060 636f 6e74 6578 7460 3a20       `context`: 
+00006ec0: 4966 2074 6865 7265 2069 7320 636f 6e74  If there is cont
+00006ed0: 6578 7420 6173 736f 6369 6174 6564 2077  ext associated w
+00006ee0: 6974 6820 7468 6520 7065 6572 2028 6c69  ith the peer (li
+00006ef0: 6b65 2063 6f6e 6e65 6374 696f 6e20 696e  ke connection in
+00006f00: 666f 726d 6174 696f 6e29 2c20 6974 2063  formation), it c
+00006f10: 616e 2062 650a 2020 2020 2020 2020 7365  an be.        se
+00006f20: 7269 616c 697a 6564 2061 6e64 2073 746f  rialized and sto
+00006f30: 7265 6420 6865 7265 2e0a 2020 2020 2020  red here..      
+00006f40: 2020 2222 220a 0a63 6c61 7373 2050 6565    """..class Pee
+00006f50: 7228 5f5f 4150 495f 5065 6572 293a 0a20  r(__API_Peer):. 
+00006f60: 2020 2022 2222 0a20 2020 2052 6570 7265     """.    Repre
+00006f70: 7365 6e74 7320 6120 5065 6572 206e 6f64  sents a Peer nod
+00006f80: 6520 696e 2074 6865 2063 6c75 7374 6572  e in the cluster
+00006f90: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00006fa0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00006fb0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+00006fc0: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+00006fd0: 7365 6c66 2920 2d3e 2022 5065 6572 5265  self) -> "PeerRe
+00006fe0: 6622 3a20 2e2e 2e0a 0a63 6c61 7373 2050  f": .....class P
+00006ff0: 6565 7252 6566 285f 5f41 5049 5f50 6565  eerRef(__API_Pee
+00007000: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
+00007010: 5265 6665 7265 6e63 6520 7479 7065 206f  Reference type o
+00007020: 6620 3a63 6c61 7373 3a60 5065 6572 602e  f :class:`Peer`.
+00007030: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+00007040: 5f5f 4150 495f 4c69 6768 7452 6561 6479  __API_LightReady
+00007050: 3a0a 2020 2020 6465 6620 636f 6d6d 6974  :.    def commit
+00007060: 5f69 6e64 6578 2873 656c 6629 202d 3e20  _index(self) -> 
+00007070: 4f70 7469 6f6e 616c 5b69 6e74 5d3a 0a20  Optional[int]:. 
+00007080: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007090: 2020 2054 6865 2063 7572 7265 6e74 2063     The current c
+000070a0: 6f6d 6d69 7420 696e 6465 782e 0a20 2020  ommit index..   
+000070b0: 2020 2020 2049 7420 7769 6c6c 2062 6520       It will be 
+000070c0: 4e6f 6e65 2073 7461 7465 2069 6620 7468  None state if th
+000070d0: 6572 6520 6973 206e 6f20 7570 6461 7465  ere is no update
+000070e0: 2e0a 2020 2020 2020 2020 4974 2069 7320  ..        It is 
+000070f0: 6e6f 7420 7265 7175 6972 6564 2074 6f20  not required to 
+00007100: 7361 7665 2069 7420 746f 2073 7461 626c  save it to stabl
+00007110: 6520 7374 6f72 6167 652e 0a20 2020 2020  e storage..     
+00007120: 2020 2022 2222 0a20 2020 2064 6566 2063     """.    def c
+00007130: 6f6d 6d69 7474 6564 5f65 6e74 7269 6573  ommitted_entries
+00007140: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
+00007150: 456e 7472 7952 6566 225d 3a0a 2020 2020  EntryRef"]:.    
+00007160: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007170: 436f 6d6d 6974 7465 6445 6e74 7269 6573  CommittedEntries
+00007180: 2073 7065 6369 6669 6573 2065 6e74 7269   specifies entri
+00007190: 6573 2074 6f20 6265 2063 6f6d 6d69 7474  es to be committ
+000071a0: 6564 2074 6f20 610a 2020 2020 2020 2020  ed to a.        
+000071b0: 7374 6f72 652f 7374 6174 652d 6d61 6368  store/state-mach
+000071c0: 696e 652e 2054 6865 7365 2068 6176 6520  ine. These have 
+000071d0: 7072 6576 696f 7573 6c79 2062 6565 6e20  previously been 
+000071e0: 636f 6d6d 6974 7465 6420 746f 2073 7461  committed to sta
+000071f0: 626c 650a 2020 2020 2020 2020 7374 6f72  ble.        stor
+00007200: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00007210: 2020 2064 6566 2074 616b 655f 636f 6d6d     def take_comm
+00007220: 6974 7465 645f 656e 7472 6965 7328 7365  itted_entries(se
+00007230: 6c66 2920 2d3e 204c 6973 745b 2245 6e74  lf) -> List["Ent
+00007240: 7279 225d 3a0a 2020 2020 2020 2020 2222  ry"]:.        ""
+00007250: 220a 2020 2020 2020 2020 5461 6b65 2074  ".        Take t
+00007260: 6865 2043 6f6d 6d69 7445 6e74 7269 6573  he CommitEntries
+00007270: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00007280: 2020 6465 6620 6d65 7373 6167 6573 2873    def messages(s
+00007290: 656c 6629 202d 3e20 4c69 7374 5b22 4d65  elf) -> List["Me
+000072a0: 7373 6167 6552 6566 225d 3a0a 2020 2020  ssageRef"]:.    
+000072b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000072c0: 4d65 7373 6167 6573 2073 7065 6369 6669  Messages specifi
+000072d0: 6573 206f 7574 626f 756e 6420 6d65 7373  es outbound mess
+000072e0: 6167 6573 2074 6f20 6265 2073 656e 742e  ages to be sent.
+000072f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007300: 2064 6566 2074 616b 655f 6d65 7373 6167   def take_messag
+00007310: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
+00007320: 5b22 4d65 7373 6167 6522 5d3a 0a20 2020  ["Message"]:.   
+00007330: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007340: 2054 616b 6520 7468 6520 4d65 7373 6167   Take the Messag
+00007350: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00007360: 0a63 6c61 7373 204c 6967 6874 5265 6164  .class LightRead
+00007370: 7928 5f5f 4150 495f 4c69 6768 7452 6561  y(__API_LightRea
+00007380: 6479 293a 0a20 2020 2022 2222 0a20 2020  dy):.    """.   
+00007390: 204c 6967 6874 5265 6164 7920 656e 6361   LightReady enca
+000073a0: 7073 756c 6174 6573 2074 6865 2063 6f6d  psulates the com
+000073b0: 6d69 7420 696e 6465 782c 2063 6f6d 6d69  mit index, commi
+000073c0: 7474 6564 2065 6e74 7269 6573 2061 6e64  tted entries and
+000073d0: 0a20 2020 206d 6573 7361 6765 7320 7468  .    messages th
+000073e0: 6174 2061 7265 2072 6561 6479 2074 6f20  at are ready to 
+000073f0: 6265 2061 7070 6c69 6564 206f 7220 6265  be applied or be
+00007400: 2073 656e 7420 746f 206f 7468 6572 2070   sent to other p
+00007410: 6565 7273 2e0a 2020 2020 2222 220a 0a20  eers..    """.. 
+00007420: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00007430: 7365 6c66 2920 2d3e 204e 6f6e 653a 202e  self) -> None: .
+00007440: 2e2e 0a20 2020 2064 6566 206d 616b 655f  ...    def make_
+00007450: 7265 6628 7365 6c66 2920 2d3e 2022 4c69  ref(self) -> "Li
+00007460: 6768 7452 6561 6479 5265 6622 3a20 2e2e  ghtReadyRef": ..
+00007470: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00007480: 686f 640a 2020 2020 6465 6620 6465 6661  hod.    def defa
+00007490: 756c 7428 2920 2d3e 2022 4c69 6768 7452  ult() -> "LightR
+000074a0: 6561 6479 223a 202e 2e2e 0a0a 636c 6173  eady": .....clas
+000074b0: 7320 4c69 6768 7452 6561 6479 5265 6628  s LightReadyRef(
+000074c0: 5f5f 4150 495f 4c69 6768 7452 6561 6479  __API_LightReady
+000074d0: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
+000074e0: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
+000074f0: 203a 636c 6173 733a 604c 6967 6874 5265   :class:`LightRe
+00007500: 6164 7960 2e0a 2020 2020 2222 220a 0a63  ady`..    """..c
+00007510: 6c61 7373 205f 5f41 5049 5f53 6e61 7073  lass __API_Snaps
+00007520: 686f 744d 6574 6164 6174 6128 5f5f 436c  hotMetadata(__Cl
+00007530: 6f6e 6561 626c 652c 205f 5f45 6e63 6f64  oneable, __Encod
+00007540: 6572 2c20 5f5f 4465 636f 6465 7229 3a0a  er, __Decoder):.
+00007550: 2020 2020 6465 6620 636c 6f6e 6528 7365      def clone(se
+00007560: 6c66 2920 2d3e 2022 536e 6170 7368 6f74  lf) -> "Snapshot
+00007570: 4d65 7461 6461 7461 223a 202e 2e2e 0a20  Metadata": .... 
+00007580: 2020 2064 6566 2067 6574 5f69 6e64 6578     def get_index
+00007590: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+000075a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000075b0: 2020 2060 696e 6465 7860 3a20 5468 6520     `index`: The 
+000075c0: 6170 706c 6965 6420 696e 6465 782e 0a20  applied index.. 
+000075d0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+000075e0: 6566 2073 6574 5f69 6e64 6578 2873 656c  ef set_index(sel
+000075f0: 662c 2069 6e64 6578 3a20 696e 7429 202d  f, index: int) -
+00007600: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00007610: 2222 220a 2020 2020 2020 2020 6069 6e64  """.        `ind
+00007620: 6578 603a 2054 6865 2061 7070 6c69 6564  ex`: The applied
+00007630: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
+00007640: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
+00007650: 725f 696e 6465 7828 7365 6c66 2920 2d3e  r_index(self) ->
+00007660: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00007670: 2222 0a20 2020 2020 2020 2060 696e 6465  "".        `inde
+00007680: 7860 3a20 5468 6520 6170 706c 6965 6420  x`: The applied 
+00007690: 696e 6465 782e 0a20 2020 2020 2020 2022  index..        "
+000076a0: 2222 0a20 2020 2064 6566 2067 6574 5f74  "".    def get_t
+000076b0: 6572 6d28 7365 6c66 2920 2d3e 2069 6e74  erm(self) -> int
+000076c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000076d0: 2020 2020 2020 6074 6572 6d60 3a20 5468        `term`: Th
+000076e0: 6520 7465 726d 206f 6620 7468 6520 6170  e term of the ap
+000076f0: 706c 6965 6420 696e 6465 782e 0a20 2020  plied index..   
+00007700: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00007710: 2073 6574 5f74 6572 6d28 7365 6c66 2c20   set_term(self, 
+00007720: 7465 726d 3a20 696e 7429 202d 3e20 4e6f  term: int) -> No
+00007730: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00007740: 2020 2020 2020 2020 6074 6572 6d60 3a20          `term`: 
+00007750: 5468 6520 7465 726d 206f 6620 7468 6520  The term of the 
+00007760: 6170 706c 6965 6420 696e 6465 782e 0a20  applied index.. 
+00007770: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00007780: 6566 2063 6c65 6172 5f74 6572 6d28 7365  ef clear_term(se
+00007790: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+000077a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000077b0: 2060 7465 726d 603a 2054 6865 2074 6572   `term`: The ter
+000077c0: 6d20 6f66 2074 6865 2061 7070 6c69 6564  m of the applied
+000077d0: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
+000077e0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+000077f0: 636f 6e66 5f73 7461 7465 2873 656c 6629  conf_state(self)
+00007800: 202d 3e20 2243 6f6e 6653 7461 7465 5265   -> "ConfStateRe
+00007810: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
+00007820: 2020 2020 2020 2020 6063 6f6e 665f 7374          `conf_st
+00007830: 6174 6560 3a20 5468 6520 6375 7272 656e  ate`: The curren
+00007840: 7420 6043 6f6e 6653 7461 7465 602e 0a20  t `ConfState`.. 
+00007850: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00007860: 6566 2073 6574 5f63 6f6e 665f 7374 6174  ef set_conf_stat
+00007870: 6528 7365 6c66 2c20 636f 6e66 5f73 7461  e(self, conf_sta
+00007880: 7465 3a20 2243 6f6e 6653 7461 7465 2220  te: "ConfState" 
+00007890: 7c20 2243 6f6e 6653 7461 7465 5265 6622  | "ConfStateRef"
+000078a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000078b0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+000078c0: 636f 6e66 5f73 7461 7465 603a 2054 6865  conf_state`: The
+000078d0: 2063 7572 7265 6e74 2060 436f 6e66 5374   current `ConfSt
+000078e0: 6174 6560 2e0a 2020 2020 2020 2020 2222  ate`..        ""
+000078f0: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
+00007900: 636f 6e66 5f73 7461 7465 2873 656c 6629  conf_state(self)
+00007910: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00007920: 2020 2222 220a 2020 2020 2020 2020 6063    """.        `c
+00007930: 6f6e 665f 7374 6174 6560 3a20 5468 6520  onf_state`: The 
+00007940: 6375 7272 656e 7420 6043 6f6e 6653 7461  current `ConfSta
+00007950: 7465 602e 0a20 2020 2020 2020 2022 2222  te`..        """
+00007960: 0a20 2020 2064 6566 2068 6173 5f63 6f6e  .    def has_con
+00007970: 665f 7374 6174 6528 7365 6c66 2920 2d3e  f_state(self) ->
+00007980: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00007990: 2222 0a20 2020 2020 2020 2060 636f 6e66  "".        `conf
+000079a0: 5f73 7461 7465 603a 2054 6865 2063 7572  _state`: The cur
+000079b0: 7265 6e74 2060 436f 6e66 5374 6174 6560  rent `ConfState`
+000079c0: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
+000079d0: 6c61 7373 2053 6e61 7073 686f 744d 6574  lass SnapshotMet
+000079e0: 6164 6174 6128 5f5f 4150 495f 536e 6170  adata(__API_Snap
+000079f0: 7368 6f74 4d65 7461 6461 7461 293a 0a20  shotMetadata):. 
+00007a00: 2020 2022 2222 2022 2222 0a0a 2020 2020     """ """..    
+00007a10: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00007a20: 6629 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  f) -> None: ....
+00007a30: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+00007a40: 640a 2020 2020 6465 6620 6465 6661 756c  d.    def defaul
+00007a50: 7428 2920 2d3e 2022 536e 6170 7368 6f74  t() -> "Snapshot
+00007a60: 4d65 7461 6461 7461 223a 202e 2e2e 0a20  Metadata": .... 
+00007a70: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00007a80: 0a20 2020 2064 6566 2064 6563 6f64 6528  .    def decode(
+00007a90: 763a 2062 7974 6573 2920 2d3e 2022 536e  v: bytes) -> "Sn
+00007aa0: 6170 7368 6f74 4d65 7461 6461 7461 223a  apshotMetadata":
+00007ab0: 202e 2e2e 0a20 2020 2064 6566 206d 616b   ....    def mak
+00007ac0: 655f 7265 6628 7365 6c66 2920 2d3e 2022  e_ref(self) -> "
+00007ad0: 536e 6170 7368 6f74 4d65 7461 6461 7461  SnapshotMetadata
+00007ae0: 5265 6622 3a20 2e2e 2e0a 0a63 6c61 7373  Ref": .....class
+00007af0: 2053 6e61 7073 686f 744d 6574 6164 6174   SnapshotMetadat
+00007b00: 6152 6566 285f 5f41 5049 5f53 6e61 7073  aRef(__API_Snaps
+00007b10: 686f 744d 6574 6164 6174 6129 3a0a 2020  hotMetadata):.  
+00007b20: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
+00007b30: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
+00007b40: 7373 3a60 536e 6170 7368 6f74 4d65 7461  ss:`SnapshotMeta
+00007b50: 6461 7461 602e 0a20 2020 2022 2222 0a0a  data`..    """..
+00007b60: 636c 6173 7320 5f5f 4150 495f 536e 6170  class __API_Snap
+00007b70: 7368 6f74 285f 5f43 6c6f 6e65 6162 6c65  shot(__Cloneable
+00007b80: 2c20 5f5f 456e 636f 6465 722c 205f 5f44  , __Encoder, __D
+00007b90: 6563 6f64 6572 293a 0a20 2020 2064 6566  ecoder):.    def
+00007ba0: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
+00007bb0: 2253 6e61 7073 686f 7422 3a20 2e2e 2e0a  "Snapshot": ....
+00007bc0: 2020 2020 6465 6620 6765 745f 6461 7461      def get_data
+00007bd0: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
+00007be0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00007bf0: 0a20 2020 2064 6566 2073 6574 5f64 6174  .    def set_dat
+00007c00: 6128 7365 6c66 2c20 6461 7461 3a20 6279  a(self, data: by
+00007c10: 7465 7329 202d 3e20 4e6f 6e65 3a0a 2020  tes) -> None:.  
+00007c20: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00007c30: 2020 6465 6620 636c 6561 725f 6461 7461    def clear_data
+00007c40: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00007c50: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00007c60: 2020 2020 6465 6620 6765 745f 6d65 7461      def get_meta
+00007c70: 6461 7461 2873 656c 6629 202d 3e20 2253  data(self) -> "S
+00007c80: 6e61 7073 686f 744d 6574 6164 6174 6152  napshotMetadataR
+00007c90: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
+00007ca0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00007cb0: 5f6d 6574 6164 6174 6128 0a20 2020 2020  _metadata(.     
+00007cc0: 2020 2073 656c 662c 206d 6574 615f 6461     self, meta_da
+00007cd0: 7461 3a20 2253 6e61 7073 686f 744d 6574  ta: "SnapshotMet
+00007ce0: 6164 6174 6122 207c 2022 536e 6170 7368  adata" | "Snapsh
+00007cf0: 6f74 4d65 7461 6461 7461 5265 6622 0a20  otMetadataRef". 
+00007d00: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+00007d10: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00007d20: 2020 6465 6620 636c 6561 725f 6d65 7461    def clear_meta
+00007d30: 6461 7461 2873 656c 6629 202d 3e20 4e6f  data(self) -> No
+00007d40: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+00007d50: 2222 220a 2020 2020 6465 6620 6861 735f  """.    def has_
+00007d60: 6d65 7461 6461 7461 2873 656c 6629 202d  metadata(self) -
+00007d70: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00007d80: 2222 2220 2222 220a 0a63 6c61 7373 2053  """ """..class S
+00007d90: 6e61 7073 686f 7428 5f5f 4150 495f 536e  napshot(__API_Sn
+00007da0: 6170 7368 6f74 293a 0a20 2020 2022 2222  apshot):.    """
+00007db0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00007dc0: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+00007dd0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 4073  None: ....    @s
+00007de0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00007df0: 6465 6620 6465 6661 756c 7428 2920 2d3e  def default() ->
+00007e00: 2022 536e 6170 7368 6f74 223a 202e 2e2e   "Snapshot": ...
+00007e10: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00007e20: 6f64 0a20 2020 2064 6566 2064 6563 6f64  od.    def decod
+00007e30: 6528 763a 2062 7974 6573 2920 2d3e 2022  e(v: bytes) -> "
+00007e40: 536e 6170 7368 6f74 223a 202e 2e2e 0a20  Snapshot": .... 
+00007e50: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+00007e60: 7365 6c66 2920 2d3e 2022 536e 6170 7368  self) -> "Snapsh
+00007e70: 6f74 5265 6622 3a20 2e2e 2e0a 0a63 6c61  otRef": .....cla
+00007e80: 7373 2053 6e61 7073 686f 7452 6566 285f  ss SnapshotRef(_
+00007e90: 5f41 5049 5f53 6e61 7073 686f 7429 3a0a  _API_Snapshot):.
+00007ea0: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
+00007eb0: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
+00007ec0: 6c61 7373 3a60 536e 6170 7368 6f74 602e  lass:`Snapshot`.
+00007ed0: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+00007ee0: 5f5f 4150 495f 4d65 7373 6167 6528 5f5f  __API_Message(__
+00007ef0: 436c 6f6e 6561 626c 652c 205f 5f45 6e63  Cloneable, __Enc
+00007f00: 6f64 6572 2c20 5f5f 4465 636f 6465 7229  oder, __Decoder)
+00007f10: 3a0a 2020 2020 6465 6620 636c 6f6e 6528  :.    def clone(
+00007f20: 7365 6c66 2920 2d3e 2022 4d65 7373 6167  self) -> "Messag
+00007f30: 6522 3a20 2e2e 2e0a 2020 2020 6465 6620  e": ....    def 
+00007f40: 6765 745f 636f 6d6d 6974 2873 656c 6629  get_commit(self)
+00007f50: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00007f60: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00007f70: 2073 6574 5f63 6f6d 6d69 7428 7365 6c66   set_commit(self
+00007f80: 2c20 636f 6d6d 6974 3a20 696e 7429 202d  , commit: int) -
+00007f90: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00007fa0: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00007fb0: 636c 6561 725f 636f 6d6d 6974 2873 656c  clear_commit(sel
+00007fc0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00007fd0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+00007fe0: 6465 6620 6765 745f 636f 6d6d 6974 5f74  def get_commit_t
+00007ff0: 6572 6d28 7365 6c66 2920 2d3e 2069 6e74  erm(self) -> int
+00008000: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+00008010: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
+00008020: 6d6d 6974 5f74 6572 6d28 7365 6c66 2c20  mmit_term(self, 
+00008030: 636f 6d6d 6974 5f74 6572 6d3a 2069 6e74  commit_term: int
+00008040: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00008050: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00008060: 6566 2063 6c65 6172 5f63 6f6d 6d69 745f  ef clear_commit_
+00008070: 7465 726d 2873 656c 6629 202d 3e20 4e6f  term(self) -> No
+00008080: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+00008090: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+000080a0: 6672 6f6d 2873 656c 6629 202d 3e20 696e  from(self) -> in
+000080b0: 743a 0a20 2020 2020 2020 2022 2222 2022  t:.        """ "
+000080c0: 2222 0a20 2020 2064 6566 2073 6574 5f66  "".    def set_f
+000080d0: 726f 6d28 7365 6c66 2c20 6672 6f6d 5f3a  rom(self, from_:
+000080e0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+000080f0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+00008100: 2020 2064 6566 2063 6c65 6172 5f66 726f     def clear_fro
+00008110: 6d28 7365 6c66 2920 2d3e 204e 6f6e 653a  m(self) -> None:
+00008120: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00008130: 0a20 2020 2064 6566 2067 6574 5f69 6e64  .    def get_ind
+00008140: 6578 2873 656c 6629 202d 3e20 696e 743a  ex(self) -> int:
+00008150: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00008160: 0a20 2020 2064 6566 2073 6574 5f69 6e64  .    def set_ind
+00008170: 6578 2873 656c 662c 2069 6e64 6578 3a20  ex(self, index: 
+00008180: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00008190: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+000081a0: 2020 6465 6620 636c 6561 725f 696e 6465    def clear_inde
+000081b0: 7828 7365 6c66 2920 2d3e 204e 6f6e 653a  x(self) -> None:
+000081c0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+000081d0: 0a20 2020 2064 6566 2067 6574 5f74 6572  .    def get_ter
+000081e0: 6d28 7365 6c66 2920 2d3e 2069 6e74 3a0a  m(self) -> int:.
+000081f0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00008200: 2020 2020 6465 6620 7365 745f 7465 726d      def set_term
+00008210: 2873 656c 662c 2074 6572 6d3a 2069 6e74  (self, term: int
+00008220: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00008230: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00008240: 6566 2063 6c65 6172 5f74 6572 6d28 7365  ef clear_term(se
+00008250: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00008260: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00008270: 2064 6566 2067 6574 5f6c 6f67 5f74 6572   def get_log_ter
+00008280: 6d28 7365 6c66 2920 2d3e 2069 6e74 3a0a  m(self) -> int:.
+00008290: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000082a0: 2020 2020 606c 6f67 5465 726d 603a 206c      `logTerm`: l
+000082b0: 6f67 5465 726d 2069 7320 6765 6e65 7261  ogTerm is genera
+000082c0: 6c6c 7920 7573 6564 2066 6f72 2061 7070  lly used for app
+000082d0: 656e 6469 6e67 2052 6166 7420 6c6f 6773  ending Raft logs
+000082e0: 2074 6f20 666f 6c6c 6f77 6572 732e 2046   to followers. F
+000082f0: 6f72 2065 7861 6d70 6c65 2c0a 2020 2020  or example,.    
+00008300: 2020 2020 2874 7970 653d 4d73 6741 7070      (type=MsgApp
+00008310: 656e 642c 696e 6465 783d 3130 302c 6c6f  end,index=100,lo
+00008320: 675f 7465 726d 3d35 2920 6d65 616e 7320  g_term=5) means 
+00008330: 6c65 6164 6572 2061 7070 656e 6473 2065  leader appends e
+00008340: 6e74 7269 6573 2073 7461 7274 696e 6720  ntries starting 
+00008350: 6174 0a20 2020 2020 2020 2069 6e64 6578  at.        index
+00008360: 3d31 3031 2c20 616e 6420 7468 6520 7465  =101, and the te
+00008370: 726d 206f 6620 656e 7472 7920 6174 2069  rm of entry at i
+00008380: 6e64 6578 2031 3030 2069 7320 352e 0a20  ndex 100 is 5.. 
+00008390: 2020 2020 2020 2028 7479 7065 3d4d 7367         (type=Msg
+000083a0: 4170 7065 6e64 5265 7370 6f6e 7365 2c72  AppendResponse,r
+000083b0: 656a 6563 743d 7472 7565 2c69 6e64 6578  eject=true,index
+000083c0: 3d31 3030 2c6c 6f67 5f74 6572 6d3d 3529  =100,log_term=5)
+000083d0: 206d 6561 6e73 2066 6f6c 6c6f 7765 7220   means follower 
+000083e0: 7265 6a65 6374 7320 736f 6d65 0a20 2020  rejects some.   
+000083f0: 2020 2020 2065 6e74 7269 6573 2066 726f       entries fro
+00008400: 6d20 6974 7320 6c65 6164 6572 2061 7320  m its leader as 
+00008410: 6974 2061 6c72 6561 6479 2068 6173 2061  it already has a
+00008420: 6e20 656e 7472 7920 7769 7468 2074 6572  n entry with ter
+00008430: 6d20 3520 6174 2069 6e64 6578 2031 3030  m 5 at index 100
+00008440: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00008450: 2020 6465 6620 7365 745f 6c6f 675f 7465    def set_log_te
+00008460: 726d 2873 656c 662c 206c 6f67 5f69 6e64  rm(self, log_ind
+00008470: 6578 3a20 696e 7429 202d 3e20 4e6f 6e65  ex: int) -> None
+00008480: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00008490: 2020 2020 2020 606c 6f67 5465 726d 603a        `logTerm`:
+000084a0: 206c 6f67 5465 726d 2069 7320 6765 6e65   logTerm is gene
+000084b0: 7261 6c6c 7920 7573 6564 2066 6f72 2061  rally used for a
+000084c0: 7070 656e 6469 6e67 2052 6166 7420 6c6f  ppending Raft lo
+000084d0: 6773 2074 6f20 666f 6c6c 6f77 6572 732e  gs to followers.
+000084e0: 2046 6f72 2065 7861 6d70 6c65 2c0a 2020   For example,.  
+000084f0: 2020 2020 2020 2874 7970 653d 4d73 6741        (type=MsgA
+00008500: 7070 656e 642c 696e 6465 783d 3130 302c  ppend,index=100,
+00008510: 6c6f 675f 7465 726d 3d35 2920 6d65 616e  log_term=5) mean
+00008520: 7320 6c65 6164 6572 2061 7070 656e 6473  s leader appends
+00008530: 2065 6e74 7269 6573 2073 7461 7274 696e   entries startin
+00008540: 6720 6174 0a20 2020 2020 2020 2069 6e64  g at.        ind
+00008550: 6578 3d31 3031 2c20 616e 6420 7468 6520  ex=101, and the 
+00008560: 7465 726d 206f 6620 656e 7472 7920 6174  term of entry at
+00008570: 2069 6e64 6578 2031 3030 2069 7320 352e   index 100 is 5.
+00008580: 0a20 2020 2020 2020 2028 7479 7065 3d4d  .        (type=M
+00008590: 7367 4170 7065 6e64 5265 7370 6f6e 7365  sgAppendResponse
+000085a0: 2c72 656a 6563 743d 7472 7565 2c69 6e64  ,reject=true,ind
+000085b0: 6578 3d31 3030 2c6c 6f67 5f74 6572 6d3d  ex=100,log_term=
+000085c0: 3529 206d 6561 6e73 2066 6f6c 6c6f 7765  5) means followe
+000085d0: 7220 7265 6a65 6374 7320 736f 6d65 0a20  r rejects some. 
+000085e0: 2020 2020 2020 2065 6e74 7269 6573 2066         entries f
+000085f0: 726f 6d20 6974 7320 6c65 6164 6572 2061  rom its leader a
+00008600: 7320 6974 2061 6c72 6561 6479 2068 6173  s it already has
+00008610: 2061 6e20 656e 7472 7920 7769 7468 2074   an entry with t
+00008620: 6572 6d20 3520 6174 2069 6e64 6578 2031  erm 5 at index 1
+00008630: 3030 2e0a 2020 2020 2020 2020 2222 220a  00..        """.
+00008640: 2020 2020 6465 6620 636c 6561 725f 6c6f      def clear_lo
+00008650: 675f 7465 726d 2873 656c 6629 202d 3e20  g_term(self) -> 
+00008660: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00008670: 220a 2020 2020 2020 2020 606c 6f67 5465  ".        `logTe
+00008680: 726d 603a 206c 6f67 5465 726d 2069 7320  rm`: logTerm is 
+00008690: 6765 6e65 7261 6c6c 7920 7573 6564 2066  generally used f
+000086a0: 6f72 2061 7070 656e 6469 6e67 2052 6166  or appending Raf
+000086b0: 7420 6c6f 6773 2074 6f20 666f 6c6c 6f77  t logs to follow
+000086c0: 6572 732e 2046 6f72 2065 7861 6d70 6c65  ers. For example
+000086d0: 2c0a 2020 2020 2020 2020 2874 7970 653d  ,.        (type=
+000086e0: 4d73 6741 7070 656e 642c 696e 6465 783d  MsgAppend,index=
+000086f0: 3130 302c 6c6f 675f 7465 726d 3d35 2920  100,log_term=5) 
+00008700: 6d65 616e 7320 6c65 6164 6572 2061 7070  means leader app
+00008710: 656e 6473 2065 6e74 7269 6573 2073 7461  ends entries sta
+00008720: 7274 696e 6720 6174 0a20 2020 2020 2020  rting at.       
+00008730: 2069 6e64 6578 3d31 3031 2c20 616e 6420   index=101, and 
+00008740: 7468 6520 7465 726d 206f 6620 656e 7472  the term of entr
+00008750: 7920 6174 2069 6e64 6578 2031 3030 2069  y at index 100 i
+00008760: 7320 352e 0a20 2020 2020 2020 2028 7479  s 5..        (ty
+00008770: 7065 3d4d 7367 4170 7065 6e64 5265 7370  pe=MsgAppendResp
+00008780: 6f6e 7365 2c72 656a 6563 743d 7472 7565  onse,reject=true
+00008790: 2c69 6e64 6578 3d31 3030 2c6c 6f67 5f74  ,index=100,log_t
+000087a0: 6572 6d3d 3529 206d 6561 6e73 2066 6f6c  erm=5) means fol
+000087b0: 6c6f 7765 7220 7265 6a65 6374 7320 736f  lower rejects so
+000087c0: 6d65 0a20 2020 2020 2020 2065 6e74 7269  me.        entri
+000087d0: 6573 2066 726f 6d20 6974 7320 6c65 6164  es from its lead
+000087e0: 6572 2061 7320 6974 2061 6c72 6561 6479  er as it already
+000087f0: 2068 6173 2061 6e20 656e 7472 7920 7769   has an entry wi
+00008800: 7468 2074 6572 6d20 3520 6174 2069 6e64  th term 5 at ind
+00008810: 6578 2031 3030 2e0a 2020 2020 2020 2020  ex 100..        
+00008820: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00008830: 7072 696f 7269 7479 2873 656c 6629 202d  priority(self) -
+00008840: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00008850: 2222 0a20 2020 2020 2020 2060 7072 696f  "".        `prio
+00008860: 7269 7479 603a 2049 6620 7468 6973 206e  rity`: If this n
+00008870: 6577 2066 6965 6c64 2069 7320 6e6f 7420  ew field is not 
+00008880: 7365 742c 2074 6865 6e20 7573 6520 7468  set, then use th
+00008890: 6520 6162 6f76 6520 6f6c 6420 6669 656c  e above old fiel
+000088a0: 643b 206f 7468 6572 7769 7365 0a20 2020  d; otherwise.   
+000088b0: 2020 2020 2075 7365 2074 6865 206e 6577       use the new
+000088c0: 2066 6965 6c64 2e20 5768 656e 2062 726f   field. When bro
+000088d0: 6164 6361 7374 696e 6720 7265 7175 6573  adcasting reques
+000088e0: 7420 766f 7465 2c20 626f 7468 2066 6965  t vote, both fie
+000088f0: 6c64 7320 6172 650a 2020 2020 2020 2020  lds are.        
+00008900: 7365 7420 6966 2074 6865 2070 7269 6f72  set if the prior
+00008910: 6974 7920 6973 206c 6172 6765 7220 7468  ity is larger th
+00008920: 616e 2030 2e20 5468 6973 2063 6861 6e67  an 0. This chang
+00008930: 6520 6973 206e 6f74 2061 2066 756c 6c79  e is not a fully
+00008940: 0a20 2020 2020 2020 2063 6f6d 7061 7469  .        compati
+00008950: 626c 6520 6368 616e 6765 2c20 6275 7420  ble change, but 
+00008960: 6974 206d 616b 6573 206d 696e 696d 616c  it makes minimal
+00008970: 2069 6d70 6163 7420 7468 6174 206f 6e6c   impact that onl
+00008980: 7920 6e65 7720 7072 696f 7269 7479 0a20  y new priority. 
+00008990: 2020 2020 2020 2069 7320 6e6f 7420 7265         is not re
+000089a0: 636f 676e 697a 6564 2062 7920 7468 6520  cognized by the 
+000089b0: 6f6c 6420 6e6f 6465 7320 6475 7269 6e67  old nodes during
+000089c0: 2072 6f6c 6c69 6e67 2075 7064 6174 652e   rolling update.
+000089d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000089e0: 2064 6566 2073 6574 5f70 7269 6f72 6974   def set_priorit
+000089f0: 7928 7365 6c66 2c20 7072 696f 7269 7479  y(self, priority
+00008a00: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00008a10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008a20: 2020 2020 6070 7269 6f72 6974 7960 3a20      `priority`: 
+00008a30: 4966 2074 6869 7320 6e65 7720 6669 656c  If this new fiel
+00008a40: 6420 6973 206e 6f74 2073 6574 2c20 7468  d is not set, th
+00008a50: 656e 2075 7365 2074 6865 2061 626f 7665  en use the above
+00008a60: 206f 6c64 2066 6965 6c64 3b20 6f74 6865   old field; othe
+00008a70: 7277 6973 650a 2020 2020 2020 2020 7573  rwise.        us
+00008a80: 6520 7468 6520 6e65 7720 6669 656c 642e  e the new field.
+00008a90: 2057 6865 6e20 6272 6f61 6463 6173 7469   When broadcasti
+00008aa0: 6e67 2072 6571 7565 7374 2076 6f74 652c  ng request vote,
+00008ab0: 2062 6f74 6820 6669 656c 6473 2061 7265   both fields are
+00008ac0: 0a20 2020 2020 2020 2073 6574 2069 6620  .        set if 
+00008ad0: 7468 6520 7072 696f 7269 7479 2069 7320  the priority is 
+00008ae0: 6c61 7267 6572 2074 6861 6e20 302e 2054  larger than 0. T
+00008af0: 6869 7320 6368 616e 6765 2069 7320 6e6f  his change is no
+00008b00: 7420 6120 6675 6c6c 790a 2020 2020 2020  t a fully.      
+00008b10: 2020 636f 6d70 6174 6962 6c65 2063 6861    compatible cha
+00008b20: 6e67 652c 2062 7574 2069 7420 6d61 6b65  nge, but it make
+00008b30: 7320 6d69 6e69 6d61 6c20 696d 7061 6374  s minimal impact
+00008b40: 2074 6861 7420 6f6e 6c79 206e 6577 2070   that only new p
+00008b50: 7269 6f72 6974 790a 2020 2020 2020 2020  riority.        
+00008b60: 6973 206e 6f74 2072 6563 6f67 6e69 7a65  is not recognize
+00008b70: 6420 6279 2074 6865 206f 6c64 206e 6f64  d by the old nod
+00008b80: 6573 2064 7572 696e 6720 726f 6c6c 696e  es during rollin
+00008b90: 6720 7570 6461 7465 2e0a 2020 2020 2020  g update..      
+00008ba0: 2020 2222 220a 2020 2020 6465 6620 636c    """.    def cl
+00008bb0: 6561 725f 7072 696f 7269 7479 2873 656c  ear_priority(sel
+00008bc0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00008bd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008be0: 6070 7269 6f72 6974 7960 3a20 4966 2074  `priority`: If t
+00008bf0: 6869 7320 6e65 7720 6669 656c 6420 6973  his new field is
+00008c00: 206e 6f74 2073 6574 2c20 7468 656e 2075   not set, then u
+00008c10: 7365 2074 6865 2061 626f 7665 206f 6c64  se the above old
+00008c20: 2066 6965 6c64 3b20 6f74 6865 7277 6973   field; otherwis
+00008c30: 650a 2020 2020 2020 2020 7573 6520 7468  e.        use th
+00008c40: 6520 6e65 7720 6669 656c 642e 2057 6865  e new field. Whe
+00008c50: 6e20 6272 6f61 6463 6173 7469 6e67 2072  n broadcasting r
+00008c60: 6571 7565 7374 2076 6f74 652c 2062 6f74  equest vote, bot
+00008c70: 6820 6669 656c 6473 2061 7265 0a20 2020  h fields are.   
+00008c80: 2020 2020 2073 6574 2069 6620 7468 6520       set if the 
+00008c90: 7072 696f 7269 7479 2069 7320 6c61 7267  priority is larg
+00008ca0: 6572 2074 6861 6e20 302e 2054 6869 7320  er than 0. This 
+00008cb0: 6368 616e 6765 2069 7320 6e6f 7420 6120  change is not a 
+00008cc0: 6675 6c6c 790a 2020 2020 2020 2020 636f  fully.        co
+00008cd0: 6d70 6174 6962 6c65 2063 6861 6e67 652c  mpatible change,
+00008ce0: 2062 7574 2069 7420 6d61 6b65 7320 6d69   but it makes mi
+00008cf0: 6e69 6d61 6c20 696d 7061 6374 2074 6861  nimal impact tha
+00008d00: 7420 6f6e 6c79 206e 6577 2070 7269 6f72  t only new prior
+00008d10: 6974 790a 2020 2020 2020 2020 6973 206e  ity.        is n
+00008d20: 6f74 2072 6563 6f67 6e69 7a65 6420 6279  ot recognized by
+00008d30: 2074 6865 206f 6c64 206e 6f64 6573 2064   the old nodes d
+00008d40: 7572 696e 6720 726f 6c6c 696e 6720 7570  uring rolling up
+00008d50: 6461 7465 2e0a 2020 2020 2020 2020 2222  date..        ""
+00008d60: 220a 2020 2020 6465 6620 6765 745f 636f  ".    def get_co
+00008d70: 6e74 6578 7428 7365 6c66 2920 2d3e 2062  ntext(self) -> b
+00008d80: 7974 6573 3a0a 2020 2020 2020 2020 2222  ytes:.        ""
+00008d90: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+00008da0: 745f 636f 6e74 6578 7428 7365 6c66 2c20  t_context(self, 
+00008db0: 636f 6e74 6578 743a 2062 7974 6573 2920  context: bytes) 
+00008dc0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00008dd0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00008de0: 2063 6c65 6172 5f63 6f6e 7465 7874 2873   clear_context(s
+00008df0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00008e00: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00008e10: 2020 6465 6620 6765 745f 7265 6a65 6374    def get_reject
+00008e20: 5f68 696e 7428 7365 6c66 2920 2d3e 2069  _hint(self) -> i
+00008e30: 6e74 3a0a 2020 2020 2020 2020 2222 2220  nt:.        """ 
+00008e40: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00008e50: 7265 6a65 6374 5f68 696e 7428 7365 6c66  reject_hint(self
+00008e60: 2c20 7265 6a65 6374 5f68 696e 743a 2062  , reject_hint: b
+00008e70: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
+00008e80: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00008e90: 2020 6465 6620 636c 6561 725f 7265 6a65    def clear_reje
+00008ea0: 6374 5f68 696e 7428 7365 6c66 2920 2d3e  ct_hint(self) ->
+00008eb0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00008ec0: 2222 2022 2222 0a20 2020 2064 6566 2067  "" """.    def g
+00008ed0: 6574 5f65 6e74 7269 6573 2873 656c 6629  et_entries(self)
+00008ee0: 202d 3e20 4c69 7374 5b22 456e 7472 7952   -> List["EntryR
+00008ef0: 6566 225d 3a0a 2020 2020 2020 2020 2222  ef"]:.        ""
+00008f00: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+00008f10: 745f 656e 7472 6965 7328 7365 6c66 2c20  t_entries(self, 
+00008f20: 656e 7473 3a20 4c69 7374 5b22 456e 7472  ents: List["Entr
+00008f30: 7922 5d20 7c20 4c69 7374 5b22 456e 7472  y"] | List["Entr
+00008f40: 7952 6566 225d 2920 2d3e 204e 6f6e 653a  yRef"]) -> None:
+00008f50: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00008f60: 0a20 2020 2064 6566 2063 6c65 6172 5f65  .    def clear_e
+00008f70: 6e74 7269 6573 2873 656c 6629 202d 3e20  ntries(self) -> 
+00008f80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00008f90: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
+00008fa0: 745f 6d73 675f 7479 7065 2873 656c 6629  t_msg_type(self)
+00008fb0: 202d 3e20 224d 6573 7361 6765 5479 7065   -> "MessageType
+00008fc0: 223a 0a20 2020 2020 2020 2022 2222 2022  ":.        """ "
+00008fd0: 2222 0a20 2020 2064 6566 2073 6574 5f6d  "".    def set_m
+00008fe0: 7367 5f74 7970 6528 7365 6c66 2c20 7479  sg_type(self, ty
+00008ff0: 703a 2022 4d65 7373 6167 6554 7970 6522  p: "MessageType"
+00009000: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00009010: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00009020: 6566 2063 6c65 6172 5f6d 7367 5f74 7970  ef clear_msg_typ
+00009030: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00009040: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00009050: 0a20 2020 2064 6566 2067 6574 5f72 656a  .    def get_rej
+00009060: 6563 7428 7365 6c66 2920 2d3e 2062 6f6f  ect(self) -> boo
+00009070: 6c3a 0a20 2020 2020 2020 2022 2222 2022  l:.        """ "
+00009080: 2222 0a20 2020 2064 6566 2073 6574 5f72  "".    def set_r
+00009090: 656a 6563 7428 7365 6c66 2c20 7265 6a65  eject(self, reje
+000090a0: 6374 3a20 626f 6f6c 2920 2d3e 204e 6f6e  ct: bool) -> Non
+000090b0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+000090c0: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+000090d0: 5f72 656a 6563 7428 7365 6c66 2920 2d3e  _reject(self) ->
+000090e0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000090f0: 2222 2022 2222 0a20 2020 2064 6566 2067  "" """.    def g
+00009100: 6574 5f73 6e61 7073 686f 7428 7365 6c66  et_snapshot(self
+00009110: 2920 2d3e 2022 536e 6170 7368 6f74 5265  ) -> "SnapshotRe
+00009120: 6622 3a0a 2020 2020 2020 2020 2222 2220  f":.        """ 
+00009130: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00009140: 736e 6170 7368 6f74 2873 656c 662c 2073  snapshot(self, s
+00009150: 6e61 7073 686f 743a 2022 536e 6170 7368  napshot: "Snapsh
+00009160: 6f74 2220 7c20 2253 6e61 7073 686f 7452  ot" | "SnapshotR
+00009170: 6566 2229 202d 3e20 4e6f 6e65 3a0a 2020  ef") -> None:.  
+00009180: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00009190: 2020 6465 6620 636c 6561 725f 736e 6170    def clear_snap
+000091a0: 7368 6f74 2873 656c 6629 202d 3e20 4e6f  shot(self) -> No
+000091b0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+000091c0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+000091d0: 746f 2873 656c 6629 202d 3e20 696e 743a  to(self) -> int:
+000091e0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+000091f0: 0a20 2020 2064 6566 2073 6574 5f74 6f28  .    def set_to(
+00009200: 7365 6c66 2c20 746f 3a20 696e 7429 202d  self, to: int) -
+00009210: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00009220: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00009230: 636c 6561 725f 746f 2873 656c 6629 202d  clear_to(self) -
+00009240: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00009250: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00009260: 6765 745f 7265 7175 6573 745f 736e 6170  get_request_snap
+00009270: 7368 6f74 2873 656c 6629 202d 3e20 696e  shot(self) -> in
+00009280: 743a 0a20 2020 2020 2020 2022 2222 2022  t:.        """ "
+00009290: 2222 0a20 2020 2064 6566 2073 6574 5f72  "".    def set_r
+000092a0: 6571 7565 7374 5f73 6e61 7073 686f 7428  equest_snapshot(
+000092b0: 7365 6c66 2c20 7265 7175 6573 745f 736e  self, request_sn
+000092c0: 6170 7368 6f74 3a20 696e 7429 202d 3e20  apshot: int) -> 
+000092d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000092e0: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
+000092f0: 6561 725f 7265 7175 6573 745f 736e 6170  ear_request_snap
+00009300: 7368 6f74 2873 656c 6629 202d 3e20 4e6f  shot(self) -> No
+00009310: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+00009320: 2222 220a 2020 2020 6465 6620 6861 735f  """.    def has_
+00009330: 736e 6170 7368 6f74 2873 656c 6629 202d  snapshot(self) -
+00009340: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00009350: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00009360: 636f 6d70 7574 655f 7369 7a65 2873 656c  compute_size(sel
+00009370: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00009380: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00009390: 6f6d 7075 7465 2061 6e64 2063 6163 6865  ompute and cache
+000093a0: 2073 697a 6520 6f66 2074 6869 7320 6d65   size of this me
+000093b0: 7373 6167 6520 616e 6420 616c 6c20 6e65  ssage and all ne
+000093c0: 7374 6564 206d 6573 7361 6765 730a 2020  sted messages.  
+000093d0: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
+000093e0: 204d 6573 7361 6765 285f 5f41 5049 5f4d   Message(__API_M
+000093f0: 6573 7361 6765 293a 0a20 2020 2022 2222  essage):.    """
+00009400: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00009410: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+00009420: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+00009430: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+00009440: 202d 3e20 224d 6573 7361 6765 5265 6622   -> "MessageRef"
+00009450: 3a20 2e2e 2e0a 2020 2020 4073 7461 7469  : ....    @stati
+00009460: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00009470: 6465 6661 756c 7428 2920 2d3e 2022 4d65  default() -> "Me
+00009480: 7373 6167 6522 3a20 2e2e 2e0a 2020 2020  ssage": ....    
+00009490: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+000094a0: 2020 6465 6620 6465 636f 6465 2876 3a20    def decode(v: 
+000094b0: 6279 7465 7329 202d 3e20 224d 6573 7361  bytes) -> "Messa
+000094c0: 6765 223a 202e 2e2e 0a0a 636c 6173 7320  ge": .....class 
+000094d0: 4d65 7373 6167 6552 6566 284d 6573 7361  MessageRef(Messa
+000094e0: 6765 293a 0a20 2020 2022 2222 0a20 2020  ge):.    """.   
+000094f0: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+00009500: 6f66 203a 636c 6173 733a 604d 6573 7361  of :class:`Messa
+00009510: 6765 602e 0a20 2020 2022 2222 0a0a 636c  ge`..    """..cl
+00009520: 6173 7320 5f5f 4150 495f 4861 7264 5374  ass __API_HardSt
+00009530: 6174 6528 5f5f 436c 6f6e 6561 626c 652c  ate(__Cloneable,
+00009540: 205f 5f45 6e63 6f64 6572 2c20 5f5f 4465   __Encoder, __De
+00009550: 636f 6465 7229 3a0a 2020 2020 6465 6620  coder):.    def 
+00009560: 636c 6f6e 6528 7365 6c66 2920 2d3e 2022  clone(self) -> "
+00009570: 4861 7264 5374 6174 6522 3a20 2e2e 2e0a  HardState": ....
+00009580: 2020 2020 6465 6620 6765 745f 7465 726d      def get_term
+00009590: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+000095a0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+000095b0: 2020 2064 6566 2073 6574 5f74 6572 6d28     def set_term(
+000095c0: 7365 6c66 2c20 7465 726d 3a20 696e 7429  self, term: int)
+000095d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000095e0: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+000095f0: 6620 636c 6561 725f 7465 726d 2873 656c  f clear_term(sel
+00009600: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00009610: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+00009620: 6465 6620 6765 745f 766f 7465 2873 656c  def get_vote(sel
+00009630: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00009640: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00009650: 6566 2073 6574 5f76 6f74 6528 7365 6c66  ef set_vote(self
+00009660: 2c20 766f 7465 3a20 696e 7429 202d 3e20  , vote: int) -> 
+00009670: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00009680: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
+00009690: 6561 725f 766f 7465 2873 656c 6629 202d  ear_vote(self) -
+000096a0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000096b0: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+000096c0: 6765 745f 636f 6d6d 6974 2873 656c 6629  get_commit(self)
+000096d0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+000096e0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+000096f0: 2073 6574 5f63 6f6d 6d69 7428 7365 6c66   set_commit(self
+00009700: 2c20 636f 6d6d 6974 3a20 696e 7429 202d  , commit: int) -
+00009710: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00009720: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00009730: 636c 6561 725f 636f 6d6d 6974 2873 656c  clear_commit(sel
+00009740: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00009750: 2020 2020 2222 2220 2222 220a 0a63 6c61      """ """..cla
+00009760: 7373 2048 6172 6453 7461 7465 285f 5f41  ss HardState(__A
+00009770: 5049 5f48 6172 6453 7461 7465 293a 0a20  PI_HardState):. 
+00009780: 2020 2022 2222 2022 2222 0a0a 2020 2020     """ """..    
+00009790: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000097a0: 6629 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  f) -> None: ....
+000097b0: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
+000097c0: 2873 656c 6629 202d 3e20 2248 6172 6453  (self) -> "HardS
+000097d0: 7461 7465 5265 6622 3a20 2e2e 2e0a 2020  tateRef": ....  
+000097e0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+000097f0: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
+00009800: 2920 2d3e 2022 4861 7264 5374 6174 6522  ) -> "HardState"
+00009810: 3a20 2e2e 2e0a 2020 2020 4073 7461 7469  : ....    @stati
+00009820: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00009830: 6465 636f 6465 2876 3a20 6279 7465 7329  decode(v: bytes)
+00009840: 202d 3e20 2248 6172 6453 7461 7465 223a   -> "HardState":
+00009850: 202e 2e2e 0a0a 636c 6173 7320 4861 7264   .....class Hard
+00009860: 5374 6174 6552 6566 285f 5f41 5049 5f48  StateRef(__API_H
+00009870: 6172 6453 7461 7465 293a 0a20 2020 2022  ardState):.    "
+00009880: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+00009890: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+000098a0: 6048 6172 6453 7461 7465 602e 0a20 2020  `HardState`..   
+000098b0: 2022 2222 0a0a 636c 6173 7320 5f5f 4150   """..class __AP
+000098c0: 495f 4765 7445 6e74 7269 6573 436f 6e74  I_GetEntriesCont
+000098d0: 6578 743a 0a20 2020 2064 6566 2063 616e  ext:.    def can
+000098e0: 5f61 7379 6e63 2873 656c 6629 202d 3e20  _async(self) -> 
+000098f0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00009900: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
+00009910: 6966 2074 6865 2063 616c 6c65 7227 7320  if the caller's 
+00009920: 636f 6e74 6578 7420 7375 7070 6f72 7420  context support 
+00009930: 6665 7463 6869 6e67 2065 6e74 7269 6573  fetching entries
+00009940: 2061 7379 6e63 6872 6f6e 6f75 736c 792e   asynchronously.
+00009950: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+00009960: 6173 7320 4765 7445 6e74 7269 6573 436f  ass GetEntriesCo
+00009970: 6e74 6578 7428 5f5f 4150 495f 4765 7445  ntext(__API_GetE
+00009980: 6e74 7269 6573 436f 6e74 6578 7429 3a0a  ntriesContext):.
+00009990: 2020 2020 2222 220a 2020 2020 5265 636f      """.    Reco
+000099a0: 7264 7320 7468 6520 636f 6e74 6578 7420  rds the context 
+000099b0: 6f66 2074 6865 2063 616c 6c65 7220 7768  of the caller wh
+000099c0: 6f20 6361 6c6c 7320 656e 7472 6965 7328  o calls entries(
+000099d0: 2920 6f66 2053 746f 7261 6765 2074 7261  ) of Storage tra
+000099e0: 6974 2e0a 2020 2020 2222 220a 0a20 2020  it..    """..   
+000099f0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00009a00: 2020 2064 6566 2065 6d70 7479 2863 616e     def empty(can
+00009a10: 5f61 7379 6e63 3a20 626f 6f6c 2920 2d3e  _async: bool) ->
+00009a20: 2022 4765 7445 6e74 7269 6573 436f 6e74   "GetEntriesCont
+00009a30: 6578 7422 3a0a 2020 2020 2020 2020 2222  ext":.        ""
+00009a40: 220a 2020 2020 2020 2020 5573 6564 2066  ".        Used f
+00009a50: 6f72 2063 616c 6c65 7273 206f 7574 206f  or callers out o
+00009a60: 6620 7261 6674 2e20 4361 6c6c 6572 2063  f raft. Caller c
+00009a70: 616e 2063 7573 746f 6d69 7a65 2069 6620  an customize if 
+00009a80: 6974 2073 7570 706f 7274 7320 6173 796e  it supports asyn
+00009a90: 632e 0a20 2020 2020 2020 2022 2222 0a20  c..        """. 
+00009aa0: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+00009ab0: 7365 6c66 2920 2d3e 2022 4765 7445 6e74  self) -> "GetEnt
+00009ac0: 7269 6573 436f 6e74 6578 7452 6566 223a  riesContextRef":
+00009ad0: 202e 2e2e 0a0a 636c 6173 7320 4765 7445   .....class GetE
+00009ae0: 6e74 7269 6573 436f 6e74 6578 7452 6566  ntriesContextRef
+00009af0: 285f 5f41 5049 5f47 6574 456e 7472 6965  (__API_GetEntrie
+00009b00: 7343 6f6e 7465 7874 293a 0a20 2020 2022  sContext):.    "
+00009b10: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+00009b20: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+00009b30: 6047 6574 456e 7472 6965 7343 6f6e 7465  `GetEntriesConte
+00009b40: 7874 602e 0a20 2020 2022 2222 0a0a 636c  xt`..    """..cl
+00009b50: 6173 7320 5f5f 4150 495f 456e 7472 7928  ass __API_Entry(
+00009b60: 5f5f 436c 6f6e 6561 626c 652c 205f 5f45  __Cloneable, __E
+00009b70: 6e63 6f64 6572 2c20 5f5f 4465 636f 6465  ncoder, __Decode
+00009b80: 7229 3a0a 2020 2020 6465 6620 636c 6f6e  r):.    def clon
+00009b90: 6528 7365 6c66 2920 2d3e 2022 456e 7472  e(self) -> "Entr
+00009ba0: 7922 3a20 2e2e 2e0a 2020 2020 6465 6620  y": ....    def 
+00009bb0: 6765 745f 636f 6e74 6578 7428 7365 6c66  get_context(self
+00009bc0: 2920 2d3e 2062 7974 6573 3a0a 2020 2020  ) -> bytes:.    
+00009bd0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+00009be0: 6465 6620 7365 745f 636f 6e74 6578 7428  def set_context(
+00009bf0: 7365 6c66 2c20 636f 6e74 6578 743a 2062  self, context: b
+00009c00: 7974 6573 2920 2d3e 204e 6f6e 653a 0a20  ytes) -> None:. 
+00009c10: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+00009c20: 2020 2064 6566 2063 6c65 6172 5f63 6f6e     def clear_con
+00009c30: 7465 7874 2873 656c 6629 202d 3e20 4e6f  text(self) -> No
+00009c40: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+00009c50: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00009c60: 6461 7461 2873 656c 6629 202d 3e20 6279  data(self) -> by
+00009c70: 7465 733a 0a20 2020 2020 2020 2022 2222  tes:.        """
+00009c80: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00009c90: 5f64 6174 6128 7365 6c66 2c20 6461 7461  _data(self, data
+00009ca0: 3a20 6279 7465 7329 202d 3e20 4e6f 6e65  : bytes) -> None
+00009cb0: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+00009cc0: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
+00009cd0: 6461 7461 2873 656c 6629 202d 3e20 4e6f  data(self) -> No
+00009ce0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+00009cf0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00009d00: 656e 7472 795f 7479 7065 2873 656c 6629  entry_type(self)
+00009d10: 202d 3e20 2245 6e74 7279 5479 7065 223a   -> "EntryType":
+00009d20: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00009d30: 0a20 2020 2064 6566 2073 6574 5f65 6e74  .    def set_ent
+00009d40: 7279 5f74 7970 6528 7365 6c66 2c20 7479  ry_type(self, ty
+00009d50: 703a 2022 456e 7472 7954 7970 6522 2920  p: "EntryType") 
+00009d60: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00009d70: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00009d80: 2063 6c65 6172 5f65 6e74 7279 5f74 7970   clear_entry_typ
+00009d90: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00009da0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00009db0: 0a20 2020 2064 6566 2067 6574 5f74 6572  .    def get_ter
+00009dc0: 6d28 7365 6c66 2920 2d3e 2069 6e74 3a0a  m(self) -> int:.
+00009dd0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00009de0: 2020 2020 6465 6620 7365 745f 7465 726d      def set_term
+00009df0: 2873 656c 662c 2074 6572 6d3a 2069 6e74  (self, term: int
+00009e00: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00009e10: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00009e20: 6566 2063 6c65 6172 5f74 6572 6d28 7365  ef clear_term(se
+00009e30: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00009e40: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009e50: 2064 6566 2067 6574 5f69 6e64 6578 2873   def get_index(s
+00009e60: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+00009e70: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009e80: 2064 6566 2073 6574 5f69 6e64 6578 2873   def set_index(s
+00009e90: 656c 662c 2069 6e64 6578 3a20 696e 7429  elf, index: int)
+00009ea0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00009eb0: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+00009ec0: 6620 636c 6561 725f 696e 6465 7828 7365  f clear_index(se
+00009ed0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00009ee0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009ef0: 2064 6566 2067 6574 5f73 796e 635f 6c6f   def get_sync_lo
+00009f00: 6728 7365 6c66 2920 2d3e 2062 6f6f 6c3a  g(self) -> bool:
+00009f10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009f20: 2020 2020 2044 6570 7265 6361 7465 6421       Deprecated!
+00009f30: 2049 7420 6973 206b 6570 7420 666f 7220   It is kept for 
+00009f40: 6261 636b 7761 7264 2063 6f6d 7061 7469  backward compati
+00009f50: 6269 6c69 7479 2e0a 2020 2020 2020 2020  bility..        
+00009f60: 544f 444f 3a20 7265 6d6f 7665 2069 7420  TODO: remove it 
+00009f70: 696e 2074 6865 206e 6578 7420 6d61 6a6f  in the next majo
+00009f80: 7220 7265 6c65 6173 652e 0a20 2020 2020  r release..     
+00009f90: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
+00009fa0: 6574 5f73 796e 635f 6c6f 6728 7365 6c66  et_sync_log(self
+00009fb0: 2c20 7379 6e63 5f6c 6f67 3a20 626f 6f6c  , sync_log: bool
+00009fc0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00009fd0: 2020 2022 2222 0a20 2020 2020 2020 2044     """.        D
+00009fe0: 6570 7265 6361 7465 6421 2049 7420 6973  eprecated! It is
+00009ff0: 206b 6570 7420 666f 7220 6261 636b 7761   kept for backwa
+0000a000: 7264 2063 6f6d 7061 7469 6269 6c69 7479  rd compatibility
+0000a010: 2e0a 2020 2020 2020 2020 544f 444f 3a20  ..        TODO: 
+0000a020: 7265 6d6f 7665 2069 7420 696e 2074 6865  remove it in the
+0000a030: 206e 6578 7420 6d61 6a6f 7220 7265 6c65   next major rele
+0000a040: 6173 652e 0a20 2020 2020 2020 2022 2222  ase..        """
+0000a050: 0a20 2020 2064 6566 2063 6c65 6172 5f73  .    def clear_s
+0000a060: 796e 635f 6c6f 6728 7365 6c66 2920 2d3e  ync_log(self) ->
+0000a070: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000a080: 2222 0a20 2020 2020 2020 2044 6570 7265  "".        Depre
+0000a090: 6361 7465 6421 2049 7420 6973 206b 6570  cated! It is kep
+0000a0a0: 7420 666f 7220 6261 636b 7761 7264 2063  t for backward c
+0000a0b0: 6f6d 7061 7469 6269 6c69 7479 2e0a 2020  ompatibility..  
+0000a0c0: 2020 2020 2020 544f 444f 3a20 7265 6d6f        TODO: remo
+0000a0d0: 7665 2069 7420 696e 2074 6865 206e 6578  ve it in the nex
+0000a0e0: 7420 6d61 6a6f 7220 7265 6c65 6173 652e  t major release.
+0000a0f0: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+0000a100: 6173 7320 456e 7472 7928 5f5f 4150 495f  ass Entry(__API_
+0000a110: 456e 7472 7929 3a0a 2020 2020 2222 220a  Entry):.    """.
+0000a120: 2020 2020 5468 6520 656e 7472 7920 6973      The entry is
+0000a130: 2061 2074 7970 6520 6f66 2063 6861 6e67   a type of chang
+0000a140: 6520 7468 6174 206e 6565 6473 2074 6f20  e that needs to 
+0000a150: 6265 2061 7070 6c69 6564 2e20 4974 2063  be applied. It c
+0000a160: 6f6e 7461 696e 7320 7477 6f20 6461 7461  ontains two data
+0000a170: 2066 6965 6c64 732e 0a20 2020 2057 6869   fields..    Whi
+0000a180: 6c65 2074 6865 2066 6965 6c64 7320 6172  le the fields ar
+0000a190: 6520 6275 696c 7420 696e 746f 2074 6865  e built into the
+0000a1a0: 206d 6f64 656c 3b20 7468 6569 7220 7573   model; their us
+0000a1b0: 6167 6520 6973 2064 6574 6572 6d69 6e65  age is determine
+0000a1c0: 6420 6279 2074 6865 2065 6e74 7279 5f74  d by the entry_t
+0000a1d0: 7970 652e 0a0a 2020 2020 466f 7220 6e6f  ype...    For no
+0000a1e0: 726d 616c 2065 6e74 7269 6573 2c20 7468  rmal entries, th
+0000a1f0: 6520 6461 7461 2066 6965 6c64 2073 686f  e data field sho
+0000a200: 756c 6420 636f 6e74 6169 6e20 7468 6520  uld contain the 
+0000a210: 6461 7461 2063 6861 6e67 6520 7468 6174  data change that
+0000a220: 2073 686f 756c 6420 6265 2061 7070 6c69   should be appli
+0000a230: 6564 2e0a 2020 2020 5468 6520 636f 6e74  ed..    The cont
+0000a240: 6578 7420 6669 656c 6420 6361 6e20 6265  ext field can be
+0000a250: 2075 7365 6420 666f 7220 616e 7920 636f   used for any co
+0000a260: 6e74 6578 7475 616c 2064 6174 6120 7468  ntextual data th
+0000a270: 6174 206d 6967 6874 2062 6520 7265 6c65  at might be rele
+0000a280: 7661 6e74 2074 6f20 7468 650a 2020 2020  vant to the.    
+0000a290: 6170 706c 6963 6174 696f 6e20 6f66 2074  application of t
+0000a2a0: 6865 2064 6174 612e 0a0a 2020 2020 466f  he data...    Fo
+0000a2b0: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
+0000a2c0: 6368 616e 6765 732c 2074 6865 2064 6174  changes, the dat
+0000a2d0: 6120 7769 6c6c 2063 6f6e 7461 696e 2074  a will contain t
+0000a2e0: 6865 2043 6f6e 6643 6861 6e67 6520 6d65  he ConfChange me
+0000a2f0: 7373 6167 6520 616e 6420 7468 650a 2020  ssage and the.  
+0000a300: 2020 636f 6e74 6578 7420 7769 6c6c 2070    context will p
+0000a310: 726f 7669 6465 2061 6e79 7468 696e 6720  rovide anything 
+0000a320: 6e65 6564 6564 2074 6f20 6173 7369 7374  needed to assist
+0000a330: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+0000a340: 6f6e 2063 6861 6e67 652e 2054 6865 2063  on change. The c
+0000a350: 6f6e 7465 7874 0a20 2020 2069 6620 666f  ontext.    if fo
+0000a360: 7220 7468 6520 7573 6572 2074 6f20 7365  r the user to se
+0000a370: 7420 616e 6420 7573 6520 696e 2074 6869  t and use in thi
+0000a380: 7320 6361 7365 2e0a 2020 2020 2222 220a  s case..    """.
+0000a390: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000a3a0: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
+0000a3b0: 202e 2e2e 0a20 2020 2064 6566 206d 616b   ....    def mak
+0000a3c0: 655f 7265 6628 7365 6c66 2920 2d3e 2022  e_ref(self) -> "
+0000a3d0: 456e 7472 7952 6566 223a 202e 2e2e 0a20  EntryRef": .... 
+0000a3e0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0000a3f0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
+0000a400: 2829 202d 3e20 2245 6e74 7279 223a 202e  () -> "Entry": .
+0000a410: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+0000a420: 7468 6f64 0a20 2020 2064 6566 2064 6563  thod.    def dec
+0000a430: 6f64 6528 763a 2062 7974 6573 2920 2d3e  ode(v: bytes) ->
+0000a440: 2022 456e 7472 7922 3a20 2e2e 2e0a 0a63   "Entry": .....c
+0000a450: 6c61 7373 2045 6e74 7279 5265 6628 5f5f  lass EntryRef(__
+0000a460: 4150 495f 456e 7472 7929 3a0a 2020 2020  API_Entry):.    
+0000a470: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
+0000a480: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
+0000a490: 3a60 456e 7472 7960 2e0a 2020 2020 2222  :`Entry`..    ""
+0000a4a0: 220a 0a63 6c61 7373 205f 5f41 5049 5f43  "..class __API_C
+0000a4b0: 6f6e 6653 7461 7465 285f 5f43 6c6f 6e65  onfState(__Clone
+0000a4c0: 6162 6c65 2c20 5f5f 456e 636f 6465 722c  able, __Encoder,
+0000a4d0: 205f 5f44 6563 6f64 6572 293a 0a20 2020   __Decoder):.   
+0000a4e0: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
+0000a4f0: 202d 3e20 2243 6f6e 6653 7461 7465 223a   -> "ConfState":
+0000a500: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+0000a510: 5f61 7574 6f5f 6c65 6176 6528 7365 6c66  _auto_leave(self
+0000a520: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0000a530: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000a540: 6566 2073 6574 5f61 7574 6f5f 6c65 6176  ef set_auto_leav
+0000a550: 6528 7365 6c66 2c20 6175 746f 5f6c 6561  e(self, auto_lea
+0000a560: 7665 3a20 626f 6f6c 2920 2d3e 204e 6f6e  ve: bool) -> Non
+0000a570: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+0000a580: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+0000a590: 5f61 7574 6f5f 6c65 6176 6528 7365 6c66  _auto_leave(self
+0000a5a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000a5b0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000a5c0: 6566 2067 6574 5f6c 6561 726e 6572 7328  ef get_learners(
+0000a5d0: 7365 6c66 2920 2d3e 204c 6973 745b 696e  self) -> List[in
+0000a5e0: 745d 3a0a 2020 2020 2020 2020 2222 2220  t]:.        """ 
+0000a5f0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0000a600: 6c65 6172 6e65 7273 2873 656c 662c 206c  learners(self, l
+0000a610: 6561 726e 6572 733a 204c 6973 745b 696e  earners: List[in
+0000a620: 745d 2920 2d3e 204e 6f6e 653a 0a20 2020  t]) -> None:.   
+0000a630: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+0000a640: 2064 6566 2063 6c65 6172 5f6c 6561 726e   def clear_learn
+0000a650: 6572 7328 7365 6c66 2920 2d3e 204e 6f6e  ers(self) -> Non
+0000a660: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+0000a670: 2222 0a20 2020 2064 6566 2067 6574 5f6c  "".    def get_l
+0000a680: 6561 726e 6572 735f 6e65 7874 2873 656c  earners_next(sel
+0000a690: 6629 202d 3e20 4c69 7374 5b69 6e74 5d3a  f) -> List[int]:
+0000a6a0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+0000a6b0: 0a20 2020 2064 6566 2073 6574 5f6c 6561  .    def set_lea
+0000a6c0: 726e 6572 735f 6e65 7874 2873 656c 662c  rners_next(self,
+0000a6d0: 206c 6561 726e 6572 735f 6e65 7874 3a20   learners_next: 
+0000a6e0: 4c69 7374 5b69 6e74 5d29 202d 3e20 4e6f  List[int]) -> No
+0000a6f0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+0000a700: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
+0000a710: 725f 6c65 6172 6e65 7273 5f6e 6578 7428  r_learners_next(
+0000a720: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000a730: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+0000a740: 2020 2064 6566 2067 6574 5f76 6f74 6572     def get_voter
+0000a750: 7328 7365 6c66 2920 2d3e 204c 6973 745b  s(self) -> List[
+0000a760: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
+0000a770: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+0000a780: 745f 766f 7465 7273 2873 656c 662c 2076  t_voters(self, v
+0000a790: 6f74 6572 733a 204c 6973 745b 696e 745d  oters: List[int]
+0000a7a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000a7b0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000a7c0: 6566 2063 6c65 6172 5f76 6f74 6572 7328  ef clear_voters(
+0000a7d0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000a7e0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+0000a7f0: 2020 2064 6566 2067 6574 5f76 6f74 6572     def get_voter
+0000a800: 735f 6f75 7467 6f69 6e67 2873 656c 6629  s_outgoing(self)
+0000a810: 202d 3e20 4c69 7374 5b69 6e74 5d3a 0a20   -> List[int]:. 
+0000a820: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+0000a830: 2020 2064 6566 2073 6574 5f76 6f74 6572     def set_voter
+0000a840: 735f 6f75 7467 6f69 6e67 2873 656c 662c  s_outgoing(self,
+0000a850: 2076 6f74 6572 735f 6f75 7467 6f69 6e67   voters_outgoing
+0000a860: 3a20 4c69 7374 5b69 6e74 5d29 202d 3e20  : List[int]) -> 
+0000a870: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000a880: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
+0000a890: 6561 725f 766f 7465 7273 5f6f 7574 676f  ear_voters_outgo
+0000a8a0: 696e 6728 7365 6c66 2920 2d3e 204e 6f6e  ing(self) -> Non
+0000a8b0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+0000a8c0: 2222 0a0a 636c 6173 7320 436f 6e66 5374  ""..class ConfSt
+0000a8d0: 6174 6528 5f5f 4150 495f 436f 6e66 5374  ate(__API_ConfSt
+0000a8e0: 6174 6529 3a0a 2020 2020 2222 2220 2222  ate):.    """ ""
+0000a8f0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+0000a900: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0000a910: 662c 2076 6f74 6572 733a 204f 7074 696f  f, voters: Optio
+0000a920: 6e61 6c5b 4c69 7374 5b69 6e74 5d5d 2c20  nal[List[int]], 
+0000a930: 6c65 6172 6e65 7273 3a20 4f70 7469 6f6e  learners: Option
+0000a940: 616c 5b4c 6973 745b 696e 745d 5d0a 2020  al[List[int]].  
+0000a950: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+0000a960: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
+0000a970: 6628 7365 6c66 2920 2d3e 2022 436f 6e66  f(self) -> "Conf
+0000a980: 5374 6174 6552 6566 223a 202e 2e2e 0a20  StateRef": .... 
+0000a990: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0000a9a0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
+0000a9b0: 2829 202d 3e20 2243 6f6e 6653 7461 7465  () -> "ConfState
+0000a9c0: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
+0000a9d0: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000a9e0: 2064 6563 6f64 6528 763a 2062 7974 6573   decode(v: bytes
+0000a9f0: 2920 2d3e 2022 436f 6e66 5374 6174 6522  ) -> "ConfState"
+0000aa00: 3a20 2e2e 2e0a 0a63 6c61 7373 2043 6f6e  : .....class Con
+0000aa10: 6653 7461 7465 5265 6628 5f5f 4150 495f  fStateRef(__API_
+0000aa20: 436f 6e66 5374 6174 6529 3a0a 2020 2020  ConfState):.    
+0000aa30: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
+0000aa40: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
+0000aa50: 3a60 436f 6e66 5374 6174 6560 2e0a 2020  :`ConfState`..  
+0000aa60: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
+0000aa70: 5049 5f43 6f6e 6643 6861 6e67 6556 3228  PI_ConfChangeV2(
+0000aa80: 5f5f 436c 6f6e 6561 626c 652c 205f 5f45  __Cloneable, __E
+0000aa90: 6e63 6f64 6572 2c20 5f5f 4465 636f 6465  ncoder, __Decode
+0000aaa0: 7229 3a0a 2020 2020 6465 6620 636c 6f6e  r):.    def clon
+0000aab0: 6528 7365 6c66 2920 2d3e 2022 436f 6e66  e(self) -> "Conf
+0000aac0: 4368 616e 6765 5632 223a 202e 2e2e 0a20  ChangeV2": .... 
+0000aad0: 2020 2064 6566 2067 6574 5f63 6861 6e67     def get_chang
+0000aae0: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
+0000aaf0: 5b22 436f 6e66 4368 616e 6765 5369 6e67  ["ConfChangeSing
+0000ab00: 6c65 5265 6622 5d3a 0a20 2020 2020 2020  leRef"]:.       
+0000ab10: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000ab20: 2073 6574 5f63 6861 6e67 6573 280a 2020   set_changes(.  
+0000ab30: 2020 2020 2020 7365 6c66 2c20 6368 616e        self, chan
+0000ab40: 6765 733a 204c 6973 745b 2243 6f6e 6643  ges: List["ConfC
+0000ab50: 6861 6e67 6553 696e 676c 6522 5d20 7c20  hangeSingle"] | 
+0000ab60: 4c69 7374 5b22 436f 6e66 4368 616e 6765  List["ConfChange
+0000ab70: 5369 6e67 6c65 5265 6622 5d0a 2020 2020  SingleRef"].    
+0000ab80: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000ab90: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000aba0: 6566 2063 6c65 6172 5f63 6861 6e67 6573  ef clear_changes
+0000abb0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000abc0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000abd0: 2020 2020 6465 6620 6765 745f 636f 6e74      def get_cont
+0000abe0: 6578 7428 7365 6c66 2920 2d3e 2062 7974  ext(self) -> byt
+0000abf0: 6573 3a0a 2020 2020 2020 2020 2222 2220  es:.        """ 
+0000ac00: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0000ac10: 636f 6e74 6578 7428 7365 6c66 2c20 636f  context(self, co
+0000ac20: 6e74 6578 743a 2062 7974 6573 2920 2d3e  ntext: bytes) ->
+0000ac30: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000ac40: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
+0000ac50: 6c65 6172 5f63 6f6e 7465 7874 2873 656c  lear_context(sel
+0000ac60: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000ac70: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+0000ac80: 6465 6620 6765 745f 7472 616e 7369 7469  def get_transiti
+0000ac90: 6f6e 2873 656c 6629 202d 3e20 2243 6f6e  on(self) -> "Con
+0000aca0: 6643 6861 6e67 6554 7261 6e73 6974 696f  fChangeTransitio
+0000acb0: 6e22 3a0a 2020 2020 2020 2020 2222 2220  n":.        """ 
+0000acc0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0000acd0: 7472 616e 7369 7469 6f6e 2873 656c 662c  transition(self,
+0000ace0: 2074 7261 6e73 6974 696f 6e3a 2022 436f   transition: "Co
+0000acf0: 6e66 4368 616e 6765 5472 616e 7369 7469  nfChangeTransiti
+0000ad00: 6f6e 2229 202d 3e20 4e6f 6e65 3a0a 2020  on") -> None:.  
+0000ad10: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+0000ad20: 2020 6465 6620 636c 6561 725f 7472 616e    def clear_tran
+0000ad30: 7369 7469 6f6e 2873 656c 6629 202d 3e20  sition(self) -> 
+0000ad40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000ad50: 2220 2222 220a 2020 2020 6465 6620 656e  " """.    def en
+0000ad60: 7465 725f 6a6f 696e 7428 7365 6c66 2920  ter_joint(self) 
+0000ad70: 2d3e 204f 7074 696f 6e61 6c5b 626f 6f6c  -> Optional[bool
+0000ad80: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000ad90: 2020 2020 2020 2043 6865 636b 7320 6966         Checks if
+0000ada0: 2075 7365 7320 4a6f 696e 7420 436f 6e73   uses Joint Cons
+0000adb0: 656e 7375 732e 0a0a 2020 2020 2020 2020  ensus...        
+0000adc0: 4974 2077 696c 6c20 7265 7475 726e 2053  It will return S
+0000add0: 6f6d 6520 6966 2061 6e64 206f 6e6c 7920  ome if and only 
+0000ade0: 6966 2074 6869 7320 636f 6e66 6967 2063  if this config c
+0000adf0: 6861 6e67 6520 7769 6c6c 2075 7365 204a  hange will use J
+0000ae00: 6f69 6e74 2043 6f6e 7365 6e73 7573 2c0a  oint Consensus,.
+0000ae10: 2020 2020 2020 2020 7768 6963 6820 6973          which is
+0000ae20: 2074 6865 2063 6173 6520 6966 2069 7420   the case if it 
+0000ae30: 636f 6e74 6169 6e73 206d 6f72 6520 7468  contains more th
+0000ae40: 616e 206f 6e65 2063 6861 6e67 6520 6f72  an one change or
+0000ae50: 2069 6620 7468 6520 7573 6520 6f66 204a   if the use of J
+0000ae60: 6f69 6e74 0a20 2020 2020 2020 2043 6f6e  oint.        Con
+0000ae70: 7365 6e73 7573 2077 6173 2072 6571 7565  sensus was reque
+0000ae80: 7374 6564 2065 7870 6c69 6369 746c 792e  sted explicitly.
+0000ae90: 2054 6865 2062 6f6f 6c20 696e 6469 6361   The bool indica
+0000aea0: 7465 7320 7768 6574 6865 7220 7468 6520  tes whether the 
+0000aeb0: 4a6f 696e 7420 5374 6174 650a 2020 2020  Joint State.    
+0000aec0: 2020 2020 7769 6c6c 2062 6520 6c65 6674      will be left
+0000aed0: 2061 7574 6f6d 6174 6963 616c 6c79 2e0a   automatically..
+0000aee0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000aef0: 6465 6620 6d65 7267 655f 6672 6f6d 5f62  def merge_from_b
+0000af00: 7974 6573 2873 656c 662c 2062 3a20 6279  ytes(self, b: by
+0000af10: 7465 7329 202d 3e20 4e6f 6e65 3a0a 2020  tes) -> None:.  
+0000af20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000af30: 2020 5570 6461 7465 2074 6869 7320 6d65    Update this me
+0000af40: 7373 6167 6520 6f62 6a65 6374 2077 6974  ssage object wit
+0000af50: 6820 6669 656c 6473 2072 6561 6420 6672  h fields read fr
+0000af60: 6f6d 2067 6976 656e 2073 7472 6561 6d2e  om given stream.
+0000af70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000af80: 2064 6566 206c 6561 7665 5f6a 6f69 6e74   def leave_joint
+0000af90: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+0000afa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000afb0: 2020 2020 4368 6563 6b73 2069 6620 7468      Checks if th
+0000afc0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+0000afd0: 6368 616e 6765 206c 6561 7665 7320 6120  change leaves a 
+0000afe0: 6a6f 696e 7420 636f 6e66 6967 7572 6174  joint configurat
+0000aff0: 696f 6e2e 0a0a 2020 2020 2020 2020 5468  ion...        Th
+0000b000: 6973 2069 7320 7468 6520 6361 7365 2069  is is the case i
+0000b010: 6620 7468 6520 436f 6e66 4368 616e 6765  f the ConfChange
+0000b020: 5632 2069 7320 7a65 726f 2c20 7769 7468  V2 is zero, with
+0000b030: 2074 6865 2070 6f73 7369 626c 6520 6578   the possible ex
+0000b040: 6365 7074 696f 6e20 6f66 0a20 2020 2020  ception of.     
+0000b050: 2020 2074 6865 2043 6f6e 7465 7874 2066     the Context f
+0000b060: 6965 6c64 2e0a 2020 2020 2020 2020 2222  ield..        ""
+0000b070: 220a 2020 2020 6465 6620 6173 5f76 3128  ".    def as_v1(
+0000b080: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
+0000b090: 6c5b 2243 6f6e 6643 6861 6e67 6552 6566  l["ConfChangeRef
+0000b0a0: 225d 3a0a 2020 2020 2020 2020 2222 220a  "]:.        """.
+0000b0b0: 2020 2020 2020 2020 436f 6e76 6572 7473          Converts
+0000b0c0: 2063 6f6e 6620 6368 616e 6765 2074 6f20   conf change to 
+0000b0d0: 6043 6f6e 6643 6861 6e67 6560 2e0a 0a20  `ConfChange`... 
+0000b0e0: 2020 2020 2020 2060 436f 6e66 4368 616e         `ConfChan
+0000b0f0: 6765 5632 6020 6361 6e27 7420 6265 2063  geV2` can't be c
+0000b100: 6861 6e67 6564 2062 6163 6b20 746f 2060  hanged back to `
+0000b110: 436f 6e66 4368 616e 6765 602e 0a20 2020  ConfChange`..   
+0000b120: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000b130: 2061 735f 7632 2873 656c 6629 202d 3e20   as_v2(self) -> 
+0000b140: 2243 6f6e 6643 6861 6e67 6556 3222 3a0a  "ConfChangeV2":.
+0000b150: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000b160: 2020 2020 4765 7473 2063 6f6e 6620 6368      Gets conf ch
+0000b170: 616e 6765 2061 7320 6043 6f6e 6643 6861  ange as `ConfCha
+0000b180: 6e67 6556 3260 2e0a 2020 2020 2020 2020  ngeV2`..        
+0000b190: 2222 220a 2020 2020 6465 6620 696e 746f  """.    def into
+0000b1a0: 5f76 3228 7365 6c66 2920 2d3e 2022 436f  _v2(self) -> "Co
+0000b1b0: 6e66 4368 616e 6765 5632 223a 0a20 2020  nfChangeV2":.   
+0000b1c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000b1d0: 2043 6f6e 7665 7274 7320 636f 6e66 2063   Converts conf c
+0000b1e0: 6861 6e67 6520 746f 2060 436f 6e66 4368  hange to `ConfCh
+0000b1f0: 616e 6765 5632 602e 0a20 2020 2020 2020  angeV2`..       
+0000b200: 2022 2222 0a0a 636c 6173 7320 436f 6e66   """..class Conf
+0000b210: 4368 616e 6765 5632 285f 5f41 5049 5f43  ChangeV2(__API_C
+0000b220: 6f6e 6643 6861 6e67 6556 3229 3a0a 2020  onfChangeV2):.  
+0000b230: 2020 2222 220a 2020 2020 436f 6e66 4368    """.    ConfCh
+0000b240: 616e 6765 5632 206d 6573 7361 6765 7320  angeV2 messages 
+0000b250: 696e 6974 6961 7465 2063 6f6e 6669 6775  initiate configu
+0000b260: 7261 7469 6f6e 2063 6861 6e67 6573 2e20  ration changes. 
+0000b270: 5468 6579 2073 7570 706f 7274 2062 6f74  They support bot
+0000b280: 6820 7468 650a 2020 2020 7369 6d70 6c65  h the.    simple
+0000b290: 2022 6f6e 6520 6174 2061 2074 696d 6522   "one at a time"
+0000b2a0: 206d 656d 6265 7273 6869 7020 6368 616e   membership chan
+0000b2b0: 6765 2070 726f 746f 636f 6c20 616e 6420  ge protocol and 
+0000b2c0: 6675 6c6c 204a 6f69 6e74 2043 6f6e 7365  full Joint Conse
+0000b2d0: 6e73 7573 0a20 2020 2061 6c6c 6f77 696e  nsus.    allowin
+0000b2e0: 6720 666f 7220 6172 6269 7472 6172 7920  g for arbitrary 
+0000b2f0: 6368 616e 6765 7320 696e 206d 656d 6265  changes in membe
+0000b300: 7273 6869 702e 0a0a 2020 2020 5468 6520  rship...    The 
+0000b310: 7375 7070 6c69 6564 2063 6f6e 7465 7874  supplied context
+0000b320: 2069 7320 7472 6561 7465 6420 6173 2061   is treated as a
+0000b330: 6e20 6f70 6171 7565 2070 6179 6c6f 6164  n opaque payload
+0000b340: 2061 6e64 2063 616e 2062 6520 7573 6564   and can be used
+0000b350: 2074 6f0a 2020 2020 6174 7461 6368 2061   to.    attach a
+0000b360: 6e20 6163 7469 6f6e 206f 6e20 7468 6520  n action on the 
+0000b370: 7374 6174 6520 6d61 6368 696e 6520 746f  state machine to
+0000b380: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+0000b390: 206f 6620 7468 6520 636f 6e66 6967 2063   of the config c
+0000b3a0: 6861 6e67 650a 2020 2020 7072 6f70 6f73  hange.    propos
+0000b3b0: 616c 2e20 4e6f 7465 2074 6861 7420 636f  al. Note that co
+0000b3c0: 6e74 7261 7279 2074 6f20 4a6f 696e 7420  ntrary to Joint 
+0000b3d0: 436f 6e73 656e 7375 7320 6173 206f 7574  Consensus as out
+0000b3e0: 6c69 6e65 6420 696e 2074 6865 2052 6166  lined in the Raf
+0000b3f0: 740a 2020 2020 7061 7065 725b 315d 2c20  t.    paper[1], 
+0000b400: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
+0000b410: 616e 6765 7320 6265 636f 6d65 2061 6374  anges become act
+0000b420: 6976 6520 7768 656e 2074 6865 7920 6172  ive when they ar
+0000b430: 6520 2a61 7070 6c69 6564 2a20 746f 2074  e *applied* to t
+0000b440: 6865 0a20 2020 2073 7461 7465 206d 6163  he.    state mac
+0000b450: 6869 6e65 2028 6e6f 7420 7768 656e 2074  hine (not when t
+0000b460: 6865 7920 6172 6520 6170 7065 6e64 6564  hey are appended
+0000b470: 2074 6f20 7468 6520 6c6f 6729 2e0a 0a20   to the log)... 
+0000b480: 2020 2054 6865 2073 696d 706c 6520 7072     The simple pr
+0000b490: 6f74 6f63 6f6c 2063 616e 2062 6520 7573  otocol can be us
+0000b4a0: 6564 2077 6865 6e65 7665 7220 6f6e 6c79  ed whenever only
+0000b4b0: 2061 2073 696e 676c 6520 6368 616e 6765   a single change
+0000b4c0: 2069 7320 6d61 6465 2e0a 0a20 2020 204e   is made...    N
+0000b4d0: 6f6e 2d73 696d 706c 6520 6368 616e 6765  on-simple change
+0000b4e0: 7320 7265 7175 6972 6520 7468 6520 7573  s require the us
+0000b4f0: 6520 6f66 204a 6f69 6e74 2043 6f6e 7365  e of Joint Conse
+0000b500: 6e73 7573 2c20 666f 7220 7768 6963 6820  nsus, for which 
+0000b510: 7477 6f0a 2020 2020 636f 6e66 6967 7572  two.    configur
+0000b520: 6174 696f 6e20 6368 616e 6765 7320 6172  ation changes ar
+0000b530: 6520 7275 6e2e 2054 6865 2066 6972 7374  e run. The first
+0000b540: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
+0000b550: 6861 6e67 6520 7370 6563 6966 6965 7320  hange specifies 
+0000b560: 7468 650a 2020 2020 6465 7369 7265 6420  the.    desired 
+0000b570: 6368 616e 6765 7320 616e 6420 7472 616e  changes and tran
+0000b580: 7369 7469 6f6e 7320 7468 6520 5261 6674  sitions the Raft
+0000b590: 2067 726f 7570 2069 6e74 6f20 7468 6520   group into the 
+0000b5a0: 6a6f 696e 7420 636f 6e66 6967 7572 6174  joint configurat
+0000b5b0: 696f 6e2c 0a20 2020 2069 6e20 7768 6963  ion,.    in whic
+0000b5c0: 6820 7175 6f72 756d 2072 6571 7569 7265  h quorum require
+0000b5d0: 7320 6120 6d61 6a6f 7269 7479 206f 6620  s a majority of 
+0000b5e0: 626f 7468 2074 6865 2070 7265 2d63 6861  both the pre-cha
+0000b5f0: 6e67 6573 2061 6e64 2070 6f73 742d 6368  nges and post-ch
+0000b600: 616e 6765 730a 2020 2020 636f 6e66 6967  anges.    config
+0000b610: 7572 6174 696f 6e2e 204a 6f69 6e74 2043  uration. Joint C
+0000b620: 6f6e 7365 6e73 7573 2061 766f 6964 7320  onsensus avoids 
+0000b630: 656e 7465 7269 6e67 2066 7261 6769 6c65  entering fragile
+0000b640: 2069 6e74 6572 6d65 6469 6174 650a 2020   intermediate.  
+0000b650: 2020 636f 6e66 6967 7572 6174 696f 6e73    configurations
+0000b660: 2074 6861 7420 636f 756c 6420 636f 6d70   that could comp
+0000b670: 726f 6d69 7365 2073 7572 7669 7661 6269  romise survivabi
+0000b680: 6c69 7479 2e20 466f 7220 6578 616d 706c  lity. For exampl
+0000b690: 652c 2077 6974 686f 7574 2074 6865 0a20  e, without the. 
+0000b6a0: 2020 2075 7365 206f 6620 4a6f 696e 7420     use of Joint 
+0000b6b0: 436f 6e73 656e 7375 7320 616e 6420 7275  Consensus and ru
+0000b6c0: 6e6e 696e 6720 6163 726f 7373 2074 6872  nning across thr
+0000b6d0: 6565 2061 7661 696c 6162 696c 6974 7920  ee availability 
+0000b6e0: 7a6f 6e65 7320 7769 7468 2061 0a20 2020  zones with a.   
+0000b6f0: 2072 6570 6c69 6361 7469 6f6e 2066 6163   replication fac
+0000b700: 746f 7220 6f66 2074 6872 6565 2c20 6974  tor of three, it
+0000b710: 2069 7320 6e6f 7420 706f 7373 6962 6c65   is not possible
+0000b720: 2074 6f20 7265 706c 6163 6520 6120 766f   to replace a vo
+0000b730: 7465 7220 7769 7468 6f75 740a 2020 2020  ter without.    
+0000b740: 656e 7465 7269 6e67 2061 6e20 696e 7465  entering an inte
+0000b750: 726d 6564 6961 7465 2063 6f6e 6669 6775  rmediate configu
+0000b760: 7261 7469 6f6e 2074 6861 7420 646f 6573  ration that does
+0000b770: 206e 6f74 2073 7572 7669 7665 2074 6865   not survive the
+0000b780: 206f 7574 6167 6520 6f66 0a20 2020 206f   outage of.    o
+0000b790: 6e65 2061 7661 696c 6162 696c 6974 7920  ne availability 
+0000b7a0: 7a6f 6e65 2e0a 0a20 2020 2054 6865 2070  zone...    The p
+0000b7b0: 726f 7669 6465 6420 436f 6e66 4368 616e  rovided ConfChan
+0000b7c0: 6765 5472 616e 7369 7469 6f6e 2073 7065  geTransition spe
+0000b7d0: 6369 6669 6573 2068 6f77 2028 616e 6420  cifies how (and 
+0000b7e0: 7768 6574 6865 7229 204a 6f69 6e74 2043  whether) Joint C
+0000b7f0: 6f6e 7365 6e73 7573 0a20 2020 2069 7320  onsensus.    is 
+0000b800: 7573 6564 2c20 616e 6420 6173 7369 676e  used, and assign
+0000b810: 7320 7468 6520 7461 736b 206f 6620 6c65  s the task of le
+0000b820: 6176 696e 6720 7468 6520 6a6f 696e 7420  aving the joint 
+0000b830: 636f 6e66 6967 7572 6174 696f 6e20 6569  configuration ei
+0000b840: 7468 6572 2074 6f0a 2020 2020 5261 6674  ther to.    Raft
+0000b850: 206f 7220 7468 6520 6170 706c 6963 6174   or the applicat
+0000b860: 696f 6e2e 204c 6561 7669 6e67 2074 6865  ion. Leaving the
+0000b870: 206a 6f69 6e74 2063 6f6e 6669 6775 7261   joint configura
+0000b880: 7469 6f6e 2069 7320 6163 636f 6d70 6c69  tion is accompli
+0000b890: 7368 6564 2062 790a 2020 2020 7072 6f70  shed by.    prop
+0000b8a0: 6f73 696e 6720 6120 436f 6e66 4368 616e  osing a ConfChan
+0000b8b0: 6765 5632 2077 6974 6820 6f6e 6c79 2061  geV2 with only a
+0000b8c0: 6e64 206f 7074 696f 6e61 6c6c 7920 7468  nd optionally th
+0000b8d0: 6520 436f 6e74 6578 7420 6669 656c 640a  e Context field.
+0000b8e0: 2020 2020 706f 7075 6c61 7465 642e 0a0a      populated...
+0000b8f0: 2020 2020 466f 7220 6465 7461 696c 7320      For details 
+0000b900: 6f6e 2052 6166 7420 6d65 6d62 6572 7368  on Raft membersh
+0000b910: 6970 2063 6861 6e67 6573 2c20 7365 653a  ip changes, see:
+0000b920: 0a0a 2020 2020 5b31 5d3a 2068 7474 7073  ..    [1]: https
+0000b930: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f6e  ://github.com/on
+0000b940: 6761 7264 6965 2f64 6973 7365 7274 6174  gardie/dissertat
+0000b950: 696f 6e2f 626c 6f62 2f6d 6173 7465 722f  ion/blob/master/
+0000b960: 6f6e 6c69 6e65 2d74 7269 6d2e 7064 660a  online-trim.pdf.
+0000b970: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+0000b980: 205f 5f69 6e69 745f 5f28 7365 6c66 2920   __init__(self) 
+0000b990: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+0000b9a0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+0000b9b0: 2020 2064 6566 2064 6566 6175 6c74 2829     def default()
+0000b9c0: 202d 3e20 2243 6f6e 6643 6861 6e67 6556   -> "ConfChangeV
+0000b9d0: 3222 3a20 2e2e 2e0a 2020 2020 6465 6620  2": ....    def 
+0000b9e0: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
+0000b9f0: 3e20 2243 6f6e 6643 6861 6e67 6556 3252  > "ConfChangeV2R
+0000ba00: 6566 223a 202e 2e2e 0a20 2020 2040 7374  ef": ....    @st
+0000ba10: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+0000ba20: 6566 2064 6563 6f64 6528 763a 2062 7974  ef decode(v: byt
+0000ba30: 6573 2920 2d3e 2022 436f 6e66 4368 616e  es) -> "ConfChan
+0000ba40: 6765 5632 223a 202e 2e2e 0a0a 636c 6173  geV2": .....clas
+0000ba50: 7320 436f 6e66 4368 616e 6765 5632 5265  s ConfChangeV2Re
+0000ba60: 6628 5f5f 4150 495f 436f 6e66 4368 616e  f(__API_ConfChan
+0000ba70: 6765 5632 293a 0a20 2020 2022 2222 0a20  geV2):.    """. 
+0000ba80: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
+0000ba90: 6520 6f66 203a 636c 6173 733a 6043 6f6e  e of :class:`Con
+0000baa0: 6643 6861 6e67 6556 3260 2e0a 2020 2020  fChangeV2`..    
+0000bab0: 2222 220a 0a63 6c61 7373 205f 5f41 5049  """..class __API
+0000bac0: 5f43 6f6e 6643 6861 6e67 6553 696e 676c  _ConfChangeSingl
+0000bad0: 6528 5f5f 436c 6f6e 6561 626c 652c 205f  e(__Cloneable, _
+0000bae0: 5f45 6e63 6f64 6572 2c20 5f5f 4465 636f  _Encoder, __Deco
+0000baf0: 6465 7229 3a0a 2020 2020 6465 6620 636c  der):.    def cl
+0000bb00: 6f6e 6528 7365 6c66 2920 2d3e 2022 436f  one(self) -> "Co
+0000bb10: 6e66 4368 616e 6765 5369 6e67 6c65 223a  nfChangeSingle":
+0000bb20: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+0000bb30: 5f6e 6f64 655f 6964 2873 656c 6629 202d  _node_id(self) -
+0000bb40: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+0000bb50: 2222 2022 2222 0a20 2020 2064 6566 2073  "" """.    def s
+0000bb60: 6574 5f6e 6f64 655f 6964 2873 656c 662c  et_node_id(self,
+0000bb70: 206e 6f64 655f 6964 3a20 696e 7429 3a0a   node_id: int):.
+0000bb80: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000bb90: 2020 2020 6465 6620 636c 6561 725f 6e6f      def clear_no
+0000bba0: 6465 5f69 6428 7365 6c66 2920 2d3e 204e  de_id(self) -> N
+0000bbb0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000bbc0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+0000bbd0: 5f63 6861 6e67 655f 7479 7065 2873 656c  _change_type(sel
+0000bbe0: 6629 202d 3e20 2243 6f6e 6643 6861 6e67  f) -> "ConfChang
+0000bbf0: 6554 7970 6522 3a0a 2020 2020 2020 2020  eType":.        
+0000bc00: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+0000bc10: 7365 745f 6368 616e 6765 5f74 7970 6528  set_change_type(
+0000bc20: 7365 6c66 2c20 7479 703a 2022 436f 6e66  self, typ: "Conf
+0000bc30: 4368 616e 6765 5479 7065 2229 202d 3e20  ChangeType") -> 
+0000bc40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000bc50: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
+0000bc60: 6561 725f 6368 616e 6765 5f74 7970 6528  ear_change_type(
+0000bc70: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000bc80: 2020 2020 2020 2022 2222 2022 2222 0a0a         """ """..
+0000bc90: 636c 6173 7320 436f 6e66 4368 616e 6765  class ConfChange
+0000bca0: 5369 6e67 6c65 285f 5f41 5049 5f43 6f6e  Single(__API_Con
+0000bcb0: 6643 6861 6e67 6553 696e 676c 6529 3a0a  fChangeSingle):.
+0000bcc0: 2020 2020 2222 220a 2020 2020 436f 6e66      """.    Conf
+0000bcd0: 4368 616e 6765 5369 6e67 6c65 2069 7320  ChangeSingle is 
+0000bce0: 616e 2069 6e64 6976 6964 7561 6c20 636f  an individual co
+0000bcf0: 6e66 6967 7572 6174 696f 6e20 6368 616e  nfiguration chan
+0000bd00: 6765 206f 7065 7261 7469 6f6e 2e20 4d75  ge operation. Mu
+0000bd10: 6c74 6970 6c65 0a20 2020 2073 7563 6820  ltiple.    such 
+0000bd20: 6f70 6572 6174 696f 6e73 2063 616e 2062  operations can b
+0000bd30: 6520 6361 7272 6965 6420 6f75 7420 6174  e carried out at
+0000bd40: 6f6d 6963 616c 6c79 2076 6961 2061 2043  omically via a C
+0000bd50: 6f6e 6643 6861 6e67 6556 322e 0a20 2020  onfChangeV2..   
+0000bd60: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+0000bd70: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+0000bd80: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000bd90: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+0000bda0: 202d 3e20 2243 6f6e 6643 6861 6e67 6553   -> "ConfChangeS
+0000bdb0: 696e 676c 6552 6566 223a 202e 2e2e 0a20  ingleRef": .... 
+0000bdc0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0000bdd0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
+0000bde0: 2829 202d 3e20 2243 6f6e 6643 6861 6e67  () -> "ConfChang
+0000bdf0: 6553 696e 676c 6522 3a20 2e2e 2e0a 2020  eSingle": ....  
+0000be00: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+0000be10: 2020 2020 6465 6620 6465 636f 6465 2876      def decode(v
+0000be20: 3a20 6279 7465 7329 202d 3e20 2243 6f6e  : bytes) -> "Con
+0000be30: 6643 6861 6e67 6553 696e 676c 6522 3a20  fChangeSingle": 
+0000be40: 2e2e 2e0a 0a63 6c61 7373 2043 6f6e 6643  .....class ConfC
+0000be50: 6861 6e67 6553 696e 676c 6552 6566 285f  hangeSingleRef(_
+0000be60: 5f41 5049 5f43 6f6e 6643 6861 6e67 6553  _API_ConfChangeS
+0000be70: 696e 676c 6529 3a0a 2020 2020 2222 220a  ingle):.    """.
+0000be80: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
+0000be90: 7065 206f 6620 3a63 6c61 7373 3a60 436f  pe of :class:`Co
+0000bea0: 6e66 4368 616e 6765 5369 6e67 6c65 602e  nfChangeSingle`.
+0000beb0: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+0000bec0: 5f5f 4150 495f 436f 6e66 4368 616e 6765  __API_ConfChange
+0000bed0: 285f 5f43 6c6f 6e65 6162 6c65 2c20 5f5f  (__Cloneable, __
+0000bee0: 456e 636f 6465 722c 205f 5f44 6563 6f64  Encoder, __Decod
+0000bef0: 6572 293a 0a20 2020 2064 6566 2063 6c6f  er):.    def clo
+0000bf00: 6e65 2873 656c 6629 202d 3e20 2243 6f6e  ne(self) -> "Con
+0000bf10: 6643 6861 6e67 6522 3a20 2e2e 2e0a 2020  fChange": ....  
+0000bf20: 2020 6465 6620 6765 745f 6964 2873 656c    def get_id(sel
+0000bf30: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+0000bf40: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000bf50: 6566 2073 6574 5f69 6428 7365 6c66 2c20  ef set_id(self, 
+0000bf60: 6964 3a20 696e 7429 202d 3e20 4e6f 6e65  id: int) -> None
+0000bf70: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+0000bf80: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
+0000bf90: 6964 2873 656c 6629 202d 3e20 4e6f 6e65  id(self) -> None
+0000bfa0: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+0000bfb0: 220a 2020 2020 6465 6620 6765 745f 6e6f  ".    def get_no
+0000bfc0: 6465 5f69 6428 7365 6c66 2920 2d3e 2069  de_id(self) -> i
+0000bfd0: 6e74 3a0a 2020 2020 2020 2020 2222 2220  nt:.        """ 
+0000bfe0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0000bff0: 6e6f 6465 5f69 6428 7365 6c66 2c20 6e6f  node_id(self, no
+0000c000: 6465 5f69 643a 2069 6e74 2920 2d3e 204e  de_id: int) -> N
+0000c010: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000c020: 2022 2222 0a20 2020 2064 6566 2063 6c65   """.    def cle
+0000c030: 6172 5f6e 6f64 655f 6964 2873 656c 6629  ar_node_id(self)
+0000c040: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000c050: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+0000c060: 6620 6765 745f 6368 616e 6765 5f74 7970  f get_change_typ
+0000c070: 6528 7365 6c66 2920 2d3e 2022 436f 6e66  e(self) -> "Conf
+0000c080: 4368 616e 6765 5479 7065 223a 0a20 2020  ChangeType":.   
+0000c090: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+0000c0a0: 2064 6566 2073 6574 5f63 6861 6e67 655f   def set_change_
+0000c0b0: 7479 7065 2873 656c 662c 2074 7970 3a20  type(self, typ: 
+0000c0c0: 2243 6f6e 6643 6861 6e67 6554 7970 6522  "ConfChangeType"
+0000c0d0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000c0e0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000c0f0: 6566 2063 6c65 6172 5f63 6861 6e67 655f  ef clear_change_
+0000c100: 7479 7065 2873 656c 6629 202d 3e20 4e6f  type(self) -> No
+0000c110: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+0000c120: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0000c130: 636f 6e74 6578 7428 7365 6c66 2920 2d3e  context(self) ->
+0000c140: 2062 7974 6573 3a0a 2020 2020 2020 2020   bytes:.        
+0000c150: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+0000c160: 7365 745f 636f 6e74 6578 7428 7365 6c66  set_context(self
+0000c170: 2c20 636f 6e74 6578 743a 2062 7974 6573  , context: bytes
+0000c180: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000c190: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000c1a0: 6566 2063 6c65 6172 5f63 6f6e 7465 7874  ef clear_context
+0000c1b0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000c1c0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000c1d0: 2020 2020 6465 6620 6d65 7267 655f 6672      def merge_fr
+0000c1e0: 6f6d 5f62 7974 6573 2873 656c 662c 2062  om_bytes(self, b
+0000c1f0: 3a20 6279 7465 7329 202d 3e20 4e6f 6e65  : bytes) -> None
+0000c200: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c210: 2020 2020 2020 5570 6461 7465 2074 6869        Update thi
+0000c220: 7320 6d65 7373 6167 6520 6f62 6a65 6374  s message object
+0000c230: 2077 6974 6820 6669 656c 6473 2072 6561   with fields rea
+0000c240: 6420 6672 6f6d 2067 6976 656e 2073 7472  d from given str
+0000c250: 6561 6d2e 0a20 2020 2020 2020 2022 2222  eam..        """
+0000c260: 0a20 2020 2064 6566 2061 735f 7631 2873  .    def as_v1(s
+0000c270: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000c280: 5b22 436f 6e66 4368 616e 6765 5265 6622  ["ConfChangeRef"
+0000c290: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000c2a0: 2020 2020 2020 2043 6f6e 7665 7274 7320         Converts 
+0000c2b0: 636f 6e66 2063 6861 6e67 6520 746f 2060  conf change to `
+0000c2c0: 436f 6e66 4368 616e 6765 602e 0a0a 2020  ConfChange`...  
+0000c2d0: 2020 2020 2020 6043 6f6e 6643 6861 6e67        `ConfChang
+0000c2e0: 6556 3260 2063 616e 2774 2062 6520 6368  eV2` can't be ch
+0000c2f0: 616e 6765 6420 6261 636b 2074 6f20 6043  anged back to `C
+0000c300: 6f6e 6643 6861 6e67 6560 2e0a 2020 2020  onfChange`..    
+0000c310: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000c320: 6173 5f76 3228 7365 6c66 2920 2d3e 2022  as_v2(self) -> "
+0000c330: 436f 6e66 4368 616e 6765 5632 223a 0a20  ConfChangeV2":. 
+0000c340: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c350: 2020 2047 6574 7320 636f 6e66 2063 6861     Gets conf cha
+0000c360: 6e67 6520 6173 2060 436f 6e66 4368 616e  nge as `ConfChan
+0000c370: 6765 5632 602e 0a20 2020 2020 2020 2022  geV2`..        "
+0000c380: 2222 0a20 2020 2064 6566 2069 6e74 6f5f  "".    def into_
+0000c390: 7632 2873 656c 6629 202d 3e20 2243 6f6e  v2(self) -> "Con
+0000c3a0: 6643 6861 6e67 6556 3222 3a0a 2020 2020  fChangeV2":.    
+0000c3b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c3c0: 436f 6e76 6572 7473 2063 6f6e 6620 6368  Converts conf ch
+0000c3d0: 616e 6765 2074 6f20 6043 6f6e 6643 6861  ange to `ConfCha
+0000c3e0: 6e67 6556 3260 2e0a 2020 2020 2020 2020  ngeV2`..        
+0000c3f0: 2222 220a 0a63 6c61 7373 2043 6f6e 6643  """..class ConfC
+0000c400: 6861 6e67 6528 5f5f 4150 495f 436f 6e66  hange(__API_Conf
+0000c410: 4368 616e 6765 293a 0a20 2020 2022 2222  Change):.    """
+0000c420: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+0000c430: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+0000c440: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000c450: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+0000c460: 202d 3e20 2243 6f6e 6643 6861 6e67 6552   -> "ConfChangeR
+0000c470: 6566 223a 202e 2e2e 0a20 2020 2040 7374  ef": ....    @st
+0000c480: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+0000c490: 6566 2064 6566 6175 6c74 2829 202d 3e20  ef default() -> 
+0000c4a0: 2243 6f6e 6643 6861 6e67 6522 3a20 2e2e  "ConfChange": ..
+0000c4b0: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0000c4c0: 686f 640a 2020 2020 6465 6620 6465 636f  hod.    def deco
+0000c4d0: 6465 2876 3a20 6279 7465 7329 202d 3e20  de(v: bytes) -> 
+0000c4e0: 2243 6f6e 6643 6861 6e67 6522 3a20 2e2e  "ConfChange": ..
+0000c4f0: 2e0a 0a63 6c61 7373 2043 6f6e 6643 6861  ...class ConfCha
+0000c500: 6e67 6552 6566 285f 5f41 5049 5f43 6f6e  ngeRef(__API_Con
+0000c510: 6643 6861 6e67 6529 3a0a 2020 2020 2222  fChange):.    ""
+0000c520: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
+0000c530: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
+0000c540: 436f 6e66 4368 616e 6765 602e 0a20 2020  ConfChange`..   
+0000c550: 2022 2222 0a0a 636c 6173 7320 5f5f 4150   """..class __AP
+0000c560: 495f 556e 7374 6162 6c65 3a0a 2020 2020  I_Unstable:.    
+0000c570: 6465 6620 6d61 7962 655f 6669 7273 745f  def maybe_first_
+0000c580: 696e 6465 7828 7365 6c66 2920 2d3e 204f  index(self) -> O
+0000c590: 7074 696f 6e61 6c5b 696e 745d 3a0a 2020  ptional[int]:.  
+0000c5a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c5b0: 2020 5265 7475 726e 7320 7468 6520 696e    Returns the in
+0000c5c0: 6465 7820 6f66 2074 6865 2066 6972 7374  dex of the first
+0000c5d0: 2070 6f73 7369 626c 6520 656e 7472 7920   possible entry 
+0000c5e0: 696e 2065 6e74 7269 6573 0a20 2020 2020  in entries.     
+0000c5f0: 2020 2069 6620 6974 2068 6173 2061 2073     if it has a s
+0000c600: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
+0000c610: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
+0000c620: 6265 5f6c 6173 745f 696e 6465 7828 7365  be_last_index(se
+0000c630: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0000c640: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
+0000c650: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+0000c660: 7320 7468 6520 6c61 7374 2069 6e64 6578  s the last index
+0000c670: 2069 6620 6974 2068 6173 2061 7420 6c65   if it has at le
+0000c680: 6173 7420 6f6e 6520 756e 7374 6162 6c65  ast one unstable
+0000c690: 2065 6e74 7279 206f 7220 736e 6170 7368   entry or snapsh
+0000c6a0: 6f74 2e0a 2020 2020 2020 2020 2222 220a  ot..        """.
+0000c6b0: 2020 2020 6465 6620 6d61 7962 655f 7465      def maybe_te
+0000c6c0: 726d 2873 656c 6629 202d 3e20 4f70 7469  rm(self) -> Opti
+0000c6d0: 6f6e 616c 5b69 6e74 5d3a 0a20 2020 2020  onal[int]:.     
+0000c6e0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+0000c6f0: 6574 7572 6e73 2074 6865 2074 6572 6d20  eturns the term 
+0000c700: 6f66 2074 6865 2065 6e74 7279 2061 7420  of the entry at 
+0000c710: 696e 6465 7820 6964 782c 2069 6620 7468  index idx, if th
+0000c720: 6572 6520 6973 2061 6e79 2e0a 2020 2020  ere is any..    
+0000c730: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000c740: 6d75 7374 5f63 6865 636b 5f6f 7574 6f66  must_check_outof
+0000c750: 626f 756e 6473 2873 656c 662c 206c 6f3a  bounds(self, lo:
+0000c760: 2069 6e74 2c20 6869 3a20 696e 7429 202d   int, hi: int) -
+0000c770: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000c780: 2222 220a 2020 2020 2020 2020 4173 7365  """.        Asse
+0000c790: 7274 7320 7468 6520 6068 6960 2061 6e64  rts the `hi` and
+0000c7a0: 2060 6c6f 6020 7661 6c75 6573 2061 6761   `lo` values aga
+0000c7b0: 696e 7374 2065 6163 6820 6f74 6865 7220  inst each other 
+0000c7c0: 616e 6420 6167 6169 6e73 7420 7468 650a  and against the.
+0000c7d0: 2020 2020 2020 2020 656e 7472 6965 7320          entries 
+0000c7e0: 7468 656d 7365 6c76 6573 2e0a 2020 2020  themselves..    
+0000c7f0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000c800: 736c 6963 6528 7365 6c66 2c20 6c6f 3a20  slice(self, lo: 
+0000c810: 696e 742c 2068 693a 2069 6e74 2920 2d3e  int, hi: int) ->
+0000c820: 204c 6973 745b 2245 6e74 7279 5265 6622   List["EntryRef"
+0000c830: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000c840: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
+0000c850: 2073 6c69 6365 206f 6620 656e 7472 6965   slice of entrie
+0000c860: 7320 6265 7477 6565 6e20 7468 6520 6869  s between the hi
+0000c870: 6768 2061 6e64 206c 6f77 2e0a 0a20 2020  gh and low...   
+0000c880: 2020 2020 2023 2050 616e 6963 730a 0a20       # Panics.. 
+0000c890: 2020 2020 2020 2050 616e 6963 7320 6966         Panics if
+0000c8a0: 2074 6865 2060 6c6f 6020 6f72 2060 6869   the `lo` or `hi
+0000c8b0: 6020 6172 6520 6f75 7420 6f66 2062 6f75  ` are out of bou
+0000c8c0: 6e64 732e 0a20 2020 2020 2020 2050 616e  nds..        Pan
+0000c8d0: 6963 7320 6966 2060 6c6f 203e 2068 6960  ics if `lo > hi`
+0000c8e0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000c8f0: 2020 6465 6620 7374 6162 6c65 5f73 6e61    def stable_sna
+0000c900: 7028 7365 6c66 2c20 696e 6465 783a 2069  p(self, index: i
+0000c910: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+0000c920: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c930: 2043 6c65 6172 7320 7468 6520 756e 7374   Clears the unst
+0000c940: 6162 6c65 2073 6e61 7073 686f 742e 0a20  able snapshot.. 
+0000c950: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000c960: 6566 2073 7461 626c 655f 656e 7472 6965  ef stable_entrie
+0000c970: 7328 7365 6c66 2c20 696e 6465 783a 2069  s(self, index: i
+0000c980: 6e74 2c20 7465 726d 3a20 696e 7429 202d  nt, term: int) -
+0000c990: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000c9a0: 2222 220a 2020 2020 2020 2020 436c 6561  """.        Clea
+0000c9b0: 7273 2074 6865 2075 6e73 7461 626c 6520  rs the unstable 
+0000c9c0: 656e 7472 6965 7320 616e 6420 6d6f 7665  entries and move
+0000c9d0: 7320 7468 6520 7374 6162 6c65 206f 6666  s the stable off
+0000c9e0: 7365 7420 7570 2074 6f20 7468 650a 2020  set up to the.  
+0000c9f0: 2020 2020 2020 6c61 7374 2069 6e64 6578        last index
+0000ca00: 2c20 6966 2074 6865 7265 2069 7320 616e  , if there is an
+0000ca10: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+0000ca20: 2020 2064 6566 2072 6573 746f 7265 2873     def restore(s
+0000ca30: 656c 662c 2073 6e61 703a 2022 536e 6170  elf, snap: "Snap
+0000ca40: 7368 6f74 5265 6622 2920 2d3e 204e 6f6e  shotRef") -> Non
+0000ca50: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0000ca60: 2020 2020 2020 2046 726f 6d20 6120 6769         From a gi
+0000ca70: 7665 6e20 736e 6170 7368 6f74 2c20 7265  ven snapshot, re
+0000ca80: 7374 6f72 6573 2074 6865 2073 6e61 7073  stores the snaps
+0000ca90: 686f 7420 746f 2073 656c 662c 2062 7574  hot to self, but
+0000caa0: 2064 6f65 736e 2774 2075 6e70 6163 6b2e   doesn't unpack.
+0000cab0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cac0: 2064 6566 2074 7275 6e63 6174 655f 616e   def truncate_an
+0000cad0: 645f 6170 7065 6e64 2873 656c 662c 2065  d_append(self, e
+0000cae0: 6e74 733a 204c 6973 745b 2245 6e74 7279  nts: List["Entry
+0000caf0: 225d 207c 204c 6973 745b 2245 6e74 7279  "] | List["Entry
+0000cb00: 5265 6622 5d29 202d 3e20 4e6f 6e65 3a0a  Ref"]) -> None:.
+0000cb10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000cb20: 2020 2020 4170 7065 6e64 2065 6e74 7269      Append entri
+0000cb30: 6573 2074 6f20 756e 7374 6162 6c65 2c20  es to unstable, 
+0000cb40: 7472 756e 6361 7465 206c 6f63 616c 2062  truncate local b
+0000cb50: 6c6f 636b 2066 6972 7374 2069 6620 6f76  lock first if ov
+0000cb60: 6572 6c61 7070 6564 2e0a 0a20 2020 2020  erlapped...     
+0000cb70: 2020 2023 2050 616e 6963 730a 0a20 2020     # Panics..   
+0000cb80: 2020 2020 2050 616e 6963 7320 6966 2074       Panics if t
+0000cb90: 7275 6e63 6174 6520 6c6f 6773 2074 6f20  runcate logs to 
+0000cba0: 7468 6520 656e 7472 7920 6265 666f 7265  the entry before
+0000cbb0: 2073 6e61 7073 686f 740a 2020 2020 2020   snapshot.      
+0000cbc0: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
+0000cbd0: 745f 656e 7472 6965 735f 7369 7a65 2873  t_entries_size(s
+0000cbe0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0000cbf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cc00: 2060 656e 7472 6965 735f 7369 7a65 603a   `entries_size`:
+0000cc10: 2054 6865 2073 697a 6520 6f66 2065 6e74   The size of ent
+0000cc20: 7269 6573 0a20 2020 2020 2020 2022 2222  ries.        """
+0000cc30: 0a20 2020 2064 6566 2073 6574 5f65 6e74  .    def set_ent
+0000cc40: 7269 6573 5f73 697a 6528 7365 6c66 2c20  ries_size(self, 
+0000cc50: 656e 7472 6965 735f 7369 7a65 3a20 696e  entries_size: in
+0000cc60: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+0000cc70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cc80: 6065 6e74 7269 6573 5f73 697a 6560 3a20  `entries_size`: 
+0000cc90: 5468 6520 7369 7a65 206f 6620 656e 7472  The size of entr
+0000cca0: 6965 730a 2020 2020 2020 2020 2222 220a  ies.        """.
+0000ccb0: 2020 2020 6465 6620 6765 745f 6f66 6673      def get_offs
+0000ccc0: 6574 2873 656c 6629 202d 3e20 696e 743a  et(self) -> int:
+0000ccd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cce0: 2020 2020 2060 6f66 6673 6574 603a 2054       `offset`: T
+0000ccf0: 6865 206f 6666 7365 7420 6672 6f6d 2074  he offset from t
+0000cd00: 6865 2076 6563 746f 7220 696e 6465 782e  he vector index.
+0000cd10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cd20: 2064 6566 2073 6574 5f6f 6666 7365 7428   def set_offset(
+0000cd30: 7365 6c66 2c20 6f66 6673 6574 3a20 696e  self, offset: in
+0000cd40: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+0000cd50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cd60: 606f 6666 7365 7460 3a20 5468 6520 6f66  `offset`: The of
+0000cd70: 6673 6574 2066 726f 6d20 7468 6520 7665  fset from the ve
+0000cd80: 6374 6f72 2069 6e64 6578 2e0a 2020 2020  ctor index..    
+0000cd90: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000cda0: 6765 745f 656e 7472 6965 7328 7365 6c66  get_entries(self
+0000cdb0: 2920 2d3e 204c 6973 745b 2245 6e74 7279  ) -> List["Entry
+0000cdc0: 5265 6622 5d3a 0a20 2020 2020 2020 2022  Ref"]:.        "
+0000cdd0: 2222 0a20 2020 2020 2020 2060 656e 7472  "".        `entr
+0000cde0: 6965 7360 3a20 416c 6c20 656e 7472 6965  ies`: All entrie
+0000cdf0: 7320 7468 6174 2068 6176 6520 6e6f 7420  s that have not 
+0000ce00: 7965 7420 6265 656e 2077 7269 7474 656e  yet been written
+0000ce10: 2074 6f20 7374 6f72 6167 652e 0a20 2020   to storage..   
+0000ce20: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000ce30: 2073 6574 5f65 6e74 7269 6573 2873 656c   set_entries(sel
+0000ce40: 662c 2065 6e74 733a 204c 6973 745b 2245  f, ents: List["E
+0000ce50: 6e74 7279 225d 207c 204c 6973 745b 2245  ntry"] | List["E
+0000ce60: 6e74 7279 5265 6622 5d29 202d 3e20 4e6f  ntryRef"]) -> No
+0000ce70: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+0000ce80: 2020 2020 2020 2020 6065 6e74 7269 6573          `entries
+0000ce90: 603a 2041 6c6c 2065 6e74 7269 6573 2074  `: All entries t
+0000cea0: 6861 7420 6861 7665 206e 6f74 2079 6574  hat have not yet
+0000ceb0: 2062 6565 6e20 7772 6974 7465 6e20 746f   been written to
+0000cec0: 2073 746f 7261 6765 2e0a 2020 2020 2020   storage..      
+0000ced0: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
+0000cee0: 745f 6c6f 6767 6572 2873 656c 6629 202d  t_logger(self) -
+0000cef0: 3e20 224c 6f67 6765 7252 6566 223a 0a20  > "LoggerRef":. 
+0000cf00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000cf10: 2020 2060 6c6f 6767 6572 603a 2054 6865     `logger`: The
+0000cf20: 2074 6167 2074 6f20 7573 6520 7768 656e   tag to use when
+0000cf30: 206c 6f67 6769 6e67 2e0a 2020 2020 2020   logging..      
+0000cf40: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+0000cf50: 745f 6c6f 6767 6572 2873 656c 662c 206c  t_logger(self, l
+0000cf60: 6f67 6765 723a 2022 4c6f 6767 6572 2220  ogger: "Logger" 
+0000cf70: 7c20 224c 6f67 6765 7252 6566 2220 7c20  | "LoggerRef" | 
+0000cf80: 2254 6872 6561 6453 6166 654c 6f67 6765  "ThreadSafeLogge
+0000cf90: 7222 2920 2d3e 204e 6f6e 653a 0a20 2020  r") -> None:.   
+0000cfa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cfb0: 2060 6c6f 6767 6572 603a 2054 6865 2074   `logger`: The t
+0000cfc0: 6167 2074 6f20 7573 6520 7768 656e 206c  ag to use when l
+0000cfd0: 6f67 6769 6e67 2e0a 2020 2020 2020 2020  ogging..        
+0000cfe0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0000cff0: 736e 6170 7368 6f74 2873 656c 6629 202d  snapshot(self) -
+0000d000: 3e20 4f70 7469 6f6e 616c 5b22 536e 6170  > Optional["Snap
+0000d010: 7368 6f74 5265 6622 5d3a 0a20 2020 2020  shotRef"]:.     
+0000d020: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+0000d030: 736e 6170 7368 6f74 603a 2054 6865 2069  snapshot`: The i
+0000d040: 6e63 6f6d 696e 6720 756e 7374 6162 6c65  ncoming unstable
+0000d050: 2073 6e61 7073 686f 742c 2069 6620 616e   snapshot, if an
+0000d060: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+0000d070: 2020 2064 6566 2073 6574 5f73 6e61 7073     def set_snaps
+0000d080: 686f 7428 7365 6c66 2c20 736e 6170 7368  hot(self, snapsh
+0000d090: 6f74 3a20 2253 6e61 7073 686f 7422 207c  ot: "Snapshot" |
+0000d0a0: 2022 536e 6170 7368 6f74 5265 6622 2920   "SnapshotRef") 
+0000d0b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000d0c0: 2022 2222 0a20 2020 2020 2020 2060 736e   """.        `sn
+0000d0d0: 6170 7368 6f74 603a 2054 6865 2069 6e63  apshot`: The inc
+0000d0e0: 6f6d 696e 6720 756e 7374 6162 6c65 2073  oming unstable s
+0000d0f0: 6e61 7073 686f 742c 2069 6620 616e 792e  napshot, if any.
+0000d100: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+0000d110: 6173 7320 556e 7374 6162 6c65 285f 5f41  ass Unstable(__A
+0000d120: 5049 5f55 6e73 7461 626c 6529 3a0a 2020  PI_Unstable):.  
+0000d130: 2020 2222 220a 2020 2020 5468 6520 6075    """.    The `u
+0000d140: 6e73 7461 626c 652e 656e 7472 6965 735b  nstable.entries[
+0000d150: 695d 6020 6861 7320 7261 6674 206c 6f67  i]` has raft log
+0000d160: 2070 6f73 6974 696f 6e20 6069 2b75 6e73   position `i+uns
+0000d170: 7461 626c 652e 6f66 6673 6574 602e 0a20  table.offset`.. 
+0000d180: 2020 204e 6f74 6520 7468 6174 2060 756e     Note that `un
+0000d190: 7374 6162 6c65 2e6f 6666 7365 7460 206d  stable.offset` m
+0000d1a0: 6179 2062 6520 6c65 7373 2074 6861 6e20  ay be less than 
+0000d1b0: 7468 6520 6869 6768 6573 7420 6c6f 670a  the highest log.
+0000d1c0: 2020 2020 706f 7369 7469 6f6e 2069 6e20      position in 
+0000d1d0: 7374 6f72 6167 653b 2074 6869 7320 6d65  storage; this me
+0000d1e0: 616e 7320 7468 6174 2074 6865 206e 6578  ans that the nex
+0000d1f0: 7420 7772 6974 6520 746f 2073 746f 7261  t write to stora
+0000d200: 6765 0a20 2020 206d 6967 6874 206e 6565  ge.    might nee
+0000d210: 6420 746f 2074 7275 6e63 6174 6520 7468  d to truncate th
+0000d220: 6520 6c6f 6720 6265 666f 7265 2070 6572  e log before per
+0000d230: 7369 7374 696e 6720 756e 7374 6162 6c65  sisting unstable
+0000d240: 2e65 6e74 7269 6573 2e0a 2020 2020 2222  .entries..    ""
+0000d250: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+0000d260: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0000d270: 662c 206f 6666 7365 743a 2069 6e74 2c20  f, offset: int, 
+0000d280: 6c6f 6767 6572 3a20 224c 6f67 6765 7222  logger: "Logger"
+0000d290: 207c 2022 4c6f 6767 6572 5265 6622 207c   | "LoggerRef" |
+0000d2a0: 2022 5468 7265 6164 5361 6665 4c6f 6767   "ThreadSafeLogg
+0000d2b0: 6572 220a 2020 2020 2920 2d3e 204e 6f6e  er".    ) -> Non
+0000d2c0: 653a 202e 2e2e 0a20 2020 2064 6566 206d  e: ....    def m
+0000d2d0: 616b 655f 7265 6628 7365 6c66 2920 2d3e  ake_ref(self) ->
+0000d2e0: 2022 556e 7374 6162 6c65 5265 6622 3a20   "UnstableRef": 
+0000d2f0: 2e2e 2e0a 0a63 6c61 7373 2055 6e73 7461  .....class Unsta
+0000d300: 626c 6552 6566 285f 5f41 5049 5f55 6e73  bleRef(__API_Uns
+0000d310: 7461 626c 6529 3a0a 2020 2020 2222 220a  table):.    """.
+0000d320: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
+0000d330: 7065 206f 6620 3a63 6c61 7373 3a60 556e  pe of :class:`Un
+0000d340: 7374 6162 6c65 602e 0a20 2020 2022 2222  stable`..    """
+0000d350: 0a0a 636c 6173 7320 5f5f 4150 495f 536f  ..class __API_So
+0000d360: 6674 5374 6174 653a 0a20 2020 2064 6566  ftState:.    def
+0000d370: 2067 6574 5f6c 6561 6465 725f 6964 2873   get_leader_id(s
+0000d380: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0000d390: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d3a0: 2060 6c65 6164 6572 5f69 6460 3a20 5468   `leader_id`: Th
+0000d3b0: 6520 706f 7465 6e74 6961 6c20 6c65 6164  e potential lead
+0000d3c0: 6572 206f 6620 7468 6520 636c 7573 7465  er of the cluste
+0000d3d0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+0000d3e0: 2020 2064 6566 2073 6574 5f6c 6561 6465     def set_leade
+0000d3f0: 725f 6964 2873 656c 662c 206c 6561 6465  r_id(self, leade
+0000d400: 725f 6964 3a20 696e 7429 202d 3e20 4e6f  r_id: int) -> No
+0000d410: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+0000d420: 2020 2020 2020 2020 606c 6561 6465 725f          `leader_
+0000d430: 6964 603a 2054 6865 2070 6f74 656e 7469  id`: The potenti
+0000d440: 616c 206c 6561 6465 7220 6f66 2074 6865  al leader of the
+0000d450: 2063 6c75 7374 6572 2e0a 2020 2020 2020   cluster..      
+0000d460: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
+0000d470: 745f 7261 6674 5f73 7461 7465 2873 656c  t_raft_state(sel
+0000d480: 6629 202d 3e20 2253 7461 7465 526f 6c65  f) -> "StateRole
+0000d490: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+0000d4a0: 2020 2020 2020 2060 7261 6674 5f73 7461         `raft_sta
+0000d4b0: 7465 603a 2054 6865 2073 6f66 7420 726f  te`: The soft ro
+0000d4c0: 6c65 2074 6869 7320 6e6f 6465 206d 6179  le this node may
+0000d4d0: 2074 616b 652e 0a20 2020 2020 2020 2022   take..        "
+0000d4e0: 2222 0a20 2020 2064 6566 2073 6574 5f72  "".    def set_r
+0000d4f0: 6166 745f 7374 6174 6528 7365 6c66 2c20  aft_state(self, 
+0000d500: 726f 6c65 3a20 2253 7461 7465 526f 6c65  role: "StateRole
+0000d510: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
+0000d520: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d530: 6072 6166 745f 7374 6174 6560 3a20 5468  `raft_state`: Th
+0000d540: 6520 736f 6674 2072 6f6c 6520 7468 6973  e soft role this
+0000d550: 206e 6f64 6520 6d61 7920 7461 6b65 2e0a   node may take..
+0000d560: 2020 2020 2020 2020 2222 220a 0a63 6c61          """..cla
+0000d570: 7373 2053 6f66 7453 7461 7465 285f 5f41  ss SoftState(__A
+0000d580: 5049 5f53 6f66 7453 7461 7465 293a 0a20  PI_SoftState):. 
+0000d590: 2020 2022 2222 0a20 2020 2053 6f66 7453     """.    SoftS
+0000d5a0: 7461 7465 2070 726f 7669 6465 7320 7374  tate provides st
+0000d5b0: 6174 6520 7468 6174 2069 7320 7573 6566  ate that is usef
+0000d5c0: 756c 2066 6f72 206c 6f67 6769 6e67 2061  ul for logging a
+0000d5d0: 6e64 2064 6562 7567 6769 6e67 2e0a 2020  nd debugging..  
+0000d5e0: 2020 5468 6520 7374 6174 6520 6973 2076    The state is v
+0000d5f0: 6f6c 6174 696c 6520 616e 6420 646f 6573  olatile and does
+0000d600: 206e 6f74 206e 6565 6420 746f 2062 6520   not need to be 
+0000d610: 7065 7273 6973 7465 6420 746f 2074 6865  persisted to the
+0000d620: 2057 414c 2e0a 2020 2020 2222 220a 0a20   WAL..    """.. 
+0000d630: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+0000d640: 7365 6c66 2920 2d3e 2022 536f 6674 5374  self) -> "SoftSt
+0000d650: 6174 6552 6566 223a 202e 2e2e 0a20 2020  ateRef": ....   
+0000d660: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+0000d670: 2020 2064 6566 2064 6566 6175 6c74 2829     def default()
+0000d680: 202d 3e20 2253 6f66 7453 7461 7465 223a   -> "SoftState":
+0000d690: 202e 2e2e 0a0a 636c 6173 7320 536f 6674   .....class Soft
+0000d6a0: 5374 6174 6552 6566 285f 5f41 5049 5f53  StateRef(__API_S
+0000d6b0: 6f66 7453 7461 7465 293a 0a20 2020 2022  oftState):.    "
+0000d6c0: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+0000d6d0: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+0000d6e0: 6053 6f66 7453 7461 7465 602e 0a20 2020  `SoftState`..   
+0000d6f0: 2022 2222 0a0a 636c 6173 7320 5f5f 4150   """..class __AP
+0000d700: 495f 5265 6164 5374 6174 6528 5f5f 436c  I_ReadState(__Cl
+0000d710: 6f6e 6561 626c 6529 3a0a 2020 2020 6465  oneable):.    de
+0000d720: 6620 636c 6f6e 6528 7365 6c66 2920 2d3e  f clone(self) ->
+0000d730: 2022 5265 6164 5374 6174 6522 3a20 2e2e   "ReadState": ..
+0000d740: 2e0a 2020 2020 6465 6620 6765 745f 696e  ..    def get_in
+0000d750: 6465 7828 7365 6c66 2920 2d3e 2069 6e74  dex(self) -> int
+0000d760: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000d770: 2020 2020 2020 6069 6e64 6578 603a 2054        `index`: T
+0000d780: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+0000d790: 7265 6164 2073 7461 7465 2e0a 2020 2020  read state..    
+0000d7a0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000d7b0: 7365 745f 696e 6465 7828 7365 6c66 2c20  set_index(self, 
+0000d7c0: 6964 783a 2069 6e74 2920 2d3e 204e 6f6e  idx: int) -> Non
+0000d7d0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0000d7e0: 2020 2020 2020 2060 696e 6465 7860 3a20         `index`: 
+0000d7f0: 5468 6520 696e 6465 7820 6f66 2074 6865  The index of the
+0000d800: 2072 6561 6420 7374 6174 652e 0a20 2020   read state..   
+0000d810: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000d820: 2067 6574 5f72 6571 7565 7374 5f63 7478   get_request_ctx
+0000d830: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
+0000d840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d850: 2020 2020 2060 7265 7175 6573 745f 6374       `request_ct
+0000d860: 7860 3a20 4120 6461 7461 6772 616d 2063  x`: A datagram c
+0000d870: 6f6e 7369 7374 696e 6720 6f66 2063 6f6e  onsisting of con
+0000d880: 7465 7874 2061 626f 7574 2074 6865 2072  text about the r
+0000d890: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
+0000d8a0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0000d8b0: 7265 7175 6573 745f 6374 7828 7365 6c66  request_ctx(self
+0000d8c0: 2c20 7265 7175 6573 745f 6374 783a 2062  , request_ctx: b
+0000d8d0: 7974 6573 2920 2d3e 204e 6f6e 653a 0a20  ytes) -> None:. 
+0000d8e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d8f0: 2020 2060 7265 7175 6573 745f 6374 7860     `request_ctx`
+0000d900: 3a20 4120 6461 7461 6772 616d 2063 6f6e  : A datagram con
+0000d910: 7369 7374 696e 6720 6f66 2063 6f6e 7465  sisting of conte
+0000d920: 7874 2061 626f 7574 2074 6865 2072 6571  xt about the req
+0000d930: 7565 7374 2e0a 2020 2020 2020 2020 2222  uest..        ""
+0000d940: 220a 0a63 6c61 7373 2052 6561 6453 7461  "..class ReadSta
+0000d950: 7465 285f 5f41 5049 5f52 6561 6453 7461  te(__API_ReadSta
+0000d960: 7465 293a 0a20 2020 2022 2222 0a20 2020  te):.    """.   
+0000d970: 2052 6561 6453 7461 7465 2070 726f 7669   ReadState provi
+0000d980: 6465 7320 7374 6174 6520 666f 7220 7265  des state for re
+0000d990: 6164 206f 6e6c 7920 7175 6572 792e 0a20  ad only query.. 
+0000d9a0: 2020 2049 7427 7320 6361 6c6c 6572 2773     It's caller's
+0000d9b0: 2072 6573 706f 6e73 6962 696c 6974 7920   responsibility 
+0000d9c0: 746f 2073 656e 6420 4d73 6752 6561 6449  to send MsgReadI
+0000d9d0: 6e64 6578 2066 6972 7374 2062 6566 6f72  ndex first befor
+0000d9e0: 6520 6765 7474 696e 670a 2020 2020 7468  e getting.    th
+0000d9f0: 6973 2073 7461 7465 2066 726f 6d20 7265  is state from re
+0000da00: 6164 792e 2049 7427 7320 616c 736f 2063  ady. It's also c
+0000da10: 616c 6c65 7227 7320 6475 7479 2074 6f20  aller's duty to 
+0000da20: 6469 6666 6572 656e 7469 6174 6520 6966  differentiate if
+0000da30: 2074 6869 730a 2020 2020 7374 6174 6520   this.    state 
+0000da40: 6973 2077 6861 7420 6974 2072 6571 7565  is what it reque
+0000da50: 7374 7320 7468 726f 7567 6820 7265 7175  sts through requ
+0000da60: 6573 745f 6374 782c 2065 2e67 2e20 6769  est_ctx, e.g. gi
+0000da70: 7665 6e20 6120 756e 6971 7565 2069 6420  ven a unique id 
+0000da80: 6173 0a20 2020 2072 6571 7565 7374 5f63  as.    request_c
+0000da90: 7478 2e0a 2020 2020 2222 220a 0a20 2020  tx..    """..   
+0000daa0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0000dab0: 6c66 2920 2d3e 204e 6f6e 653a 202e 2e2e  lf) -> None: ...
+0000dac0: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
+0000dad0: 6628 7365 6c66 2920 2d3e 2022 5265 6164  f(self) -> "Read
+0000dae0: 5374 6174 6552 6566 223a 202e 2e2e 0a0a  StateRef": .....
+0000daf0: 636c 6173 7320 5265 6164 5374 6174 6552  class ReadStateR
+0000db00: 6566 285f 5f41 5049 5f52 6561 6453 7461  ef(__API_ReadSta
+0000db10: 7465 293a 0a20 2020 2022 2222 0a20 2020  te):.    """.   
+0000db20: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+0000db30: 6f66 203a 636c 6173 733a 6052 6561 6453  of :class:`ReadS
+0000db40: 7461 7465 602e 0a20 2020 2022 2222 0a0a  tate`..    """..
+0000db50: 636c 6173 7320 5f5f 4150 495f 5261 6674  class __API_Raft
+0000db60: 4c6f 673a 0a20 2020 2064 6566 2065 6e74  Log:.    def ent
+0000db70: 7269 6573 280a 2020 2020 2020 2020 7365  ries(.        se
+0000db80: 6c66 2c20 6964 783a 2069 6e74 2c20 636f  lf, idx: int, co
+0000db90: 6e74 6578 743a 2022 4765 7445 6e74 7269  ntext: "GetEntri
+0000dba0: 6573 436f 6e74 6578 7452 6566 222c 206d  esContextRef", m
+0000dbb0: 6178 5f73 697a 653a 204f 7074 696f 6e61  ax_size: Optiona
+0000dbc0: 6c5b 696e 745d 0a20 2020 2029 202d 3e20  l[int].    ) -> 
+0000dbd0: 4c69 7374 5b22 456e 7472 7922 5d3a 0a20  List["Entry"]:. 
+0000dbe0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000dbf0: 2020 2052 6574 7572 6e73 2065 6e74 7269     Returns entri
+0000dc00: 6573 2073 7461 7274 696e 6720 6672 6f6d  es starting from
+0000dc10: 2061 2070 6172 7469 6375 6c61 7220 696e   a particular in
+0000dc20: 6465 7820 616e 6420 6e6f 7420 6578 6365  dex and not exce
+0000dc30: 6564 696e 6720 6120 6279 7465 7369 7a65  eding a bytesize
+0000dc40: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000dc50: 2020 6465 6620 616c 6c5f 656e 7472 6965    def all_entrie
+0000dc60: 7328 7365 6c66 2920 2d3e 204c 6973 745b  s(self) -> List[
+0000dc70: 2245 6e74 7279 225d 3a0a 2020 2020 2020  "Entry"]:.      
+0000dc80: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000dc90: 7475 726e 7320 616c 6c20 7468 6520 656e  turns all the en
+0000dca0: 7472 6965 732e 204f 6e6c 7920 7573 6564  tries. Only used
+0000dcb0: 2062 7920 7465 7374 732e 0a20 2020 2020   by tests..     
+0000dcc0: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
+0000dcd0: 7070 656e 6428 7365 6c66 2c20 656e 7473  ppend(self, ents
+0000dce0: 3a20 4c69 7374 5b22 456e 7472 7922 5d20  : List["Entry"] 
+0000dcf0: 7c20 4c69 7374 5b22 456e 7472 7952 6566  | List["EntryRef
+0000dd00: 225d 2920 2d3e 2069 6e74 3a0a 2020 2020  "]) -> int:.    
+0000dd10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000dd20: 4170 7065 6e64 7320 6120 7365 7420 6f66  Appends a set of
+0000dd30: 2065 6e74 7269 6573 2074 6f20 7468 6520   entries to the 
+0000dd40: 756e 7374 6162 6c65 206c 6973 742e 0a20  unstable list.. 
+0000dd50: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000dd60: 6566 2061 7070 6c69 6564 2873 656c 6629  ef applied(self)
+0000dd70: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000dd80: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+0000dd90: 7572 6e73 2074 6865 206c 6173 7420 6170  urns the last ap
+0000dda0: 706c 6965 6420 696e 6465 782e 0a20 2020  plied index..   
+0000ddb0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000ddc0: 2066 696e 645f 636f 6e66 6c69 6374 2873   find_conflict(s
+0000ddd0: 656c 662c 2065 6e74 733a 204c 6973 745b  elf, ents: List[
+0000dde0: 2245 6e74 7279 225d 207c 204c 6973 745b  "Entry"] | List[
+0000ddf0: 2245 6e74 7279 5265 6622 5d29 202d 3e20  "EntryRef"]) -> 
+0000de00: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+0000de10: 0a20 2020 2020 2020 2046 696e 6473 2074  .        Finds t
+0000de20: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+0000de30: 636f 6e66 6c69 6374 2e0a 0a20 2020 2020  conflict...     
+0000de40: 2020 2049 7420 7265 7475 726e 7320 7468     It returns th
+0000de50: 6520 6669 7273 7420 696e 6465 7820 6f66  e first index of
+0000de60: 2063 6f6e 666c 6963 7469 6e67 2065 6e74   conflicting ent
+0000de70: 7269 6573 2062 6574 7765 656e 2074 6865  ries between the
+0000de80: 2065 7869 7374 696e 670a 2020 2020 2020   existing.      
+0000de90: 2020 656e 7472 6965 7320 616e 6420 7468    entries and th
+0000dea0: 6520 6769 7665 6e20 656e 7472 6965 732c  e given entries,
+0000deb0: 2069 6620 7468 6572 6520 6172 6520 616e   if there are an
+0000dec0: 792e 0a0a 2020 2020 2020 2020 4966 2074  y...        If t
+0000ded0: 6865 7265 2061 7265 206e 6f20 636f 6e66  here are no conf
+0000dee0: 6c69 6374 696e 6720 656e 7472 6965 732c  licting entries,
+0000def0: 2061 6e64 2074 6865 2065 7869 7374 696e   and the existin
+0000df00: 6720 656e 7472 6965 7320 636f 6e74 6169  g entries contai
+0000df10: 6e0a 2020 2020 2020 2020 616c 6c20 7468  n.        all th
+0000df20: 6520 6769 7665 6e20 656e 7472 6965 732c  e given entries,
+0000df30: 207a 6572 6f20 7769 6c6c 2062 6520 7265   zero will be re
+0000df40: 7475 726e 6564 2e0a 0a20 2020 2020 2020  turned...       
+0000df50: 2049 6620 7468 6572 6520 6172 6520 6e6f   If there are no
+0000df60: 2063 6f6e 666c 6963 7469 6e67 2065 6e74   conflicting ent
+0000df70: 7269 6573 2c20 6275 7420 7468 6520 6769  ries, but the gi
+0000df80: 7665 6e20 656e 7472 6965 7320 636f 6e74  ven entries cont
+0000df90: 6169 6e73 206e 6577 0a20 2020 2020 2020  ains new.       
+0000dfa0: 2065 6e74 7269 6573 2c20 7468 6520 696e   entries, the in
+0000dfb0: 6465 7820 6f66 2074 6865 2066 6972 7374  dex of the first
+0000dfc0: 206e 6577 2065 6e74 7279 2077 696c 6c20   new entry will 
+0000dfd0: 6265 2072 6574 7572 6e65 642e 0a0a 2020  be returned...  
+0000dfe0: 2020 2020 2020 416e 2065 6e74 7279 2069        An entry i
+0000dff0: 7320 636f 6e73 6964 6572 6564 2074 6f20  s considered to 
+0000e000: 6265 2063 6f6e 666c 6963 7469 6e67 2069  be conflicting i
+0000e010: 6620 6974 2068 6173 2074 6865 2073 616d  f it has the sam
+0000e020: 6520 696e 6465 7820 6275 740a 2020 2020  e index but.    
+0000e030: 2020 2020 6120 6469 6666 6572 656e 7420      a different 
+0000e040: 7465 726d 2e0a 0a20 2020 2020 2020 2054  term...        T
+0000e050: 6865 2066 6972 7374 2065 6e74 7279 204d  he first entry M
+0000e060: 5553 5420 6861 7665 2061 6e20 696e 6465  UST have an inde
+0000e070: 7820 6571 7561 6c20 746f 2074 6865 2061  x equal to the a
+0000e080: 7267 756d 656e 7420 2766 726f 6d27 2e0a  rgument 'from'..
+0000e090: 2020 2020 2020 2020 5468 6520 696e 6465          The inde
+0000e0a0: 7820 6f66 2074 6865 2067 6976 656e 2065  x of the given e
+0000e0b0: 6e74 7269 6573 204d 5553 5420 6265 2063  ntries MUST be c
+0000e0c0: 6f6e 7469 6e75 6f75 736c 7920 696e 6372  ontinuously incr
+0000e0d0: 6561 7369 6e67 2e0a 2020 2020 2020 2020  easing..        
+0000e0e0: 2222 220a 2020 2020 6465 6620 6669 6e64  """.    def find
+0000e0f0: 5f63 6f6e 666c 6963 745f 6279 5f74 6572  _conflict_by_ter
+0000e100: 6d28 7365 6c66 2c20 696e 6465 783a 2069  m(self, index: i
+0000e110: 6e74 2c20 7465 726d 3a20 696e 7429 202d  nt, term: int) -
+0000e120: 3e20 5475 706c 655b 696e 742c 204f 7074  > Tuple[int, Opt
+0000e130: 696f 6e61 6c5b 696e 745d 5d3a 0a20 2020  ional[int]]:.   
+0000e140: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000e150: 2066 696e 645f 636f 6e66 6c69 6374 5f62   find_conflict_b
+0000e160: 795f 7465 726d 2074 616b 6573 2061 6e20  y_term takes an 
+0000e170: 2860 696e 6465 7860 2c20 6074 6572 6d60  (`index`, `term`
+0000e180: 2920 7061 6972 2028 696e 6469 6361 7469  ) pair (indicati
+0000e190: 6e67 2061 2063 6f6e 666c 6963 7469 6e67  ng a conflicting
+0000e1a0: 206c 6f67 0a20 2020 2020 2020 2065 6e74   log.        ent
+0000e1b0: 7279 206f 6e20 6120 6c65 6164 6572 2f66  ry on a leader/f
+0000e1c0: 6f6c 6c6f 7765 7220 6475 7269 6e67 2061  ollower during a
+0000e1d0: 6e20 6170 7065 6e64 2920 616e 6420 6669  n append) and fi
+0000e1e0: 6e64 7320 7468 6520 6c61 7267 6573 7420  nds the largest 
+0000e1f0: 696e 6465 7820 696e 0a20 2020 2020 2020  index in.       
+0000e200: 206c 6f67 2077 6974 6820 6c6f 672e 7465   log with log.te
+0000e210: 726d 203c 3d20 6074 6572 6d60 2061 6e64  rm <= `term` and
+0000e220: 206c 6f67 2e69 6e64 6578 203c 3d20 6069   log.index <= `i
+0000e230: 6e64 6578 602e 2049 6620 6e6f 2073 7563  ndex`. If no suc
+0000e240: 6820 696e 6465 7820 6578 6973 7473 0a20  h index exists. 
+0000e250: 2020 2020 2020 2069 6e20 7468 6520 6c6f         in the lo
+0000e260: 672c 2074 6865 206c 6f67 2773 2066 6972  g, the log's fir
+0000e270: 7374 2069 6e64 6578 2069 7320 7265 7475  st index is retu
+0000e280: 726e 6564 2e0a 0a20 2020 2020 2020 2054  rned...        T
+0000e290: 6865 2069 6e64 6578 2070 726f 7669 6465  he index provide
+0000e2a0: 6420 4d55 5354 2062 6520 6571 7561 6c20  d MUST be equal 
+0000e2b0: 746f 206f 7220 6c65 7373 2074 6861 6e20  to or less than 
+0000e2c0: 7365 6c66 2e6c 6173 745f 696e 6465 7828  self.last_index(
+0000e2d0: 292e 2049 6e76 616c 6964 0a20 2020 2020  ). Invalid.     
+0000e2e0: 2020 2069 6e70 7574 7320 6c6f 6720 6120     inputs log a 
+0000e2f0: 7761 726e 696e 6720 616e 6420 7468 6520  warning and the 
+0000e300: 696e 7075 7420 696e 6465 7820 6973 2072  input index is r
+0000e310: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
+0000e320: 2020 5265 7475 726e 2028 696e 6465 782c    Return (index,
+0000e330: 2074 6572 6d29 0a20 2020 2020 2020 2022   term).        "
+0000e340: 2222 0a20 2020 2064 6566 2063 6f6d 6d69  "".    def commi
+0000e350: 745f 746f 2873 656c 662c 2074 6f5f 636f  t_to(self, to_co
+0000e360: 6d6d 6974 3a20 696e 7429 202d 3e20 4e6f  mmit: int) -> No
+0000e370: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+0000e380: 2020 2020 2020 2020 5365 7473 2074 6865          Sets the
+0000e390: 206c 6173 7420 636f 6d6d 6974 7465 6420   last committed 
+0000e3a0: 7661 6c75 6520 746f 2074 6865 2070 6173  value to the pas
+0000e3b0: 7365 6420 696e 2076 616c 7565 2e0a 0a20  sed in value... 
+0000e3c0: 2020 2020 2020 2023 2050 616e 6963 730a         # Panics.
+0000e3d0: 0a20 2020 2020 2020 2050 616e 6963 7320  .        Panics 
+0000e3e0: 6966 2074 6865 2069 6e64 6578 2067 6f65  if the index goe
+0000e3f0: 7320 7061 7374 2074 6865 206c 6173 7420  s past the last 
+0000e400: 696e 6465 782e 0a20 2020 2020 2020 2022  index..        "
+0000e410: 2222 0a20 2020 2064 6566 2063 6f6d 6d69  "".    def commi
+0000e420: 745f 696e 666f 2873 656c 6629 202d 3e20  t_info(self) -> 
+0000e430: 5475 706c 655b 696e 742c 2069 6e74 5d3a  Tuple[int, int]:
+0000e440: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e450: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
+0000e460: 2063 6f6d 6d69 7474 6564 2069 6e64 6578   committed index
+0000e470: 2061 6e64 2069 7473 2074 6572 6d2e 0a20   and its term.. 
+0000e480: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000e490: 6566 2073 746f 7265 2873 656c 6629 202d  ef store(self) -
+0000e4a0: 3e20 224d 656d 5374 6f72 6167 6552 6566  > "MemStorageRef
+0000e4b0: 223a 0a20 2020 2020 2020 2022 2222 2022  ":.        """ "
+0000e4c0: 2222 0a20 2020 2064 6566 206e 6578 745f  "".    def next_
+0000e4d0: 656e 7472 6965 7328 7365 6c66 2c20 6d61  entries(self, ma
+0000e4e0: 785f 7369 7a65 3a20 4f70 7469 6f6e 616c  x_size: Optional
+0000e4f0: 5b69 6e74 5d29 202d 3e20 4f70 7469 6f6e  [int]) -> Option
+0000e500: 616c 5b4c 6973 745b 2245 6e74 7279 225d  al[List["Entry"]
+0000e510: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000e520: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
+0000e530: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+0000e540: 2065 6e74 7269 6573 2066 6f72 2065 7865   entries for exe
+0000e550: 6375 7469 6f6e 2e0a 2020 2020 2020 2020  cution..        
+0000e560: 4966 2061 7070 6c69 6564 2069 7320 736d  If applied is sm
+0000e570: 616c 6c65 7220 7468 616e 2074 6865 2069  aller than the i
+0000e580: 6e64 6578 206f 6620 736e 6170 7368 6f74  ndex of snapshot
+0000e590: 2c20 6974 2072 6574 7572 6e73 2061 6c6c  , it returns all
+0000e5a0: 2063 6f6d 6d69 7474 6564 0a20 2020 2020   committed.     
+0000e5b0: 2020 2065 6e74 7269 6573 2061 6674 6572     entries after
+0000e5c0: 2074 6865 2069 6e64 6578 206f 6620 736e   the index of sn
+0000e5d0: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
+0000e5e0: 2222 220a 2020 2020 6465 6620 6e65 7874  """.    def next
+0000e5f0: 5f65 6e74 7269 6573 5f73 696e 6365 280a  _entries_since(.
+0000e600: 2020 2020 2020 2020 7365 6c66 2c20 7369          self, si
+0000e610: 6e63 655f 6964 783a 2069 6e74 2c20 6d61  nce_idx: int, ma
+0000e620: 785f 7369 7a65 3a20 4f70 7469 6f6e 616c  x_size: Optional
+0000e630: 5b69 6e74 5d0a 2020 2020 2920 2d3e 204f  [int].    ) -> O
+0000e640: 7074 696f 6e61 6c5b 4c69 7374 5b22 456e  ptional[List["En
+0000e650: 7472 7922 5d5d 3a0a 2020 2020 2020 2020  try"]]:.        
+0000e660: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000e670: 726e 7320 636f 6d6d 6974 7465 6420 616e  rns committed an
+0000e680: 6420 7065 7273 6973 7465 6420 656e 7472  d persisted entr
+0000e690: 6965 7320 7369 6e63 6520 6d61 7828 6073  ies since max(`s
+0000e6a0: 696e 6365 5f69 6478 6020 2b20 312c 2066  ince_idx` + 1, f
+0000e6b0: 6972 7374 5f69 6e64 6578 292e 0a20 2020  irst_index)..   
+0000e6c0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000e6d0: 2068 6173 5f6e 6578 745f 656e 7472 6965   has_next_entrie
+0000e6e0: 7328 7365 6c66 2920 2d3e 2062 6f6f 6c3a  s(self) -> bool:
+0000e6f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e700: 2020 2020 2052 6574 7572 6e73 2077 6865       Returns whe
+0000e710: 7468 6572 2074 6865 7265 2061 7265 206e  ther there are n
+0000e720: 6577 2065 6e74 7269 6573 2e0a 2020 2020  ew entries..    
+0000e730: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000e740: 6861 735f 6e65 7874 5f65 6e74 7269 6573  has_next_entries
+0000e750: 5f73 696e 6365 2873 656c 662c 2073 696e  _since(self, sin
+0000e760: 6365 5f69 6478 3a20 696e 7429 202d 3e20  ce_idx: int) -> 
+0000e770: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+0000e780: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+0000e790: 7320 7768 6574 6865 7220 7468 6572 6520  s whether there 
+0000e7a0: 6172 6520 636f 6d6d 6974 7465 6420 616e  are committed an
+0000e7b0: 6420 7065 7273 6973 7465 6420 656e 7472  d persisted entr
+0000e7c0: 6965 7320 7369 6e63 650a 2020 2020 2020  ies since.      
+0000e7d0: 2020 6d61 7828 6073 696e 6365 5f69 6478    max(`since_idx
+0000e7e0: 6020 2b20 312c 2066 6972 7374 5f69 6e64  ` + 1, first_ind
+0000e7f0: 6578 292e 0a20 2020 2020 2020 2022 2222  ex)..        """
+0000e800: 0a20 2020 2064 6566 2069 735f 7570 5f74  .    def is_up_t
+0000e810: 6f5f 6461 7465 2873 656c 662c 206c 6173  o_date(self, las
+0000e820: 745f 696e 6465 783a 2069 6e74 2c20 7465  t_index: int, te
+0000e830: 726d 3a20 696e 7429 202d 3e20 626f 6f6c  rm: int) -> bool
+0000e840: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000e850: 2020 2020 2020 4465 7465 726d 696e 6573        Determines
+0000e860: 2069 6620 7468 6520 6769 7665 6e20 286c   if the given (l
+0000e870: 6173 7449 6e64 6578 2c74 6572 6d29 206c  astIndex,term) l
+0000e880: 6f67 2069 7320 6d6f 7265 2075 702d 746f  og is more up-to
+0000e890: 2d64 6174 650a 2020 2020 2020 2020 6279  -date.        by
+0000e8a0: 2063 6f6d 7061 7269 6e67 2074 6865 2069   comparing the i
+0000e8b0: 6e64 6578 2061 6e64 2074 6572 6d20 6f66  ndex and term of
+0000e8c0: 2074 6865 206c 6173 7420 656e 7472 7920   the last entry 
+0000e8d0: 696e 2074 6865 2065 7869 7374 696e 6720  in the existing 
+0000e8e0: 6c6f 6773 2e0a 2020 2020 2020 2020 4966  logs..        If
+0000e8f0: 2074 6865 206c 6f67 7320 6861 7665 206c   the logs have l
+0000e900: 6173 7420 656e 7472 7920 7769 7468 2064  ast entry with d
+0000e910: 6966 6665 7265 6e74 2074 6572 6d73 2c20  ifferent terms, 
+0000e920: 7468 656e 2074 6865 206c 6f67 2077 6974  then the log wit
+0000e930: 6820 7468 650a 2020 2020 2020 2020 6c61  h the.        la
+0000e940: 7465 7220 7465 726d 2069 7320 6d6f 7265  ter term is more
+0000e950: 2075 702d 746f 2d64 6174 652e 2049 6620   up-to-date. If 
+0000e960: 7468 6520 6c6f 6773 2065 6e64 2077 6974  the logs end wit
+0000e970: 6820 7468 6520 7361 6d65 2074 6572 6d2c  h the same term,
+0000e980: 2074 6865 6e0a 2020 2020 2020 2020 7768   then.        wh
+0000e990: 6963 6865 7665 7220 6c6f 6720 6861 7320  ichever log has 
+0000e9a0: 7468 6520 6c61 7267 6572 206c 6173 745f  the larger last_
+0000e9b0: 696e 6465 7820 6973 206d 6f72 6520 7570  index is more up
+0000e9c0: 2d74 6f2d 6461 7465 2e20 4966 2074 6865  -to-date. If the
+0000e9d0: 206c 6f67 7320 6172 650a 2020 2020 2020   logs are.      
+0000e9e0: 2020 7468 6520 7361 6d65 2c20 7468 6520    the same, the 
+0000e9f0: 6769 7665 6e20 6c6f 6720 6973 2075 702d  given log is up-
+0000ea00: 746f 2d64 6174 652e 0a20 2020 2020 2020  to-date..       
+0000ea10: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
+0000ea20: 6265 5f63 6f6d 6d69 7428 7365 6c66 2c20  be_commit(self, 
+0000ea30: 6d61 785f 696e 6465 783a 2069 6e74 2c20  max_index: int, 
+0000ea40: 7465 726d 3a20 696e 7429 202d 3e20 626f  term: int) -> bo
+0000ea50: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+0000ea60: 2020 2020 2020 2020 4174 7465 6d70 7473          Attempts
+0000ea70: 2074 6f20 636f 6d6d 6974 2074 6865 2069   to commit the i
+0000ea80: 6e64 6578 2061 6e64 2074 6572 6d20 616e  ndex and term an
+0000ea90: 6420 7265 7475 726e 7320 7768 6574 6865  d returns whethe
+0000eaa0: 7220 6974 2064 6964 2e0a 2020 2020 2020  r it did..      
+0000eab0: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
+0000eac0: 7962 655f 7065 7273 6973 7428 7365 6c66  ybe_persist(self
+0000ead0: 2c20 696e 6465 783a 2069 6e74 2c20 7465  , index: int, te
+0000eae0: 726d 3a20 696e 7429 202d 3e20 626f 6f6c  rm: int) -> bool
+0000eaf0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000eb00: 2020 2020 2020 4174 7465 6d70 7473 2074        Attempts t
+0000eb10: 6f20 7065 7273 6973 7420 7468 6520 696e  o persist the in
+0000eb20: 6465 7820 616e 6420 7465 726d 2061 6e64  dex and term and
+0000eb30: 2072 6574 7572 6e73 2077 6865 7468 6572   returns whether
+0000eb40: 2069 7420 6469 642e 0a20 2020 2020 2020   it did..       
+0000eb50: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
+0000eb60: 6265 5f70 6572 7369 7374 5f73 6e61 7028  be_persist_snap(
+0000eb70: 7365 6c66 2c20 696e 6465 783a 2069 6e74  self, index: int
+0000eb80: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0000eb90: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
+0000eba0: 7474 656d 7074 7320 746f 2070 6572 7369  ttempts to persi
+0000ebb0: 7374 2074 6865 2073 6e61 7073 686f 7420  st the snapshot 
+0000ebc0: 616e 6420 7265 7475 726e 7320 7768 6574  and returns whet
+0000ebd0: 6865 7220 6974 2064 6964 2e0a 2020 2020  her it did..    
+0000ebe0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000ebf0: 6d61 7962 655f 6170 7065 6e64 280a 2020  maybe_append(.  
+0000ec00: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000ec10: 2020 2020 6964 783a 2069 6e74 2c0a 2020      idx: int,.  
+0000ec20: 2020 2020 2020 7465 726d 3a20 696e 742c        term: int,
+0000ec30: 0a20 2020 2020 2020 2063 6f6d 6d69 7474  .        committ
+0000ec40: 6564 3a20 696e 742c 0a20 2020 2020 2020  ed: int,.       
+0000ec50: 2065 6e74 733a 204c 6973 745b 2245 6e74   ents: List["Ent
+0000ec60: 7279 225d 207c 204c 6973 745b 2245 6e74  ry"] | List["Ent
+0000ec70: 7279 5265 6622 5d2c 0a20 2020 2029 202d  ryRef"],.    ) -
+0000ec80: 3e20 4f70 7469 6f6e 616c 5b54 7570 6c65  > Optional[Tuple
+0000ec90: 5b69 6e74 2c20 696e 745d 5d3a 0a20 2020  [int, int]]:.   
+0000eca0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ecb0: 2052 6574 7572 6e73 204e 6f6e 6520 6966   Returns None if
+0000ecc0: 2074 6865 2065 6e74 7269 6573 2063 616e   the entries can
+0000ecd0: 6e6f 7420 6265 2061 7070 656e 6465 642e  not be appended.
+0000ece0: 204f 7468 6572 7769 7365 2c0a 2020 2020   Otherwise,.    
+0000ecf0: 2020 2020 6974 2072 6574 7572 6e73 2053      it returns S
+0000ed00: 6f6d 6528 2863 6f6e 666c 6963 745f 696e  ome((conflict_in
+0000ed10: 6465 782c 206c 6173 745f 696e 6465 7829  dex, last_index)
+0000ed20: 292e 0a0a 2020 2020 2020 2020 2320 5061  )...        # Pa
+0000ed30: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
+0000ed40: 6e69 6373 2069 6620 6974 2066 696e 6473  nics if it finds
+0000ed50: 2061 2063 6f6e 666c 6963 7469 6e67 2069   a conflicting i
+0000ed60: 6e64 6578 206c 6573 7320 7468 616e 2063  ndex less than c
+0000ed70: 6f6d 6d69 7474 6564 2069 6e64 6578 2e0a  ommitted index..
+0000ed80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000ed90: 6465 6620 736e 6170 7368 6f74 2873 656c  def snapshot(sel
+0000eda0: 662c 2072 6571 7565 7374 5f69 6e64 6578  f, request_index
+0000edb0: 3a20 696e 742c 2074 6f3a 2069 6e74 2920  : int, to: int) 
+0000edc0: 2d3e 2022 536e 6170 7368 6f74 5265 6622  -> "SnapshotRef"
+0000edd0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000ede0: 2020 2020 2020 5265 7475 726e 7320 7468        Returns th
+0000edf0: 6520 6375 7272 656e 7420 736e 6170 7368  e current snapsh
+0000ee00: 6f74 0a20 2020 2020 2020 2022 2222 0a20  ot.        """. 
+0000ee10: 2020 2064 6566 2073 7461 626c 655f 656e     def stable_en
+0000ee20: 7472 6965 7328 7365 6c66 2c20 696e 6465  tries(self, inde
+0000ee30: 783a 2069 6e74 2c20 7465 726d 3a20 696e  x: int, term: in
+0000ee40: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+0000ee50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ee60: 436c 6561 7273 2074 6865 2075 6e73 7461  Clears the unsta
+0000ee70: 626c 6520 656e 7472 6965 7320 616e 6420  ble entries and 
+0000ee80: 6d6f 7665 7320 7468 6520 7374 6162 6c65  moves the stable
+0000ee90: 206f 6666 7365 7420 7570 2074 6f20 7468   offset up to th
+0000eea0: 650a 2020 2020 2020 2020 6c61 7374 2069  e.        last i
+0000eeb0: 6e64 6578 2c20 6966 2074 6865 7265 2069  ndex, if there i
+0000eec0: 7320 616e 792e 0a20 2020 2020 2020 2022  s any..        "
+0000eed0: 2222 0a20 2020 2064 6566 2073 7461 626c  "".    def stabl
+0000eee0: 655f 736e 6170 2873 656c 662c 2069 6e64  e_snap(self, ind
+0000eef0: 6578 3a20 696e 7429 202d 3e20 4e6f 6e65  ex: int) -> None
 0000ef00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000ef10: 2020 2020 2020 466f 7220 6120 6769 7665        For a give
-0000ef20: 6e20 696e 6465 782c 2066 696e 6473 2074  n index, finds t
-0000ef30: 6865 2074 6572 6d20 6173 736f 6369 6174  he term associat
-0000ef40: 6564 2077 6974 6820 6974 2e0a 2020 2020  ed with it..    
-0000ef50: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000ef60: 6c61 7374 5f74 6572 6d28 7365 6c66 2920  last_term(self) 
-0000ef70: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-0000ef80: 2222 220a 2020 2020 2020 2020 4772 6162  """.        Grab
-0000ef90: 7320 7468 6520 7465 726d 2066 726f 6d20  s the term from 
-0000efa0: 7468 6520 6c61 7374 2065 6e74 7279 2e0a  the last entry..
-0000efb0: 0a20 2020 2020 2020 2023 2050 616e 6963  .        # Panic
-0000efc0: 730a 0a20 2020 2020 2020 2050 616e 6963  s..        Panic
-0000efd0: 7320 6966 2074 6865 7265 2061 7265 2065  s if there are e
-0000efe0: 6e74 7269 6573 2062 7574 2074 6865 206c  ntries but the l
-0000eff0: 6173 7420 7465 726d 2068 6173 2062 6565  ast term has bee
-0000f000: 6e20 6469 7363 6172 6465 642e 0a20 2020  n discarded..   
-0000f010: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000f020: 206d 6174 6368 5f74 6572 6d28 7365 6c66   match_term(self
-0000f030: 2c20 6964 783a 2069 6e74 2c20 7465 726d  , idx: int, term
-0000f040: 3a20 696e 7429 202d 3e20 626f 6f6c 3a0a  : int) -> bool:.
-0000f050: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f060: 2020 2020 416e 7377 6572 7320 7468 6520      Answers the 
-0000f070: 7175 6573 7469 6f6e 3a20 446f 6573 2074  question: Does t
-0000f080: 6869 7320 696e 6465 7820 6265 6c6f 6e67  his index belong
-0000f090: 2074 6f20 7468 6973 2074 6572 6d3f 0a20   to this term?. 
-0000f0a0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000f0b0: 6566 2066 6972 7374 5f69 6e64 6578 2873  ef first_index(s
-0000f0c0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-0000f0d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f0e0: 2052 6574 7572 6e73 2074 6820 6669 7273   Returns th firs
-0000f0f0: 7420 696e 6465 7820 696e 2074 6865 2073  t index in the s
-0000f100: 746f 7265 2074 6861 7420 6973 2061 7661  tore that is ava
-0000f110: 696c 6162 6c65 2076 6961 2065 6e74 7269  ilable via entri
-0000f120: 6573 0a0a 2020 2020 2020 2020 2320 5061  es..        # Pa
-0000f130: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
-0000f140: 6e69 6373 2069 6620 7468 6520 7374 6f72  nics if the stor
-0000f150: 6520 646f 6573 6e27 7420 6861 7665 2061  e doesn't have a
-0000f160: 2066 6972 7374 2069 6e64 6578 2e0a 2020   first index..  
-0000f170: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000f180: 6620 6c61 7374 5f69 6e64 6578 2873 656c  f last_index(sel
-0000f190: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-0000f1a0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000f1b0: 6574 7572 6e73 2074 6865 206c 6173 7420  eturns the last 
-0000f1c0: 696e 6465 7820 696e 2074 6865 2073 746f  index in the sto
-0000f1d0: 7265 2074 6861 7420 6973 2061 7661 696c  re that is avail
-0000f1e0: 6162 6c65 2076 6961 2065 6e74 7269 6573  able via entries
-0000f1f0: 2e0a 0a20 2020 2020 2020 2023 2050 616e  ...        # Pan
-0000f200: 6963 730a 0a20 2020 2020 2020 2050 616e  ics..        Pan
-0000f210: 6963 7320 6966 2074 6865 2073 746f 7265  ics if the store
-0000f220: 2064 6f65 736e 2774 2068 6176 6520 6120   doesn't have a 
-0000f230: 6c61 7374 2069 6e64 6578 2e0a 2020 2020  last index..    
-0000f240: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000f250: 756e 7374 6162 6c65 2873 656c 6629 202d  unstable(self) -
-0000f260: 3e20 2255 6e73 7461 626c 6552 6566 223a  > "UnstableRef":
-0000f270: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f280: 2020 2020 2052 6574 7572 6e73 2061 2072       Returns a r
-0000f290: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
-0000f2a0: 756e 7374 6162 6c65 206c 6f67 2e0a 2020  unstable log..  
-0000f2b0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000f2c0: 6620 756e 7374 6162 6c65 5f65 6e74 7269  f unstable_entri
-0000f2d0: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
-0000f2e0: 5b22 456e 7472 7952 6566 225d 3a0a 2020  ["EntryRef"]:.  
-0000f2f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000f300: 2020 5265 7475 726e 7320 736c 6963 6520    Returns slice 
-0000f310: 6f66 2065 6e74 7269 6573 2074 6861 7420  of entries that 
-0000f320: 6172 6520 6e6f 7420 7065 7273 6973 7465  are not persiste
-0000f330: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
-0000f340: 2020 2064 6566 2075 6e73 7461 626c 655f     def unstable_
-0000f350: 736e 6170 7368 6f74 2873 656c 6629 202d  snapshot(self) -
-0000f360: 3e20 4f70 7469 6f6e 616c 5b22 536e 6170  > Optional["Snap
-0000f370: 7368 6f74 5265 6622 5d3a 0a20 2020 2020  shotRef"]:.     
-0000f380: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000f390: 6574 7572 6e73 2074 6865 2073 6e61 7073  eturns the snaps
-0000f3a0: 686f 7420 7468 6174 2061 7265 206e 6f74  hot that are not
-0000f3b0: 2070 6572 7369 7374 6564 2e0a 2020 2020   persisted..    
-0000f3c0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000f3d0: 6765 745f 6170 706c 6965 6428 7365 6c66  get_applied(self
-0000f3e0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-0000f3f0: 2020 2222 220a 2020 2020 2020 2020 6061    """.        `a
-0000f400: 7070 6c69 6564 603a 2054 6865 2068 6967  pplied`: The hig
-0000f410: 6865 7374 206c 6f67 2070 6f73 6974 696f  hest log positio
-0000f420: 6e20 7468 6174 2074 6865 2061 7070 6c69  n that the appli
-0000f430: 6361 7469 6f6e 2068 6173 2062 6565 6e20  cation has been 
-0000f440: 696e 7374 7275 6374 6564 0a20 2020 2020  instructed.     
-0000f450: 2020 2074 6f20 6170 706c 7920 746f 2069     to apply to i
-0000f460: 7473 2073 7461 7465 206d 6163 6869 6e65  ts state machine
-0000f470: 2e0a 0a20 2020 2020 2020 2049 6e76 6172  ...        Invar
-0000f480: 6961 6e74 3a20 6170 706c 6965 6420 3c3d  iant: applied <=
-0000f490: 206d 696e 2863 6f6d 6d69 7474 6564 2c20   min(committed, 
-0000f4a0: 7065 7273 6973 7465 6429 0a20 2020 2020  persisted).     
-0000f4b0: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
-0000f4c0: 6574 5f61 7070 6c69 6564 2873 656c 662c  et_applied(self,
-0000f4d0: 2061 7070 6c69 6564 3a20 696e 7429 202d   applied: int) -
-0000f4e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000f4f0: 2222 220a 2020 2020 2020 2020 6061 7070  """.        `app
-0000f500: 6c69 6564 603a 2054 6865 2068 6967 6865  lied`: The highe
-0000f510: 7374 206c 6f67 2070 6f73 6974 696f 6e20  st log position 
-0000f520: 7468 6174 2074 6865 2061 7070 6c69 6361  that the applica
-0000f530: 7469 6f6e 2068 6173 2062 6565 6e20 696e  tion has been in
-0000f540: 7374 7275 6374 6564 0a20 2020 2020 2020  structed.       
-0000f550: 2074 6f20 6170 706c 7920 746f 2069 7473   to apply to its
-0000f560: 2073 7461 7465 206d 6163 6869 6e65 2e0a   state machine..
-0000f570: 0a20 2020 2020 2020 2049 6e76 6172 6961  .        Invaria
-0000f580: 6e74 3a20 6170 706c 6965 6420 3c3d 206d  nt: applied <= m
-0000f590: 696e 2863 6f6d 6d69 7474 6564 2c20 7065  in(committed, pe
-0000f5a0: 7273 6973 7465 6429 0a20 2020 2020 2020  rsisted).       
-0000f5b0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-0000f5c0: 5f63 6f6d 6d69 7474 6564 2873 656c 6629  _committed(self)
-0000f5d0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-0000f5e0: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
-0000f5f0: 6d6d 6974 7465 6460 3a20 5468 6520 6869  mmitted`: The hi
-0000f600: 6768 6573 7420 6c6f 6720 706f 7369 7469  ghest log positi
-0000f610: 6f6e 2074 6861 7420 6973 206b 6e6f 776e  on that is known
-0000f620: 2074 6f20 6265 2069 6e20 7374 6162 6c65   to be in stable
-0000f630: 2073 746f 7261 6765 0a20 2020 2020 2020   storage.       
-0000f640: 206f 6e20 6120 7175 6f72 756d 206f 6620   on a quorum of 
-0000f650: 6e6f 6465 732e 0a0a 2020 2020 2020 2020  nodes...        
-0000f660: 496e 7661 7269 616e 743a 2061 7070 6c69  Invariant: appli
-0000f670: 6564 203c 3d20 636f 6d6d 6974 7465 640a  ed <= committed.
-0000f680: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f690: 6465 6620 7365 745f 636f 6d6d 6974 7465  def set_committe
-0000f6a0: 6428 7365 6c66 2c20 636f 6d6d 6974 7465  d(self, committe
-0000f6b0: 643a 2069 6e74 2920 2d3e 204e 6f6e 653a  d: int) -> None:
-0000f6c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f6d0: 2020 2020 2060 636f 6d6d 6974 7465 6460       `committed`
-0000f6e0: 3a20 5468 6520 6869 6768 6573 7420 6c6f  : The highest lo
-0000f6f0: 6720 706f 7369 7469 6f6e 2074 6861 7420  g position that 
-0000f700: 6973 206b 6e6f 776e 2074 6f20 6265 2069  is known to be i
-0000f710: 6e20 7374 6162 6c65 2073 746f 7261 6765  n stable storage
-0000f720: 0a20 2020 2020 2020 206f 6e20 6120 7175  .        on a qu
-0000f730: 6f72 756d 206f 6620 6e6f 6465 732e 0a0a  orum of nodes...
-0000f740: 2020 2020 2020 2020 496e 7661 7269 616e          Invarian
-0000f750: 743a 2061 7070 6c69 6564 203c 3d20 636f  t: applied <= co
-0000f760: 6d6d 6974 7465 640a 2020 2020 2020 2020  mmitted.        
-0000f770: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-0000f780: 7065 7273 6973 7465 6428 7365 6c66 2920  persisted(self) 
-0000f790: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-0000f7a0: 2222 220a 2020 2020 2020 2020 6070 6572  """.        `per
-0000f7b0: 7369 7374 6564 603a 2054 6865 2068 6967  sisted`: The hig
-0000f7c0: 6865 7374 206c 6f67 2070 6f73 6974 696f  hest log positio
-0000f7d0: 6e20 7468 6174 2069 7320 6b6e 6f77 6e20  n that is known 
-0000f7e0: 746f 2062 6520 7065 7273 6973 7465 6420  to be persisted 
-0000f7f0: 696e 2073 7461 626c 650a 2020 2020 2020  in stable.      
-0000f800: 2020 7374 6f72 6167 652e 2049 7427 7320    storage. It's 
-0000f810: 7573 6564 2066 6f72 206c 696d 6974 696e  used for limitin
-0000f820: 6720 7468 6520 7570 7065 7220 626f 756e  g the upper boun
-0000f830: 6420 6f66 2063 6f6d 6d69 7474 6564 2061  d of committed a
-0000f840: 6e64 0a20 2020 2020 2020 2070 6572 7369  nd.        persi
-0000f850: 7374 6564 2065 6e74 7269 6573 2e0a 0a20  sted entries... 
-0000f860: 2020 2020 2020 2049 6e76 6172 6961 6e74         Invariant
-0000f870: 3a20 7065 7273 6973 7465 6420 3c20 756e  : persisted < un
-0000f880: 7374 6162 6c65 2e6f 6666 7365 7420 2626  stable.offset &&
-0000f890: 2061 7070 6c69 6564 203c 3d20 7065 7273   applied <= pers
-0000f8a0: 6973 7465 640a 2020 2020 2020 2020 2222  isted.        ""
-0000f8b0: 220a 2020 2020 6465 6620 7365 745f 7065  ".    def set_pe
-0000f8c0: 7273 6973 7465 6428 7365 6c66 2c20 7065  rsisted(self, pe
-0000f8d0: 7273 6973 7465 643a 2069 6e74 2920 2d3e  rsisted: int) ->
-0000f8e0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000f8f0: 2222 0a20 2020 2020 2020 2060 7065 7273  "".        `pers
-0000f900: 6973 7465 6460 3a20 5468 6520 6869 6768  isted`: The high
-0000f910: 6573 7420 6c6f 6720 706f 7369 7469 6f6e  est log position
-0000f920: 2074 6861 7420 6973 206b 6e6f 776e 2074   that is known t
-0000f930: 6f20 6265 2070 6572 7369 7374 6564 2069  o be persisted i
-0000f940: 6e20 7374 6162 6c65 0a20 2020 2020 2020  n stable.       
-0000f950: 2073 746f 7261 6765 2e20 4974 2773 2075   storage. It's u
-0000f960: 7365 6420 666f 7220 6c69 6d69 7469 6e67  sed for limiting
-0000f970: 2074 6865 2075 7070 6572 2062 6f75 6e64   the upper bound
-0000f980: 206f 6620 636f 6d6d 6974 7465 6420 616e   of committed an
-0000f990: 640a 2020 2020 2020 2020 7065 7273 6973  d.        persis
-0000f9a0: 7465 6420 656e 7472 6965 732e 0a0a 2020  ted entries...  
-0000f9b0: 2020 2020 2020 496e 7661 7269 616e 743a        Invariant:
-0000f9c0: 2070 6572 7369 7374 6564 203c 2075 6e73   persisted < uns
-0000f9d0: 7461 626c 652e 6f66 6673 6574 2026 2620  table.offset && 
-0000f9e0: 6170 706c 6965 6420 3c3d 2070 6572 7369  applied <= persi
-0000f9f0: 7374 6564 0a20 2020 2020 2020 2022 2222  sted.        """
-0000fa00: 0a20 2020 2064 6566 2073 6c69 6365 280a  .    def slice(.
-0000fa10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000fa20: 2020 2020 2020 6c6f 773a 2069 6e74 2c0a        low: int,.
-0000fa30: 2020 2020 2020 2020 6869 6768 3a20 696e          high: in
-0000fa40: 742c 0a20 2020 2020 2020 206d 6178 5f73  t,.        max_s
-0000fa50: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
-0000fa60: 745d 2c0a 2020 2020 2020 2020 636f 6e74  t],.        cont
-0000fa70: 6578 743a 2022 4765 7445 6e74 7269 6573  ext: "GetEntries
-0000fa80: 436f 6e74 6578 7452 6566 222c 0a20 2020  ContextRef",.   
-0000fa90: 2029 202d 3e20 4c69 7374 5b22 456e 7472   ) -> List["Entr
-0000faa0: 7952 6566 225d 3a0a 2020 2020 2020 2020  yRef"]:.        
-0000fab0: 2222 220a 2020 2020 2020 2020 4772 6162  """.        Grab
-0000fac0: 7320 6120 736c 6963 6520 6f66 2065 6e74  s a slice of ent
-0000fad0: 7269 6573 2066 726f 6d20 7468 6520 7261  ries from the ra
-0000fae0: 6674 2e20 556e 6c69 6b65 2061 2072 7573  ft. Unlike a rus
-0000faf0: 7420 736c 6963 6520 706f 696e 7465 722c  t slice pointer,
-0000fb00: 2074 6865 7365 2061 7265 0a20 2020 2020   these are.     
-0000fb10: 2020 2072 6574 7572 6e65 6420 6279 2076     returned by v
-0000fb20: 616c 7565 2e20 5468 6520 7265 7375 6c74  alue. The result
-0000fb30: 2069 7320 7472 756e 6361 7465 6420 746f   is truncated to
-0000fb40: 2074 6865 206d 6178 5f73 697a 6520 696e   the max_size in
-0000fb50: 2062 7974 6573 2e0a 2020 2020 2020 2020   bytes..        
-0000fb60: 2222 220a 2020 2020 6465 6620 7265 7374  """.    def rest
-0000fb70: 6f72 6528 7365 6c66 2c20 736e 6170 7368  ore(self, snapsh
-0000fb80: 6f74 3a20 2253 6e61 7073 686f 7422 207c  ot: "Snapshot" |
-0000fb90: 2022 536e 6170 7368 6f74 5265 6622 2920   "SnapshotRef") 
-0000fba0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000fbb0: 2022 2222 0a20 2020 2020 2020 2052 6573   """.        Res
-0000fbc0: 746f 7265 7320 7468 6520 6375 7272 656e  tores the curren
-0000fbd0: 7420 6c6f 6720 6672 6f6d 2061 2073 6e61  t log from a sna
-0000fbe0: 7073 686f 742e 0a20 2020 2020 2020 2022  pshot..        "
-0000fbf0: 2222 0a0a 636c 6173 7320 496e 4d65 6d6f  ""..class InMemo
-0000fc00: 7279 5261 6674 4c6f 6728 5f5f 4150 495f  ryRaftLog(__API_
-0000fc10: 5261 6674 4c6f 6729 3a0a 2020 2020 2222  RaftLog):.    ""
-0000fc20: 220a 2020 2020 5261 6674 206c 6f67 2069  ".    Raft log i
-0000fc30: 6d70 6c65 6d65 6e74 6174 696f 6e0a 2020  mplementation.  
-0000fc40: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-0000fc50: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000fc60: 2073 656c 662c 2073 746f 7265 3a20 224d   self, store: "M
-0000fc70: 656d 5374 6f72 6167 6552 6566 222c 206c  emStorageRef", l
-0000fc80: 6f67 6765 723a 2022 4c6f 6767 6572 2220  ogger: "Logger" 
-0000fc90: 7c20 224c 6f67 6765 7252 6566 220a 2020  | "LoggerRef".  
-0000fca0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-0000fcb0: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
-0000fcc0: 6628 7365 6c66 2920 2d3e 2022 496e 4d65  f(self) -> "InMe
-0000fcd0: 6d6f 7279 5261 6674 4c6f 6752 6566 223a  moryRaftLogRef":
-0000fce0: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
-0000fcf0: 5f73 746f 7265 2873 656c 6629 202d 3e20  _store(self) -> 
-0000fd00: 224d 656d 5374 6f72 6167 6552 6566 223a  "MemStorageRef":
-0000fd10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000fd20: 2020 2020 2047 7261 6220 6120 7265 6164       Grab a read
-0000fd30: 2d6f 6e6c 7920 7265 6665 7265 6e63 6520  -only reference 
-0000fd40: 746f 2074 6865 2075 6e64 6572 6c79 696e  to the underlyin
-0000fd50: 6720 7374 6f72 6167 652e 0a20 2020 2020  g storage..     
-0000fd60: 2020 2022 2222 0a0a 636c 6173 7320 496e     """..class In
-0000fd70: 4d65 6d6f 7279 5261 6674 4c6f 6752 6566  MemoryRaftLogRef
-0000fd80: 285f 5f41 5049 5f52 6166 744c 6f67 293a  (__API_RaftLog):
-0000fd90: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
-0000fda0: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
-0000fdb0: 636c 6173 733a 6049 6e4d 656d 6f72 7952  class:`InMemoryR
-0000fdc0: 6166 744c 6f67 602e 0a20 2020 2022 2222  aftLog`..    """
-0000fdd0: 0a0a 2020 2020 6465 6620 6765 745f 7374  ..    def get_st
-0000fde0: 6f72 6528 7365 6c66 2920 2d3e 2022 4d65  ore(self) -> "Me
-0000fdf0: 6d53 746f 7261 6765 5265 6622 3a0a 2020  mStorageRef":.  
-0000fe00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000fe10: 2020 4772 6162 2061 2072 6561 642d 6f6e    Grab a read-on
-0000fe20: 6c79 2072 6566 6572 656e 6365 2074 6f20  ly reference to 
-0000fe30: 7468 6520 756e 6465 726c 7969 6e67 2073  the underlying s
-0000fe40: 746f 7261 6765 2e0a 2020 2020 2020 2020  torage..        
-0000fe50: 2222 220a 0a63 6c61 7373 2052 6166 744c  """..class RaftL
-0000fe60: 6f67 285f 5f41 5049 5f52 6166 744c 6f67  og(__API_RaftLog
-0000fe70: 293a 0a20 2020 2022 2222 2022 2222 0a0a  ):.    """ """..
-0000fe80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000fe90: 2873 656c 662c 2073 746f 7265 3a20 2253  (self, store: "S
-0000fea0: 746f 7261 6765 5265 6622 2c20 6c6f 6767  torageRef", logg
-0000feb0: 6572 3a20 224c 6f67 6765 7222 207c 2022  er: "Logger" | "
-0000fec0: 4c6f 6767 6572 5265 6622 2920 2d3e 204e  LoggerRef") -> N
-0000fed0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-0000fee0: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
-0000fef0: 2d3e 2022 5261 6674 4c6f 6752 6566 223a  -> "RaftLogRef":
-0000ff00: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
-0000ff10: 5f73 746f 7265 2873 656c 6629 202d 3e20  _store(self) -> 
-0000ff20: 2253 746f 7261 6765 5265 6622 3a0a 2020  "StorageRef":.  
-0000ff30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ff40: 2020 4772 6162 2061 2072 6561 642d 6f6e    Grab a read-on
-0000ff50: 6c79 2072 6566 6572 656e 6365 2074 6f20  ly reference to 
-0000ff60: 7468 6520 756e 6465 726c 7969 6e67 2073  the underlying s
-0000ff70: 746f 7261 6765 2e0a 2020 2020 2020 2020  torage..        
-0000ff80: 2222 220a 0a63 6c61 7373 2052 6166 744c  """..class RaftL
-0000ff90: 6f67 5265 6628 5f5f 4150 495f 5261 6674  ogRef(__API_Raft
-0000ffa0: 4c6f 6729 3a0a 2020 2020 2222 220a 2020  Log):.    """.  
-0000ffb0: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
-0000ffc0: 206f 6620 3a63 6c61 7373 3a60 5261 6674   of :class:`Raft
-0000ffd0: 4c6f 6760 2e0a 2020 2020 2222 220a 0a20  Log`..    """.. 
-0000ffe0: 2020 2064 6566 2067 6574 5f73 746f 7265     def get_store
-0000fff0: 2873 656c 6629 202d 3e20 2253 746f 7261  (self) -> "Stora
-00010000: 6765 5265 6622 3a0a 2020 2020 2020 2020  geRef":.        
-00010010: 2222 220a 2020 2020 2020 2020 4772 6162  """.        Grab
-00010020: 2061 2072 6561 642d 6f6e 6c79 2072 6566   a read-only ref
-00010030: 6572 656e 6365 2074 6f20 7468 6520 756e  erence to the un
-00010040: 6465 726c 7969 6e67 2073 746f 7261 6765  derlying storage
-00010050: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
-00010060: 6c61 7373 205f 5f41 5049 5f52 6166 743a  lass __API_Raft:
-00010070: 0a20 2020 2064 6566 2061 7070 656e 645f  .    def append_
-00010080: 656e 7472 7928 7365 6c66 2c20 656e 7473  entry(self, ents
-00010090: 3a20 4c69 7374 5b22 456e 7472 7922 5d20  : List["Entry"] 
-000100a0: 7c20 4c69 7374 5b22 456e 7472 7952 6566  | List["EntryRef
-000100b0: 225d 2920 2d3e 2062 6f6f 6c3a 0a20 2020  "]) -> bool:.   
-000100c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000100d0: 2041 7070 656e 6473 2061 2073 6c69 6365   Appends a slice
-000100e0: 206f 6620 656e 7472 6965 7320 746f 2074   of entries to t
-000100f0: 6865 206c 6f67 2e0a 2020 2020 2020 2020  he log..        
-00010100: 5468 6520 656e 7472 6965 7320 6172 6520  The entries are 
-00010110: 7570 6461 7465 6420 746f 206d 6174 6368  updated to match
-00010120: 2074 6865 2063 7572 7265 6e74 2069 6e64   the current ind
-00010130: 6578 2061 6e64 2074 6572 6d2e 0a20 2020  ex and term..   
-00010140: 2020 2020 204f 6e6c 7920 6361 6c6c 6564       Only called
-00010150: 2062 7920 6c65 6164 6572 2063 7572 7265   by leader curre
-00010160: 6e74 6c79 0a20 2020 2020 2020 2022 2222  ntly.        """
-00010170: 0a20 2020 2064 6566 2073 656e 645f 6170  .    def send_ap
-00010180: 7065 6e64 2873 656c 662c 2074 6f3a 2069  pend(self, to: i
-00010190: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000101a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000101b0: 2053 656e 6473 2061 6e20 6170 7065 6e64   Sends an append
-000101c0: 2052 5043 2077 6974 6820 6e65 7720 656e   RPC with new en
-000101d0: 7472 6965 7320 2869 6620 616e 7929 2061  tries (if any) a
-000101e0: 6e64 2074 6865 2063 7572 7265 6e74 2063  nd the current c
-000101f0: 6f6d 6d69 7420 696e 6465 7820 746f 2074  ommit index to t
-00010200: 6865 2067 6976 656e 0a20 2020 2020 2020  he given.       
-00010210: 2070 6565 722e 0a20 2020 2020 2020 2022   peer..        "
-00010220: 2222 0a20 2020 2064 6566 206f 6e5f 7065  "".    def on_pe
-00010230: 7273 6973 745f 656e 7472 6965 7328 7365  rsist_entries(se
-00010240: 6c66 2c20 696e 6465 783a 2069 6e74 2c20  lf, index: int, 
-00010250: 7465 726d 3a20 696e 7429 202d 3e20 4e6f  term: int) -> No
-00010260: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00010270: 2020 2020 2020 2020 4e6f 7469 6669 6573          Notifies
-00010280: 2074 6861 7420 7468 6573 6520 7261 6674   that these raft
-00010290: 206c 6f67 7320 6861 7665 2062 6565 6e20   logs have been 
-000102a0: 7065 7273 6973 7465 642e 0a20 2020 2020  persisted..     
-000102b0: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
-000102c0: 7070 6c79 5f74 6f5f 6375 7272 656e 745f  pply_to_current_
-000102d0: 7465 726d 2873 656c 6629 202d 3e20 626f  term(self) -> bo
-000102e0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-000102f0: 2020 2020 2020 2020 4368 6563 6b73 2069          Checks i
-00010300: 6620 6c6f 6773 2061 7265 2061 7070 6c69  f logs are appli
-00010310: 6564 2074 6f20 6375 7272 656e 7420 7465  ed to current te
-00010320: 726d 2e0a 2020 2020 2020 2020 2222 220a  rm..        """.
-00010330: 2020 2020 6465 6620 636f 6d6d 6974 5f74      def commit_t
-00010340: 6f5f 6375 7272 656e 745f 7465 726d 2873  o_current_term(s
-00010350: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-00010360: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010370: 2020 4368 6563 6b73 2069 6620 6c6f 6773    Checks if logs
-00010380: 2061 7265 2063 6f6d 6d69 7474 6564 2074   are committed t
-00010390: 6f20 6974 7320 7465 726d 2e0a 0a20 2020  o its term...   
-000103a0: 2020 2020 2054 6865 2063 6865 636b 2069       The check i
-000103b0: 7320 7573 6566 756c 2075 7375 616c 6c79  s useful usually
-000103c0: 2077 6865 6e20 7261 6674 2069 7320 6c65   when raft is le
-000103d0: 6164 6572 2e0a 2020 2020 2020 2020 2222  ader..        ""
-000103e0: 220a 2020 2020 6465 6620 6772 6f75 705f  ".    def group_
-000103f0: 636f 6d6d 6974 2873 656c 6629 202d 3e20  commit(self) -> 
-00010400: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00010410: 220a 2020 2020 2020 2020 5768 6574 6865  ".        Whethe
-00010420: 7220 656e 6162 6c65 2067 726f 7570 2063  r enable group c
-00010430: 6f6d 6d69 742e 0a20 2020 2020 2020 2022  ommit..        "
-00010440: 2222 0a20 2020 2064 6566 2065 6e61 626c  "".    def enabl
-00010450: 655f 6772 6f75 705f 636f 6d6d 6974 2873  e_group_commit(s
-00010460: 656c 662c 2065 6e61 626c 653a 2062 6f6f  elf, enable: boo
-00010470: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
-00010480: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010490: 436f 6e66 6967 7572 6573 2067 726f 7570  Configures group
-000104a0: 2063 6f6d 6d69 742e 0a0a 2020 2020 2020   commit...      
-000104b0: 2020 4966 2067 726f 7570 2063 6f6d 6d69    If group commi
-000104c0: 7420 6973 2065 6e61 626c 6564 2c20 6f6e  t is enabled, on
-000104d0: 6c79 206c 6f67 7320 7265 706c 6963 6174  ly logs replicat
-000104e0: 6564 2074 6f20 6174 206c 6561 7374 2074  ed to at least t
-000104f0: 776f 0a20 2020 2020 2020 2064 6966 6665  wo.        diffe
-00010500: 7265 6e74 2067 726f 7570 7320 6172 6520  rent groups are 
-00010510: 636f 6d6d 6974 7465 642e 0a0a 2020 2020  committed...    
-00010520: 2020 2020 596f 7520 7368 6f75 6c64 2075      You should u
-00010530: 7365 2060 6173 7369 676e 5f63 6f6d 6d69  se `assign_commi
-00010540: 745f 6772 6f75 7073 6020 746f 2063 6f6e  t_groups` to con
-00010550: 6669 6775 7265 2070 6565 7220 6772 6f75  figure peer grou
-00010560: 7073 2e0a 2020 2020 2020 2020 2222 220a  ps..        """.
-00010570: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
-00010580: 6d6d 6974 5f67 726f 7570 2873 656c 6629  mmit_group(self)
-00010590: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000105a0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-000105b0: 6d6f 7665 7320 616c 6c20 636f 6d6d 6974  moves all commit
-000105c0: 2067 726f 7570 2063 6f6e 6669 6775 7261   group configura
-000105d0: 7469 6f6e 732e 0a20 2020 2020 2020 2022  tions..        "
-000105e0: 2222 0a20 2020 2064 6566 2063 6865 636b  "".    def check
-000105f0: 5f67 726f 7570 5f63 6f6d 6d69 745f 636f  _group_commit_co
-00010600: 6e73 6973 7465 6e74 2873 656c 6629 202d  nsistent(self) -
-00010610: 3e20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  > Optional[bool]
-00010620: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010630: 2020 2020 2020 4368 6563 6b73 2077 6865        Checks whe
-00010640: 7468 6572 2074 6865 2072 6166 7420 6772  ther the raft gr
-00010650: 6f75 7020 6973 2075 7369 6e67 2067 726f  oup is using gro
-00010660: 7570 2063 6f6d 6d69 7420 616e 6420 636f  up commit and co
-00010670: 6e73 6973 7465 6e74 0a20 2020 2020 2020  nsistent.       
-00010680: 206f 7665 7220 6772 6f75 702e 0a0a 2020   over group...  
-00010690: 2020 2020 2020 4966 2069 7420 6361 6e27        If it can'
-000106a0: 7420 6765 7420 6120 636f 7272 6563 7420  t get a correct 
-000106b0: 616e 7377 6572 2c20 604e 6f6e 6560 2069  answer, `None` i
-000106c0: 7320 7265 7475 726e 6564 2e0a 2020 2020  s returned..    
-000106d0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-000106e0: 6173 7369 676e 5f63 6f6d 6d69 745f 6772  assign_commit_gr
-000106f0: 6f75 7073 2873 656c 662c 2069 6473 3a20  oups(self, ids: 
-00010700: 4c69 7374 5b54 7570 6c65 5b69 6e74 2c20  List[Tuple[int, 
-00010710: 696e 745d 5d29 202d 3e20 4e6f 6e65 3a0a  int]]) -> None:.
-00010720: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010730: 2020 2020 4173 7369 676e 7320 6772 6f75      Assigns grou
-00010740: 7073 2074 6f20 7065 6572 732e 0a0a 2020  ps to peers...  
-00010750: 2020 2020 2020 5468 6520 7475 706c 6520        The tuple 
-00010760: 6973 2028 6070 6565 725f 6964 602c 2060  is (`peer_id`, `
-00010770: 6772 6f75 705f 6964 6029 2e20 6067 726f  group_id`). `gro
-00010780: 7570 5f69 6460 2073 686f 756c 6420 6265  up_id` should be
-00010790: 206c 6172 6765 7220 7468 616e 2030 2e0a   larger than 0..
-000107a0: 0a20 2020 2020 2020 2054 6865 2067 726f  .        The gro
-000107b0: 7570 2069 6e66 6f72 6d61 7469 6f6e 2069  up information i
-000107c0: 7320 6f6e 6c79 2073 746f 7265 6420 696e  s only stored in
-000107d0: 206d 656d 6f72 792e 2053 6f20 796f 7520   memory. So you 
-000107e0: 6e65 6564 2074 6f20 636f 6e66 6967 7572  need to configur
-000107f0: 650a 2020 2020 2020 2020 6974 2065 7665  e.        it eve
-00010800: 7279 2074 696d 6520 6120 7261 6674 2073  ry time a raft s
-00010810: 7461 7465 206d 6163 6869 6e65 2069 7320  tate machine is 
-00010820: 696e 6974 6961 6c69 7a65 6420 6f72 2061  initialized or a
-00010830: 2073 6e61 7073 686f 7420 6973 2061 7070   snapshot is app
-00010840: 6c69 6564 2e0a 2020 2020 2020 2020 2222  lied..        ""
-00010850: 220a 2020 2020 6465 6620 636f 6d6d 6974  ".    def commit
-00010860: 5f61 7070 6c79 2873 656c 662c 2061 7070  _apply(self, app
-00010870: 6c69 6564 3a20 696e 7429 202d 3e20 4e6f  lied: int) -> No
-00010880: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00010890: 2020 2020 2020 2020 436f 6d6d 6974 2074          Commit t
-000108a0: 6861 7420 7468 6520 5261 6674 2070 6565  hat the Raft pee
-000108b0: 7220 6861 7320 6170 706c 6965 6420 7570  r has applied up
-000108c0: 2074 6f20 7468 6520 6769 7665 6e20 696e   to the given in
-000108d0: 6465 782e 0a0a 2020 2020 2020 2020 5265  dex...        Re
-000108e0: 6769 7374 6572 7320 7468 6520 6e65 7720  gisters the new 
-000108f0: 6170 706c 6965 6420 696e 6465 7820 746f  applied index to
-00010900: 2074 6865 2052 6166 7420 6c6f 672e 0a0a   the Raft log...
-00010910: 2020 2020 2020 2020 2320 486f 6f6b 730a          # Hooks.
-00010920: 0a20 2020 2020 2020 202a 2050 6f73 743a  .        * Post:
-00010930: 2043 6865 636b 7320 746f 2073 6565 2069   Checks to see i
-00010940: 6620 6974 2773 2074 696d 6520 746f 2066  f it's time to f
-00010950: 696e 616c 697a 6520 6120 4a6f 696e 7420  inalize a Joint 
-00010960: 436f 6e73 656e 7375 7320 7374 6174 652e  Consensus state.
-00010970: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010980: 2064 6566 206d 6179 6265 5f63 6f6d 6d69   def maybe_commi
-00010990: 7428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  t(self) -> bool:
-000109a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000109b0: 2020 2020 2041 7474 656d 7074 7320 746f       Attempts to
-000109c0: 2061 6476 616e 6365 2074 6865 2063 6f6d   advance the com
-000109d0: 6d69 7420 696e 6465 782e 2052 6574 7572  mit index. Retur
-000109e0: 6e73 2074 7275 6520 6966 2074 6865 2063  ns true if the c
-000109f0: 6f6d 6d69 7420 696e 6465 780a 2020 2020  ommit index.    
-00010a00: 2020 2020 6368 616e 6765 6420 2869 6e20      changed (in 
-00010a10: 7768 6963 6820 6361 7365 2074 6865 2063  which case the c
-00010a20: 616c 6c65 7220 7368 6f75 6c64 2063 616c  aller should cal
-00010a30: 6c20 6072 2e62 6361 7374 5f61 7070 656e  l `r.bcast_appen
-00010a40: 6460 292e 0a20 2020 2020 2020 2022 2222  d`)..        """
-00010a50: 0a20 2020 2064 6566 2075 6e63 6f6d 6d69  .    def uncommi
-00010a60: 7474 6564 5f73 697a 6528 7365 6c66 2920  tted_size(self) 
-00010a70: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00010a80: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-00010a90: 726e 2063 7572 7265 6e74 2075 6e63 6f6d  rn current uncom
-00010aa0: 6d69 7474 6564 2073 697a 6520 7265 636f  mitted size reco
-00010ab0: 7264 6564 2062 7920 756e 636f 6d6d 6974  rded by uncommit
-00010ac0: 7465 645f 7374 6174 650a 2020 2020 2020  ted_state.      
-00010ad0: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
-00010ae0: 7962 655f 696e 6372 6561 7365 5f75 6e63  ybe_increase_unc
-00010af0: 6f6d 6d69 7474 6564 5f73 697a 6528 0a20  ommitted_size(. 
-00010b00: 2020 2020 2020 2073 656c 662c 2065 6e74         self, ent
-00010b10: 733a 204c 6973 745b 2245 6e74 7279 225d  s: List["Entry"]
-00010b20: 207c 204c 6973 745b 2245 6e74 7279 5265   | List["EntryRe
-00010b30: 6622 5d0a 2020 2020 2920 2d3e 2062 6f6f  f"].    ) -> boo
-00010b40: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-00010b50: 2020 2020 2020 2049 6e63 7265 6173 6520         Increase 
-00010b60: 7369 7a65 206f 6620 2765 6e74 7327 2074  size of 'ents' t
-00010b70: 6f20 756e 636f 6d6d 6974 7465 6420 7369  o uncommitted si
-00010b80: 7a65 2e20 5265 7475 726e 2074 7275 6520  ze. Return true 
-00010b90: 7768 656e 2073 697a 6520 6c69 6d69 740a  when size limit.
-00010ba0: 2020 2020 2020 2020 6973 2073 6174 6973          is satis
-00010bb0: 6669 6564 2e20 4f74 6865 7277 6973 6520  fied. Otherwise 
-00010bc0: 7265 7475 726e 2066 616c 7365 2061 6e64  return false and
-00010bd0: 2075 6e63 6f6d 6d69 7474 6564 2073 697a   uncommitted siz
-00010be0: 6520 7265 6d61 696e 7320 756e 6368 616e  e remains unchan
-00010bf0: 6765 642e 0a20 2020 2020 2020 2046 6f72  ged..        For
-00010c00: 2072 6166 7420 7769 7468 206e 6f20 6c69   raft with no li
-00010c10: 6d69 7428 6f72 206e 6f6e 2d6c 6561 6465  mit(or non-leade
-00010c20: 7220 7261 6674 292c 2069 7420 616c 7761  r raft), it alwa
-00010c30: 7973 2072 6574 7572 6e20 7472 7565 2e0a  ys return true..
-00010c40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010c50: 6465 6620 7265 6475 6365 5f75 6e63 6f6d  def reduce_uncom
-00010c60: 6d69 7474 6564 5f73 697a 6528 7365 6c66  mitted_size(self
-00010c70: 2c20 656e 7473 3a20 4c69 7374 5b22 456e  , ents: List["En
-00010c80: 7472 7922 5d20 7c20 4c69 7374 5b22 456e  try"] | List["En
-00010c90: 7472 7952 6566 225d 2920 2d3e 204e 6f6e  tryRef"]) -> Non
-00010ca0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00010cb0: 2020 2020 2020 2052 6564 7563 6520 7369         Reduce si
-00010cc0: 7a65 206f 6620 2765 6e74 7327 2066 726f  ze of 'ents' fro
-00010cd0: 6d20 756e 636f 6d6d 6974 7465 6420 7369  m uncommitted si
-00010ce0: 7a65 2e0a 2020 2020 2020 2020 2222 220a  ze..        """.
-00010cf0: 2020 2020 6465 6620 6263 6173 745f 6170      def bcast_ap
-00010d00: 7065 6e64 2873 656c 6629 202d 3e20 4e6f  pend(self) -> No
-00010d10: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00010d20: 2020 2020 2020 2020 5365 6e64 7320 5250          Sends RP
-00010d30: 432c 2077 6974 6820 656e 7472 6965 7320  C, with entries 
-00010d40: 746f 2061 6c6c 2070 6565 7273 2074 6861  to all peers tha
-00010d50: 7420 6172 6520 6e6f 7420 7570 2d74 6f2d  t are not up-to-
-00010d60: 6461 7465 0a20 2020 2020 2020 2061 6363  date.        acc
-00010d70: 6f72 6469 6e67 2074 6f20 7468 6520 7072  ording to the pr
-00010d80: 6f67 7265 7373 2072 6563 6f72 6465 6420  ogress recorded 
-00010d90: 696e 2072 2e70 7273 2829 2e0a 2020 2020  in r.prs()..    
-00010da0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00010db0: 6263 6173 745f 6865 6172 7462 6561 7428  bcast_heartbeat(
-00010dc0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00010dd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010de0: 2020 2053 656e 6473 2052 5043 2c20 7769     Sends RPC, wi
-00010df0: 7468 6f75 7420 656e 7472 6965 7320 746f  thout entries to
-00010e00: 2061 6c6c 2074 6865 2070 6565 7273 2e0a   all the peers..
-00010e10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010e20: 6465 6620 7368 6f75 6c64 5f62 6361 7374  def should_bcast
-00010e30: 5f63 6f6d 6d69 7428 7365 6c66 2920 2d3e  _commit(self) ->
-00010e40: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00010e50: 2222 0a20 2020 2020 2020 2053 7065 6369  "".        Speci
-00010e60: 6669 6573 2069 6620 7468 6520 636f 6d6d  fies if the comm
-00010e70: 6974 2073 686f 756c 6420 6265 2062 726f  it should be bro
-00010e80: 6164 6361 7374 2e0a 2020 2020 2020 2020  adcast..        
-00010e90: 2222 220a 2020 2020 6465 6620 736b 6970  """.    def skip
-00010ea0: 5f62 6361 7374 5f63 6f6d 6d69 7428 7365  _bcast_commit(se
-00010eb0: 6c66 2c20 736b 6970 3a20 626f 6f6c 2920  lf, skip: bool) 
-00010ec0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00010ed0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
-00010ee0: 2077 6865 7468 6572 2073 6b69 7020 6272   whether skip br
-00010ef0: 6f61 6463 6173 7420 656d 7074 7920 636f  oadcast empty co
-00010f00: 6d6d 6974 206d 6573 7361 6765 7320 6174  mmit messages at
-00010f10: 2072 756e 7469 6d65 2e0a 2020 2020 2020   runtime..      
-00010f20: 2020 2222 220a 2020 2020 6465 6620 6265    """.    def be
-00010f30: 636f 6d65 5f6c 6561 6465 7228 7365 6c66  come_leader(self
-00010f40: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00010f50: 2020 2022 2222 0a20 2020 2020 2020 204d     """.        M
-00010f60: 616b 6573 2074 6869 7320 7261 6674 2074  akes this raft t
-00010f70: 6865 206c 6561 6465 722e 0a0a 2020 2020  he leader...    
-00010f80: 2020 2020 2320 5061 6e69 6373 0a0a 2020      # Panics..  
-00010f90: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
-00010fa0: 7468 6973 2069 7320 6120 666f 6c6c 6f77  this is a follow
-00010fb0: 6572 206e 6f64 652e 0a20 2020 2020 2020  er node..       
-00010fc0: 2022 2222 0a20 2020 2064 6566 2062 6563   """.    def bec
-00010fd0: 6f6d 655f 666f 6c6c 6f77 6572 2873 656c  ome_follower(sel
-00010fe0: 662c 2074 6572 6d3a 2069 6e74 2c20 6c65  f, term: int, le
-00010ff0: 6164 6572 5f69 643a 2069 6e74 2920 2d3e  ader_id: int) ->
-00011000: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00011010: 2222 0a20 2020 2020 2020 2043 6f6e 7665  "".        Conve
-00011020: 7274 7320 7468 6973 206e 6f64 6520 746f  rts this node to
-00011030: 2061 2066 6f6c 6c6f 7765 722e 0a20 2020   a follower..   
-00011040: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00011050: 2062 6563 6f6d 655f 7072 655f 6361 6e64   become_pre_cand
-00011060: 6964 6174 6528 7365 6c66 2920 2d3e 204e  idate(self) -> N
-00011070: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00011080: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-00011090: 7320 7468 6973 206e 6f64 6520 746f 2061  s this node to a
-000110a0: 2070 7265 2d63 616e 6469 6461 7465 0a0a   pre-candidate..
-000110b0: 2020 2020 2020 2020 2320 5061 6e69 6373          # Panics
-000110c0: 0a0a 2020 2020 2020 2020 5061 6e69 6373  ..        Panics
-000110d0: 2069 6620 6120 6c65 6164 6572 2061 6c72   if a leader alr
-000110e0: 6561 6479 2065 7869 7374 732e 0a20 2020  eady exists..   
-000110f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00011100: 2062 6563 6f6d 655f 6361 6e64 6964 6174   become_candidat
+0000ef10: 2020 2020 2020 436c 6561 7273 2074 6865        Clears the
+0000ef20: 2075 6e73 7461 626c 6520 736e 6170 7368   unstable snapsh
+0000ef30: 6f74 2e0a 2020 2020 2020 2020 2222 220a  ot..        """.
+0000ef40: 2020 2020 6465 6620 7465 726d 2873 656c      def term(sel
+0000ef50: 662c 2069 6478 3a20 696e 7429 202d 3e20  f, idx: int) -> 
+0000ef60: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+0000ef70: 0a20 2020 2020 2020 2046 6f72 2061 2067  .        For a g
+0000ef80: 6976 656e 2069 6e64 6578 2c20 6669 6e64  iven index, find
+0000ef90: 7320 7468 6520 7465 726d 2061 7373 6f63  s the term assoc
+0000efa0: 6961 7465 6420 7769 7468 2069 742e 0a20  iated with it.. 
+0000efb0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000efc0: 6566 206c 6173 745f 7465 726d 2873 656c  ef last_term(sel
+0000efd0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+0000efe0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+0000eff0: 7261 6273 2074 6865 2074 6572 6d20 6672  rabs the term fr
+0000f000: 6f6d 2074 6865 206c 6173 7420 656e 7472  om the last entr
+0000f010: 792e 0a0a 2020 2020 2020 2020 2320 5061  y...        # Pa
+0000f020: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
+0000f030: 6e69 6373 2069 6620 7468 6572 6520 6172  nics if there ar
+0000f040: 6520 656e 7472 6965 7320 6275 7420 7468  e entries but th
+0000f050: 6520 6c61 7374 2074 6572 6d20 6861 7320  e last term has 
+0000f060: 6265 656e 2064 6973 6361 7264 6564 2e0a  been discarded..
+0000f070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f080: 6465 6620 6d61 7463 685f 7465 726d 2873  def match_term(s
+0000f090: 656c 662c 2069 6478 3a20 696e 742c 2074  elf, idx: int, t
+0000f0a0: 6572 6d3a 2069 6e74 2920 2d3e 2062 6f6f  erm: int) -> boo
+0000f0b0: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+0000f0c0: 2020 2020 2020 2041 6e73 7765 7273 2074         Answers t
+0000f0d0: 6865 2071 7565 7374 696f 6e3a 2044 6f65  he question: Doe
+0000f0e0: 7320 7468 6973 2069 6e64 6578 2062 656c  s this index bel
+0000f0f0: 6f6e 6720 746f 2074 6869 7320 7465 726d  ong to this term
+0000f100: 3f0a 2020 2020 2020 2020 2222 220a 2020  ?.        """.  
+0000f110: 2020 6465 6620 6669 7273 745f 696e 6465    def first_inde
+0000f120: 7828 7365 6c66 2920 2d3e 2069 6e74 3a0a  x(self) -> int:.
+0000f130: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f140: 2020 2020 5265 7475 726e 7320 7468 2066      Returns th f
+0000f150: 6972 7374 2069 6e64 6578 2069 6e20 7468  irst index in th
+0000f160: 6520 7374 6f72 6520 7468 6174 2069 7320  e store that is 
+0000f170: 6176 6169 6c61 626c 6520 7669 6120 656e  available via en
+0000f180: 7472 6965 730a 0a20 2020 2020 2020 2023  tries..        #
+0000f190: 2050 616e 6963 730a 0a20 2020 2020 2020   Panics..       
+0000f1a0: 2050 616e 6963 7320 6966 2074 6865 2073   Panics if the s
+0000f1b0: 746f 7265 2064 6f65 736e 2774 2068 6176  tore doesn't hav
+0000f1c0: 6520 6120 6669 7273 7420 696e 6465 782e  e a first index.
+0000f1d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f1e0: 2064 6566 206c 6173 745f 696e 6465 7828   def last_index(
+0000f1f0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+0000f200: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f210: 2020 5265 7475 726e 7320 7468 6520 6c61    Returns the la
+0000f220: 7374 2069 6e64 6578 2069 6e20 7468 6520  st index in the 
+0000f230: 7374 6f72 6520 7468 6174 2069 7320 6176  store that is av
+0000f240: 6169 6c61 626c 6520 7669 6120 656e 7472  ailable via entr
+0000f250: 6965 732e 0a0a 2020 2020 2020 2020 2320  ies...        # 
+0000f260: 5061 6e69 6373 0a0a 2020 2020 2020 2020  Panics..        
+0000f270: 5061 6e69 6373 2069 6620 7468 6520 7374  Panics if the st
+0000f280: 6f72 6520 646f 6573 6e27 7420 6861 7665  ore doesn't have
+0000f290: 2061 206c 6173 7420 696e 6465 782e 0a20   a last index.. 
+0000f2a0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000f2b0: 6566 2075 6e73 7461 626c 6528 7365 6c66  ef unstable(self
+0000f2c0: 2920 2d3e 2022 556e 7374 6162 6c65 5265  ) -> "UnstableRe
+0000f2d0: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
+0000f2e0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+0000f2f0: 6120 7265 6665 7265 6e63 6520 746f 2074  a reference to t
+0000f300: 6865 2075 6e73 7461 626c 6520 6c6f 672e  he unstable log.
+0000f310: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f320: 2064 6566 2075 6e73 7461 626c 655f 656e   def unstable_en
+0000f330: 7472 6965 7328 7365 6c66 2920 2d3e 204c  tries(self) -> L
+0000f340: 6973 745b 2245 6e74 7279 5265 6622 5d3a  ist["EntryRef"]:
+0000f350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f360: 2020 2020 2052 6574 7572 6e73 2073 6c69       Returns sli
+0000f370: 6365 206f 6620 656e 7472 6965 7320 7468  ce of entries th
+0000f380: 6174 2061 7265 206e 6f74 2070 6572 7369  at are not persi
+0000f390: 7374 6564 2e0a 2020 2020 2020 2020 2222  sted..        ""
+0000f3a0: 220a 2020 2020 6465 6620 756e 7374 6162  ".    def unstab
+0000f3b0: 6c65 5f73 6e61 7073 686f 7428 7365 6c66  le_snapshot(self
+0000f3c0: 2920 2d3e 204f 7074 696f 6e61 6c5b 2253  ) -> Optional["S
+0000f3d0: 6e61 7073 686f 7452 6566 225d 3a0a 2020  napshotRef"]:.  
+0000f3e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f3f0: 2020 5265 7475 726e 7320 7468 6520 736e    Returns the sn
+0000f400: 6170 7368 6f74 2074 6861 7420 6172 6520  apshot that are 
+0000f410: 6e6f 7420 7065 7273 6973 7465 642e 0a20  not persisted.. 
+0000f420: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000f430: 6566 2067 6574 5f61 7070 6c69 6564 2873  ef get_applied(s
+0000f440: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0000f450: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f460: 2060 6170 706c 6965 6460 3a20 5468 6520   `applied`: The 
+0000f470: 6869 6768 6573 7420 6c6f 6720 706f 7369  highest log posi
+0000f480: 7469 6f6e 2074 6861 7420 7468 6520 6170  tion that the ap
+0000f490: 706c 6963 6174 696f 6e20 6861 7320 6265  plication has be
+0000f4a0: 656e 2069 6e73 7472 7563 7465 640a 2020  en instructed.  
+0000f4b0: 2020 2020 2020 746f 2061 7070 6c79 2074        to apply t
+0000f4c0: 6f20 6974 7320 7374 6174 6520 6d61 6368  o its state mach
+0000f4d0: 696e 652e 0a0a 2020 2020 2020 2020 496e  ine...        In
+0000f4e0: 7661 7269 616e 743a 2061 7070 6c69 6564  variant: applied
+0000f4f0: 203c 3d20 6d69 6e28 636f 6d6d 6974 7465   <= min(committe
+0000f500: 642c 2070 6572 7369 7374 6564 290a 2020  d, persisted).  
+0000f510: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+0000f520: 6620 7365 745f 6170 706c 6965 6428 7365  f set_applied(se
+0000f530: 6c66 2c20 6170 706c 6965 643a 2069 6e74  lf, applied: int
+0000f540: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000f550: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+0000f560: 6170 706c 6965 6460 3a20 5468 6520 6869  applied`: The hi
+0000f570: 6768 6573 7420 6c6f 6720 706f 7369 7469  ghest log positi
+0000f580: 6f6e 2074 6861 7420 7468 6520 6170 706c  on that the appl
+0000f590: 6963 6174 696f 6e20 6861 7320 6265 656e  ication has been
+0000f5a0: 2069 6e73 7472 7563 7465 640a 2020 2020   instructed.    
+0000f5b0: 2020 2020 746f 2061 7070 6c79 2074 6f20      to apply to 
+0000f5c0: 6974 7320 7374 6174 6520 6d61 6368 696e  its state machin
+0000f5d0: 652e 0a0a 2020 2020 2020 2020 496e 7661  e...        Inva
+0000f5e0: 7269 616e 743a 2061 7070 6c69 6564 203c  riant: applied <
+0000f5f0: 3d20 6d69 6e28 636f 6d6d 6974 7465 642c  = min(committed,
+0000f600: 2070 6572 7369 7374 6564 290a 2020 2020   persisted).    
+0000f610: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000f620: 6765 745f 636f 6d6d 6974 7465 6428 7365  get_committed(se
+0000f630: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+0000f640: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f650: 6063 6f6d 6d69 7474 6564 603a 2054 6865  `committed`: The
+0000f660: 2068 6967 6865 7374 206c 6f67 2070 6f73   highest log pos
+0000f670: 6974 696f 6e20 7468 6174 2069 7320 6b6e  ition that is kn
+0000f680: 6f77 6e20 746f 2062 6520 696e 2073 7461  own to be in sta
+0000f690: 626c 6520 7374 6f72 6167 650a 2020 2020  ble storage.    
+0000f6a0: 2020 2020 6f6e 2061 2071 756f 7275 6d20      on a quorum 
+0000f6b0: 6f66 206e 6f64 6573 2e0a 0a20 2020 2020  of nodes...     
+0000f6c0: 2020 2049 6e76 6172 6961 6e74 3a20 6170     Invariant: ap
+0000f6d0: 706c 6965 6420 3c3d 2063 6f6d 6d69 7474  plied <= committ
+0000f6e0: 6564 0a20 2020 2020 2020 2022 2222 0a20  ed.        """. 
+0000f6f0: 2020 2064 6566 2073 6574 5f63 6f6d 6d69     def set_commi
+0000f700: 7474 6564 2873 656c 662c 2063 6f6d 6d69  tted(self, commi
+0000f710: 7474 6564 3a20 696e 7429 202d 3e20 4e6f  tted: int) -> No
+0000f720: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+0000f730: 2020 2020 2020 2020 6063 6f6d 6d69 7474          `committ
+0000f740: 6564 603a 2054 6865 2068 6967 6865 7374  ed`: The highest
+0000f750: 206c 6f67 2070 6f73 6974 696f 6e20 7468   log position th
+0000f760: 6174 2069 7320 6b6e 6f77 6e20 746f 2062  at is known to b
+0000f770: 6520 696e 2073 7461 626c 6520 7374 6f72  e in stable stor
+0000f780: 6167 650a 2020 2020 2020 2020 6f6e 2061  age.        on a
+0000f790: 2071 756f 7275 6d20 6f66 206e 6f64 6573   quorum of nodes
+0000f7a0: 2e0a 0a20 2020 2020 2020 2049 6e76 6172  ...        Invar
+0000f7b0: 6961 6e74 3a20 6170 706c 6965 6420 3c3d  iant: applied <=
+0000f7c0: 2063 6f6d 6d69 7474 6564 0a20 2020 2020   committed.     
+0000f7d0: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+0000f7e0: 6574 5f70 6572 7369 7374 6564 2873 656c  et_persisted(sel
+0000f7f0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+0000f800: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+0000f810: 7065 7273 6973 7465 6460 3a20 5468 6520  persisted`: The 
+0000f820: 6869 6768 6573 7420 6c6f 6720 706f 7369  highest log posi
+0000f830: 7469 6f6e 2074 6861 7420 6973 206b 6e6f  tion that is kno
+0000f840: 776e 2074 6f20 6265 2070 6572 7369 7374  wn to be persist
+0000f850: 6564 2069 6e20 7374 6162 6c65 0a20 2020  ed in stable.   
+0000f860: 2020 2020 2073 746f 7261 6765 2e20 4974       storage. It
+0000f870: 2773 2075 7365 6420 666f 7220 6c69 6d69  's used for limi
+0000f880: 7469 6e67 2074 6865 2075 7070 6572 2062  ting the upper b
+0000f890: 6f75 6e64 206f 6620 636f 6d6d 6974 7465  ound of committe
+0000f8a0: 6420 616e 640a 2020 2020 2020 2020 7065  d and.        pe
+0000f8b0: 7273 6973 7465 6420 656e 7472 6965 732e  rsisted entries.
+0000f8c0: 0a0a 2020 2020 2020 2020 496e 7661 7269  ..        Invari
+0000f8d0: 616e 743a 2070 6572 7369 7374 6564 203c  ant: persisted <
+0000f8e0: 2075 6e73 7461 626c 652e 6f66 6673 6574   unstable.offset
+0000f8f0: 2026 2620 6170 706c 6965 6420 3c3d 2070   && applied <= p
+0000f900: 6572 7369 7374 6564 0a20 2020 2020 2020  ersisted.       
+0000f910: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+0000f920: 5f70 6572 7369 7374 6564 2873 656c 662c  _persisted(self,
+0000f930: 2070 6572 7369 7374 6564 3a20 696e 7429   persisted: int)
+0000f940: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000f950: 2020 2222 220a 2020 2020 2020 2020 6070    """.        `p
+0000f960: 6572 7369 7374 6564 603a 2054 6865 2068  ersisted`: The h
+0000f970: 6967 6865 7374 206c 6f67 2070 6f73 6974  ighest log posit
+0000f980: 696f 6e20 7468 6174 2069 7320 6b6e 6f77  ion that is know
+0000f990: 6e20 746f 2062 6520 7065 7273 6973 7465  n to be persiste
+0000f9a0: 6420 696e 2073 7461 626c 650a 2020 2020  d in stable.    
+0000f9b0: 2020 2020 7374 6f72 6167 652e 2049 7427      storage. It'
+0000f9c0: 7320 7573 6564 2066 6f72 206c 696d 6974  s used for limit
+0000f9d0: 696e 6720 7468 6520 7570 7065 7220 626f  ing the upper bo
+0000f9e0: 756e 6420 6f66 2063 6f6d 6d69 7474 6564  und of committed
+0000f9f0: 2061 6e64 0a20 2020 2020 2020 2070 6572   and.        per
+0000fa00: 7369 7374 6564 2065 6e74 7269 6573 2e0a  sisted entries..
+0000fa10: 0a20 2020 2020 2020 2049 6e76 6172 6961  .        Invaria
+0000fa20: 6e74 3a20 7065 7273 6973 7465 6420 3c20  nt: persisted < 
+0000fa30: 756e 7374 6162 6c65 2e6f 6666 7365 7420  unstable.offset 
+0000fa40: 2626 2061 7070 6c69 6564 203c 3d20 7065  && applied <= pe
+0000fa50: 7273 6973 7465 640a 2020 2020 2020 2020  rsisted.        
+0000fa60: 2222 220a 2020 2020 6465 6620 736c 6963  """.    def slic
+0000fa70: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
+0000fa80: 0a20 2020 2020 2020 206c 6f77 3a20 696e  .        low: in
+0000fa90: 742c 0a20 2020 2020 2020 2068 6967 683a  t,.        high:
+0000faa0: 2069 6e74 2c0a 2020 2020 2020 2020 6d61   int,.        ma
+0000fab0: 785f 7369 7a65 3a20 4f70 7469 6f6e 616c  x_size: Optional
+0000fac0: 5b69 6e74 5d2c 0a20 2020 2020 2020 2063  [int],.        c
+0000fad0: 6f6e 7465 7874 3a20 2247 6574 456e 7472  ontext: "GetEntr
+0000fae0: 6965 7343 6f6e 7465 7874 5265 6622 2c0a  iesContextRef",.
+0000faf0: 2020 2020 2920 2d3e 204c 6973 745b 2245      ) -> List["E
+0000fb00: 6e74 7279 5265 6622 5d3a 0a20 2020 2020  ntryRef"]:.     
+0000fb10: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+0000fb20: 7261 6273 2061 2073 6c69 6365 206f 6620  rabs a slice of 
+0000fb30: 656e 7472 6965 7320 6672 6f6d 2074 6865  entries from the
+0000fb40: 2072 6166 742e 2055 6e6c 696b 6520 6120   raft. Unlike a 
+0000fb50: 7275 7374 2073 6c69 6365 2070 6f69 6e74  rust slice point
+0000fb60: 6572 2c20 7468 6573 6520 6172 650a 2020  er, these are.  
+0000fb70: 2020 2020 2020 7265 7475 726e 6564 2062        returned b
+0000fb80: 7920 7661 6c75 652e 2054 6865 2072 6573  y value. The res
+0000fb90: 756c 7420 6973 2074 7275 6e63 6174 6564  ult is truncated
+0000fba0: 2074 6f20 7468 6520 6d61 785f 7369 7a65   to the max_size
+0000fbb0: 2069 6e20 6279 7465 732e 0a20 2020 2020   in bytes..     
+0000fbc0: 2020 2022 2222 0a20 2020 2064 6566 2072     """.    def r
+0000fbd0: 6573 746f 7265 2873 656c 662c 2073 6e61  estore(self, sna
+0000fbe0: 7073 686f 743a 2022 536e 6170 7368 6f74  pshot: "Snapshot
+0000fbf0: 2220 7c20 2253 6e61 7073 686f 7452 6566  " | "SnapshotRef
+0000fc00: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
+0000fc10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000fc20: 5265 7374 6f72 6573 2074 6865 2063 7572  Restores the cur
+0000fc30: 7265 6e74 206c 6f67 2066 726f 6d20 6120  rent log from a 
+0000fc40: 736e 6170 7368 6f74 2e0a 2020 2020 2020  snapshot..      
+0000fc50: 2020 2222 220a 0a63 6c61 7373 2049 6e4d    """..class InM
+0000fc60: 656d 6f72 7952 6166 744c 6f67 285f 5f41  emoryRaftLog(__A
+0000fc70: 5049 5f52 6166 744c 6f67 293a 0a20 2020  PI_RaftLog):.   
+0000fc80: 2022 2222 0a20 2020 2052 6166 7420 6c6f   """.    Raft lo
+0000fc90: 6720 696d 706c 656d 656e 7461 7469 6f6e  g implementation
+0000fca0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+0000fcb0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0000fcc0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000fcd0: 2020 7374 6f72 653a 2022 4d65 6d53 746f    store: "MemSto
+0000fce0: 7261 6765 5265 6622 2c0a 2020 2020 2020  rageRef",.      
+0000fcf0: 2020 6c6f 6767 6572 3a20 224c 6f67 6765    logger: "Logge
+0000fd00: 7222 207c 2022 4c6f 6767 6572 5265 6622  r" | "LoggerRef"
+0000fd10: 207c 2022 5468 7265 6164 5361 6665 4c6f   | "ThreadSafeLo
+0000fd20: 6767 6572 222c 0a20 2020 2029 202d 3e20  gger",.    ) -> 
+0000fd30: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000fd40: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+0000fd50: 202d 3e20 2249 6e4d 656d 6f72 7952 6166   -> "InMemoryRaf
+0000fd60: 744c 6f67 5265 6622 3a20 2e2e 2e0a 2020  tLogRef": ....  
+0000fd70: 2020 6465 6620 6765 745f 7374 6f72 6528    def get_store(
+0000fd80: 7365 6c66 2920 2d3e 2022 4d65 6d53 746f  self) -> "MemSto
+0000fd90: 7261 6765 5265 6622 3a0a 2020 2020 2020  rageRef":.      
+0000fda0: 2020 2222 220a 2020 2020 2020 2020 4772    """.        Gr
+0000fdb0: 6162 2061 2072 6561 642d 6f6e 6c79 2072  ab a read-only r
+0000fdc0: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
+0000fdd0: 756e 6465 726c 7969 6e67 2073 746f 7261  underlying stora
+0000fde0: 6765 2e0a 2020 2020 2020 2020 2222 220a  ge..        """.
+0000fdf0: 0a63 6c61 7373 2049 6e4d 656d 6f72 7952  .class InMemoryR
+0000fe00: 6166 744c 6f67 5265 6628 5f5f 4150 495f  aftLogRef(__API_
+0000fe10: 5261 6674 4c6f 6729 3a0a 2020 2020 2222  RaftLog):.    ""
+0000fe20: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
+0000fe30: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
+0000fe40: 496e 4d65 6d6f 7279 5261 6674 4c6f 6760  InMemoryRaftLog`
+0000fe50: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+0000fe60: 6566 2067 6574 5f73 746f 7265 2873 656c  ef get_store(sel
+0000fe70: 6629 202d 3e20 224d 656d 5374 6f72 6167  f) -> "MemStorag
+0000fe80: 6552 6566 223a 0a20 2020 2020 2020 2022  eRef":.        "
+0000fe90: 2222 0a20 2020 2020 2020 2047 7261 6220  "".        Grab 
+0000fea0: 6120 7265 6164 2d6f 6e6c 7920 7265 6665  a read-only refe
+0000feb0: 7265 6e63 6520 746f 2074 6865 2075 6e64  rence to the und
+0000fec0: 6572 6c79 696e 6720 7374 6f72 6167 652e  erlying storage.
+0000fed0: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+0000fee0: 6173 7320 5261 6674 4c6f 6728 5f5f 4150  ass RaftLog(__AP
+0000fef0: 495f 5261 6674 4c6f 6729 3a0a 2020 2020  I_RaftLog):.    
+0000ff00: 2222 2220 2222 220a 0a20 2020 2064 6566  """ """..    def
+0000ff10: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0000ff20: 2020 2073 656c 662c 2073 746f 7265 3a20     self, store: 
+0000ff30: 2253 746f 7261 6765 5265 6622 2c20 6c6f  "StorageRef", lo
+0000ff40: 6767 6572 3a20 224c 6f67 6765 7222 207c  gger: "Logger" |
+0000ff50: 2022 4c6f 6767 6572 5265 6622 207c 2022   "LoggerRef" | "
+0000ff60: 5468 7265 6164 5361 6665 4c6f 6767 6572  ThreadSafeLogger
+0000ff70: 220a 2020 2020 2920 2d3e 204e 6f6e 653a  ".    ) -> None:
+0000ff80: 202e 2e2e 0a20 2020 2064 6566 206d 616b   ....    def mak
+0000ff90: 655f 7265 6628 7365 6c66 2920 2d3e 2022  e_ref(self) -> "
+0000ffa0: 5261 6674 4c6f 6752 6566 223a 202e 2e2e  RaftLogRef": ...
+0000ffb0: 0a20 2020 2064 6566 2067 6574 5f73 746f  .    def get_sto
+0000ffc0: 7265 2873 656c 6629 202d 3e20 2253 746f  re(self) -> "Sto
+0000ffd0: 7261 6765 5265 6622 3a0a 2020 2020 2020  rageRef":.      
+0000ffe0: 2020 2222 220a 2020 2020 2020 2020 4772    """.        Gr
+0000fff0: 6162 2061 2072 6561 642d 6f6e 6c79 2072  ab a read-only r
+00010000: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
+00010010: 756e 6465 726c 7969 6e67 2073 746f 7261  underlying stora
+00010020: 6765 2e0a 2020 2020 2020 2020 2222 220a  ge..        """.
+00010030: 0a63 6c61 7373 2052 6166 744c 6f67 5265  .class RaftLogRe
+00010040: 6628 5f5f 4150 495f 5261 6674 4c6f 6729  f(__API_RaftLog)
+00010050: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+00010060: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
+00010070: 3a63 6c61 7373 3a60 5261 6674 4c6f 6760  :class:`RaftLog`
+00010080: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00010090: 6566 2067 6574 5f73 746f 7265 2873 656c  ef get_store(sel
+000100a0: 6629 202d 3e20 2253 746f 7261 6765 5265  f) -> "StorageRe
+000100b0: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
+000100c0: 2020 2020 2020 2020 4772 6162 2061 2072          Grab a r
+000100d0: 6561 642d 6f6e 6c79 2072 6566 6572 656e  ead-only referen
+000100e0: 6365 2074 6f20 7468 6520 756e 6465 726c  ce to the underl
+000100f0: 7969 6e67 2073 746f 7261 6765 2e0a 2020  ying storage..  
+00010100: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
+00010110: 205f 5f41 5049 5f52 6166 743a 0a20 2020   __API_Raft:.   
+00010120: 2064 6566 2061 7070 656e 645f 656e 7472   def append_entr
+00010130: 7928 7365 6c66 2c20 656e 7473 3a20 4c69  y(self, ents: Li
+00010140: 7374 5b22 456e 7472 7922 5d20 7c20 4c69  st["Entry"] | Li
+00010150: 7374 5b22 456e 7472 7952 6566 225d 2920  st["EntryRef"]) 
+00010160: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00010170: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
+00010180: 656e 6473 2061 2073 6c69 6365 206f 6620  ends a slice of 
+00010190: 656e 7472 6965 7320 746f 2074 6865 206c  entries to the l
+000101a0: 6f67 2e0a 2020 2020 2020 2020 5468 6520  og..        The 
+000101b0: 656e 7472 6965 7320 6172 6520 7570 6461  entries are upda
+000101c0: 7465 6420 746f 206d 6174 6368 2074 6865  ted to match the
+000101d0: 2063 7572 7265 6e74 2069 6e64 6578 2061   current index a
+000101e0: 6e64 2074 6572 6d2e 0a20 2020 2020 2020  nd term..       
+000101f0: 204f 6e6c 7920 6361 6c6c 6564 2062 7920   Only called by 
+00010200: 6c65 6164 6572 2063 7572 7265 6e74 6c79  leader currently
+00010210: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010220: 2064 6566 2073 656e 645f 6170 7065 6e64   def send_append
+00010230: 2873 656c 662c 2074 6f3a 2069 6e74 2920  (self, to: int) 
+00010240: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00010250: 2022 2222 0a20 2020 2020 2020 2053 656e   """.        Sen
+00010260: 6473 2061 6e20 6170 7065 6e64 2052 5043  ds an append RPC
+00010270: 2077 6974 6820 6e65 7720 656e 7472 6965   with new entrie
+00010280: 7320 2869 6620 616e 7929 2061 6e64 2074  s (if any) and t
+00010290: 6865 2063 7572 7265 6e74 2063 6f6d 6d69  he current commi
+000102a0: 7420 696e 6465 7820 746f 2074 6865 2067  t index to the g
+000102b0: 6976 656e 0a20 2020 2020 2020 2070 6565  iven.        pee
+000102c0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+000102d0: 2020 2064 6566 206f 6e5f 7065 7273 6973     def on_persis
+000102e0: 745f 656e 7472 6965 7328 7365 6c66 2c20  t_entries(self, 
+000102f0: 696e 6465 783a 2069 6e74 2c20 7465 726d  index: int, term
+00010300: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00010310: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010320: 2020 2020 4e6f 7469 6669 6573 2074 6861      Notifies tha
+00010330: 7420 7468 6573 6520 7261 6674 206c 6f67  t these raft log
+00010340: 7320 6861 7665 2062 6565 6e20 7065 7273  s have been pers
+00010350: 6973 7465 642e 0a20 2020 2020 2020 2022  isted..        "
+00010360: 2222 0a20 2020 2064 6566 2061 7070 6c79  "".    def apply
+00010370: 5f74 6f5f 6375 7272 656e 745f 7465 726d  _to_current_term
+00010380: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+00010390: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000103a0: 2020 2020 4368 6563 6b73 2069 6620 6c6f      Checks if lo
+000103b0: 6773 2061 7265 2061 7070 6c69 6564 2074  gs are applied t
+000103c0: 6f20 6375 7272 656e 7420 7465 726d 2e0a  o current term..
+000103d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000103e0: 6465 6620 636f 6d6d 6974 5f74 6f5f 6375  def commit_to_cu
+000103f0: 7272 656e 745f 7465 726d 2873 656c 6629  rrent_term(self)
+00010400: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00010410: 2020 2222 220a 2020 2020 2020 2020 4368    """.        Ch
+00010420: 6563 6b73 2069 6620 6c6f 6773 2061 7265  ecks if logs are
+00010430: 2063 6f6d 6d69 7474 6564 2074 6f20 6974   committed to it
+00010440: 7320 7465 726d 2e0a 0a20 2020 2020 2020  s term...       
+00010450: 2054 6865 2063 6865 636b 2069 7320 7573   The check is us
+00010460: 6566 756c 2075 7375 616c 6c79 2077 6865  eful usually whe
+00010470: 6e20 7261 6674 2069 7320 6c65 6164 6572  n raft is leader
+00010480: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00010490: 2020 6465 6620 6772 6f75 705f 636f 6d6d    def group_comm
+000104a0: 6974 2873 656c 6629 202d 3e20 626f 6f6c  it(self) -> bool
+000104b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000104c0: 2020 2020 2020 5768 6574 6865 7220 656e        Whether en
+000104d0: 6162 6c65 2067 726f 7570 2063 6f6d 6d69  able group commi
+000104e0: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+000104f0: 2020 2064 6566 2065 6e61 626c 655f 6772     def enable_gr
+00010500: 6f75 705f 636f 6d6d 6974 2873 656c 662c  oup_commit(self,
+00010510: 2065 6e61 626c 653a 2062 6f6f 6c29 202d   enable: bool) -
+00010520: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00010530: 2222 220a 2020 2020 2020 2020 436f 6e66  """.        Conf
+00010540: 6967 7572 6573 2067 726f 7570 2063 6f6d  igures group com
+00010550: 6d69 742e 0a0a 2020 2020 2020 2020 4966  mit...        If
+00010560: 2067 726f 7570 2063 6f6d 6d69 7420 6973   group commit is
+00010570: 2065 6e61 626c 6564 2c20 6f6e 6c79 206c   enabled, only l
+00010580: 6f67 7320 7265 706c 6963 6174 6564 2074  ogs replicated t
+00010590: 6f20 6174 206c 6561 7374 2074 776f 0a20  o at least two. 
+000105a0: 2020 2020 2020 2064 6966 6665 7265 6e74         different
+000105b0: 2067 726f 7570 7320 6172 6520 636f 6d6d   groups are comm
+000105c0: 6974 7465 642e 0a0a 2020 2020 2020 2020  itted...        
+000105d0: 596f 7520 7368 6f75 6c64 2075 7365 2060  You should use `
+000105e0: 6173 7369 676e 5f63 6f6d 6d69 745f 6772  assign_commit_gr
+000105f0: 6f75 7073 6020 746f 2063 6f6e 6669 6775  oups` to configu
+00010600: 7265 2070 6565 7220 6772 6f75 7073 2e0a  re peer groups..
+00010610: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010620: 6465 6620 636c 6561 725f 636f 6d6d 6974  def clear_commit
+00010630: 5f67 726f 7570 2873 656c 6629 202d 3e20  _group(self) -> 
+00010640: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00010650: 220a 2020 2020 2020 2020 5265 6d6f 7665  ".        Remove
+00010660: 7320 616c 6c20 636f 6d6d 6974 2067 726f  s all commit gro
+00010670: 7570 2063 6f6e 6669 6775 7261 7469 6f6e  up configuration
+00010680: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00010690: 2020 2064 6566 2063 6865 636b 5f67 726f     def check_gro
+000106a0: 7570 5f63 6f6d 6d69 745f 636f 6e73 6973  up_commit_consis
+000106b0: 7465 6e74 2873 656c 6629 202d 3e20 4f70  tent(self) -> Op
+000106c0: 7469 6f6e 616c 5b62 6f6f 6c5d 3a0a 2020  tional[bool]:.  
+000106d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000106e0: 2020 4368 6563 6b73 2077 6865 7468 6572    Checks whether
+000106f0: 2074 6865 2072 6166 7420 6772 6f75 7020   the raft group 
+00010700: 6973 2075 7369 6e67 2067 726f 7570 2063  is using group c
+00010710: 6f6d 6d69 7420 616e 6420 636f 6e73 6973  ommit and consis
+00010720: 7465 6e74 0a20 2020 2020 2020 206f 7665  tent.        ove
+00010730: 7220 6772 6f75 702e 0a0a 2020 2020 2020  r group...      
+00010740: 2020 4966 2069 7420 6361 6e27 7420 6765    If it can't ge
+00010750: 7420 6120 636f 7272 6563 7420 616e 7377  t a correct answ
+00010760: 6572 2c20 604e 6f6e 6560 2069 7320 7265  er, `None` is re
+00010770: 7475 726e 6564 2e0a 2020 2020 2020 2020  turned..        
+00010780: 2222 220a 2020 2020 6465 6620 6173 7369  """.    def assi
+00010790: 676e 5f63 6f6d 6d69 745f 6772 6f75 7073  gn_commit_groups
+000107a0: 2873 656c 662c 2069 6473 3a20 4c69 7374  (self, ids: List
+000107b0: 5b54 7570 6c65 5b69 6e74 2c20 696e 745d  [Tuple[int, int]
+000107c0: 5d29 202d 3e20 4e6f 6e65 3a0a 2020 2020  ]) -> None:.    
+000107d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000107e0: 4173 7369 676e 7320 6772 6f75 7073 2074  Assigns groups t
+000107f0: 6f20 7065 6572 732e 0a0a 2020 2020 2020  o peers...      
+00010800: 2020 5468 6520 7475 706c 6520 6973 2028    The tuple is (
+00010810: 6070 6565 725f 6964 602c 2060 6772 6f75  `peer_id`, `grou
+00010820: 705f 6964 6029 2e20 6067 726f 7570 5f69  p_id`). `group_i
+00010830: 6460 2073 686f 756c 6420 6265 206c 6172  d` should be lar
+00010840: 6765 7220 7468 616e 2030 2e0a 0a20 2020  ger than 0...   
+00010850: 2020 2020 2054 6865 2067 726f 7570 2069       The group i
+00010860: 6e66 6f72 6d61 7469 6f6e 2069 7320 6f6e  nformation is on
+00010870: 6c79 2073 746f 7265 6420 696e 206d 656d  ly stored in mem
+00010880: 6f72 792e 2053 6f20 796f 7520 6e65 6564  ory. So you need
+00010890: 2074 6f20 636f 6e66 6967 7572 650a 2020   to configure.  
+000108a0: 2020 2020 2020 6974 2065 7665 7279 2074        it every t
+000108b0: 696d 6520 6120 7261 6674 2073 7461 7465  ime a raft state
+000108c0: 206d 6163 6869 6e65 2069 7320 696e 6974   machine is init
+000108d0: 6961 6c69 7a65 6420 6f72 2061 2073 6e61  ialized or a sna
+000108e0: 7073 686f 7420 6973 2061 7070 6c69 6564  pshot is applied
+000108f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00010900: 2020 6465 6620 636f 6d6d 6974 5f61 7070    def commit_app
+00010910: 6c79 2873 656c 662c 2061 7070 6c69 6564  ly(self, applied
+00010920: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00010930: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010940: 2020 2020 436f 6d6d 6974 2074 6861 7420      Commit that 
+00010950: 7468 6520 5261 6674 2070 6565 7220 6861  the Raft peer ha
+00010960: 7320 6170 706c 6965 6420 7570 2074 6f20  s applied up to 
+00010970: 7468 6520 6769 7665 6e20 696e 6465 782e  the given index.
+00010980: 0a0a 2020 2020 2020 2020 5265 6769 7374  ..        Regist
+00010990: 6572 7320 7468 6520 6e65 7720 6170 706c  ers the new appl
+000109a0: 6965 6420 696e 6465 7820 746f 2074 6865  ied index to the
+000109b0: 2052 6166 7420 6c6f 672e 0a0a 2020 2020   Raft log...    
+000109c0: 2020 2020 2320 486f 6f6b 730a 0a20 2020      # Hooks..   
+000109d0: 2020 2020 202a 2050 6f73 743a 2043 6865       * Post: Che
+000109e0: 636b 7320 746f 2073 6565 2069 6620 6974  cks to see if it
+000109f0: 2773 2074 696d 6520 746f 2066 696e 616c  's time to final
+00010a00: 697a 6520 6120 4a6f 696e 7420 436f 6e73  ize a Joint Cons
+00010a10: 656e 7375 7320 7374 6174 652e 0a20 2020  ensus state..   
+00010a20: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00010a30: 206d 6179 6265 5f63 6f6d 6d69 7428 7365   maybe_commit(se
+00010a40: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00010a50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010a60: 2041 7474 656d 7074 7320 746f 2061 6476   Attempts to adv
+00010a70: 616e 6365 2074 6865 2063 6f6d 6d69 7420  ance the commit 
+00010a80: 696e 6465 782e 2052 6574 7572 6e73 2074  index. Returns t
+00010a90: 7275 6520 6966 2074 6865 2063 6f6d 6d69  rue if the commi
+00010aa0: 7420 696e 6465 780a 2020 2020 2020 2020  t index.        
+00010ab0: 6368 616e 6765 6420 2869 6e20 7768 6963  changed (in whic
+00010ac0: 6820 6361 7365 2074 6865 2063 616c 6c65  h case the calle
+00010ad0: 7220 7368 6f75 6c64 2063 616c 6c20 6072  r should call `r
+00010ae0: 2e62 6361 7374 5f61 7070 656e 6460 292e  .bcast_append`).
+00010af0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010b00: 2064 6566 2075 6e63 6f6d 6d69 7474 6564   def uncommitted
+00010b10: 5f73 697a 6528 7365 6c66 2920 2d3e 2069  _size(self) -> i
+00010b20: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+00010b30: 2020 2020 2020 2020 5265 7475 726e 2063          Return c
+00010b40: 7572 7265 6e74 2075 6e63 6f6d 6d69 7474  urrent uncommitt
+00010b50: 6564 2073 697a 6520 7265 636f 7264 6564  ed size recorded
+00010b60: 2062 7920 756e 636f 6d6d 6974 7465 645f   by uncommitted_
+00010b70: 7374 6174 650a 2020 2020 2020 2020 2222  state.        ""
+00010b80: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
+00010b90: 696e 6372 6561 7365 5f75 6e63 6f6d 6d69  increase_uncommi
+00010ba0: 7474 6564 5f73 697a 6528 0a20 2020 2020  tted_size(.     
+00010bb0: 2020 2073 656c 662c 2065 6e74 733a 204c     self, ents: L
+00010bc0: 6973 745b 2245 6e74 7279 225d 207c 204c  ist["Entry"] | L
+00010bd0: 6973 745b 2245 6e74 7279 5265 6622 5d0a  ist["EntryRef"].
+00010be0: 2020 2020 2920 2d3e 2062 6f6f 6c3a 0a20      ) -> bool:. 
+00010bf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010c00: 2020 2049 6e63 7265 6173 6520 7369 7a65     Increase size
+00010c10: 206f 6620 2765 6e74 7327 2074 6f20 756e   of 'ents' to un
+00010c20: 636f 6d6d 6974 7465 6420 7369 7a65 2e20  committed size. 
+00010c30: 5265 7475 726e 2074 7275 6520 7768 656e  Return true when
+00010c40: 2073 697a 6520 6c69 6d69 740a 2020 2020   size limit.    
+00010c50: 2020 2020 6973 2073 6174 6973 6669 6564      is satisfied
+00010c60: 2e20 4f74 6865 7277 6973 6520 7265 7475  . Otherwise retu
+00010c70: 726e 2066 616c 7365 2061 6e64 2075 6e63  rn false and unc
+00010c80: 6f6d 6d69 7474 6564 2073 697a 6520 7265  ommitted size re
+00010c90: 6d61 696e 7320 756e 6368 616e 6765 642e  mains unchanged.
+00010ca0: 0a20 2020 2020 2020 2046 6f72 2072 6166  .        For raf
+00010cb0: 7420 7769 7468 206e 6f20 6c69 6d69 7428  t with no limit(
+00010cc0: 6f72 206e 6f6e 2d6c 6561 6465 7220 7261  or non-leader ra
+00010cd0: 6674 292c 2069 7420 616c 7761 7973 2072  ft), it always r
+00010ce0: 6574 7572 6e20 7472 7565 2e0a 2020 2020  eturn true..    
+00010cf0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00010d00: 7265 6475 6365 5f75 6e63 6f6d 6d69 7474  reduce_uncommitt
+00010d10: 6564 5f73 697a 6528 7365 6c66 2c20 656e  ed_size(self, en
+00010d20: 7473 3a20 4c69 7374 5b22 456e 7472 7922  ts: List["Entry"
+00010d30: 5d20 7c20 4c69 7374 5b22 456e 7472 7952  ] | List["EntryR
+00010d40: 6566 225d 2920 2d3e 204e 6f6e 653a 0a20  ef"]) -> None:. 
+00010d50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010d60: 2020 2052 6564 7563 6520 7369 7a65 206f     Reduce size o
+00010d70: 6620 2765 6e74 7327 2066 726f 6d20 756e  f 'ents' from un
+00010d80: 636f 6d6d 6974 7465 6420 7369 7a65 2e0a  committed size..
+00010d90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010da0: 6465 6620 6263 6173 745f 6170 7065 6e64  def bcast_append
+00010db0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00010dc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010dd0: 2020 2020 5365 6e64 7320 5250 432c 2077      Sends RPC, w
+00010de0: 6974 6820 656e 7472 6965 7320 746f 2061  ith entries to a
+00010df0: 6c6c 2070 6565 7273 2074 6861 7420 6172  ll peers that ar
+00010e00: 6520 6e6f 7420 7570 2d74 6f2d 6461 7465  e not up-to-date
+00010e10: 0a20 2020 2020 2020 2061 6363 6f72 6469  .        accordi
+00010e20: 6e67 2074 6f20 7468 6520 7072 6f67 7265  ng to the progre
+00010e30: 7373 2072 6563 6f72 6465 6420 696e 2072  ss recorded in r
+00010e40: 2e70 7273 2829 2e0a 2020 2020 2020 2020  .prs()..        
+00010e50: 2222 220a 2020 2020 6465 6620 6263 6173  """.    def bcas
+00010e60: 745f 6865 6172 7462 6561 7428 7365 6c66  t_heartbeat(self
+00010e70: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00010e80: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00010e90: 656e 6473 2052 5043 2c20 7769 7468 6f75  ends RPC, withou
+00010ea0: 7420 656e 7472 6965 7320 746f 2061 6c6c  t entries to all
+00010eb0: 2074 6865 2070 6565 7273 2e0a 2020 2020   the peers..    
+00010ec0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00010ed0: 7368 6f75 6c64 5f62 6361 7374 5f63 6f6d  should_bcast_com
+00010ee0: 6d69 7428 7365 6c66 2920 2d3e 2062 6f6f  mit(self) -> boo
+00010ef0: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00010f00: 2020 2020 2020 2053 7065 6369 6669 6573         Specifies
+00010f10: 2069 6620 7468 6520 636f 6d6d 6974 2073   if the commit s
+00010f20: 686f 756c 6420 6265 2062 726f 6164 6361  hould be broadca
+00010f30: 7374 2e0a 2020 2020 2020 2020 2222 220a  st..        """.
+00010f40: 2020 2020 6465 6620 736b 6970 5f62 6361      def skip_bca
+00010f50: 7374 5f63 6f6d 6d69 7428 7365 6c66 2c20  st_commit(self, 
+00010f60: 736b 6970 3a20 626f 6f6c 2920 2d3e 204e  skip: bool) -> N
+00010f70: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00010f80: 0a20 2020 2020 2020 2053 6574 2077 6865  .        Set whe
+00010f90: 7468 6572 2073 6b69 7020 6272 6f61 6463  ther skip broadc
+00010fa0: 6173 7420 656d 7074 7920 636f 6d6d 6974  ast empty commit
+00010fb0: 206d 6573 7361 6765 7320 6174 2072 756e   messages at run
+00010fc0: 7469 6d65 2e0a 2020 2020 2020 2020 2222  time..        ""
+00010fd0: 220a 2020 2020 6465 6620 6265 636f 6d65  ".    def become
+00010fe0: 5f6c 6561 6465 7228 7365 6c66 2920 2d3e  _leader(self) ->
+00010ff0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00011000: 2222 0a20 2020 2020 2020 204d 616b 6573  "".        Makes
+00011010: 2074 6869 7320 7261 6674 2074 6865 206c   this raft the l
+00011020: 6561 6465 722e 0a0a 2020 2020 2020 2020  eader...        
+00011030: 2320 5061 6e69 6373 0a0a 2020 2020 2020  # Panics..      
+00011040: 2020 5061 6e69 6373 2069 6620 7468 6973    Panics if this
+00011050: 2069 7320 6120 666f 6c6c 6f77 6572 206e   is a follower n
+00011060: 6f64 652e 0a20 2020 2020 2020 2022 2222  ode..        """
+00011070: 0a20 2020 2064 6566 2062 6563 6f6d 655f  .    def become_
+00011080: 666f 6c6c 6f77 6572 2873 656c 662c 2074  follower(self, t
+00011090: 6572 6d3a 2069 6e74 2c20 6c65 6164 6572  erm: int, leader
+000110a0: 5f69 643a 2069 6e74 2920 2d3e 204e 6f6e  _id: int) -> Non
+000110b0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000110c0: 2020 2020 2020 2043 6f6e 7665 7274 7320         Converts 
+000110d0: 7468 6973 206e 6f64 6520 746f 2061 2066  this node to a f
+000110e0: 6f6c 6c6f 7765 722e 0a20 2020 2020 2020  ollower..       
+000110f0: 2022 2222 0a20 2020 2064 6566 2062 6563   """.    def bec
+00011100: 6f6d 655f 7072 655f 6361 6e64 6964 6174  ome_pre_candidat
 00011110: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
 00011120: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
 00011130: 2020 2020 2043 6f6e 7665 7274 7320 7468       Converts th
-00011140: 6973 206e 6f64 6520 746f 2061 2063 616e  is node to a can
-00011150: 6469 6461 7465 0a0a 2020 2020 2020 2020  didate..        
-00011160: 2320 5061 6e69 6373 0a0a 2020 2020 2020  # Panics..      
-00011170: 2020 5061 6e69 6373 2069 6620 6120 6c65    Panics if a le
-00011180: 6164 6572 2061 6c72 6561 6479 2065 7869  ader already exi
-00011190: 7374 732e 0a20 2020 2020 2020 2022 2222  sts..        """
-000111a0: 0a20 2020 2064 6566 2068 6561 7274 6265  .    def heartbe
-000111b0: 6174 5f74 696d 656f 7574 2873 656c 6629  at_timeout(self)
-000111c0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-000111d0: 2022 2222 0a20 2020 2020 2020 2046 6574   """.        Fet
-000111e0: 6368 2074 6865 206c 656e 6774 6820 6f66  ch the length of
-000111f0: 2074 6865 2068 6561 7274 6265 6174 2074   the heartbeat t
-00011200: 696d 656f 7574 0a20 2020 2020 2020 2022  imeout.        "
-00011210: 2222 0a20 2020 2064 6566 2068 6561 7274  "".    def heart
-00011220: 6265 6174 5f65 6c61 7073 6564 2873 656c  beat_elapsed(sel
-00011230: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00011240: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
-00011250: 6574 6368 2074 6865 206e 756d 6265 7220  etch the number 
-00011260: 6f66 2074 6963 6b73 2065 6c61 7073 6564  of ticks elapsed
-00011270: 2073 696e 6365 206c 6173 7420 6865 6172   since last hear
-00011280: 7462 6561 742e 0a20 2020 2020 2020 2022  tbeat..        "
-00011290: 2222 0a20 2020 2064 6566 2065 6c65 6374  "".    def elect
-000112a0: 696f 6e5f 7469 6d65 6f75 7428 7365 6c66  ion_timeout(self
-000112b0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-000112c0: 2020 2222 220a 2020 2020 2020 2020 4665    """.        Fe
-000112d0: 7463 6820 7468 6520 6c65 6e67 7468 206f  tch the length o
-000112e0: 6620 7468 6520 656c 6563 7469 6f6e 2074  f the election t
-000112f0: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
-00011300: 2222 220a 2020 2020 6465 6620 7261 6e64  """.    def rand
-00011310: 6f6d 697a 6564 5f65 6c65 6374 696f 6e5f  omized_election_
-00011320: 7469 6d65 6f75 7428 7365 6c66 2920 2d3e  timeout(self) ->
-00011330: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00011340: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-00011350: 2074 6865 206c 656e 6774 6820 6f66 2074   the length of t
-00011360: 6865 2063 7572 7265 6e74 2072 616e 646f  he current rando
-00011370: 6d69 7a65 6420 656c 6563 7469 6f6e 2074  mized election t
-00011380: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
-00011390: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-000113a0: 7261 6e64 6f6d 697a 6564 5f65 6c65 6374  randomized_elect
-000113b0: 696f 6e5f 7469 6d65 6f75 7428 7365 6c66  ion_timeout(self
-000113c0: 2c20 7261 6e64 6f6d 697a 6564 5f65 6c65  , randomized_ele
-000113d0: 6374 696f 6e5f 7469 6d65 6f75 743a 2069  ction_timeout: i
-000113e0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000113f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011400: 2046 6f72 2074 6573 7469 6e67 206c 6561   For testing lea
-00011410: 6465 7220 6c65 6173 650a 2020 2020 2020  der lease.      
-00011420: 2020 2222 220a 2020 2020 6465 6620 7265    """.    def re
-00011430: 7365 745f 7261 6e64 6f6d 697a 6564 5f65  set_randomized_e
-00011440: 6c65 6374 696f 6e5f 7469 6d65 6f75 7428  lection_timeout(
-00011450: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00011460: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011470: 2020 2052 6567 656e 6572 6174 6573 2061     Regenerates a
-00011480: 6e64 2073 746f 7265 7320 7468 6520 656c  nd stores the el
-00011490: 6563 7469 6f6e 2074 696d 656f 7574 2e0a  ection timeout..
-000114a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000114b0: 6465 6620 7061 7373 5f65 6c65 6374 696f  def pass_electio
-000114c0: 6e5f 7469 6d65 6f75 7428 7365 6c66 2920  n_timeout(self) 
-000114d0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-000114e0: 2022 2222 0a20 2020 2020 2020 2060 7061   """.        `pa
-000114f0: 7373 5f65 6c65 6374 696f 6e5f 7469 6d65  ss_election_time
-00011500: 6f75 7460 2072 6574 7572 6e73 2074 7275  out` returns tru
-00011510: 6520 6966 2060 656c 6563 7469 6f6e 5f65  e if `election_e
-00011520: 6c61 7073 6564 6020 6973 2067 7265 6174  lapsed` is great
-00011530: 6572 0a20 2020 2020 2020 2074 6861 6e20  er.        than 
-00011540: 6f72 2065 7175 616c 2074 6f20 7468 6520  or equal to the 
-00011550: 7261 6e64 6f6d 697a 6564 2065 6c65 6374  randomized elect
-00011560: 696f 6e20 7469 6d65 6f75 7420 696e 0a20  ion timeout in. 
-00011570: 2020 2020 2020 205b 6065 6c65 6374 696f         [`electio
-00011580: 6e5f 7469 6d65 6f75 7460 2c20 3220 2a20  n_timeout`, 2 * 
-00011590: 6065 6c65 6374 696f 6e5f 7469 6d65 6f75  `election_timeou
-000115a0: 7460 202d 2031 5d2e 0a20 2020 2020 2020  t` - 1]..       
-000115b0: 2022 2222 0a20 2020 2064 6566 2073 656e   """.    def sen
-000115c0: 645f 7469 6d65 6f75 745f 6e6f 7728 7365  d_timeout_now(se
-000115d0: 6c66 2c20 746f 3a20 696e 7429 202d 3e20  lf, to: int) -> 
-000115e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000115f0: 220a 2020 2020 2020 2020 4973 7375 6573  ".        Issues
-00011600: 2061 206d 6573 7361 6765 2074 6f20 7469   a message to ti
-00011610: 6d65 6f75 7420 696d 6d65 6469 6174 656c  meout immediatel
-00011620: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
-00011630: 2020 2064 6566 2072 6561 6479 5f72 6561     def ready_rea
-00011640: 645f 636f 756e 7428 7365 6c66 2920 2d3e  d_count(self) ->
-00011650: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00011660: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-00011670: 7320 686f 7720 6d61 6e79 2072 6561 6420  s how many read 
-00011680: 7374 6174 6573 2065 7869 7374 2e0a 2020  states exist..  
-00011690: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000116a0: 6620 7065 6e64 696e 675f 7265 6164 5f63  f pending_read_c
-000116b0: 6f75 6e74 2873 656c 6629 202d 3e20 696e  ount(self) -> in
-000116c0: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-000116d0: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
-000116e0: 6865 206e 756d 6265 7220 6f66 2070 656e  he number of pen
-000116f0: 6469 6e67 2072 6561 642d 6f6e 6c79 206d  ding read-only m
-00011700: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
-00011710: 2022 2222 0a20 2020 2064 6566 206c 6f61   """.    def loa
-00011720: 645f 7374 6174 6528 7365 6c66 2c20 6873  d_state(self, hs
-00011730: 3a20 2248 6172 6453 7461 7465 2220 7c20  : "HardState" | 
-00011740: 2248 6172 6453 7461 7465 5265 6622 2920  "HardStateRef") 
-00011750: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00011760: 2022 2222 0a20 2020 2020 2020 2046 6f72   """.        For
-00011770: 2061 2067 6976 656e 2068 6172 6473 7461   a given hardsta
-00011780: 7465 2c20 6c6f 6164 2074 6865 2073 7461  te, load the sta
-00011790: 7465 2069 6e74 6f20 7365 6c66 2e0a 2020  te into self..  
-000117a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000117b0: 6620 736f 6674 5f73 7461 7465 2873 656c  f soft_state(sel
-000117c0: 6629 202d 3e20 2253 6f66 7453 7461 7465  f) -> "SoftState
-000117d0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-000117e0: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
-000117f0: 2076 616c 7565 2072 6570 7265 7365 6e74   value represent
-00011800: 696e 6720 7468 6520 736f 6674 7374 6174  ing the softstat
-00011810: 6520 6174 2074 6865 2074 696d 6520 6f66  e at the time of
-00011820: 2063 616c 6c69 6e67 2e0a 2020 2020 2020   calling..      
-00011830: 2020 2222 220a 2020 2020 6465 6620 6861    """.    def ha
-00011840: 7264 5f73 7461 7465 2873 656c 6629 202d  rd_state(self) -
-00011850: 3e20 2248 6172 6453 7461 7465 223a 0a20  > "HardState":. 
-00011860: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011870: 2020 2052 6574 7572 6e73 2061 2076 616c     Returns a val
-00011880: 7565 2072 6570 7265 7365 6e74 696e 6720  ue representing 
-00011890: 7468 6520 6861 7264 7374 6174 6520 6174  the hardstate at
-000118a0: 2074 6865 2074 696d 6520 6f66 2063 616c   the time of cal
-000118b0: 6c69 6e67 2e0a 2020 2020 2020 2020 2222  ling..        ""
-000118c0: 220a 2020 2020 6465 6620 7069 6e67 2873  ".    def ping(s
-000118d0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-000118e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000118f0: 2020 4272 6f61 6463 6173 7473 2068 6561    Broadcasts hea
-00011900: 7274 6265 6174 7320 746f 2061 6c6c 2074  rtbeats to all t
-00011910: 6865 2066 6f6c 6c6f 7765 7273 2069 6620  he followers if 
-00011920: 6974 2773 206c 6561 6465 722e 0a20 2020  it's leader..   
-00011930: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00011940: 2074 6963 6b28 7365 6c66 2920 2d3e 2062   tick(self) -> b
-00011950: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00011960: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00011970: 2074 7275 6520 746f 2069 6e64 6963 6174   true to indicat
-00011980: 6520 7468 6174 2074 6865 7265 2077 696c  e that there wil
-00011990: 6c20 7072 6f62 6162 6c79 2062 6520 736f  l probably be so
-000119a0: 6d65 2072 6561 6469 6e65 7373 206e 6565  me readiness nee
-000119b0: 6420 746f 2062 6520 6861 6e64 6c65 642e  d to be handled.
-000119c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000119d0: 2064 6566 2074 6963 6b5f 656c 6563 7469   def tick_electi
-000119e0: 6f6e 2873 656c 6629 202d 3e20 626f 6f6c  on(self) -> bool
-000119f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00011a00: 2020 2020 2020 5275 6e20 6279 2066 6f6c        Run by fol
-00011a10: 6c6f 7765 7273 2061 6e64 2063 616e 6469  lowers and candi
-00011a20: 6461 7465 7320 6166 7465 7220 7365 6c66  dates after self
-00011a30: 2e65 6c65 6374 696f 6e5f 7469 6d65 6f75  .election_timeou
-00011a40: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
-00011a50: 726e 7320 7472 7565 2074 6f20 696e 6469  rns true to indi
-00011a60: 6361 7465 2074 6861 7420 7468 6572 6520  cate that there 
-00011a70: 7769 6c6c 2070 726f 6261 626c 7920 6265  will probably be
-00011a80: 2073 6f6d 6520 7265 6164 696e 6573 7320   some readiness 
-00011a90: 6e65 6564 2074 6f20 6265 2068 616e 646c  need to be handl
-00011aa0: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
-00011ab0: 2020 2020 6465 6620 7374 6570 2873 656c      def step(sel
-00011ac0: 662c 206d 7367 3a20 224d 6573 7361 6765  f, msg: "Message
-00011ad0: 2220 7c20 224d 6573 7361 6765 5265 6622  " | "MessageRef"
-00011ae0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00011af0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00011b00: 7465 7073 2074 6865 2072 6166 7420 616c  teps the raft al
-00011b10: 6f6e 6720 7669 6120 6120 6d65 7373 6167  ong via a messag
-00011b20: 652e 2054 6869 7320 7368 6f75 6c64 2062  e. This should b
-00011b30: 6520 6361 6c6c 6564 2065 7665 7279 7469  e called everyti
-00011b40: 6d65 2079 6f75 7220 7261 6674 2072 6563  me your raft rec
-00011b50: 6569 7665 7320 610a 2020 2020 2020 2020  eives a.        
-00011b60: 6d65 7373 6167 6520 6672 6f6d 2061 2070  message from a p
-00011b70: 6565 722e 0a20 2020 2020 2020 2022 2222  eer..        """
-00011b80: 0a20 2020 2064 6566 2068 6173 5f70 656e  .    def has_pen
-00011b90: 6469 6e67 5f63 6f6e 6628 7365 6c66 2920  ding_conf(self) 
-00011ba0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00011bb0: 2022 2222 0a20 2020 2020 2020 2043 6865   """.        Che
-00011bc0: 636b 2069 6620 7468 6572 6520 6973 2061  ck if there is a
-00011bd0: 6e79 2070 656e 6469 6e67 2063 6f6e 6663  ny pending confc
-00011be0: 6861 6e67 652e 0a0a 2020 2020 2020 2020  hange...        
-00011bf0: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-00011c00: 6265 2066 616c 7365 2070 6f73 6974 6976  be false positiv
-00011c10: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00011c20: 2020 2064 6566 2070 726f 6d6f 7461 626c     def promotabl
-00011c30: 6528 7365 6c66 2920 2d3e 2062 6f6f 6c3a  e(self) -> bool:
-00011c40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011c50: 2020 2020 2049 6e64 6963 6174 6573 2077       Indicates w
-00011c60: 6865 7468 6572 2073 7461 7465 206d 6163  hether state mac
-00011c70: 6869 6e65 2063 616e 2062 6520 7072 6f6d  hine can be prom
-00011c80: 6f74 6564 2074 6f20 6c65 6164 6572 2c0a  oted to leader,.
-00011c90: 2020 2020 2020 2020 7768 6963 6820 6973          which is
-00011ca0: 2074 7275 6520 7768 656e 2069 7427 7320   true when it's 
-00011cb0: 6120 766f 7465 7220 616e 6420 6974 7320  a voter and its 
-00011cc0: 6f77 6e20 6964 2069 7320 696e 2070 726f  own id is in pro
-00011cd0: 6772 6573 7320 6c69 7374 2e0a 2020 2020  gress list..    
-00011ce0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00011cf0: 706f 7374 5f63 6f6e 665f 6368 616e 6765  post_conf_change
-00011d00: 2873 656c 6629 202d 3e20 2243 6f6e 6653  (self) -> "ConfS
-00011d10: 7461 7465 5265 6622 3a0a 2020 2020 2020  tateRef":.      
-00011d20: 2020 2222 220a 2020 2020 2020 2020 5570    """.        Up
-00011d30: 6461 7465 7320 7468 6520 696e 2d6d 656d  dates the in-mem
-00011d40: 6f72 7920 7374 6174 6520 616e 642c 2077  ory state and, w
-00011d50: 6865 6e20 6e65 6365 7373 6172 792c 2063  hen necessary, c
-00011d60: 6172 7269 6573 206f 7574 2061 6464 6974  arries out addit
-00011d70: 696f 6e61 6c20 6163 7469 6f6e 730a 2020  ional actions.  
-00011d80: 2020 2020 2020 7375 6368 2061 7320 7265        such as re
-00011d90: 6163 7469 6e67 2074 6f20 7468 6520 7265  acting to the re
-00011da0: 6d6f 7661 6c20 6f66 206e 6f64 6573 206f  moval of nodes o
-00011db0: 7220 6368 616e 6765 6420 7175 6f72 756d  r changed quorum
-00011dc0: 2072 6571 7569 7265 6d65 6e74 732e 0a20   requirements.. 
-00011dd0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00011de0: 6566 2069 6e5f 6c65 6173 6528 7365 6c66  ef in_lease(self
-00011df0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00011e00: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00011e10: 6574 7572 6e73 2077 6865 7468 6572 2074  eturns whether t
-00011e20: 6865 2063 7572 7265 6e74 2072 6166 7420  he current raft 
-00011e30: 6973 2069 6e20 6c65 6173 652e 0a20 2020  is in lease..   
-00011e40: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00011e50: 2068 616e 646c 655f 6865 6172 7462 6561   handle_heartbea
-00011e60: 7428 7365 6c66 2c20 6d73 673a 2022 4d65  t(self, msg: "Me
-00011e70: 7373 6167 6522 207c 2022 4d65 7373 6167  ssage" | "Messag
-00011e80: 6552 6566 2229 202d 3e20 4e6f 6e65 3a0a  eRef") -> None:.
-00011e90: 2020 2020 2020 2020 2222 2246 6f72 2061          """For a
-00011ea0: 206d 6573 7361 6765 2c20 636f 6d6d 6974   message, commit
-00011eb0: 2061 6e64 2073 656e 6420 6f75 7420 6865   and send out he
-00011ec0: 6172 7462 6561 742e 2222 220a 2020 2020  artbeat.""".    
-00011ed0: 6465 6620 6861 6e64 6c65 5f61 7070 656e  def handle_appen
-00011ee0: 645f 656e 7472 6965 7328 7365 6c66 2c20  d_entries(self, 
-00011ef0: 6d73 673a 2022 4d65 7373 6167 6522 207c  msg: "Message" |
-00011f00: 2022 4d65 7373 6167 6552 6566 2229 202d   "MessageRef") -
-00011f10: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00011f20: 2222 2246 6f72 2061 2067 6976 656e 206d  """For a given m
-00011f30: 6573 7361 6765 2c20 6170 7065 6e64 2074  essage, append t
-00011f40: 6865 2065 6e74 7269 6573 2074 6f20 7468  he entries to th
-00011f50: 6520 6c6f 672e 2222 220a 2020 2020 6465  e log.""".    de
-00011f60: 6620 7265 7175 6573 745f 736e 6170 7368  f request_snapsh
-00011f70: 6f74 2873 656c 6629 202d 3e20 4e6f 6e65  ot(self) -> None
-00011f80: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00011f90: 2020 2020 2020 5265 7175 6573 7420 6120        Request a 
-00011fa0: 736e 6170 7368 6f74 2066 726f 6d20 6120  snapshot from a 
-00011fb0: 6c65 6164 6572 2e0a 2020 2020 2020 2020  leader..        
-00011fc0: 2222 220a 2020 2020 6465 6620 7072 7328  """.    def prs(
-00011fd0: 7365 6c66 2920 2d3e 2022 5072 6f67 7265  self) -> "Progre
-00011fe0: 7373 5472 6163 6b65 7252 6566 223a 0a20  ssTrackerRef":. 
-00011ff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012000: 2020 2052 6574 7572 6e73 2061 2072 6561     Returns a rea
-00012010: 642d 6f6e 6c79 2072 6566 6572 656e 6365  d-only reference
-00012020: 2074 6f20 7468 6520 7072 6f67 7265 7373   to the progress
-00012030: 2073 6574 2e0a 2020 2020 2020 2020 2222   set..        ""
-00012040: 220a 2020 2020 6465 6620 7265 7365 7428  ".    def reset(
-00012050: 7365 6c66 2c20 7465 726d 3a20 696e 7429  self, term: int)
-00012060: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00012070: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00012080: 7365 7473 2074 6865 2063 7572 7265 6e74  sets the current
-00012090: 206e 6f64 6520 746f 2061 2067 6976 656e   node to a given
-000120a0: 2074 6572 6d2e 0a20 2020 2020 2020 2022   term..        "
-000120b0: 2222 0a20 2020 2064 6566 2072 6573 746f  "".    def resto
-000120c0: 7265 2873 656c 662c 2073 6e61 7073 686f  re(self, snapsho
-000120d0: 743a 2022 536e 6170 7368 6f74 2220 7c20  t: "Snapshot" | 
-000120e0: 2253 6e61 7073 686f 7452 6566 2229 202d  "SnapshotRef") -
-000120f0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00012100: 2222 220a 2020 2020 2020 2020 5265 636f  """.        Reco
-00012110: 7665 7273 2074 6865 2073 7461 7465 206d  vers the state m
-00012120: 6163 6869 6e65 2066 726f 6d20 6120 736e  achine from a sn
-00012130: 6170 7368 6f74 2e20 4974 2072 6573 746f  apshot. It resto
-00012140: 7265 7320 7468 6520 6c6f 6720 616e 6420  res the log and 
-00012150: 7468 650a 2020 2020 2020 2020 636f 6e66  the.        conf
-00012160: 6967 7572 6174 696f 6e20 6f66 2073 7461  iguration of sta
-00012170: 7465 206d 6163 6869 6e65 2e0a 2020 2020  te machine..    
-00012180: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00012190: 736e 6170 2873 656c 6629 202d 3e20 4f70  snap(self) -> Op
-000121a0: 7469 6f6e 616c 5b22 536e 6170 7368 6f74  tional["Snapshot
-000121b0: 5265 6622 5d3a 0a20 2020 2020 2020 2022  Ref"]:.        "
-000121c0: 2222 0a20 2020 2020 2020 2047 7261 6273  "".        Grabs
-000121d0: 2061 2072 6566 6572 656e 6365 2074 6f20   a reference to 
-000121e0: 7468 6520 736e 6170 7368 6f74 0a20 2020  the snapshot.   
-000121f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00012200: 2073 746f 7265 2873 656c 6629 202d 3e20   store(self) -> 
-00012210: 224d 656d 5374 6f72 6167 6552 6566 223a  "MemStorageRef":
-00012220: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012230: 2020 2020 2047 7261 6273 2061 6e20 696d       Grabs an im
-00012240: 6d75 7461 626c 6520 7265 6665 7265 6e63  mutable referenc
-00012250: 6520 746f 2074 6865 2073 746f 7265 2e0a  e to the store..
-00012260: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012270: 6465 6620 6f6e 5f70 6572 7369 7374 5f73  def on_persist_s
-00012280: 6e61 7028 7365 6c66 2c20 696e 6465 783a  nap(self, index:
-00012290: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-000122a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000122b0: 2020 204e 6f74 6966 6965 7320 7468 6174     Notifies that
-000122c0: 2074 6865 2073 6e61 7073 686f 7420 6861   the snapshot ha
-000122d0: 7665 2062 6565 6e20 7065 7273 6973 7465  ve been persiste
-000122e0: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
-000122f0: 2020 2064 6566 2061 626f 7274 5f6c 6561     def abort_lea
-00012300: 6465 725f 7472 616e 7366 6572 2873 656c  der_transfer(sel
-00012310: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00012320: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012330: 5374 6f70 7320 7468 6520 7472 616e 7366  Stops the transf
-00012340: 6572 206f 6620 6120 6c65 6164 6572 2e0a  er of a leader..
-00012350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012360: 6465 6620 6361 6d70 6169 676e 2873 656c  def campaign(sel
-00012370: 662c 2074 7970 3a20 7374 7229 202d 3e20  f, typ: str) -> 
-00012380: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00012390: 220a 2020 2020 2020 2020 4361 6d70 6169  ".        Campai
-000123a0: 676e 2074 6f20 6174 7465 6d70 7420 746f  gn to attempt to
-000123b0: 2062 6563 6f6d 6520 6120 6c65 6164 6572   become a leader
-000123c0: 2e0a 0a20 2020 2020 2020 2049 6620 7072  ...        If pr
-000123d0: 6576 6f74 6520 6973 2065 6e61 626c 6564  evote is enabled
-000123e0: 2c20 7468 6973 2069 7320 6861 6e64 6c65  , this is handle
-000123f0: 6420 6173 2077 656c 6c2e 0a20 2020 2020  d as well..     
-00012400: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-00012410: 6574 5f6c 6561 645f 7472 616e 7366 6572  et_lead_transfer
-00012420: 6565 2873 656c 6629 202d 3e20 4f70 7469  ee(self) -> Opti
-00012430: 6f6e 616c 5b69 6e74 5d3a 0a20 2020 2020  onal[int]:.     
-00012440: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00012450: 6c65 6164 5f74 7261 6e73 6665 7265 6560  lead_transferee`
-00012460: 3a20 4944 206f 6620 7468 6520 6c65 6164  : ID of the lead
-00012470: 6572 2074 7261 6e73 6665 7220 7461 7267  er transfer targ
-00012480: 6574 2077 6865 6e20 6974 7320 7661 6c75  et when its valu
-00012490: 6520 6973 206e 6f74 204e 6f6e 652e 0a0a  e is not None...
-000124a0: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
-000124b0: 6973 2053 6f6d 6528 6964 292c 2077 6520  is Some(id), we 
-000124c0: 666f 6c6c 6f77 2074 6865 2070 726f 6365  follow the proce
-000124d0: 6475 7265 2064 6566 696e 6564 2069 6e20  dure defined in 
-000124e0: 7261 6674 2074 6865 7369 7320 332e 3130  raft thesis 3.10
-000124f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00012500: 2020 6465 6620 7365 745f 6c65 6164 5f74    def set_lead_t
-00012510: 7261 6e73 6665 7265 6528 7365 6c66 2c20  ransferee(self, 
-00012520: 6c65 6164 5f74 7261 6e73 6665 7265 653a  lead_transferee:
-00012530: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-00012540: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012550: 2020 2060 6c65 6164 5f74 7261 6e73 6665     `lead_transfe
-00012560: 7265 6560 3a20 4944 206f 6620 7468 6520  ree`: ID of the 
-00012570: 6c65 6164 6572 2074 7261 6e73 6665 7220  leader transfer 
-00012580: 7461 7267 6574 2077 6865 6e20 6974 7320  target when its 
-00012590: 7661 6c75 6520 6973 206e 6f74 204e 6f6e  value is not Non
-000125a0: 652e 0a0a 2020 2020 2020 2020 4966 2074  e...        If t
-000125b0: 6869 7320 6973 2053 6f6d 6528 6964 292c  his is Some(id),
-000125c0: 2077 6520 666f 6c6c 6f77 2074 6865 2070   we follow the p
-000125d0: 726f 6365 6475 7265 2064 6566 696e 6564  rocedure defined
-000125e0: 2069 6e20 7261 6674 2074 6865 7369 7320   in raft thesis 
-000125f0: 332e 3130 2e0a 2020 2020 2020 2020 2222  3.10..        ""
-00012600: 220a 2020 2020 6465 6620 6765 745f 7465  ".    def get_te
-00012610: 726d 2873 656c 6629 202d 3e20 696e 743a  rm(self) -> int:
-00012620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012630: 2020 2020 2060 7465 726d 603a 2054 6865       `term`: The
-00012640: 2063 7572 7265 6e74 2065 6c65 6374 696f   current electio
-00012650: 6e20 7465 726d 2e0a 2020 2020 2020 2020  n term..        
-00012660: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00012670: 7465 726d 2873 656c 662c 2074 6572 6d3a  term(self, term:
-00012680: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-00012690: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000126a0: 2020 2060 7465 726d 603a 2054 6865 2063     `term`: The c
-000126b0: 7572 7265 6e74 2065 6c65 6374 696f 6e20  urrent election 
-000126c0: 7465 726d 2e0a 2020 2020 2020 2020 2222  term..        ""
-000126d0: 220a 2020 2020 6465 6620 6765 745f 766f  ".    def get_vo
-000126e0: 7465 2873 656c 6629 202d 3e20 696e 743a  te(self) -> int:
-000126f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012700: 2020 2020 2060 766f 7465 603a 2057 6869       `vote`: Whi
-00012710: 6368 2070 6565 7220 7468 6973 2072 6166  ch peer this raf
-00012720: 7420 6973 2076 6f74 696e 6720 666f 722e  t is voting for.
-00012730: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012740: 2064 6566 2073 6574 5f76 6f74 6528 7365   def set_vote(se
-00012750: 6c66 2c20 766f 7465 3a20 696e 7429 202d  lf, vote: int) -
-00012760: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00012770: 2222 220a 2020 2020 2020 2020 6076 6f74  """.        `vot
-00012780: 6560 3a20 5768 6963 6820 7065 6572 2074  e`: Which peer t
-00012790: 6869 7320 7261 6674 2069 7320 766f 7469  his raft is voti
-000127a0: 6e67 2066 6f72 2e0a 2020 2020 2020 2020  ng for..        
-000127b0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-000127c0: 7072 696f 7269 7479 2873 656c 6629 202d  priority(self) -
-000127d0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-000127e0: 2222 0a20 2020 2020 2020 2060 7072 696f  "".        `prio
-000127f0: 7269 7479 603a 2054 6865 2065 6c65 6374  rity`: The elect
-00012800: 696f 6e20 7072 696f 7269 7479 206f 6620  ion priority of 
-00012810: 7468 6973 206e 6f64 652e 0a20 2020 2020  this node..     
-00012820: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
-00012830: 6574 5f70 7269 6f72 6974 7928 7365 6c66  et_priority(self
-00012840: 2c20 7072 696f 7269 7479 3a20 696e 7429  , priority: int)
-00012850: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00012860: 2020 2222 220a 2020 2020 2020 2020 6070    """.        `p
-00012870: 7269 6f72 6974 7960 3a20 5468 6520 656c  riority`: The el
-00012880: 6563 7469 6f6e 2070 7269 6f72 6974 7920  ection priority 
-00012890: 6f66 2074 6869 7320 6e6f 6465 2e0a 2020  of this node..  
-000128a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000128b0: 6620 6765 745f 6c65 6164 6572 5f69 6428  f get_leader_id(
-000128c0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-000128d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000128e0: 2020 606c 6561 6465 725f 6964 603a 2054    `leader_id`: T
-000128f0: 6865 206c 6561 6465 7220 6964 0a20 2020  he leader id.   
-00012900: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00012910: 2073 6574 5f6c 6561 6465 725f 6964 2873   set_leader_id(s
-00012920: 656c 662c 206c 6561 6465 725f 6964 3a20  elf, leader_id: 
-00012930: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00012940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012950: 2020 606c 6561 6465 725f 6964 603a 2054    `leader_id`: T
-00012960: 6865 206c 6561 6465 7220 6964 0a20 2020  he leader id.   
-00012970: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00012980: 2067 6574 5f6d 6178 5f6d 7367 5f73 697a   get_max_msg_siz
-00012990: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0a  e(self) -> int:.
-000129a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000129b0: 2020 2020 606d 6178 5f6d 7367 5f73 697a      `max_msg_siz
-000129c0: 6560 3a20 5468 6520 6d61 7869 6d75 6d20  e`: The maximum 
-000129d0: 6c65 6e67 7468 2028 696e 2062 7974 6573  length (in bytes
-000129e0: 2920 6f66 2061 6c6c 2074 6865 2065 6e74  ) of all the ent
-000129f0: 7269 6573 2e0a 2020 2020 2020 2020 2222  ries..        ""
-00012a00: 220a 2020 2020 6465 6620 7365 745f 6d61  ".    def set_ma
-00012a10: 785f 6d73 675f 7369 7a65 2873 656c 662c  x_msg_size(self,
-00012a20: 206d 6178 5f6d 7367 5f73 697a 653a 2069   max_msg_size: i
-00012a30: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00012a40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012a50: 2060 6d61 785f 6d73 675f 7369 7a65 603a   `max_msg_size`:
-00012a60: 2054 6865 206d 6178 696d 756d 206c 656e   The maximum len
-00012a70: 6774 6820 2869 6e20 6279 7465 7329 206f  gth (in bytes) o
-00012a80: 6620 616c 6c20 7468 6520 656e 7472 6965  f all the entrie
-00012a90: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00012aa0: 2020 2064 6566 2067 6574 5f70 656e 6469     def get_pendi
-00012ab0: 6e67 5f63 6f6e 665f 696e 6465 7828 7365  ng_conf_index(se
-00012ac0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00012ad0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012ae0: 6070 656e 6469 6e67 5f63 6f6e 665f 696e  `pending_conf_in
-00012af0: 6465 7860 3a20 4f6e 6c79 206f 6e65 2063  dex`: Only one c
-00012b00: 6f6e 6620 6368 616e 6765 206d 6179 2062  onf change may b
-00012b10: 6520 7065 6e64 696e 6720 2869 6e20 7468  e pending (in th
-00012b20: 6520 6c6f 672c 2062 7574 206e 6f74 2079  e log, but not y
-00012b30: 6574 0a20 2020 2020 2020 2061 7070 6c69  et.        appli
-00012b40: 6564 2920 6174 2061 2074 696d 652e 2054  ed) at a time. T
-00012b50: 6869 7320 6973 2065 6e66 6f72 6365 6420  his is enforced 
-00012b60: 7669 6120 6070 656e 6469 6e67 5f63 6f6e  via `pending_con
-00012b70: 665f 696e 6465 7860 2c20 7768 6963 680a  f_index`, which.
-00012b80: 2020 2020 2020 2020 6973 2073 6574 2074          is set t
-00012b90: 6f20 6120 7661 6c75 6520 3e3d 2074 6865  o a value >= the
-00012ba0: 206c 6f67 2069 6e64 6578 206f 6620 7468   log index of th
-00012bb0: 6520 6c61 7465 7374 2070 656e 6469 6e67  e latest pending
-00012bc0: 0a20 2020 2020 2020 2063 6f6e 6669 6775  .        configu
-00012bd0: 7261 7469 6f6e 2063 6861 6e67 6520 2869  ration change (i
-00012be0: 6620 616e 7929 2e20 436f 6e66 6967 2063  f any). Config c
-00012bf0: 6861 6e67 6573 2061 7265 206f 6e6c 7920  hanges are only 
-00012c00: 616c 6c6f 7765 6420 746f 0a20 2020 2020  allowed to.     
-00012c10: 2020 2062 6520 7072 6f70 6f73 6564 2069     be proposed i
-00012c20: 6620 7468 6520 6c65 6164 6572 2773 2061  f the leader's a
-00012c30: 7070 6c69 6564 2069 6e64 6578 2069 7320  pplied index is 
-00012c40: 6772 6561 7465 7220 7468 616e 2074 6869  greater than thi
-00012c50: 730a 2020 2020 2020 2020 7661 6c75 652e  s.        value.
-00012c60: 0a0a 2020 2020 2020 2020 5468 6973 2076  ..        This v
-00012c70: 616c 7565 2069 7320 636f 6e73 6572 7661  alue is conserva
-00012c80: 7469 7665 6c79 2073 6574 2069 6e20 6361  tively set in ca
-00012c90: 7365 7320 7768 6572 6520 7468 6572 6520  ses where there 
-00012ca0: 6d61 7920 6265 2061 2063 6f6e 6669 6775  may be a configu
-00012cb0: 7261 7469 6f6e 2063 6861 6e67 6520 7065  ration change pe
-00012cc0: 6e64 696e 672c 0a20 2020 2020 2020 2062  nding,.        b
-00012cd0: 7574 2073 6361 6e6e 696e 6720 7468 6520  ut scanning the 
-00012ce0: 6c6f 6720 6973 2070 6f73 7369 626c 7920  log is possibly 
-00012cf0: 6578 7065 6e73 6976 652e 2054 6869 7320  expensive. This 
-00012d00: 696d 706c 6965 7320 7468 6174 2074 6865  implies that the
-00012d10: 2069 6e64 6578 2073 7461 7465 6420 6865   index stated he
-00012d20: 7265 206d 6179 206e 6f74 0a20 2020 2020  re may not.     
-00012d30: 2020 206e 6563 6573 7361 7269 6c79 2062     necessarily b
-00012d40: 6520 6120 636f 6e66 6967 2063 6861 6e67  e a config chang
-00012d50: 6520 656e 7472 792c 2061 6e64 2069 7420  e entry, and it 
-00012d60: 6d61 7920 6e6f 7420 6265 2061 2060 4265  may not be a `Be
-00012d70: 6769 6e4d 656d 6265 7273 6869 7043 6861  ginMembershipCha
-00012d80: 6e67 6560 2065 6e74 7279 2c20 6576 656e  nge` entry, even
-00012d90: 2069 660a 2020 2020 2020 2020 7765 2073   if.        we s
-00012da0: 6574 2074 6869 7320 746f 206f 6e65 2e0a  et this to one..
-00012db0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012dc0: 6465 6620 7365 745f 7065 6e64 696e 675f  def set_pending_
-00012dd0: 636f 6e66 5f69 6e64 6578 2873 656c 662c  conf_index(self,
-00012de0: 2070 656e 6469 6e67 5f63 6f6e 665f 696e   pending_conf_in
-00012df0: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
-00012e00: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00012e10: 2020 2020 2020 2060 7065 6e64 696e 675f         `pending_
-00012e20: 636f 6e66 5f69 6e64 6578 603a 204f 6e6c  conf_index`: Onl
-00012e30: 7920 6f6e 6520 636f 6e66 2063 6861 6e67  y one conf chang
-00012e40: 6520 6d61 7920 6265 2070 656e 6469 6e67  e may be pending
-00012e50: 2028 696e 2074 6865 206c 6f67 2c20 6275   (in the log, bu
-00012e60: 7420 6e6f 7420 7965 740a 2020 2020 2020  t not yet.      
-00012e70: 2020 6170 706c 6965 6429 2061 7420 6120    applied) at a 
-00012e80: 7469 6d65 2e20 5468 6973 2069 7320 656e  time. This is en
-00012e90: 666f 7263 6564 2076 6961 2060 7065 6e64  forced via `pend
-00012ea0: 696e 675f 636f 6e66 5f69 6e64 6578 602c  ing_conf_index`,
-00012eb0: 2077 6869 6368 0a20 2020 2020 2020 2069   which.        i
-00012ec0: 7320 7365 7420 746f 2061 2076 616c 7565  s set to a value
-00012ed0: 203e 3d20 7468 6520 6c6f 6720 696e 6465   >= the log inde
-00012ee0: 7820 6f66 2074 6865 206c 6174 6573 7420  x of the latest 
-00012ef0: 7065 6e64 696e 670a 2020 2020 2020 2020  pending.        
-00012f00: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
-00012f10: 616e 6765 2028 6966 2061 6e79 292e 2043  ange (if any). C
-00012f20: 6f6e 6669 6720 6368 616e 6765 7320 6172  onfig changes ar
-00012f30: 6520 6f6e 6c79 2061 6c6c 6f77 6564 2074  e only allowed t
-00012f40: 6f0a 2020 2020 2020 2020 6265 2070 726f  o.        be pro
-00012f50: 706f 7365 6420 6966 2074 6865 206c 6561  posed if the lea
-00012f60: 6465 7227 7320 6170 706c 6965 6420 696e  der's applied in
-00012f70: 6465 7820 6973 2067 7265 6174 6572 2074  dex is greater t
-00012f80: 6861 6e20 7468 6973 0a20 2020 2020 2020  han this.       
-00012f90: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
-00012fa0: 2054 6869 7320 7661 6c75 6520 6973 2063   This value is c
-00012fb0: 6f6e 7365 7276 6174 6976 656c 7920 7365  onservatively se
-00012fc0: 7420 696e 2063 6173 6573 2077 6865 7265  t in cases where
-00012fd0: 2074 6865 7265 206d 6179 2062 6520 6120   there may be a 
-00012fe0: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
-00012ff0: 616e 6765 2070 656e 6469 6e67 2c0a 2020  ange pending,.  
-00013000: 2020 2020 2020 6275 7420 7363 616e 6e69        but scanni
-00013010: 6e67 2074 6865 206c 6f67 2069 7320 706f  ng the log is po
-00013020: 7373 6962 6c79 2065 7870 656e 7369 7665  ssibly expensive
-00013030: 2e20 5468 6973 2069 6d70 6c69 6573 2074  . This implies t
-00013040: 6861 7420 7468 6520 696e 6465 7820 7374  hat the index st
-00013050: 6174 6564 2068 6572 6520 6d61 7920 6e6f  ated here may no
-00013060: 740a 2020 2020 2020 2020 6e65 6365 7373  t.        necess
-00013070: 6172 696c 7920 6265 2061 2063 6f6e 6669  arily be a confi
-00013080: 6720 6368 616e 6765 2065 6e74 7279 2c20  g change entry, 
-00013090: 616e 6420 6974 206d 6179 206e 6f74 2062  and it may not b
-000130a0: 6520 6120 6042 6567 696e 4d65 6d62 6572  e a `BeginMember
-000130b0: 7368 6970 4368 616e 6765 6020 656e 7472  shipChange` entr
-000130c0: 792c 2065 7665 6e20 6966 0a20 2020 2020  y, even if.     
-000130d0: 2020 2077 6520 7365 7420 7468 6973 2074     we set this t
-000130e0: 6f20 6f6e 652e 0a20 2020 2020 2020 2022  o one..        "
-000130f0: 2222 0a20 2020 2064 6566 2067 6574 5f70  "".    def get_p
-00013100: 656e 6469 6e67 5f72 6571 7565 7374 5f73  ending_request_s
-00013110: 6e61 7073 686f 7428 7365 6c66 2920 2d3e  napshot(self) ->
-00013120: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00013130: 220a 2020 2020 2020 2020 6070 656e 6469  ".        `pendi
-00013140: 6e67 5f72 6571 7565 7374 5f73 6e61 7073  ng_request_snaps
-00013150: 686f 7460 3a20 5468 6520 7065 6572 2069  hot`: The peer i
-00013160: 7320 7265 7175 6573 7469 6e67 2073 6e61  s requesting sna
-00013170: 7073 686f 742c 2069 7420 6973 2074 6865  pshot, it is the
-00013180: 2069 6e64 6578 2074 6861 7420 7468 6520   index that the 
-00013190: 666f 6c6c 6f77 6572 0a20 2020 2020 2020  follower.       
-000131a0: 206e 6565 6473 2069 7420 746f 2062 6520   needs it to be 
-000131b0: 696e 636c 7564 6564 2069 6e20 6120 736e  included in a sn
-000131c0: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
-000131d0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-000131e0: 7065 6e64 696e 675f 7265 7175 6573 745f  pending_request_
-000131f0: 736e 6170 7368 6f74 2873 656c 662c 2070  snapshot(self, p
-00013200: 656e 6469 6e67 5f72 6571 7565 7374 5f73  ending_request_s
-00013210: 6e61 7073 686f 743a 2069 6e74 2920 2d3e  napshot: int) ->
-00013220: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00013230: 2222 0a20 2020 2020 2020 2060 7065 6e64  "".        `pend
-00013240: 696e 675f 7265 7175 6573 745f 736e 6170  ing_request_snap
-00013250: 7368 6f74 603a 2054 6865 2070 6565 7220  shot`: The peer 
-00013260: 6973 2072 6571 7565 7374 696e 6720 736e  is requesting sn
-00013270: 6170 7368 6f74 2c20 6974 2069 7320 7468  apshot, it is th
-00013280: 6520 696e 6465 7820 7468 6174 2074 6865  e index that the
-00013290: 2066 6f6c 6c6f 7765 720a 2020 2020 2020   follower.      
-000132a0: 2020 6e65 6564 7320 6974 2074 6f20 6265    needs it to be
-000132b0: 2069 6e63 6c75 6465 6420 696e 2061 2073   included in a s
-000132c0: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
-000132d0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-000132e0: 5f69 6428 7365 6c66 2920 2d3e 2069 6e74  _id(self) -> int
-000132f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013300: 2020 2020 2020 6069 6460 3a20 5468 6520        `id`: The 
-00013310: 4944 206f 6620 7468 6973 206e 6f64 652e  ID of this node.
-00013320: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013330: 2064 6566 2073 6574 5f69 6428 7365 6c66   def set_id(self
-00013340: 2c20 6964 3a20 696e 7429 202d 3e20 4e6f  , id: int) -> No
-00013350: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00013360: 2020 2020 2020 2020 6069 6460 3a20 5468          `id`: Th
-00013370: 6520 4944 206f 6620 7468 6973 206e 6f64  e ID of this nod
-00013380: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00013390: 2020 2064 6566 2067 6574 5f6d 7367 7328     def get_msgs(
-000133a0: 7365 6c66 2920 2d3e 204c 6973 745b 224d  self) -> List["M
-000133b0: 6573 7361 6765 5265 6622 5d3a 0a20 2020  essageRef"]:.   
-000133c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000133d0: 2060 6d73 6773 603a 2054 6865 206c 6973   `msgs`: The lis
-000133e0: 7420 6f66 206d 6573 7361 6765 732e 0a20  t of messages.. 
-000133f0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00013400: 6566 2073 6574 5f6d 7367 7328 7365 6c66  ef set_msgs(self
-00013410: 2c20 6d73 6773 3a20 4c69 7374 5b22 4d65  , msgs: List["Me
-00013420: 7373 6167 6522 207c 2022 4d65 7373 6167  ssage" | "Messag
-00013430: 6552 6566 225d 2920 2d3e 204e 6f6e 653a  eRef"]) -> None:
-00013440: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013450: 2020 2020 2060 6d73 6773 603a 2054 6865       `msgs`: The
-00013460: 206c 6973 7420 6f66 206d 6573 7361 6765   list of message
-00013470: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00013480: 2020 2064 6566 2074 616b 655f 6d73 6773     def take_msgs
-00013490: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
-000134a0: 4d65 7373 6167 6522 5d3a 0a20 2020 2020  Message"]:.     
-000134b0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-000134c0: 6d73 6773 603a 2054 6865 206c 6973 7420  msgs`: The list 
-000134d0: 6f66 206d 6573 7361 6765 732e 0a20 2020  of messages..   
-000134e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-000134f0: 2067 6574 5f6d 6178 5f69 6e66 6c69 6768   get_max_infligh
-00013500: 7428 7365 6c66 2920 2d3e 2069 6e74 3a0a  t(self) -> int:.
-00013510: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013520: 2020 2020 606d 6178 5f69 6e66 6c69 6768      `max_infligh
-00013530: 7460 3a20 5468 6520 6d61 7869 6d75 6d20  t`: The maximum 
-00013540: 6e75 6d62 6572 206f 6620 6d65 7373 6167  number of messag
-00013550: 6573 2074 6861 7420 6361 6e20 6265 2069  es that can be i
-00013560: 6e66 6c69 6768 742e 0a20 2020 2020 2020  nflight..       
-00013570: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00013580: 5f6d 6178 5f69 6e66 6c69 6768 7428 7365  _max_inflight(se
-00013590: 6c66 2c20 6d61 785f 696e 666c 6967 6874  lf, max_inflight
-000135a0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-000135b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000135c0: 2020 2020 606d 6178 5f69 6e66 6c69 6768      `max_infligh
-000135d0: 7460 3a20 5468 6520 6d61 7869 6d75 6d20  t`: The maximum 
-000135e0: 6e75 6d62 6572 206f 6620 6d65 7373 6167  number of messag
-000135f0: 6573 2074 6861 7420 6361 6e20 6265 2069  es that can be i
-00013600: 6e66 6c69 6768 742e 0a20 2020 2020 2020  nflight..       
-00013610: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00013620: 5f73 7461 7465 2873 656c 6629 202d 3e20  _state(self) -> 
-00013630: 2253 7461 7465 526f 6c65 223a 0a20 2020  "StateRole":.   
-00013640: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013650: 2060 7374 6174 6560 3a20 5468 6520 6375   `state`: The cu
-00013660: 7272 656e 7420 726f 6c65 206f 6620 7468  rrent role of th
-00013670: 6973 206e 6f64 652e 0a20 2020 2020 2020  is node..       
-00013680: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00013690: 5f73 7461 7465 2873 656c 662c 2073 7461  _state(self, sta
-000136a0: 7465 5f72 6f6c 653a 2022 5374 6174 6552  te_role: "StateR
-000136b0: 6f6c 6522 2920 2d3e 204e 6f6e 653a 0a20  ole") -> None:. 
-000136c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000136d0: 2020 2060 7374 6174 6560 3a20 5468 6520     `state`: The 
-000136e0: 6375 7272 656e 7420 726f 6c65 206f 6620  current role of 
-000136f0: 7468 6973 206e 6f64 652e 0a20 2020 2020  this node..     
-00013700: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-00013710: 6574 5f65 6c65 6374 696f 6e5f 656c 6170  et_election_elap
-00013720: 7365 6428 7365 6c66 2920 2d3e 2069 6e74  sed(self) -> int
-00013730: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013740: 2020 2020 2020 6065 6c65 6374 696f 6e5f        `election_
-00013750: 656c 6170 7365 6460 3a20 5469 636b 7320  elapsed`: Ticks 
-00013760: 7369 6e63 6520 6974 2072 6561 6368 6564  since it reached
-00013770: 206c 6173 7420 656c 6563 7469 6f6e 5469   last electionTi
-00013780: 6d65 6f75 7420 7768 656e 2069 7420 6973  meout when it is
-00013790: 206c 6561 6465 7220 6f72 2063 616e 6469   leader or candi
-000137a0: 6461 7465 2e0a 2020 2020 2020 2020 4e75  date..        Nu
-000137b0: 6d62 6572 206f 6620 7469 636b 7320 7369  mber of ticks si
-000137c0: 6e63 6520 6974 2072 6561 6368 6564 206c  nce it reached l
-000137d0: 6173 7420 656c 6563 7469 6f6e 5469 6d65  ast electionTime
-000137e0: 6f75 7420 6f72 2072 6563 6569 7665 6420  out or received 
-000137f0: 610a 2020 2020 2020 2020 7661 6c69 6420  a.        valid 
-00013800: 6d65 7373 6167 6520 6672 6f6d 2063 7572  message from cur
-00013810: 7265 6e74 206c 6561 6465 7220 7768 656e  rent leader when
-00013820: 2069 7420 6973 2061 2066 6f6c 6c6f 7765   it is a followe
-00013830: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-00013840: 2020 2064 6566 2073 6574 5f65 6c65 6374     def set_elect
-00013850: 696f 6e5f 656c 6170 7365 6428 7365 6c66  ion_elapsed(self
-00013860: 2c20 656c 6563 7469 6f6e 5f65 6c61 7073  , election_elaps
-00013870: 6564 3a20 696e 7429 202d 3e20 4e6f 6e65  ed: int) -> None
-00013880: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013890: 2020 2020 2020 6065 6c65 6374 696f 6e5f        `election_
-000138a0: 656c 6170 7365 6460 3a20 5469 636b 7320  elapsed`: Ticks 
-000138b0: 7369 6e63 6520 6974 2072 6561 6368 6564  since it reached
-000138c0: 206c 6173 7420 656c 6563 7469 6f6e 5469   last electionTi
-000138d0: 6d65 6f75 7420 7768 656e 2069 7420 6973  meout when it is
-000138e0: 206c 6561 6465 7220 6f72 2063 616e 6469   leader or candi
-000138f0: 6461 7465 2e0a 2020 2020 2020 2020 4e75  date..        Nu
-00013900: 6d62 6572 206f 6620 7469 636b 7320 7369  mber of ticks si
-00013910: 6e63 6520 6974 2072 6561 6368 6564 206c  nce it reached l
-00013920: 6173 7420 656c 6563 7469 6f6e 5469 6d65  ast electionTime
-00013930: 6f75 7420 6f72 2072 6563 6569 7665 6420  out or received 
-00013940: 610a 2020 2020 2020 2020 7661 6c69 6420  a.        valid 
-00013950: 6d65 7373 6167 6520 6672 6f6d 2063 7572  message from cur
-00013960: 7265 6e74 206c 6561 6465 7220 7768 656e  rent leader when
-00013970: 2069 7420 6973 2061 2066 6f6c 6c6f 7765   it is a followe
-00013980: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-00013990: 2020 2064 6566 2067 6574 5f63 6865 636b     def get_check
-000139a0: 5f71 756f 7275 6d28 7365 6c66 2920 2d3e  _quorum(self) ->
-000139b0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-000139c0: 2222 0a20 2020 2020 2020 2060 6368 6563  "".        `chec
-000139d0: 6b5f 7175 6f72 756d 603a 2057 6865 7468  k_quorum`: Wheth
-000139e0: 6572 2074 6f20 6368 6563 6b20 7468 6520  er to check the 
-000139f0: 7175 6f72 756d 0a20 2020 2020 2020 2022  quorum.        "
-00013a00: 2222 0a20 2020 2064 6566 2073 6574 5f63  "".    def set_c
-00013a10: 6865 636b 5f71 756f 7275 6d28 7365 6c66  heck_quorum(self
-00013a20: 2c20 6368 6563 6b5f 7175 6f72 756d 3a20  , check_quorum: 
-00013a30: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-00013a40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013a50: 2020 2060 6368 6563 6b5f 7175 6f72 756d     `check_quorum
-00013a60: 603a 2057 6865 7468 6572 2074 6f20 6368  `: Whether to ch
-00013a70: 6563 6b20 7468 6520 7175 6f72 756d 0a20  eck the quorum. 
-00013a80: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00013a90: 6566 2067 6574 5f70 7265 5f76 6f74 6528  ef get_pre_vote(
-00013aa0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-00013ab0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013ac0: 2020 2060 7072 655f 766f 7465 603a 2045     `pre_vote`: E
-00013ad0: 6e61 626c 6520 7468 6520 7072 6576 6f74  nable the prevot
-00013ae0: 6520 616c 676f 7269 7468 6d2e 0a0a 2020  e algorithm...  
-00013af0: 2020 2020 2020 5468 6973 2065 6e61 626c        This enabl
-00013b00: 6573 2061 2070 7265 2d65 6c65 6374 696f  es a pre-electio
-00013b10: 6e20 766f 7465 2072 6f75 6e64 206f 6e20  n vote round on 
-00013b20: 4361 6e64 6964 6174 6573 2070 7269 6f72  Candidates prior
-00013b30: 2074 6f20 6469 7372 7570 7469 6e67 2074   to disrupting t
-00013b40: 6865 2063 6c75 7374 6572 2e0a 0a20 2020  he cluster...   
-00013b50: 2020 2020 2045 6e61 626c 6520 7468 6973       Enable this
-00013b60: 2069 6620 6772 6561 7465 7220 636c 7573   if greater clus
-00013b70: 7465 7220 7374 6162 696c 6974 7920 6973  ter stability is
-00013b80: 2070 7265 6665 7272 6564 206f 7665 7220   preferred over 
-00013b90: 6661 7374 6572 2065 6c65 6374 696f 6e73  faster elections
-00013ba0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00013bb0: 2020 6465 6620 7365 745f 7072 655f 766f    def set_pre_vo
-00013bc0: 7465 2873 656c 662c 2070 7265 5f76 6f74  te(self, pre_vot
-00013bd0: 653a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  e: bool) -> None
-00013be0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00013bf0: 2020 2020 2020 6070 7265 5f76 6f74 6560        `pre_vote`
-00013c00: 3a20 456e 6162 6c65 2074 6865 2070 7265  : Enable the pre
-00013c10: 766f 7465 2061 6c67 6f72 6974 686d 2e0a  vote algorithm..
-00013c20: 0a20 2020 2020 2020 2054 6869 7320 656e  .        This en
-00013c30: 6162 6c65 7320 6120 7072 652d 656c 6563  ables a pre-elec
-00013c40: 7469 6f6e 2076 6f74 6520 726f 756e 6420  tion vote round 
-00013c50: 6f6e 2043 616e 6469 6461 7465 7320 7072  on Candidates pr
-00013c60: 696f 7220 746f 2064 6973 7275 7074 696e  ior to disruptin
-00013c70: 6720 7468 6520 636c 7573 7465 722e 0a0a  g the cluster...
-00013c80: 2020 2020 2020 2020 456e 6162 6c65 2074          Enable t
-00013c90: 6869 7320 6966 2067 7265 6174 6572 2063  his if greater c
-00013ca0: 6c75 7374 6572 2073 7461 6269 6c69 7479  luster stability
-00013cb0: 2069 7320 7072 6566 6572 7265 6420 6f76   is preferred ov
-00013cc0: 6572 2066 6173 7465 7220 656c 6563 7469  er faster electi
-00013cd0: 6f6e 732e 0a20 2020 2020 2020 2022 2222  ons..        """
-00013ce0: 0a20 2020 2064 6566 2061 7070 6c79 5f63  .    def apply_c
-00013cf0: 6f6e 665f 6368 616e 6765 2873 656c 662c  onf_change(self,
-00013d00: 2063 6f6e 665f 6368 616e 6765 3a20 2243   conf_change: "C
-00013d10: 6f6e 6643 6861 6e67 6556 3252 6566 2229  onfChangeV2Ref")
-00013d20: 202d 3e20 2243 6f6e 6643 6861 6e67 6552   -> "ConfChangeR
-00013d30: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-00013d40: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00013d50: 5f72 6561 645f 7374 6174 6573 2873 656c  _read_states(sel
-00013d60: 6629 202d 3e20 4c69 7374 5b22 5265 6164  f) -> List["Read
-00013d70: 5374 6174 6522 5d3a 0a20 2020 2020 2020  State"]:.       
-00013d80: 2022 2222 0a20 2020 2020 2020 2060 7265   """.        `re
-00013d90: 6164 5f73 7461 7465 7360 3a20 5468 6520  ad_states`: The 
-00013da0: 6375 7272 656e 7420 7265 6164 2073 7461  current read sta
-00013db0: 7465 732e 0a20 2020 2020 2020 2022 2222  tes..        """
-00013dc0: 0a20 2020 2064 6566 2073 6574 5f72 6561  .    def set_rea
-00013dd0: 645f 7374 6174 6573 280a 2020 2020 2020  d_states(.      
-00013de0: 2020 7365 6c66 2c20 7265 6164 5f73 7461    self, read_sta
-00013df0: 7465 733a 204c 6973 745b 2252 6561 6453  tes: List["ReadS
-00013e00: 7461 7465 225d 207c 204c 6973 745b 2252  tate"] | List["R
-00013e10: 6561 6453 7461 7465 5265 6622 5d0a 2020  eadStateRef"].  
-00013e20: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-00013e30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013e40: 2060 7265 6164 5f73 7461 7465 7360 3a20   `read_states`: 
-00013e50: 5468 6520 6375 7272 656e 7420 7265 6164  The current read
-00013e60: 2073 7461 7465 732e 0a20 2020 2020 2020   states..       
-00013e70: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00013e80: 5f72 6561 645f 6f6e 6c79 5f6f 7074 696f  _read_only_optio
-00013e90: 6e28 7365 6c66 2920 2d3e 2022 5265 6164  n(self) -> "Read
-00013ea0: 4f6e 6c79 4f70 7469 6f6e 223a 0a20 2020  OnlyOption":.   
-00013eb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013ec0: 2060 7265 6164 5f6f 6e6c 795f 6f70 7469   `read_only_opti
-00013ed0: 6f6e 603a 2043 686f 6f73 6520 7468 6520  on`: Choose the 
-00013ee0: 6c69 6e65 6172 697a 6162 696c 6974 7920  linearizability 
-00013ef0: 6d6f 6465 206f 7220 7468 6520 6c65 6173  mode or the leas
-00013f00: 6520 6d6f 6465 2074 6f20 7265 6164 2064  e mode to read d
-00013f10: 6174 612e 2049 6620 796f 7520 646f 6ee2  ata. If you don.
-00013f20: 8099 7420 6361 7265 2061 626f 7574 2074  ..t care about t
-00013f30: 6865 2072 6561 6420 636f 6e73 6973 7465  he read consiste
-00013f40: 6e63 7920 616e 6420 7761 6e74 2061 2068  ncy and want a h
-00013f50: 6967 6865 7220 7265 6164 2070 6572 666f  igher read perfo
-00013f60: 726d 616e 6365 2c20 796f 7520 6361 6e20  rmance, you can 
-00013f70: 7573 6520 7468 6520 6c65 6173 6520 6d6f  use the lease mo
-00013f80: 6465 2e0a 2020 2020 2020 2020 5365 7474  de..        Sett
-00013f90: 696e 6720 7468 6973 2074 6f20 604c 6561  ing this to `Lea
-00013fa0: 7365 4261 7365 6460 2072 6571 7569 7265  seBased` require
-00013fb0: 7320 6063 6865 636b 5f71 756f 7275 6d20  s `check_quorum 
-00013fc0: 3d20 7472 7565 602e 0a20 2020 2020 2020  = true`..       
-00013fd0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00013fe0: 5f72 6561 645f 6f6e 6c79 5f6f 7074 696f  _read_only_optio
-00013ff0: 6e28 7365 6c66 2c20 6f70 7469 6f6e 3a20  n(self, option: 
-00014000: 2252 6561 644f 6e6c 794f 7074 696f 6e22  "ReadOnlyOption"
-00014010: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00014020: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00014030: 7265 6164 5f6f 6e6c 795f 6f70 7469 6f6e  read_only_option
-00014040: 603a 2043 686f 6f73 6520 7468 6520 6c69  `: Choose the li
-00014050: 6e65 6172 697a 6162 696c 6974 7920 6d6f  nearizability mo
-00014060: 6465 206f 7220 7468 6520 6c65 6173 6520  de or the lease 
-00014070: 6d6f 6465 2074 6f20 7265 6164 2064 6174  mode to read dat
-00014080: 612e 2049 6620 796f 7520 646f 6ee2 8099  a. If you don...
-00014090: 7420 6361 7265 2061 626f 7574 2074 6865  t care about the
-000140a0: 2072 6561 6420 636f 6e73 6973 7465 6e63   read consistenc
-000140b0: 7920 616e 6420 7761 6e74 2061 2068 6967  y and want a hig
-000140c0: 6865 7220 7265 6164 2070 6572 666f 726d  her read perform
-000140d0: 616e 6365 2c20 796f 7520 6361 6e20 7573  ance, you can us
-000140e0: 6520 7468 6520 6c65 6173 6520 6d6f 6465  e the lease mode
-000140f0: 2e0a 2020 2020 2020 2020 5365 7474 696e  ..        Settin
-00014100: 6720 7468 6973 2074 6f20 604c 6561 7365  g this to `Lease
-00014110: 4261 7365 6460 2072 6571 7569 7265 7320  Based` requires 
-00014120: 6063 6865 636b 5f71 756f 7275 6d20 3d20  `check_quorum = 
-00014130: 7472 7565 602e 0a20 2020 2020 2020 2022  true`..        "
-00014140: 2222 0a20 2020 2064 6566 2069 6e66 6c69  "".    def infli
-00014150: 6768 745f 6275 6666 6572 735f 7369 7a65  ght_buffers_size
-00014160: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00014170: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-00014180: 6520 696e 666c 6967 6874 2062 7566 6665  e inflight buffe
-00014190: 7220 7369 7a65 2e22 2222 0a20 2020 2064  r size.""".    d
-000141a0: 6566 206d 6179 6265 5f66 7265 655f 696e  ef maybe_free_in
-000141b0: 666c 6967 6874 5f62 7566 6665 7273 2873  flight_buffers(s
-000141c0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-000141d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000141e0: 2020 4120 5261 6674 206c 6561 6465 7220    A Raft leader 
-000141f0: 616c 6c6f 6361 7465 7320 6120 7665 6374  allocates a vect
-00014200: 6f72 2077 6974 6820 6361 7061 6369 7479  or with capacity
-00014210: 2060 6d61 785f 696e 666c 6967 6874 5f6d   `max_inflight_m
-00014220: 7367 7360 2066 6f72 2065 7665 7279 2070  sgs` for every p
-00014230: 6565 722e 0a20 2020 2020 2020 2049 7420  eer..        It 
-00014240: 7461 6b65 7320 6120 6c6f 7420 6f66 206d  takes a lot of m
-00014250: 656d 6f72 7920 6966 2074 6865 7265 2061  emory if there a
-00014260: 7265 2074 6f6f 206d 616e 7920 5261 6674  re too many Raft
-00014270: 2067 726f 7570 732e 2060 6d61 7962 655f   groups. `maybe_
-00014280: 6672 6565 5f69 6e66 6c69 6768 745f 6275  free_inflight_bu
-00014290: 6666 6572 7360 0a20 2020 2020 2020 2069  ffers`.        i
-000142a0: 7320 7573 6564 2074 6f20 6672 6565 206d  s used to free m
-000142b0: 656d 6f72 7920 6966 206e 6563 6573 7361  emory if necessa
-000142c0: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
-000142d0: 2020 2020 6465 6620 6164 6a75 7374 5f6d      def adjust_m
-000142e0: 6178 5f69 6e66 6c69 6768 745f 6d73 6773  ax_inflight_msgs
-000142f0: 2873 656c 662c 2074 6172 6765 743a 2069  (self, target: i
-00014300: 6e74 2c20 6361 703a 2069 6e74 2920 2d3e  nt, cap: int) ->
-00014310: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00014320: 2222 0a20 2020 2020 2020 2054 6f20 6164  "".        To ad
-00014330: 6a75 7374 2060 6d61 785f 696e 666c 6967  just `max_inflig
-00014340: 6874 5f6d 7367 7360 2066 6f72 2074 6865  ht_msgs` for the
-00014350: 2073 7065 6369 6669 6564 2070 6565 722e   specified peer.
-00014360: 0a20 2020 2020 2020 2053 6574 2074 6f20  .        Set to 
-00014370: 6030 6020 7769 6c6c 2064 6973 6162 6c65  `0` will disable
-00014380: 2074 6865 2070 726f 6772 6573 732e 0a20   the progress.. 
-00014390: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-000143a0: 6566 2067 6574 5f72 6561 646f 6e6c 795f  ef get_readonly_
-000143b0: 7265 6164 5f69 6e64 6578 5f71 7565 7565  read_index_queue
-000143c0: 2873 656c 6629 202d 3e20 4c69 7374 5b4c  (self) -> List[L
-000143d0: 6973 745b 696e 745d 5d3a 0a20 2020 2020  ist[int]]:.     
-000143e0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-000143f0: 6566 2073 6574 5f62 6174 6368 5f61 7070  ef set_batch_app
-00014400: 656e 6428 7365 6c66 2c20 6261 7463 685f  end(self, batch_
-00014410: 6170 7065 6e64 3a20 626f 6f6c 2920 2d3e  append: bool) ->
-00014420: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00014430: 2222 0a20 2020 2020 2020 2053 6574 2077  "".        Set w
-00014440: 6865 7468 6572 2062 6174 6368 2061 7070  hether batch app
-00014450: 656e 6420 6d73 6720 6174 2072 756e 7469  end msg at runti
-00014460: 6d65 2e0a 2020 2020 2020 2020 2222 220a  me..        """.
-00014470: 2020 2020 6465 6620 7365 745f 6d61 785f      def set_max_
-00014480: 636f 6d6d 6974 7465 645f 7369 7a65 5f70  committed_size_p
-00014490: 6572 5f72 6561 6479 2873 656c 662c 2073  er_ready(self, s
-000144a0: 697a 653a 2069 6e74 2920 2d3e 204e 6f6e  ize: int) -> Non
-000144b0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000144c0: 2020 2020 2020 2053 6574 2060 6d61 785f         Set `max_
-000144d0: 636f 6d6d 6974 7465 645f 7369 7a65 5f70  committed_size_p
-000144e0: 6572 5f72 6561 6479 6020 746f 2060 7369  er_ready` to `si
-000144f0: 7a65 602e 0a20 2020 2020 2020 2022 2222  ze`..        """
-00014500: 0a0a 636c 6173 7320 496e 4d65 6d6f 7279  ..class InMemory
-00014510: 5261 6674 285f 5f41 5049 5f52 6166 7429  Raft(__API_Raft)
-00014520: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
-00014530: 7374 7275 6374 2074 6861 7420 7265 7072  struct that repr
-00014540: 6573 656e 7473 2074 6865 2072 6166 7420  esents the raft 
-00014550: 636f 6e73 656e 7375 7320 6974 7365 6c66  consensus itself
-00014560: 2e20 5374 6f72 6573 2064 6574 6169 6c73  . Stores details
-00014570: 2063 6f6e 6365 726e 696e 6720 7468 6520   concerning the 
-00014580: 6375 7272 656e 740a 2020 2020 616e 6420  current.    and 
-00014590: 706f 7373 6962 6c65 2073 7461 7465 2074  possible state t
-000145a0: 6865 2073 7973 7465 6d20 6361 6e20 7461  he system can ta
-000145b0: 6b65 2e0a 2020 2020 2222 220a 0a20 2020  ke..    """..   
-000145c0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000145d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000145e0: 2020 2020 2063 6667 3a20 2243 6f6e 6669       cfg: "Confi
-000145f0: 6722 207c 2022 436f 6e66 6967 5265 6622  g" | "ConfigRef"
-00014600: 2c0a 2020 2020 2020 2020 7374 6f72 653a  ,.        store:
-00014610: 2022 4d65 6d53 746f 7261 6765 2220 7c20   "MemStorage" | 
-00014620: 224d 656d 5374 6f72 6167 6552 6566 222c  "MemStorageRef",
-00014630: 0a20 2020 2020 2020 206c 6f67 6765 723a  .        logger:
-00014640: 2022 4c6f 6767 6572 2220 7c20 224c 6f67   "Logger" | "Log
-00014650: 6765 7252 6566 222c 0a20 2020 2029 202d  gerRef",.    ) -
-00014660: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00014670: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
-00014680: 6629 202d 3e20 2249 6e4d 656d 6f72 7952  f) -> "InMemoryR
-00014690: 6166 7452 6566 223a 202e 2e2e 0a20 2020  aftRef": ....   
-000146a0: 2064 6566 2067 6574 5f72 6166 745f 6c6f   def get_raft_lo
-000146b0: 6728 7365 6c66 2920 2d3e 2022 496e 4d65  g(self) -> "InMe
-000146c0: 6d6f 7279 5261 6674 4c6f 6752 6566 223a  moryRaftLogRef":
-000146d0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-000146e0: 0a0a 636c 6173 7320 496e 4d65 6d6f 7279  ..class InMemory
-000146f0: 5261 6674 5265 6628 5f5f 4150 495f 5261  RaftRef(__API_Ra
-00014700: 6674 293a 0a20 2020 2022 2222 0a20 2020  ft):.    """.   
-00014710: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-00014720: 6f66 203a 636c 6173 733a 6049 6e4d 656d  of :class:`InMem
-00014730: 6f72 7952 6166 7460 2e0a 2020 2020 2222  oryRaft`..    ""
-00014740: 220a 0a20 2020 2064 6566 2067 6574 5f72  "..    def get_r
-00014750: 6166 745f 6c6f 6728 7365 6c66 2920 2d3e  aft_log(self) ->
-00014760: 2022 496e 4d65 6d6f 7279 5261 6674 4c6f   "InMemoryRaftLo
-00014770: 6752 6566 223a 0a20 2020 2020 2020 2022  gRef":.        "
-00014780: 2222 2022 2222 0a0a 636c 6173 7320 5261  "" """..class Ra
-00014790: 6674 285f 5f41 5049 5f52 6166 7429 3a0a  ft(__API_Raft):.
-000147a0: 2020 2020 2222 220a 2020 2020 4120 7374      """.    A st
-000147b0: 7275 6374 2074 6861 7420 7265 7072 6573  ruct that repres
-000147c0: 656e 7473 2074 6865 2072 6166 7420 636f  ents the raft co
-000147d0: 6e73 656e 7375 7320 6974 7365 6c66 2e20  nsensus itself. 
-000147e0: 5374 6f72 6573 2064 6574 6169 6c73 2063  Stores details c
-000147f0: 6f6e 6365 726e 696e 6720 7468 6520 6375  oncerning the cu
-00014800: 7272 656e 740a 2020 2020 616e 6420 706f  rrent.    and po
-00014810: 7373 6962 6c65 2073 7461 7465 2074 6865  ssible state the
-00014820: 2073 7973 7465 6d20 6361 6e20 7461 6b65   system can take
-00014830: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00014840: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00014850: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00014860: 2020 2063 6667 3a20 2243 6f6e 6669 6722     cfg: "Config"
-00014870: 207c 2022 436f 6e66 6967 5265 6622 2c0a   | "ConfigRef",.
-00014880: 2020 2020 2020 2020 7374 6f72 653a 2022          store: "
-00014890: 5374 6f72 6167 6522 207c 2022 5374 6f72  Storage" | "Stor
-000148a0: 6167 6552 6566 222c 0a20 2020 2020 2020  ageRef",.       
-000148b0: 206c 6f67 6765 723a 2022 4c6f 6767 6572   logger: "Logger
-000148c0: 2220 7c20 224c 6f67 6765 7252 6566 222c  " | "LoggerRef",
-000148d0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
-000148e0: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-000148f0: 5f72 6566 2873 656c 6629 202d 3e20 2252  _ref(self) -> "R
-00014900: 6166 7452 6566 223a 202e 2e2e 0a20 2020  aftRef": ....   
-00014910: 2064 6566 2067 6574 5f72 6166 745f 6c6f   def get_raft_lo
-00014920: 6728 7365 6c66 2920 2d3e 2022 5261 6674  g(self) -> "Raft
-00014930: 4c6f 6752 6566 223a 0a20 2020 2020 2020  LogRef":.       
-00014940: 2022 2222 2022 2222 0a0a 636c 6173 7320   """ """..class 
-00014950: 5261 6674 5265 6628 5f5f 4150 495f 5261  RaftRef(__API_Ra
-00014960: 6674 293a 0a20 2020 2022 2222 0a20 2020  ft):.    """.   
-00014970: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-00014980: 6f66 203a 636c 6173 733a 6052 6166 7460  of :class:`Raft`
-00014990: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-000149a0: 6566 2067 6574 5f72 6166 745f 6c6f 6728  ef get_raft_log(
-000149b0: 7365 6c66 2920 2d3e 2022 5261 6674 4c6f  self) -> "RaftLo
-000149c0: 6752 6566 223a 0a20 2020 2020 2020 2022  gRef":.        "
-000149d0: 2222 2022 2222 0a0a 636c 6173 7320 5072  "" """..class Pr
-000149e0: 6f67 7265 7373 4d61 7049 7465 6d3a 0a20  ogressMapItem:. 
-000149f0: 2020 2064 6566 2069 6428 7365 6c66 2920     def id(self) 
-00014a00: 2d3e 2069 6e74 3a20 2e2e 2e0a 2020 2020  -> int: ....    
-00014a10: 6465 6620 7072 6f67 7265 7373 2873 656c  def progress(sel
-00014a20: 6629 202d 3e20 2250 726f 6772 6573 7322  f) -> "Progress"
-00014a30: 3a20 2e2e 2e0a 0a63 6c61 7373 205f 5f41  : .....class __A
-00014a40: 5049 5f50 726f 6772 6573 7354 7261 636b  PI_ProgressTrack
-00014a50: 6572 285f 5f43 6c6f 6e65 6162 6c65 293a  er(__Cloneable):
-00014a60: 0a20 2020 2064 6566 2063 6c6f 6e65 2873  .    def clone(s
-00014a70: 656c 6629 202d 3e20 2250 726f 6772 6573  elf) -> "Progres
-00014a80: 7354 7261 636b 6572 223a 202e 2e2e 0a20  sTracker": .... 
-00014a90: 2020 2064 6566 2067 6574 2873 656c 662c     def get(self,
-00014aa0: 2069 643a 2069 6e74 2920 2d3e 204f 7074   id: int) -> Opt
-00014ab0: 696f 6e61 6c5b 2250 726f 6772 6573 7352  ional["ProgressR
-00014ac0: 6566 225d 3a0a 2020 2020 2020 2020 2222  ef"]:.        ""
-00014ad0: 2222 2222 0a20 2020 2064 6566 2067 726f  """".    def gro
-00014ae0: 7570 5f63 6f6d 6d69 7428 7365 6c66 2920  up_commit(self) 
-00014af0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00014b00: 2022 2222 0a20 2020 2020 2020 2057 6865   """.        Whe
-00014b10: 7468 6572 2065 6e61 626c 6520 6772 6f75  ther enable grou
-00014b20: 7020 636f 6d6d 6974 2e0a 2020 2020 2020  p commit..      
-00014b30: 2020 2222 220a 2020 2020 6465 6620 656e    """.    def en
-00014b40: 6162 6c65 5f67 726f 7570 5f63 6f6d 6d69  able_group_commi
-00014b50: 7428 7365 6c66 2c20 656e 6162 6c65 3a20  t(self, enable: 
-00014b60: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-00014b70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014b80: 2020 2043 6f6e 6669 6775 7265 7320 6772     Configures gr
-00014b90: 6f75 7020 636f 6d6d 6974 2e0a 2020 2020  oup commit..    
-00014ba0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00014bb0: 6861 735f 7175 6f72 756d 2873 656c 662c  has_quorum(self,
-00014bc0: 2070 6f74 656e 7469 616c 5f71 756f 7275   potential_quoru
-00014bd0: 6d3a 2053 6574 5b69 6e74 5d29 202d 3e20  m: Set[int]) -> 
-00014be0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00014bf0: 220a 2020 2020 2020 2020 4465 7465 726d  ".        Determ
-00014c00: 696e 6520 6966 2061 2071 756f 7275 6d20  ine if a quorum 
-00014c10: 6973 2066 6f72 6d65 6420 6672 6f6d 2074  is formed from t
-00014c20: 6865 2067 6976 656e 2073 6574 206f 6620  he given set of 
-00014c30: 6e6f 6465 732e 0a0a 2020 2020 2020 2020  nodes...        
-00014c40: 5468 6973 2069 7320 7468 6520 6f6e 6c79  This is the only
-00014c50: 2063 6f72 7265 6374 2077 6179 2074 6f20   correct way to 
-00014c60: 7665 7269 6679 2079 6f75 2068 6176 6520  verify you have 
-00014c70: 7265 6163 6865 6420 6120 7175 6f72 756d  reached a quorum
-00014c80: 2066 6f72 2074 6865 2077 686f 6c65 2067   for the whole g
-00014c90: 726f 7570 2e0a 2020 2020 2020 2020 2222  roup..        ""
-00014ca0: 220a 2020 2020 6465 6620 6973 5f73 696e  ".    def is_sin
-00014cb0: 676c 6574 6f6e 2873 656c 6629 202d 3e20  gleton(self) -> 
-00014cc0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00014cd0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-00014ce0: 7320 7472 7565 2069 6620 2861 6e64 206f  s true if (and o
-00014cf0: 6e6c 7920 6966 2920 7468 6572 6520 6973  nly if) there is
-00014d00: 206f 6e6c 7920 6f6e 6520 766f 7469 6e67   only one voting
-00014d10: 206d 656d 6265 720a 2020 2020 2020 2020   member.        
-00014d20: 2869 2e65 2e20 7468 6520 6c65 6164 6572  (i.e. the leader
-00014d30: 2920 696e 2074 6865 2063 7572 7265 6e74  ) in the current
-00014d40: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0a   configuration..
-00014d50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014d60: 6465 6620 7175 6f72 756d 5f72 6563 656e  def quorum_recen
-00014d70: 746c 795f 6163 7469 7665 2873 656c 662c  tly_active(self,
-00014d80: 2070 6572 7370 6563 7469 7665 5f6f 663a   perspective_of:
-00014d90: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
-00014da0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014db0: 2020 2044 6574 6572 6d69 6e65 7320 6966     Determines if
-00014dc0: 2074 6865 2063 7572 7265 6e74 2071 756f   the current quo
-00014dd0: 7275 6d20 6973 2061 6374 6976 6520 6163  rum is active ac
-00014de0: 636f 7264 696e 6720 746f 2074 6865 2074  cording to the t
-00014df0: 6869 7320 7261 6674 206e 6f64 652e 0a20  his raft node.. 
-00014e00: 2020 2020 2020 2044 6f69 6e67 2074 6869         Doing thi
-00014e10: 7320 7769 6c6c 2073 6574 2074 6865 2060  s will set the `
-00014e20: 7265 6365 6e74 5f61 6374 6976 6560 206f  recent_active` o
-00014e30: 6620 6561 6368 2070 6565 7220 746f 2066  f each peer to f
-00014e40: 616c 7365 2e0a 0a20 2020 2020 2020 2054  alse...        T
-00014e50: 6869 7320 7368 6f75 6c64 206f 6e6c 7920  his should only 
-00014e60: 6265 2063 616c 6c65 6420 6279 2074 6865  be called by the
-00014e70: 206c 6561 6465 722e 0a20 2020 2020 2020   leader..       
-00014e80: 2022 2222 0a20 2020 2064 6566 206d 6178   """.    def max
-00014e90: 696d 616c 5f63 6f6d 6d69 7474 6564 5f69  imal_committed_i
-00014ea0: 6e64 6578 2873 656c 6629 202d 3e20 5475  ndex(self) -> Tu
-00014eb0: 706c 655b 696e 742c 2062 6f6f 6c5d 3a0a  ple[int, bool]:.
-00014ec0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014ed0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
-00014ee0: 6d61 7869 6d61 6c20 636f 6d6d 6974 7465  maximal committe
-00014ef0: 6420 696e 6465 7820 666f 7220 7468 6520  d index for the 
-00014f00: 636c 7573 7465 722e 2054 6865 2062 6f6f  cluster. The boo
-00014f10: 6c20 666c 6167 2069 6e64 6963 6174 6573  l flag indicates
-00014f20: 2077 6865 7468 6572 0a20 2020 2020 2020   whether.       
-00014f30: 2074 6865 2069 6e64 6578 2069 7320 636f   the index is co
-00014f40: 6d70 7574 6564 2062 7920 6772 6f75 7020  mputed by group 
-00014f50: 636f 6d6d 6974 2061 6c67 6f72 6974 686d  commit algorithm
-00014f60: 2073 7563 6365 7373 6675 6c6c 790a 0a20   successfully.. 
-00014f70: 2020 2020 2020 2045 672e 2049 6620 7468         Eg. If th
-00014f80: 6520 6d61 7463 6865 6420 696e 6465 7865  e matched indexe
-00014f90: 7320 6172 6520 605b 322c 322c 322c 342c  s are `[2,2,2,4,
-00014fa0: 355d 602c 2069 7420 7769 6c6c 2072 6574  5]`, it will ret
-00014fb0: 7572 6e20 6032 602e 0a20 2020 2020 2020  urn `2`..       
-00014fc0: 2049 6620 7468 6520 6d61 7463 6865 6420   If the matched 
-00014fd0: 696e 6465 7865 7320 616e 6420 6772 6f75  indexes and grou
-00014fe0: 7073 2061 7265 2060 5b28 312c 2031 292c  ps are `[(1, 1),
-00014ff0: 2028 322c 2032 292c 2028 332c 2032 295d   (2, 2), (3, 2)]
-00015000: 602c 2069 7420 7769 6c6c 2072 6574 7572  `, it will retur
-00015010: 6e20 6031 602e 0a20 2020 2020 2020 2022  n `1`..        "
-00015020: 2222 0a20 2020 2064 6566 2072 6563 6f72  "".    def recor
-00015030: 645f 766f 7465 2873 656c 662c 2069 643a  d_vote(self, id:
-00015040: 2069 6e74 2c20 766f 7465 3a20 626f 6f6c   int, vote: bool
-00015050: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00015060: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00015070: 6563 6f72 6473 2074 6861 7420 7468 6520  ecords that the 
-00015080: 6e6f 6465 2077 6974 6820 7468 6520 6769  node with the gi
-00015090: 7665 6e20 6964 2076 6f74 6564 2066 6f72  ven id voted for
-000150a0: 2074 6869 7320 5261 6674 0a20 2020 2020   this Raft.     
-000150b0: 2020 2069 6e73 7461 6e63 6520 6966 2076     instance if v
-000150c0: 203d 3d20 7472 7565 2028 616e 6420 6465   == true (and de
-000150d0: 636c 696e 6564 2069 7420 6f74 6865 7277  clined it otherw
-000150e0: 6973 6529 2e0a 2020 2020 2020 2020 2222  ise)..        ""
-000150f0: 220a 2020 2020 6465 6620 7265 7365 745f  ".    def reset_
-00015100: 766f 7465 7328 7365 6c66 2920 2d3e 204e  votes(self) -> N
-00015110: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00015120: 0a20 2020 2020 2020 2050 7265 7061 7265  .        Prepare
-00015130: 7320 666f 7220 6120 6e65 7720 726f 756e  s for a new roun
-00015140: 6420 6f66 2076 6f74 6520 636f 756e 7469  d of vote counti
-00015150: 6e67 2076 6961 2072 6563 6f72 6456 6f74  ng via recordVot
-00015160: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00015170: 2020 2064 6566 2063 6f6e 665f 766f 7465     def conf_vote
-00015180: 7273 2873 656c 6629 202d 3e20 224a 6f69  rs(self) -> "Joi
-00015190: 6e74 436f 6e66 6967 5265 6622 3a0a 2020  ntConfigRef":.  
-000151a0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-000151b0: 2020 6465 6620 636f 6e66 5f6c 6561 726e    def conf_learn
-000151c0: 6572 7328 7365 6c66 2920 2d3e 2053 6574  ers(self) -> Set
-000151d0: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
-000151e0: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-000151f0: 6f6c 6c65 6374 2873 656c 6629 202d 3e20  ollect(self) -> 
-00015200: 4c69 7374 5b22 5072 6f67 7265 7373 4d61  List["ProgressMa
-00015210: 7049 7465 6d22 5d3a 0a20 2020 2020 2020  pItem"]:.       
-00015220: 2022 2222 2022 2222 0a0a 636c 6173 7320   """ """..class 
-00015230: 5072 6f67 7265 7373 5472 6163 6b65 7228  ProgressTracker(
-00015240: 5f5f 4150 495f 5072 6f67 7265 7373 5472  __API_ProgressTr
-00015250: 6163 6b65 7229 3a0a 2020 2020 2222 220a  acker):.    """.
-00015260: 2020 2020 6050 726f 6772 6573 7354 7261      `ProgressTra
-00015270: 636b 6572 6020 636f 6e74 6169 6e73 2073  cker` contains s
-00015280: 6576 6572 616c 2060 5072 6f67 7265 7373  everal `Progress
-00015290: 6065 732c 0a20 2020 2077 6869 6368 2063  `es,.    which c
-000152a0: 6f75 6c64 2062 6520 604c 6561 6465 7260  ould be `Leader`
-000152b0: 2c20 6046 6f6c 6c6f 7765 7260 2061 6e64  , `Follower` and
-000152c0: 2060 4c65 6172 6e65 7260 2e0a 2020 2020   `Learner`..    
-000152d0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-000152e0: 6e69 745f 5f28 7365 6c66 2c20 6d61 785f  nit__(self, max_
-000152f0: 696e 666c 6967 6874 3a20 696e 7429 202d  inflight: int) -
-00015300: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00015310: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
-00015320: 6629 202d 3e20 2250 726f 6772 6573 7354  f) -> "ProgressT
-00015330: 7261 636b 6572 5265 6622 3a20 2e2e 2e0a  rackerRef": ....
-00015340: 0a63 6c61 7373 2050 726f 6772 6573 7354  .class ProgressT
-00015350: 7261 636b 6572 5265 6628 5f5f 4150 495f  rackerRef(__API_
-00015360: 5072 6f67 7265 7373 5472 6163 6b65 7229  ProgressTracker)
-00015370: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00015380: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
-00015390: 3a63 6c61 7373 3a60 5072 6f67 7265 7373  :class:`Progress
-000153a0: 5472 6163 6b65 7260 2e0a 2020 2020 2222  Tracker`..    ""
-000153b0: 220a 0a63 6c61 7373 205f 5f41 5049 5f50  "..class __API_P
-000153c0: 726f 6772 6573 7328 5f5f 436c 6f6e 6561  rogress(__Clonea
-000153d0: 626c 6529 3a0a 2020 2020 6465 6620 636c  ble):.    def cl
-000153e0: 6f6e 6528 7365 6c66 2920 2d3e 2022 5072  one(self) -> "Pr
-000153f0: 6f67 7265 7373 223a 202e 2e2e 0a20 2020  ogress": ....   
-00015400: 2064 6566 2062 6563 6f6d 655f 7072 6f62   def become_prob
-00015410: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-00015420: 0a20 2020 2020 2020 2022 2222 4368 616e  .        """Chan
-00015430: 6765 7320 7468 6520 7072 6f67 7265 7373  ges the progress
-00015440: 2074 6f20 6120 7072 6f62 652e 2222 220a   to a probe.""".
-00015450: 2020 2020 6465 6620 6265 636f 6d65 5f72      def become_r
-00015460: 6570 6c69 6361 7465 2873 656c 6629 202d  eplicate(self) -
-00015470: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00015480: 2222 2243 6861 6e67 6573 2074 6865 2070  """Changes the p
-00015490: 726f 6772 6573 7320 746f 2061 2052 6570  rogress to a Rep
-000154a0: 6c69 6361 7465 2e22 2222 0a20 2020 2064  licate.""".    d
-000154b0: 6566 2062 6563 6f6d 655f 736e 6170 7368  ef become_snapsh
-000154c0: 6f74 2873 656c 662c 2073 6e61 7073 686f  ot(self, snapsho
-000154d0: 745f 6964 783a 2069 6e74 2920 2d3e 204e  t_idx: int) -> N
-000154e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000154f0: 4368 616e 6765 7320 7468 6520 7072 6f67  Changes the prog
-00015500: 7265 7373 2074 6f20 6120 736e 6170 7368  ress to a snapsh
-00015510: 6f74 2e22 2222 0a20 2020 2064 6566 206d  ot.""".    def m
-00015520: 6179 6265 5f75 7064 6174 6528 7365 6c66  aybe_update(self
-00015530: 2c20 6e3a 2069 6e74 2920 2d3e 2062 6f6f  , n: int) -> boo
-00015540: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-00015550: 2020 2020 2020 2052 6574 7572 6e73 2066         Returns f
-00015560: 616c 7365 2069 6620 7468 6520 6769 7665  alse if the give
-00015570: 6e20 6e20 696e 6465 7820 636f 6d65 7320  n n index comes 
-00015580: 6672 6f6d 2061 6e20 6f75 7464 6174 6564  from an outdated
-00015590: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
-000155a0: 2020 4f74 6865 7277 6973 6520 6974 2075    Otherwise it u
-000155b0: 7064 6174 6573 2074 6865 2070 726f 6772  pdates the progr
-000155c0: 6573 7320 616e 6420 7265 7475 726e 7320  ess and returns 
-000155d0: 7472 7565 2e0a 2020 2020 2020 2020 2222  true..        ""
-000155e0: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
-000155f0: 6465 6372 5f74 6f28 0a20 2020 2020 2020  decr_to(.       
-00015600: 2073 656c 662c 2072 656a 6563 7465 643a   self, rejected:
-00015610: 2069 6e74 2c20 6d61 7463 685f 6869 6e74   int, match_hint
-00015620: 3a20 696e 742c 2072 6571 7565 7374 5f73  : int, request_s
-00015630: 6e61 7073 686f 743a 2069 6e74 0a20 2020  napshot: int.   
-00015640: 2029 202d 3e20 626f 6f6c 3a0a 2020 2020   ) -> bool:.    
-00015650: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00015660: 5265 7475 726e 7320 6661 6c73 6520 6966  Returns false if
-00015670: 2074 6865 2067 6976 656e 2069 6e64 6578   the given index
-00015680: 2063 6f6d 6573 2066 726f 6d20 616e 206f   comes from an o
-00015690: 7574 206f 6620 6f72 6465 7220 6d65 7373  ut of order mess
-000156a0: 6167 652e 0a20 2020 2020 2020 204f 7468  age..        Oth
-000156b0: 6572 7769 7365 2069 7420 6465 6372 6561  erwise it decrea
-000156c0: 7365 7320 7468 6520 7072 6f67 7265 7373  ses the progress
-000156d0: 206e 6578 7420 696e 6465 7820 746f 206d   next index to m
-000156e0: 696e 2872 656a 6563 7465 642c 206c 6173  in(rejected, las
-000156f0: 7429 0a20 2020 2020 2020 2061 6e64 2072  t).        and r
-00015700: 6574 7572 6e73 2074 7275 652e 0a20 2020  eturns true..   
-00015710: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00015720: 2073 6e61 7073 686f 745f 6661 696c 7572   snapshot_failur
-00015730: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-00015740: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015750: 2020 2020 2053 6574 7320 7468 6520 736e       Sets the sn
-00015760: 6170 7368 6f74 2074 6f20 6661 696c 7572  apshot to failur
-00015770: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00015780: 2020 2064 6566 2070 6175 7365 2873 656c     def pause(sel
-00015790: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-000157a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000157b0: 5061 7573 6520 7072 6f67 7265 7373 2e0a  Pause progress..
-000157c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000157d0: 6465 6620 6973 5f70 6175 7365 6428 7365  def is_paused(se
-000157e0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-000157f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015800: 2044 6574 6572 6d69 6e65 2077 6865 7468   Determine wheth
-00015810: 6572 2070 726f 6772 6573 7320 6973 2070  er progress is p
-00015820: 6175 7365 642e 0a20 2020 2020 2020 2022  aused..        "
-00015830: 2222 0a20 2020 2064 6566 2069 735f 736e  "".    def is_sn
-00015840: 6170 7368 6f74 5f63 6175 6768 745f 7570  apshot_caught_up
-00015850: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-00015860: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015870: 2020 2020 5265 7475 726e 7320 7472 7565      Returns true
-00015880: 2069 6620 4d61 7463 6820 6973 2065 7175   if Match is equ
-00015890: 616c 206f 7220 6869 6768 6572 2074 6861  al or higher tha
-000158a0: 6e20 7468 6520 7065 6e64 696e 6753 6e61  n the pendingSna
-000158b0: 7073 686f 742e 0a20 2020 2020 2020 2022  pshot..        "
-000158c0: 2222 0a20 2020 2064 6566 2072 6573 756d  "".    def resum
-000158d0: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
-000158e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000158f0: 2020 2020 2052 6573 756d 6520 7072 6f67       Resume prog
-00015900: 7265 7373 0a20 2020 2020 2020 2022 2222  ress.        """
-00015910: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
-00015920: 7374 6174 6528 7365 6c66 2c20 6c61 7374  state(self, last
-00015930: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00015940: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015950: 2020 2020 5570 6461 7465 2069 6e66 6c69      Update infli
-00015960: 6768 7420 6d73 6773 2061 6e64 206e 6578  ght msgs and nex
-00015970: 745f 6964 780a 2020 2020 2020 2020 2222  t_idx.        ""
-00015980: 220a 2020 2020 6465 6620 7570 6461 7465  ".    def update
-00015990: 5f63 6f6d 6d69 7474 6564 2873 656c 662c  _committed(self,
-000159a0: 2063 6f6d 6d69 7474 6564 5f69 6e64 6578   committed_index
-000159b0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-000159c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000159d0: 2020 2020 5570 6461 7465 2063 6f6d 6d69      Update commi
-000159e0: 7474 6564 5f69 6e64 6578 2e0a 2020 2020  tted_index..    
-000159f0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00015a00: 6f70 7469 6d69 7374 6963 5f75 7064 6174  optimistic_updat
-00015a10: 6528 7365 6c66 2c20 6e3a 2069 6e74 2920  e(self, n: int) 
-00015a20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00015a30: 2022 2222 0a20 2020 2020 2020 204f 7074   """.        Opt
-00015a40: 696d 6973 7469 6361 6c6c 7920 6164 7661  imistically adva
-00015a50: 6e63 6520 7468 6520 696e 6465 780a 2020  nce the index.  
-00015a60: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00015a70: 6620 6765 745f 696e 7328 7365 6c66 2920  f get_ins(self) 
-00015a80: 2d3e 2022 496e 666c 6967 6874 7352 6566  -> "InflightsRef
-00015a90: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-00015aa0: 2020 2020 2020 2060 696e 7360 3a20 496e         `ins`: In
-00015ab0: 666c 6967 6874 7320 6973 2061 2073 6c69  flights is a sli
-00015ac0: 6469 6e67 2077 696e 646f 7720 666f 7220  ding window for 
-00015ad0: 7468 6520 696e 666c 6967 6874 206d 6573  the inflight mes
-00015ae0: 7361 6765 732e 0a20 2020 2020 2020 2057  sages..        W
-00015af0: 6865 6e20 696e 666c 6967 6874 7320 6973  hen inflights is
-00015b00: 2066 756c 6c2c 206e 6f20 6d6f 7265 206d   full, no more m
-00015b10: 6573 7361 6765 2073 686f 756c 6420 6265  essage should be
-00015b20: 2073 656e 742e 0a20 2020 2020 2020 2057   sent..        W
-00015b30: 6865 6e20 6120 6c65 6164 6572 2073 656e  hen a leader sen
-00015b40: 6473 206f 7574 2061 206d 6573 7361 6765  ds out a message
-00015b50: 2c20 7468 6520 696e 6465 7820 6f66 2074  , the index of t
-00015b60: 6865 206c 6173 740a 2020 2020 2020 2020  he last.        
-00015b70: 656e 7472 7920 7368 6f75 6c64 2062 6520  entry should be 
-00015b80: 6164 6465 6420 746f 2069 6e66 6c69 6768  added to infligh
-00015b90: 7473 2e20 5468 6520 696e 6465 7820 4d55  ts. The index MU
-00015ba0: 5354 2062 6520 6164 6465 640a 2020 2020  ST be added.    
-00015bb0: 2020 2020 696e 746f 2069 6e66 6c69 6768      into infligh
-00015bc0: 7473 2069 6e20 6f72 6465 722e 0a20 2020  ts in order..   
-00015bd0: 2020 2020 2057 6865 6e20 6120 6c65 6164       When a lead
-00015be0: 6572 2072 6563 6569 7665 7320 6120 7265  er receives a re
-00015bf0: 706c 792c 2074 6865 2070 7265 7669 6f75  ply, the previou
-00015c00: 7320 696e 666c 6967 6874 7320 7368 6f75  s inflights shou
-00015c10: 6c64 0a20 2020 2020 2020 2062 6520 6672  ld.        be fr
-00015c20: 6565 6420 6279 2063 616c 6c69 6e67 2069  eed by calling i
-00015c30: 6e66 6c69 6768 7473 2e66 7265 6554 6f2e  nflights.freeTo.
-00015c40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015c50: 2064 6566 2073 6574 5f69 6e73 2873 656c   def set_ins(sel
-00015c60: 662c 2069 6e66 6c69 6768 7473 3a20 2249  f, inflights: "I
-00015c70: 6e66 6c69 6768 7473 2220 7c20 2249 6e66  nflights" | "Inf
-00015c80: 6c69 6768 7473 5265 6622 2920 2d3e 204e  lightsRef") -> N
-00015c90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00015ca0: 0a20 2020 2020 2020 2060 696e 7360 3a20  .        `ins`: 
-00015cb0: 496e 666c 6967 6874 7320 6973 2061 2073  Inflights is a s
-00015cc0: 6c69 6469 6e67 2077 696e 646f 7720 666f  liding window fo
-00015cd0: 7220 7468 6520 696e 666c 6967 6874 206d  r the inflight m
-00015ce0: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
-00015cf0: 2057 6865 6e20 696e 666c 6967 6874 7320   When inflights 
-00015d00: 6973 2066 756c 6c2c 206e 6f20 6d6f 7265  is full, no more
-00015d10: 206d 6573 7361 6765 2073 686f 756c 6420   message should 
-00015d20: 6265 2073 656e 742e 0a20 2020 2020 2020  be sent..       
-00015d30: 2057 6865 6e20 6120 6c65 6164 6572 2073   When a leader s
-00015d40: 656e 6473 206f 7574 2061 206d 6573 7361  ends out a messa
-00015d50: 6765 2c20 7468 6520 696e 6465 7820 6f66  ge, the index of
-00015d60: 2074 6865 206c 6173 740a 2020 2020 2020   the last.      
-00015d70: 2020 656e 7472 7920 7368 6f75 6c64 2062    entry should b
-00015d80: 6520 6164 6465 6420 746f 2069 6e66 6c69  e added to infli
-00015d90: 6768 7473 2e20 5468 6520 696e 6465 7820  ghts. The index 
-00015da0: 4d55 5354 2062 6520 6164 6465 640a 2020  MUST be added.  
-00015db0: 2020 2020 2020 696e 746f 2069 6e66 6c69        into infli
-00015dc0: 6768 7473 2069 6e20 6f72 6465 722e 0a20  ghts in order.. 
-00015dd0: 2020 2020 2020 2057 6865 6e20 6120 6c65         When a le
-00015de0: 6164 6572 2072 6563 6569 7665 7320 6120  ader receives a 
-00015df0: 7265 706c 792c 2074 6865 2070 7265 7669  reply, the previ
-00015e00: 6f75 7320 696e 666c 6967 6874 7320 7368  ous inflights sh
-00015e10: 6f75 6c64 0a20 2020 2020 2020 2062 6520  ould.        be 
-00015e20: 6672 6565 6420 6279 2063 616c 6c69 6e67  freed by calling
-00015e30: 2069 6e66 6c69 6768 7473 2e66 7265 6554   inflights.freeT
-00015e40: 6f2e 0a20 2020 2020 2020 2022 2222 0a20  o..        """. 
-00015e50: 2020 2064 6566 2067 6574 5f63 6f6d 6d69     def get_commi
-00015e60: 745f 6772 6f75 705f 6964 2873 656c 6629  t_group_id(self)
-00015e70: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00015e80: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
-00015e90: 6d6d 6974 5f67 726f 7570 5f69 6460 3a20  mmit_group_id`: 
-00015ea0: 4f6e 6c79 206c 6f67 7320 7265 706c 6963  Only logs replic
-00015eb0: 6174 6564 2074 6f20 6469 6666 6572 656e  ated to differen
-00015ec0: 7420 6772 6f75 7020 7769 6c6c 2062 6520  t group will be 
-00015ed0: 636f 6d6d 6974 7465 6420 6966 2061 6e79  committed if any
-00015ee0: 2067 726f 7570 2069 7320 636f 6e66 6967   group is config
-00015ef0: 7572 6564 2e0a 2020 2020 2020 2020 2222  ured..        ""
-00015f00: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
-00015f10: 6d6d 6974 5f67 726f 7570 5f69 6428 7365  mmit_group_id(se
-00015f20: 6c66 2c20 636f 6d6d 6974 5f67 726f 7570  lf, commit_group
-00015f30: 5f69 643a 2069 6e74 2920 2d3e 204e 6f6e  _id: int) -> Non
-00015f40: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00015f50: 2020 2020 2020 2060 636f 6d6d 6974 5f67         `commit_g
-00015f60: 726f 7570 5f69 6460 3a20 4f6e 6c79 206c  roup_id`: Only l
-00015f70: 6f67 7320 7265 706c 6963 6174 6564 2074  ogs replicated t
-00015f80: 6f20 6469 6666 6572 656e 7420 6772 6f75  o different grou
-00015f90: 7020 7769 6c6c 2062 6520 636f 6d6d 6974  p will be commit
-00015fa0: 7465 6420 6966 2061 6e79 2067 726f 7570  ted if any group
-00015fb0: 2069 7320 636f 6e66 6967 7572 6564 2e0a   is configured..
-00015fc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015fd0: 6465 6620 6765 745f 636f 6d6d 6974 7465  def get_committe
-00015fe0: 645f 696e 6465 7828 7365 6c66 2920 2d3e  d_index(self) ->
-00015ff0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00016000: 220a 2020 2020 2020 2020 6063 6f6d 6d69  ".        `commi
-00016010: 7474 6564 5f69 6e64 6578 603a 2043 6f6d  tted_index`: Com
-00016020: 6d69 7474 6564 2069 6e64 6578 2069 6e20  mitted index in 
-00016030: 7261 6674 5f6c 6f67 0a20 2020 2020 2020  raft_log.       
-00016040: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00016050: 5f63 6f6d 6d69 7474 6564 5f69 6e64 6578  _committed_index
-00016060: 2873 656c 662c 2063 6f6d 6d69 7474 6564  (self, committed
-00016070: 5f69 6e64 6578 3a20 696e 7429 202d 3e20  _index: int) -> 
-00016080: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00016090: 220a 2020 2020 2020 2020 6063 6f6d 6d69  ".        `commi
-000160a0: 7474 6564 5f69 6e64 6578 603a 2043 6f6d  tted_index`: Com
-000160b0: 6d69 7474 6564 2069 6e64 6578 2069 6e20  mitted index in 
-000160c0: 7261 6674 5f6c 6f67 0a20 2020 2020 2020  raft_log.       
-000160d0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-000160e0: 5f6d 6174 6368 6564 2873 656c 6629 202d  _matched(self) -
-000160f0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-00016100: 2222 0a20 2020 2020 2020 2060 6d61 7463  "".        `matc
-00016110: 6865 6460 3a20 486f 7720 6d75 6368 2073  hed`: How much s
-00016120: 7461 7465 2069 7320 6d61 7463 6865 642e  tate is matched.
-00016130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016140: 2064 6566 2073 6574 5f6d 6174 6368 6564   def set_matched
-00016150: 2873 656c 662c 206d 6174 6368 6564 3a20  (self, matched: 
-00016160: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00016170: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016180: 2020 606d 6174 6368 6564 603a 2048 6f77    `matched`: How
-00016190: 206d 7563 6820 7374 6174 6520 6973 206d   much state is m
-000161a0: 6174 6368 6564 2e0a 2020 2020 2020 2020  atched..        
-000161b0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-000161c0: 6e65 7874 5f69 6478 2873 656c 6629 202d  next_idx(self) -
-000161d0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-000161e0: 2222 0a20 2020 2020 2020 2060 6e65 7874  "".        `next
-000161f0: 5f69 6478 603a 2054 6865 206e 6578 7420  _idx`: The next 
-00016200: 696e 6465 7820 746f 2061 7070 6c79 0a20  index to apply. 
-00016210: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00016220: 6566 2073 6574 5f6e 6578 745f 6964 7828  ef set_next_idx(
-00016230: 7365 6c66 2c20 6e65 7874 5f69 6478 3a20  self, next_idx: 
-00016240: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00016250: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00016260: 2020 606e 6578 745f 6964 7860 3a20 5468    `next_idx`: Th
-00016270: 6520 6e65 7874 2069 6e64 6578 2074 6f20  e next index to 
-00016280: 6170 706c 790a 2020 2020 2020 2020 2222  apply.        ""
-00016290: 220a 2020 2020 6465 6620 6765 745f 7065  ".    def get_pe
-000162a0: 6e64 696e 675f 736e 6170 7368 6f74 2873  nding_snapshot(s
-000162b0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-000162c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000162d0: 2060 7065 6e64 696e 675f 736e 6170 7368   `pending_snapsh
-000162e0: 6f74 603a 2054 6869 7320 6669 656c 6420  ot`: This field 
-000162f0: 6973 2075 7365 6420 696e 2050 726f 6772  is used in Progr
-00016300: 6573 7353 7461 7465 536e 6170 7368 6f74  essStateSnapshot
-00016310: 2e0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
-00016320: 7265 2069 7320 6120 7065 6e64 696e 6720  re is a pending 
-00016330: 736e 6170 7368 6f74 2c20 7468 6520 7065  snapshot, the pe
-00016340: 6e64 696e 6753 6e61 7073 686f 7420 7769  ndingSnapshot wi
-00016350: 6c6c 2062 6520 7365 7420 746f 2074 6865  ll be set to the
-00016360: 0a20 2020 2020 2020 2069 6e64 6578 206f  .        index o
-00016370: 6620 7468 6520 736e 6170 7368 6f74 2e20  f the snapshot. 
-00016380: 4966 2070 656e 6469 6e67 536e 6170 7368  If pendingSnapsh
-00016390: 6f74 2069 7320 7365 742c 2074 6865 2072  ot is set, the r
-000163a0: 6570 6c69 6361 7469 6f6e 2070 726f 6365  eplication proce
-000163b0: 7373 206f 660a 2020 2020 2020 2020 7468  ss of.        th
-000163c0: 6973 2050 726f 6772 6573 7320 7769 6c6c  is Progress will
-000163d0: 2062 6520 7061 7573 6564 2e20 7261 6674   be paused. raft
-000163e0: 2077 696c 6c20 6e6f 7420 7265 7365 6e64   will not resend
-000163f0: 2073 6e61 7073 686f 7420 756e 7469 6c20   snapshot until 
-00016400: 7468 6520 7065 6e64 696e 6720 6f6e 650a  the pending one.
-00016410: 2020 2020 2020 2020 6973 2072 6570 6f72          is repor
-00016420: 7465 6420 746f 2062 6520 6661 696c 6564  ted to be failed
-00016430: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00016440: 2020 6465 6620 7365 745f 7065 6e64 696e    def set_pendin
-00016450: 675f 736e 6170 7368 6f74 2873 656c 662c  g_snapshot(self,
-00016460: 2070 656e 6469 6e67 5f73 6e61 7073 686f   pending_snapsho
-00016470: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-00016480: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016490: 2020 2020 2060 7065 6e64 696e 675f 736e       `pending_sn
-000164a0: 6170 7368 6f74 603a 2054 6869 7320 6669  apshot`: This fi
-000164b0: 656c 6420 6973 2075 7365 6420 696e 2050  eld is used in P
-000164c0: 726f 6772 6573 7353 7461 7465 536e 6170  rogressStateSnap
-000164d0: 7368 6f74 2e0a 2020 2020 2020 2020 4966  shot..        If
-000164e0: 2074 6865 7265 2069 7320 6120 7065 6e64   there is a pend
-000164f0: 696e 6720 736e 6170 7368 6f74 2c20 7468  ing snapshot, th
-00016500: 6520 7065 6e64 696e 6753 6e61 7073 686f  e pendingSnapsho
-00016510: 7420 7769 6c6c 2062 6520 7365 7420 746f  t will be set to
-00016520: 2074 6865 0a20 2020 2020 2020 2069 6e64   the.        ind
-00016530: 6578 206f 6620 7468 6520 736e 6170 7368  ex of the snapsh
-00016540: 6f74 2e20 4966 2070 656e 6469 6e67 536e  ot. If pendingSn
-00016550: 6170 7368 6f74 2069 7320 7365 742c 2074  apshot is set, t
-00016560: 6865 2072 6570 6c69 6361 7469 6f6e 2070  he replication p
-00016570: 726f 6365 7373 206f 660a 2020 2020 2020  rocess of.      
-00016580: 2020 7468 6973 2050 726f 6772 6573 7320    this Progress 
-00016590: 7769 6c6c 2062 6520 7061 7573 6564 2e20  will be paused. 
-000165a0: 7261 6674 2077 696c 6c20 6e6f 7420 7265  raft will not re
-000165b0: 7365 6e64 2073 6e61 7073 686f 7420 756e  send snapshot un
-000165c0: 7469 6c20 7468 6520 7065 6e64 696e 6720  til the pending 
-000165d0: 6f6e 650a 2020 2020 2020 2020 6973 2072  one.        is r
-000165e0: 6570 6f72 7465 6420 746f 2062 6520 6661  eported to be fa
-000165f0: 696c 6564 2e0a 2020 2020 2020 2020 2222  iled..        ""
-00016600: 220a 2020 2020 6465 6620 6765 745f 7065  ".    def get_pe
-00016610: 6e64 696e 675f 7265 7175 6573 745f 736e  nding_request_sn
-00016620: 6170 7368 6f74 2873 656c 6629 202d 3e20  apshot(self) -> 
-00016630: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00016640: 0a20 2020 2020 2020 2060 7065 6e64 696e  .        `pendin
-00016650: 675f 7265 7175 6573 745f 736e 6170 7368  g_request_snapsh
-00016660: 6f74 603a 2054 6869 7320 6669 656c 6420  ot`: This field 
-00016670: 6973 2075 7365 6420 696e 2072 6571 7565  is used in reque
-00016680: 7374 2073 6e61 7073 686f 742e 0a20 2020  st snapshot..   
-00016690: 2020 2020 2049 6620 7468 6572 6520 6973       If there is
-000166a0: 2061 2070 656e 6469 6e67 2072 6571 7565   a pending reque
-000166b0: 7374 2073 6e61 7073 686f 742c 2074 6869  st snapshot, thi
-000166c0: 7320 7769 6c6c 2062 6520 7365 7420 746f  s will be set to
-000166d0: 2074 6865 2072 6571 7565 7374 0a20 2020   the request.   
-000166e0: 2020 2020 2069 6e64 6578 206f 6620 7468       index of th
-000166f0: 6520 736e 6170 7368 6f74 2e0a 2020 2020  e snapshot..    
-00016700: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00016710: 7365 745f 7065 6e64 696e 675f 7265 7175  set_pending_requ
-00016720: 6573 745f 736e 6170 7368 6f74 2873 656c  est_snapshot(sel
-00016730: 662c 2070 656e 6469 6e67 5f72 6571 7565  f, pending_reque
-00016740: 7374 5f73 6e61 7073 686f 743a 2069 6e74  st_snapshot: int
-00016750: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00016760: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00016770: 7065 6e64 696e 675f 7265 7175 6573 745f  pending_request_
-00016780: 736e 6170 7368 6f74 603a 2054 6869 7320  snapshot`: This 
-00016790: 6669 656c 6420 6973 2075 7365 6420 696e  field is used in
-000167a0: 2072 6571 7565 7374 2073 6e61 7073 686f   request snapsho
-000167b0: 742e 0a20 2020 2020 2020 2049 6620 7468  t..        If th
-000167c0: 6572 6520 6973 2061 2070 656e 6469 6e67  ere is a pending
-000167d0: 2072 6571 7565 7374 2073 6e61 7073 686f   request snapsho
-000167e0: 742c 2074 6869 7320 7769 6c6c 2062 6520  t, this will be 
-000167f0: 7365 7420 746f 2074 6865 2072 6571 7565  set to the reque
-00016800: 7374 0a20 2020 2020 2020 2069 6e64 6578  st.        index
-00016810: 206f 6620 7468 6520 736e 6170 7368 6f74   of the snapshot
-00016820: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00016830: 2020 6465 6620 6765 745f 7265 6365 6e74    def get_recent
-00016840: 5f61 6374 6976 6528 7365 6c66 2920 2d3e  _active(self) ->
-00016850: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00016860: 2222 0a20 2020 2020 2020 2060 7265 6365  "".        `rece
-00016870: 6e74 5f61 6374 6976 6560 3a20 5468 6973  nt_active`: This
-00016880: 2069 7320 7472 7565 2069 6620 7468 6520   is true if the 
-00016890: 7072 6f67 7265 7373 2069 7320 7265 6365  progress is rece
-000168a0: 6e74 6c79 2061 6374 6976 652e 2052 6563  ntly active. Rec
-000168b0: 6569 7669 6e67 2061 6e79 206d 6573 7361  eiving any messa
-000168c0: 6765 730a 2020 2020 2020 2020 6672 6f6d  ges.        from
-000168d0: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
-000168e0: 6e67 2066 6f6c 6c6f 7765 7220 696e 6469  ng follower indi
-000168f0: 6361 7465 7320 7468 6520 7072 6f67 7265  cates the progre
-00016900: 7373 2069 7320 6163 7469 7665 2e0a 2020  ss is active..  
-00016910: 2020 2020 2020 5265 6365 6e74 4163 7469        RecentActi
-00016920: 7665 2063 616e 2062 6520 7265 7365 7420  ve can be reset 
-00016930: 746f 2066 616c 7365 2061 6674 6572 2061  to false after a
-00016940: 6e20 656c 6563 7469 6f6e 2074 696d 656f  n election timeo
-00016950: 7574 2e0a 2020 2020 2020 2020 2222 220a  ut..        """.
-00016960: 2020 2020 6465 6620 7365 745f 7265 6365      def set_rece
-00016970: 6e74 5f61 6374 6976 6528 7365 6c66 2c20  nt_active(self, 
-00016980: 7265 6365 6e74 5f61 6374 6976 653a 2062  recent_active: b
-00016990: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
-000169a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000169b0: 2020 6072 6563 656e 745f 6163 7469 7665    `recent_active
-000169c0: 603a 2054 6869 7320 6973 2074 7275 6520  `: This is true 
-000169d0: 6966 2074 6865 2070 726f 6772 6573 7320  if the progress 
-000169e0: 6973 2072 6563 656e 746c 7920 6163 7469  is recently acti
-000169f0: 7665 2e20 5265 6365 6976 696e 6720 616e  ve. Receiving an
-00016a00: 7920 6d65 7373 6167 6573 0a20 2020 2020  y messages.     
-00016a10: 2020 2066 726f 6d20 7468 6520 636f 7272     from the corr
-00016a20: 6573 706f 6e64 696e 6720 666f 6c6c 6f77  esponding follow
-00016a30: 6572 2069 6e64 6963 6174 6573 2074 6865  er indicates the
-00016a40: 2070 726f 6772 6573 7320 6973 2061 6374   progress is act
-00016a50: 6976 652e 0a20 2020 2020 2020 2052 6563  ive..        Rec
-00016a60: 656e 7441 6374 6976 6520 6361 6e20 6265  entActive can be
-00016a70: 2072 6573 6574 2074 6f20 6661 6c73 6520   reset to false 
-00016a80: 6166 7465 7220 616e 2065 6c65 6374 696f  after an electio
-00016a90: 6e20 7469 6d65 6f75 742e 0a20 2020 2020  n timeout..     
-00016aa0: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-00016ab0: 6574 5f70 6175 7365 6428 7365 6c66 2920  et_paused(self) 
-00016ac0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-00016ad0: 2022 2222 0a20 2020 2020 2020 2060 7061   """.        `pa
-00016ae0: 7573 6564 603a 2050 6175 7365 6420 6973  used`: Paused is
-00016af0: 2075 7365 6420 696e 2050 726f 6772 6573   used in Progres
-00016b00: 7353 7461 7465 5072 6f62 652e 0a20 2020  sStateProbe..   
-00016b10: 2020 2020 2057 6865 6e20 5061 7573 6564       When Paused
-00016b20: 2069 7320 7472 7565 2c20 7261 6674 2073   is true, raft s
-00016b30: 686f 756c 6420 7061 7573 6520 7365 6e64  hould pause send
-00016b40: 696e 6720 7265 706c 6963 6174 696f 6e20  ing replication 
-00016b50: 6d65 7373 6167 6520 746f 2074 6869 7320  message to this 
-00016b60: 7065 6572 2e0a 2020 2020 2020 2020 2222  peer..        ""
-00016b70: 220a 2020 2020 6465 6620 7365 745f 7061  ".    def set_pa
-00016b80: 7573 6564 2873 656c 662c 2070 6175 7365  used(self, pause
-00016b90: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
-00016ba0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00016bb0: 2020 2020 2020 6070 6175 7365 6460 3a20        `paused`: 
-00016bc0: 5061 7573 6564 2069 7320 7573 6564 2069  Paused is used i
-00016bd0: 6e20 5072 6f67 7265 7373 5374 6174 6550  n ProgressStateP
-00016be0: 726f 6265 2e0a 2020 2020 2020 2020 5768  robe..        Wh
-00016bf0: 656e 2050 6175 7365 6420 6973 2074 7275  en Paused is tru
-00016c00: 652c 2072 6166 7420 7368 6f75 6c64 2070  e, raft should p
-00016c10: 6175 7365 2073 656e 6469 6e67 2072 6570  ause sending rep
-00016c20: 6c69 6361 7469 6f6e 206d 6573 7361 6765  lication message
-00016c30: 2074 6f20 7468 6973 2070 6565 722e 0a20   to this peer.. 
-00016c40: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00016c50: 6566 2067 6574 5f73 7461 7465 2873 656c  ef get_state(sel
-00016c60: 6629 202d 3e20 2250 726f 6772 6573 7353  f) -> "ProgressS
-00016c70: 7461 7465 223a 0a20 2020 2020 2020 2022  tate":.        "
-00016c80: 2222 0a20 2020 2020 2020 2060 7374 6174  "".        `stat
-00016c90: 6560 3a20 5768 656e 2069 6e20 5072 6f67  e`: When in Prog
-00016ca0: 7265 7373 5374 6174 6550 726f 6265 2c20  ressStateProbe, 
-00016cb0: 6c65 6164 6572 2073 656e 6473 2061 7420  leader sends at 
-00016cc0: 6d6f 7374 206f 6e65 2072 6570 6c69 6361  most one replica
-00016cd0: 7469 6f6e 206d 6573 7361 6765 0a20 2020  tion message.   
-00016ce0: 2020 2020 2070 6572 2068 6561 7274 6265       per heartbe
-00016cf0: 6174 2069 6e74 6572 7661 6c2e 2049 7420  at interval. It 
-00016d00: 616c 736f 2070 726f 6265 7320 6163 7475  also probes actu
-00016d10: 616c 2070 726f 6772 6573 7320 6f66 2074  al progress of t
-00016d20: 6865 2066 6f6c 6c6f 7765 722e 0a0a 2020  he follower...  
-00016d30: 2020 2020 2020 5768 656e 2069 6e20 5072        When in Pr
-00016d40: 6f67 7265 7373 5374 6174 6552 6570 6c69  ogressStateRepli
-00016d50: 6361 7465 2c20 6c65 6164 6572 206f 7074  cate, leader opt
-00016d60: 696d 6973 7469 6361 6c6c 7920 696e 6372  imistically incr
-00016d70: 6561 7365 7320 6e65 7874 0a20 2020 2020  eases next.     
-00016d80: 2020 2074 6f20 7468 6520 6c61 7465 7374     to the latest
-00016d90: 2065 6e74 7279 2073 656e 7420 6166 7465   entry sent afte
-00016da0: 7220 7365 6e64 696e 6720 7265 706c 6963  r sending replic
-00016db0: 6174 696f 6e20 6d65 7373 6167 652e 2054  ation message. T
-00016dc0: 6869 7320 6973 0a20 2020 2020 2020 2061  his is.        a
-00016dd0: 6e20 6f70 7469 6d69 7a65 6420 7374 6174  n optimized stat
-00016de0: 6520 666f 7220 6661 7374 2072 6570 6c69  e for fast repli
-00016df0: 6361 7469 6e67 206c 6f67 2065 6e74 7269  cating log entri
-00016e00: 6573 2074 6f20 7468 6520 666f 6c6c 6f77  es to the follow
-00016e10: 6572 2e0a 0a20 2020 2020 2020 2057 6865  er...        Whe
-00016e20: 6e20 696e 2050 726f 6772 6573 7353 7461  n in ProgressSta
-00016e30: 7465 536e 6170 7368 6f74 2c20 6c65 6164  teSnapshot, lead
-00016e40: 6572 2073 686f 756c 6420 6861 7665 2073  er should have s
-00016e50: 656e 7420 6f75 7420 736e 6170 7368 6f74  ent out snapshot
-00016e60: 0a20 2020 2020 2020 2062 6566 6f72 6520  .        before 
-00016e70: 616e 6420 7374 6f70 2073 656e 6469 6e67  and stop sending
-00016e80: 2061 6e79 2072 6570 6c69 6361 7469 6f6e   any replication
-00016e90: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
-00016ea0: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00016eb0: 745f 7374 6174 6528 7365 6c66 2c20 7374  t_state(self, st
-00016ec0: 6174 653a 2022 5072 6f67 7265 7373 5374  ate: "ProgressSt
-00016ed0: 6174 6522 2920 2d3e 204e 6f6e 653a 0a20  ate") -> None:. 
-00016ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016ef0: 2020 2060 7374 6174 6560 3a20 5768 656e     `state`: When
-00016f00: 2069 6e20 5072 6f67 7265 7373 5374 6174   in ProgressStat
-00016f10: 6550 726f 6265 2c20 6c65 6164 6572 2073  eProbe, leader s
-00016f20: 656e 6473 2061 7420 6d6f 7374 206f 6e65  ends at most one
-00016f30: 2072 6570 6c69 6361 7469 6f6e 206d 6573   replication mes
-00016f40: 7361 6765 0a20 2020 2020 2020 2070 6572  sage.        per
-00016f50: 2068 6561 7274 6265 6174 2069 6e74 6572   heartbeat inter
-00016f60: 7661 6c2e 2049 7420 616c 736f 2070 726f  val. It also pro
-00016f70: 6265 7320 6163 7475 616c 2070 726f 6772  bes actual progr
-00016f80: 6573 7320 6f66 2074 6865 2066 6f6c 6c6f  ess of the follo
-00016f90: 7765 722e 0a0a 2020 2020 2020 2020 5768  wer...        Wh
-00016fa0: 656e 2069 6e20 5072 6f67 7265 7373 5374  en in ProgressSt
-00016fb0: 6174 6552 6570 6c69 6361 7465 2c20 6c65  ateReplicate, le
-00016fc0: 6164 6572 206f 7074 696d 6973 7469 6361  ader optimistica
-00016fd0: 6c6c 7920 696e 6372 6561 7365 7320 6e65  lly increases ne
-00016fe0: 7874 0a20 2020 2020 2020 2074 6f20 7468  xt.        to th
-00016ff0: 6520 6c61 7465 7374 2065 6e74 7279 2073  e latest entry s
-00017000: 656e 7420 6166 7465 7220 7365 6e64 696e  ent after sendin
-00017010: 6720 7265 706c 6963 6174 696f 6e20 6d65  g replication me
-00017020: 7373 6167 652e 2054 6869 7320 6973 0a20  ssage. This is. 
-00017030: 2020 2020 2020 2061 6e20 6f70 7469 6d69         an optimi
-00017040: 7a65 6420 7374 6174 6520 666f 7220 6661  zed state for fa
-00017050: 7374 2072 6570 6c69 6361 7469 6e67 206c  st replicating l
-00017060: 6f67 2065 6e74 7269 6573 2074 6f20 7468  og entries to th
-00017070: 6520 666f 6c6c 6f77 6572 2e0a 0a20 2020  e follower...   
-00017080: 2020 2020 2057 6865 6e20 696e 2050 726f       When in Pro
-00017090: 6772 6573 7353 7461 7465 536e 6170 7368  gressStateSnapsh
-000170a0: 6f74 2c20 6c65 6164 6572 2073 686f 756c  ot, leader shoul
-000170b0: 6420 6861 7665 2073 656e 7420 6f75 7420  d have sent out 
-000170c0: 736e 6170 7368 6f74 0a20 2020 2020 2020  snapshot.       
-000170d0: 2062 6566 6f72 6520 616e 6420 7374 6f70   before and stop
-000170e0: 2073 656e 6469 6e67 2061 6e79 2072 6570   sending any rep
-000170f0: 6c69 6361 7469 6f6e 206d 6573 7361 6765  lication message
-00017100: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
-00017110: 6c61 7373 2050 726f 6772 6573 7328 5f5f  lass Progress(__
-00017120: 4150 495f 5072 6f67 7265 7373 293a 0a20  API_Progress):. 
-00017130: 2020 2022 2222 0a20 2020 2054 6865 2070     """.    The p
-00017140: 726f 6772 6573 7320 6f66 2063 6174 6368  rogress of catch
-00017150: 696e 6720 7570 2066 726f 6d20 6120 7265  ing up from a re
-00017160: 7374 6172 742e 0a20 2020 2022 2222 0a0a  start..    """..
-00017170: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00017180: 2873 656c 662c 206e 6578 745f 6964 783a  (self, next_idx:
-00017190: 2069 6e74 2c20 696e 735f 7369 7a65 3a20   int, ins_size: 
-000171a0: 696e 7429 202d 3e20 4e6f 6e65 3a20 2e2e  int) -> None: ..
-000171b0: 2e0a 2020 2020 6465 6620 6d61 6b65 5f72  ..    def make_r
-000171c0: 6566 2873 656c 6629 202d 3e20 2250 726f  ef(self) -> "Pro
-000171d0: 6772 6573 7352 6566 223a 202e 2e2e 0a0a  gressRef": .....
-000171e0: 636c 6173 7320 5072 6f67 7265 7373 5265  class ProgressRe
-000171f0: 6628 5f5f 4150 495f 5072 6f67 7265 7373  f(__API_Progress
-00017200: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
-00017210: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
-00017220: 203a 636c 6173 733a 6050 726f 6772 6573   :class:`Progres
-00017230: 7360 2e0a 2020 2020 2222 220a 0a63 6c61  s`..    """..cla
-00017240: 7373 205f 5f41 5049 5f4a 6f69 6e74 436f  ss __API_JointCo
-00017250: 6e66 6967 285f 5f43 6c6f 6e65 6162 6c65  nfig(__Cloneable
-00017260: 293a 0a20 2020 2064 6566 2063 6c6f 6e65  ):.    def clone
-00017270: 2873 656c 6629 202d 3e20 224a 6f69 6e74  (self) -> "Joint
-00017280: 436f 6e66 6967 223a 202e 2e2e 0a20 2020  Config": ....   
-00017290: 2064 6566 2063 6c65 6172 2873 656c 6629   def clear(self)
-000172a0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000172b0: 2020 2222 2243 6c65 6172 7320 616c 6c20    """Clears all 
-000172c0: 4944 732e 2222 220a 2020 2020 6465 6620  IDs.""".    def 
-000172d0: 636f 6e74 6169 6e73 2873 656c 662c 2069  contains(self, i
-000172e0: 643a 2069 6e74 2920 2d3e 2062 6f6f 6c3a  d: int) -> bool:
-000172f0: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
-00017300: 6b20 6966 2061 6e20 6964 2069 7320 6120  k if an id is a 
-00017310: 766f 7465 722e 2222 220a 2020 2020 6465  voter.""".    de
-00017320: 6620 6964 7328 2920 2d3e 2053 6574 5b69  f ids() -> Set[i
-00017330: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
-00017340: 5265 7475 726e 7320 616e 2069 7465 7261  Returns an itera
-00017350: 746f 7220 6f76 6572 2074 776f 2068 6173  tor over two has
-00017360: 6820 7365 7420 7769 7468 6f75 7420 636c  h set without cl
-00017370: 6f6e 696e 672e 2222 220a 2020 2020 6465  oning.""".    de
-00017380: 6620 6973 5f73 696e 676c 6574 6f6e 2873  f is_singleton(s
-00017390: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-000173a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000173b0: 2020 5265 7475 726e 7320 7472 7565 2069    Returns true i
-000173c0: 6620 2861 6e64 206f 6e6c 7920 6966 2920  f (and only if) 
-000173d0: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
-000173e0: 6520 766f 7469 6e67 206d 656d 6265 720a  e voting member.
-000173f0: 2020 2020 2020 2020 2869 2e65 2e20 7468          (i.e. th
-00017400: 6520 6c65 6164 6572 2920 696e 2074 6865  e leader) in the
-00017410: 2063 7572 7265 6e74 2063 6f6e 6669 6775   current configu
-00017420: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00017430: 2222 220a 0a63 6c61 7373 204a 6f69 6e74  """..class Joint
-00017440: 436f 6e66 6967 285f 5f41 5049 5f4a 6f69  Config(__API_Joi
-00017450: 6e74 436f 6e66 6967 293a 0a20 2020 2022  ntConfig):.    "
-00017460: 2222 0a20 2020 2041 2063 6f6e 6669 6775  "".    A configu
-00017470: 7261 7469 6f6e 206f 6620 7477 6f20 6772  ration of two gr
-00017480: 6f75 7073 206f 6620 2870 6f73 7369 626c  oups of (possibl
-00017490: 7920 6f76 6572 6c61 7070 696e 6729 206d  y overlapping) m
-000174a0: 616a 6f72 6974 7920 636f 6e66 6967 7572  ajority configur
-000174b0: 6174 696f 6e73 2e0a 2020 2020 4465 6369  ations..    Deci
-000174c0: 7369 6f6e 7320 7265 7175 6972 6520 7468  sions require th
-000174d0: 6520 7375 7070 6f72 7420 6f66 2062 6f74  e support of bot
-000174e0: 6820 6d61 6a6f 7269 7469 6573 2e0a 2020  h majorities..  
-000174f0: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-00017500: 5f69 6e69 745f 5f28 7365 6c66 2c20 766f  _init__(self, vo
-00017510: 7465 7273 3a20 5365 745b 696e 745d 2920  ters: Set[int]) 
-00017520: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-00017530: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
-00017540: 6c66 2920 2d3e 2022 4a6f 696e 7443 6f6e  lf) -> "JointCon
-00017550: 6669 6752 6566 223a 202e 2e2e 0a0a 636c  figRef": .....cl
-00017560: 6173 7320 4a6f 696e 7443 6f6e 6669 6752  ass JointConfigR
-00017570: 6566 285f 5f41 5049 5f4a 6f69 6e74 436f  ef(__API_JointCo
-00017580: 6e66 6967 293a 0a20 2020 2022 2222 0a20  nfig):.    """. 
-00017590: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
-000175a0: 6520 6f66 203a 636c 6173 733a 604a 6f69  e of :class:`Joi
-000175b0: 6e74 436f 6e66 6967 602e 0a20 2020 2022  ntConfig`..    "
-000175c0: 2222 0a0a 636c 6173 7320 5f5f 4150 495f  ""..class __API_
-000175d0: 4d61 6a6f 7269 7479 436f 6e66 6967 285f  MajorityConfig(_
-000175e0: 5f43 6c6f 6e65 6162 6c65 293a 0a20 2020  _Cloneable):.   
-000175f0: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
-00017600: 202d 3e20 224d 616a 6f72 6974 7943 6f6e   -> "MajorityCon
-00017610: 6669 6722 3a20 2e2e 2e0a 2020 2020 6465  fig": ....    de
-00017620: 6620 7261 775f 736c 6963 6528 7365 6c66  f raw_slice(self
-00017630: 2920 2d3e 204c 6973 745b 696e 745d 3a0a  ) -> List[int]:.
-00017640: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017650: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
-00017660: 4d61 6a6f 7269 7479 436f 6e66 6967 2061  MajorityConfig a
-00017670: 7320 6120 736c 6963 652e 0a20 2020 2020  s a slice..     
-00017680: 2020 2022 2222 0a20 2020 2064 6566 2063     """.    def c
-00017690: 6170 6163 6974 7928 7365 6c66 2920 2d3e  apacity(self) ->
-000176a0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-000176b0: 2222 2222 0a20 2020 2064 6566 2065 7874  """".    def ext
-000176c0: 656e 6428 7365 6c66 2c20 6f74 6865 725f  end(self, other_
-000176d0: 7365 743a 2053 6574 5b69 6e74 5d29 202d  set: Set[int]) -
-000176e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000176f0: 2222 2222 2222 0a20 2020 2064 6566 2067  """""".    def g
-00017700: 6574 2873 656c 662c 2069 6e64 6578 3a20  et(self, index: 
-00017710: 696e 7429 202d 3e20 4f70 7469 6f6e 616c  int) -> Optional
-00017720: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
-00017730: 2222 2222 220a 2020 2020 6465 6620 696e  """"".    def in
-00017740: 7365 7274 2873 656c 662c 2076 616c 7565  sert(self, value
-00017750: 3a20 696e 7429 202d 3e20 626f 6f6c 3a0a  : int) -> bool:.
-00017760: 2020 2020 2020 2020 2222 2222 2222 0a20          """""". 
-00017770: 2020 2064 6566 2072 6570 6c61 6365 2873     def replace(s
-00017780: 656c 662c 2076 616c 7565 3a20 696e 7429  elf, value: int)
-00017790: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-000177a0: 2022 2222 2222 220a 2020 2020 6465 6620   """""".    def 
-000177b0: 6973 5f64 6973 6a6f 696e 7428 7365 6c66  is_disjoint(self
-000177c0: 2c20 6f74 6865 723a 2053 6574 5b69 6e74  , other: Set[int
-000177d0: 5d29 202d 3e20 626f 6f6c 3a0a 2020 2020  ]) -> bool:.    
-000177e0: 2020 2020 2222 2222 2222 0a20 2020 2064      """""".    d
-000177f0: 6566 2069 735f 7375 7065 7273 6574 2873  ef is_superset(s
-00017800: 656c 662c 206f 7468 6572 3a20 5365 745b  elf, other: Set[
-00017810: 696e 745d 2920 2d3e 2062 6f6f 6c3a 0a20  int]) -> bool:. 
-00017820: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
-00017830: 2020 6465 6620 6973 5f73 7562 7365 7428    def is_subset(
-00017840: 7365 6c66 2c20 6f74 6865 723a 2053 6574  self, other: Set
-00017850: 5b69 6e74 5d29 202d 3e20 626f 6f6c 3a0a  [int]) -> bool:.
-00017860: 2020 2020 2020 2020 2222 2222 2222 0a20          """""". 
-00017870: 2020 2064 6566 2072 6573 6572 7665 2873     def reserve(s
-00017880: 656c 662c 2061 6464 6974 696f 6e61 6c3a  elf, additional:
-00017890: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-000178a0: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
-000178b0: 2020 6465 6620 7265 6d6f 7665 2873 656c    def remove(sel
-000178c0: 662c 2076 616c 7565 3a20 696e 7429 202d  f, value: int) -
-000178d0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-000178e0: 2222 2222 2222 0a20 2020 2064 6566 2073  """""".    def s
-000178f0: 6872 696e 6b5f 746f 2873 656c 662c 206d  hrink_to(self, m
-00017900: 696e 5f63 6170 6163 6974 793a 2069 6e74  in_capacity: int
-00017910: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00017920: 2020 2022 2222 2222 220a 2020 2020 6465     """""".    de
-00017930: 6620 7368 7269 6e6b 5f74 6f5f 6669 7428  f shrink_to_fit(
-00017940: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00017950: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
-00017960: 2020 6465 6620 7472 795f 7265 7365 7276    def try_reserv
-00017970: 6528 7365 6c66 2c20 6164 6469 7469 6f6e  e(self, addition
-00017980: 616c 3a20 696e 7429 202d 3e20 4e6f 6e65  al: int) -> None
-00017990: 3a0a 2020 2020 2020 2020 2222 2222 2222  :.        """"""
-000179a0: 0a0a 636c 6173 7320 4d61 6a6f 7269 7479  ..class Majority
-000179b0: 436f 6e66 6967 285f 5f41 5049 5f4d 616a  Config(__API_Maj
-000179c0: 6f72 6974 7943 6f6e 6669 6729 3a0a 2020  orityConfig):.  
-000179d0: 2020 2222 220a 2020 2020 4120 7365 7420    """.    A set 
-000179e0: 6f66 2049 4473 2074 6861 7420 7573 6573  of IDs that uses
-000179f0: 206d 616a 6f72 6974 7920 7175 6f72 756d   majority quorum
-00017a00: 7320 746f 206d 616b 6520 6465 6369 7369  s to make decisi
-00017a10: 6f6e 732e 0a20 2020 2022 2222 0a0a 2020  ons..    """..  
-00017a20: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00017a30: 656c 662c 2076 6f74 6572 733a 2053 6574  elf, voters: Set
-00017a40: 5b69 6e74 5d29 202d 3e20 4e6f 6e65 3a20  [int]) -> None: 
-00017a50: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-00017a60: 5f72 6566 2873 656c 6629 202d 3e20 224d  _ref(self) -> "M
-00017a70: 616a 6f72 6974 7943 6f6e 6669 6752 6566  ajorityConfigRef
-00017a80: 223a 202e 2e2e 0a0a 636c 6173 7320 4d61  ": .....class Ma
-00017a90: 6a6f 7269 7479 436f 6e66 6967 5265 6628  jorityConfigRef(
-00017aa0: 5f5f 4150 495f 4d61 6a6f 7269 7479 436f  __API_MajorityCo
-00017ab0: 6e66 6967 293a 0a20 2020 2022 2222 0a20  nfig):.    """. 
-00017ac0: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
-00017ad0: 6520 6f66 203a 636c 6173 733a 604d 616a  e of :class:`Maj
-00017ae0: 6f72 6974 7943 6f6e 6669 6760 2e0a 2020  orityConfig`..  
-00017af0: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-00017b00: 5049 5f49 6e66 6c69 6768 7473 285f 5f43  PI_Inflights(__C
-00017b10: 6c6f 6e65 6162 6c65 293a 0a20 2020 2064  loneable):.    d
-00017b20: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-00017b30: 3e20 2249 6e66 6c69 6768 7473 223a 202e  > "Inflights": .
-00017b40: 2e2e 0a20 2020 2064 6566 2061 6464 2873  ...    def add(s
-00017b50: 656c 662c 2069 6e66 6c69 6768 743a 2069  elf, inflight: i
-00017b60: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00017b70: 2020 2020 2022 2222 4164 6473 2061 6e20       """Adds an 
-00017b80: 696e 666c 6967 6874 2069 6e74 6f20 696e  inflight into in
-00017b90: 666c 6967 6874 7322 2222 0a20 2020 2064  flights""".    d
-00017ba0: 6566 2066 756c 6c28 7365 6c66 2920 2d3e  ef full(self) ->
-00017bb0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00017bc0: 2222 5265 7475 726e 7320 7472 7565 2069  ""Returns true i
-00017bd0: 6620 7468 6520 696e 666c 6967 6874 7320  f the inflights 
-00017be0: 6973 2066 756c 6c2e 2222 220a 2020 2020  is full.""".    
-00017bf0: 6465 6620 7265 7365 7428 7365 6c66 2920  def reset(self) 
-00017c00: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00017c10: 2022 2222 4672 6565 7320 616c 6c20 696e   """Frees all in
-00017c20: 666c 6967 6874 732e 2222 220a 2020 2020  flights.""".    
-00017c30: 6465 6620 6672 6565 5f74 6f28 7365 6c66  def free_to(self
-00017c40: 2c20 746f 3a20 696e 7429 202d 3e20 4e6f  , to: int) -> No
-00017c50: 6e65 3a0a 2020 2020 2020 2020 2222 2246  ne:.        """F
-00017c60: 7265 6573 2074 6865 2069 6e66 6c69 6768  rees the infligh
-00017c70: 7473 2073 6d61 6c6c 6572 206f 7220 6571  ts smaller or eq
-00017c80: 7561 6c20 746f 2074 6865 2067 6976 656e  ual to the given
-00017c90: 2060 746f 6020 666c 6967 6874 2e22 2222   `to` flight."""
-00017ca0: 0a20 2020 2064 6566 2066 7265 655f 6669  .    def free_fi
-00017cb0: 7273 745f 6f6e 6528 7365 6c66 2920 2d3e  rst_one(self) ->
-00017cc0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00017cd0: 2222 4672 6565 7320 7468 6520 6669 7273  ""Frees the firs
-00017ce0: 7420 6275 6666 6572 2065 6e74 7279 2e22  t buffer entry."
-00017cf0: 2222 0a20 2020 2064 6566 206d 6179 6265  "".    def maybe
-00017d00: 5f66 7265 655f 6275 6666 6572 2873 656c  _free_buffer(sel
-00017d10: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-00017d20: 2020 2020 2222 2246 7265 6520 756e 7573      """Free unus
-00017d30: 6564 206d 656d 6f72 7922 2222 0a20 2020  ed memory""".   
-00017d40: 2064 6566 2062 7566 6665 725f 6361 7061   def buffer_capa
-00017d50: 6369 7479 2873 656c 6629 202d 3e20 696e  city(self) -> in
-00017d60: 743a 0a20 2020 2020 2020 2022 2222 4361  t:.        """Ca
-00017d70: 7061 6369 7479 206f 6620 7468 6520 696e  pacity of the in
-00017d80: 7465 726e 616c 2062 7566 6665 722e 2222  ternal buffer.""
-00017d90: 220a 2020 2020 6465 6620 6275 6666 6572  ".    def buffer
-00017da0: 5f69 735f 616c 6c6f 6361 7465 6428 7365  _is_allocated(se
-00017db0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00017dc0: 2020 2020 2022 2222 5768 6574 6865 7220       """Whether 
-00017dd0: 6275 6666 6572 2069 7320 616c 6c6f 6361  buffer is alloca
-00017de0: 7465 6420 6f72 206e 6f74 2e20 4974 2773  ted or not. It's
-00017df0: 2066 6f72 2074 6573 7473 2e22 2222 0a20   for tests.""". 
-00017e00: 2020 2064 6566 2063 6f75 6e74 2873 656c     def count(sel
-00017e10: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00017e20: 2020 2022 2222 4e75 6d62 6572 206f 6620     """Number of 
-00017e30: 696e 666c 6967 6874 206d 6573 7361 6765  inflight message
-00017e40: 732e 2049 7427 7320 666f 7220 7465 7374  s. It's for test
-00017e50: 732e 2222 220a 2020 2020 6465 6620 7365  s.""".    def se
-00017e60: 745f 6361 7028 7365 6c66 2c20 696e 636f  t_cap(self, inco
-00017e70: 6d69 6e67 5f63 6170 3a20 696e 7429 202d  ming_cap: int) -
-00017e80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00017e90: 2222 220a 2020 2020 2020 2020 4164 6a75  """.        Adju
-00017ea0: 7374 2069 6e66 6c69 6768 7420 6275 6666  st inflight buff
-00017eb0: 6572 2063 6170 6163 6974 792e 2053 6574  er capacity. Set
-00017ec0: 2069 7420 746f 2060 3060 2077 696c 6c20   it to `0` will 
-00017ed0: 6469 7361 626c 6520 7468 6520 7072 6f67  disable the prog
-00017ee0: 7265 7373 2e0a 2020 2020 2020 2020 4361  ress..        Ca
-00017ef0: 6c6c 696e 6720 6974 2062 6574 7765 656e  lling it between
-00017f00: 2060 7365 6c66 2e66 756c 6c28 2960 2061   `self.full()` a
-00017f10: 6e64 2060 7365 6c66 2e61 6464 2829 6020  nd `self.add()` 
-00017f20: 6361 6e20 6361 7573 6520 6120 7061 6e69  can cause a pani
-00017f30: 632e 0a20 2020 2020 2020 2022 2222 0a0a  c..        """..
-00017f40: 636c 6173 7320 496e 666c 6967 6874 7328  class Inflights(
-00017f50: 5f5f 4150 495f 496e 666c 6967 6874 7329  __API_Inflights)
-00017f60: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
-00017f70: 6275 6666 6572 206f 6620 696e 666c 6967  buffer of inflig
-00017f80: 6874 206d 6573 7361 6765 732e 0a20 2020  ht messages..   
-00017f90: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
-00017fa0: 696e 6974 5f5f 2873 656c 662c 2063 6170  init__(self, cap
-00017fb0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a20  : int) -> None: 
-00017fc0: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-00017fd0: 5f72 6566 2873 656c 6629 202d 3e20 2249  _ref(self) -> "I
-00017fe0: 6e66 6c69 6768 7473 5265 6622 3a20 2e2e  nflightsRef": ..
-00017ff0: 2e0a 0a63 6c61 7373 2049 6e66 6c69 6768  ...class Infligh
-00018000: 7473 5265 6628 5f5f 4150 495f 496e 666c  tsRef(__API_Infl
-00018010: 6967 6874 7329 3a0a 2020 2020 2222 220a  ights):.    """.
-00018020: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
-00018030: 7065 206f 6620 3a63 6c61 7373 3a60 496e  pe of :class:`In
-00018040: 666c 6967 6874 7352 6566 602e 0a20 2020  flightsRef`..   
-00018050: 2022 2222 0a0a 636c 6173 7320 5f5f 4150   """..class __AP
-00018060: 495f 436f 6e66 6967 285f 5f43 6c6f 6e65  I_Config(__Clone
-00018070: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
-00018080: 6c6f 6e65 2873 656c 6629 202d 3e20 2243  lone(self) -> "C
-00018090: 6f6e 6669 6722 3a20 2e2e 2e0a 2020 2020  onfig": ....    
-000180a0: 6465 6620 6d69 6e5f 656c 6563 7469 6f6e  def min_election
-000180b0: 5f74 6963 6b28 7365 6c66 2920 2d3e 2069  _tick(self) -> i
-000180c0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-000180d0: 2020 2020 2020 2020 606d 696e 5f65 6c65          `min_ele
-000180e0: 6374 696f 6e5f 7469 636b 603a 2054 6865  ction_tick`: The
-000180f0: 206d 696e 696d 756d 206e 756d 6265 7220   minimum number 
-00018100: 6f66 2074 6963 6b73 2062 6566 6f72 6520  of ticks before 
-00018110: 616e 2065 6c65 6374 696f 6e2e 0a20 2020  an election..   
-00018120: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00018130: 2073 6574 5f6d 696e 5f65 6c65 6374 696f   set_min_electio
-00018140: 6e5f 7469 636b 2873 656c 662c 206d 696e  n_tick(self, min
-00018150: 5f65 6c65 6374 696f 6e5f 7469 636b 3a20  _election_tick: 
-00018160: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00018170: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00018180: 2020 606d 696e 5f65 6c65 6374 696f 6e5f    `min_election_
-00018190: 7469 636b 603a 2054 6865 206d 696e 696d  tick`: The minim
-000181a0: 756d 206e 756d 6265 7220 6f66 2074 6963  um number of tic
-000181b0: 6b73 2062 6566 6f72 6520 616e 2065 6c65  ks before an ele
-000181c0: 6374 696f 6e2e 0a20 2020 2020 2020 2022  ction..        "
-000181d0: 2222 0a20 2020 2064 6566 206d 6178 5f65  "".    def max_e
-000181e0: 6c65 6374 696f 6e5f 7469 636b 2873 656c  lection_tick(sel
-000181f0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00018200: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00018210: 6d61 785f 656c 6563 7469 6f6e 5f74 6963  max_election_tic
-00018220: 6b60 3a20 5468 6520 6d61 7869 6d75 6d20  k`: The maximum 
-00018230: 6e75 6d62 6572 206f 6620 7469 636b 7320  number of ticks 
-00018240: 6265 666f 7265 2061 6e20 656c 6563 7469  before an electi
-00018250: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-00018260: 2020 2020 6465 6620 7365 745f 6d61 785f      def set_max_
-00018270: 656c 6563 7469 6f6e 5f74 6963 6b28 7365  election_tick(se
-00018280: 6c66 2c20 6d61 785f 656c 6563 7469 6f6e  lf, max_election
-00018290: 5f74 6963 6b3a 2069 6e74 2920 2d3e 204e  _tick: int) -> N
-000182a0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000182b0: 0a20 2020 2020 2020 2060 6d61 785f 656c  .        `max_el
-000182c0: 6563 7469 6f6e 5f74 6963 6b60 3a20 5468  ection_tick`: Th
-000182d0: 6520 6d61 7869 6d75 6d20 6e75 6d62 6572  e maximum number
-000182e0: 206f 6620 7469 636b 7320 6265 666f 7265   of ticks before
-000182f0: 2061 6e20 656c 6563 7469 6f6e 2e0a 2020   an election..  
-00018300: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00018310: 6620 6765 745f 7265 6164 5f6f 6e6c 795f  f get_read_only_
-00018320: 6f70 7469 6f6e 2873 656c 6629 202d 3e20  option(self) -> 
-00018330: 2252 6561 644f 6e6c 794f 7074 696f 6e22  "ReadOnlyOption"
-00018340: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00018350: 2020 2020 2020 6072 6561 645f 6f6e 6c79        `read_only
-00018360: 5f6f 7074 696f 6e60 3a20 4368 6f6f 7365  _option`: Choose
-00018370: 2074 6865 206c 696e 6561 7269 7a61 6269   the linearizabi
-00018380: 6c69 7479 206d 6f64 6520 6f72 2074 6865  lity mode or the
-00018390: 206c 6561 7365 206d 6f64 6520 746f 2072   lease mode to r
-000183a0: 6561 6420 6461 7461 2e20 4966 2079 6f75  ead data. If you
-000183b0: 2064 6f6e e280 9974 2063 6172 6520 6162   don...t care ab
-000183c0: 6f75 7420 7468 6520 7265 6164 2063 6f6e  out the read con
-000183d0: 7369 7374 656e 6379 2061 6e64 2077 616e  sistency and wan
-000183e0: 7420 6120 6869 6768 6572 2072 6561 6420  t a higher read 
-000183f0: 7065 7266 6f72 6d61 6e63 652c 2079 6f75  performance, you
-00018400: 2063 616e 2075 7365 2074 6865 206c 6561   can use the lea
-00018410: 7365 206d 6f64 652e 0a20 2020 2020 2020  se mode..       
-00018420: 2053 6574 7469 6e67 2074 6869 7320 746f   Setting this to
-00018430: 2060 4c65 6173 6542 6173 6564 6020 7265   `LeaseBased` re
-00018440: 7175 6972 6573 2060 6368 6563 6b5f 7175  quires `check_qu
-00018450: 6f72 756d 203d 2074 7275 6560 2e0a 2020  orum = true`..  
-00018460: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00018470: 6620 7365 745f 7265 6164 5f6f 6e6c 795f  f set_read_only_
-00018480: 6f70 7469 6f6e 2873 656c 662c 2072 6561  option(self, rea
-00018490: 645f 6f6e 6c79 5f6f 7074 696f 6e3a 2022  d_only_option: "
-000184a0: 5265 6164 4f6e 6c79 4f70 7469 6f6e 2229  ReadOnlyOption")
-000184b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000184c0: 2020 2222 220a 2020 2020 2020 2020 6072    """.        `r
-000184d0: 6561 645f 6f6e 6c79 5f6f 7074 696f 6e60  ead_only_option`
-000184e0: 3a20 4368 6f6f 7365 2074 6865 206c 696e  : Choose the lin
-000184f0: 6561 7269 7a61 6269 6c69 7479 206d 6f64  earizability mod
-00018500: 6520 6f72 2074 6865 206c 6561 7365 206d  e or the lease m
-00018510: 6f64 6520 746f 2072 6561 6420 6461 7461  ode to read data
-00018520: 2e20 4966 2079 6f75 2064 6f6e e280 9974  . If you don...t
-00018530: 2063 6172 6520 6162 6f75 7420 7468 6520   care about the 
-00018540: 7265 6164 2063 6f6e 7369 7374 656e 6379  read consistency
-00018550: 2061 6e64 2077 616e 7420 6120 6869 6768   and want a high
-00018560: 6572 2072 6561 6420 7065 7266 6f72 6d61  er read performa
-00018570: 6e63 652c 2079 6f75 2063 616e 2075 7365  nce, you can use
-00018580: 2074 6865 206c 6561 7365 206d 6f64 652e   the lease mode.
-00018590: 0a20 2020 2020 2020 2053 6574 7469 6e67  .        Setting
-000185a0: 2074 6869 7320 746f 2060 4c65 6173 6542   this to `LeaseB
-000185b0: 6173 6564 6020 7265 7175 6972 6573 2060  ased` requires `
-000185c0: 6368 6563 6b5f 7175 6f72 756d 203d 2074  check_quorum = t
-000185d0: 7275 6560 2e0a 2020 2020 2020 2020 2222  rue`..        ""
-000185e0: 220a 2020 2020 6465 6620 6765 745f 6964  ".    def get_id
-000185f0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00018600: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00018610: 2020 2060 6964 603a 2054 6865 2069 6465     `id`: The ide
-00018620: 6e74 6974 7920 6f66 2074 6865 206c 6f63  ntity of the loc
-00018630: 616c 2072 6166 742e 2049 7420 6361 6e6e  al raft. It cann
-00018640: 6f74 2062 6520 302c 2061 6e64 206d 7573  ot be 0, and mus
-00018650: 7420 6265 2075 6e69 7175 6520 696e 2074  t be unique in t
-00018660: 6865 2067 726f 7570 2e0a 2020 2020 2020  he group..      
-00018670: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00018680: 745f 6964 2873 656c 662c 2069 643a 2069  t_id(self, id: i
-00018690: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000186a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000186b0: 2060 6964 603a 2054 6865 2069 6465 6e74   `id`: The ident
-000186c0: 6974 7920 6f66 2074 6865 206c 6f63 616c  ity of the local
-000186d0: 2072 6166 742e 2049 7420 6361 6e6e 6f74   raft. It cannot
-000186e0: 2062 6520 302c 2061 6e64 206d 7573 7420   be 0, and must 
-000186f0: 6265 2075 6e69 7175 6520 696e 2074 6865  be unique in the
-00018700: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
-00018710: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-00018720: 656c 6563 7469 6f6e 5f74 6963 6b28 7365  election_tick(se
-00018730: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00018740: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00018750: 6065 6c65 6374 696f 6e5f 7469 636b 603a  `election_tick`:
-00018760: 2054 6865 206e 756d 6265 7220 6f66 206e   The number of n
-00018770: 6f64 652e 7469 636b 2069 6e76 6f63 6174  ode.tick invocat
-00018780: 696f 6e73 2074 6861 7420 6d75 7374 2070  ions that must p
-00018790: 6173 7320 6265 7477 6565 6e0a 2020 2020  ass between.    
-000187a0: 2020 2020 656c 6563 7469 6f6e 732e 2054      elections. T
-000187b0: 6861 7420 6973 2c20 6966 2061 2066 6f6c  hat is, if a fol
-000187c0: 6c6f 7765 7220 646f 6573 206e 6f74 2072  lower does not r
-000187d0: 6563 6569 7665 2061 6e79 206d 6573 7361  eceive any messa
-000187e0: 6765 2066 726f 6d20 7468 650a 2020 2020  ge from the.    
-000187f0: 2020 2020 6c65 6164 6572 206f 6620 6375      leader of cu
-00018800: 7272 656e 7420 7465 726d 2062 6566 6f72  rrent term befor
-00018810: 6520 456c 6563 7469 6f6e 5469 636b 2068  e ElectionTick h
-00018820: 6173 2065 6c61 7073 6564 2c20 6974 2077  as elapsed, it w
-00018830: 696c 6c20 6265 636f 6d65 0a20 2020 2020  ill become.     
-00018840: 2020 2063 616e 6469 6461 7465 2061 6e64     candidate and
-00018850: 2073 7461 7274 2061 6e20 656c 6563 7469   start an electi
-00018860: 6f6e 2e20 656c 6563 7469 6f6e 5f74 6963  on. election_tic
-00018870: 6b20 6d75 7374 2062 6520 6772 6561 7465  k must be greate
-00018880: 7220 7468 616e 0a20 2020 2020 2020 2048  r than.        H
-00018890: 6561 7274 6265 6174 5469 636b 2e20 5765  eartbeatTick. We
-000188a0: 2073 7567 6765 7374 2065 6c65 6374 696f   suggest electio
-000188b0: 6e5f 7469 636b 203d 2031 3020 2a20 4865  n_tick = 10 * He
-000188c0: 6172 7462 6561 7454 6963 6b20 746f 2061  artbeatTick to a
-000188d0: 766f 6964 0a20 2020 2020 2020 2075 6e6e  void.        unn
-000188e0: 6563 6573 7361 7279 206c 6561 6465 7220  ecessary leader 
-000188f0: 7377 6974 6368 696e 670a 2020 2020 2020  switching.      
-00018900: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00018910: 745f 656c 6563 7469 6f6e 5f74 6963 6b28  t_election_tick(
-00018920: 7365 6c66 2c20 656c 6563 7469 6f6e 5f74  self, election_t
-00018930: 6963 6b3a 2069 6e74 2920 2d3e 204e 6f6e  ick: int) -> Non
-00018940: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00018950: 2020 2020 2020 2060 656c 6563 7469 6f6e         `election
-00018960: 5f74 6963 6b60 3a20 5468 6520 6e75 6d62  _tick`: The numb
-00018970: 6572 206f 6620 6e6f 6465 2e74 6963 6b20  er of node.tick 
-00018980: 696e 766f 6361 7469 6f6e 7320 7468 6174  invocations that
-00018990: 206d 7573 7420 7061 7373 2062 6574 7765   must pass betwe
-000189a0: 656e 0a20 2020 2020 2020 2065 6c65 6374  en.        elect
-000189b0: 696f 6e73 2e20 5468 6174 2069 732c 2069  ions. That is, i
-000189c0: 6620 6120 666f 6c6c 6f77 6572 2064 6f65  f a follower doe
-000189d0: 7320 6e6f 7420 7265 6365 6976 6520 616e  s not receive an
-000189e0: 7920 6d65 7373 6167 6520 6672 6f6d 2074  y message from t
-000189f0: 6865 0a20 2020 2020 2020 206c 6561 6465  he.        leade
-00018a00: 7220 6f66 2063 7572 7265 6e74 2074 6572  r of current ter
-00018a10: 6d20 6265 666f 7265 2045 6c65 6374 696f  m before Electio
-00018a20: 6e54 6963 6b20 6861 7320 656c 6170 7365  nTick has elapse
-00018a30: 642c 2069 7420 7769 6c6c 2062 6563 6f6d  d, it will becom
-00018a40: 650a 2020 2020 2020 2020 6361 6e64 6964  e.        candid
-00018a50: 6174 6520 616e 6420 7374 6172 7420 616e  ate and start an
-00018a60: 2065 6c65 6374 696f 6e2e 2065 6c65 6374   election. elect
-00018a70: 696f 6e5f 7469 636b 206d 7573 7420 6265  ion_tick must be
-00018a80: 2067 7265 6174 6572 2074 6861 6e0a 2020   greater than.  
-00018a90: 2020 2020 2020 4865 6172 7462 6561 7454        HeartbeatT
-00018aa0: 6963 6b2e 2057 6520 7375 6767 6573 7420  ick. We suggest 
-00018ab0: 656c 6563 7469 6f6e 5f74 6963 6b20 3d20  election_tick = 
-00018ac0: 3130 202a 2048 6561 7274 6265 6174 5469  10 * HeartbeatTi
-00018ad0: 636b 2074 6f20 6176 6f69 640a 2020 2020  ck to avoid.    
-00018ae0: 2020 2020 756e 6e65 6365 7373 6172 7920      unnecessary 
-00018af0: 6c65 6164 6572 2073 7769 7463 6869 6e67  leader switching
-00018b00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00018b10: 2064 6566 2067 6574 5f68 6561 7274 6265   def get_heartbe
-00018b20: 6174 5f74 6963 6b28 7365 6c66 2920 2d3e  at_tick(self) ->
-00018b30: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00018b40: 220a 2020 2020 2020 2020 6068 6561 7274  ".        `heart
-00018b50: 6265 6174 5f74 6963 6b60 3a20 4865 6172  beat_tick`: Hear
-00018b60: 7462 6561 7454 6963 6b20 6973 2074 6865  tbeatTick is the
-00018b70: 206e 756d 6265 7220 6f66 206e 6f64 652e   number of node.
-00018b80: 7469 636b 2069 6e76 6f63 6174 696f 6e73  tick invocations
-00018b90: 2074 6861 7420 6d75 7374 2070 6173 7320   that must pass 
-00018ba0: 6265 7477 6565 6e0a 2020 2020 2020 2020  between.        
-00018bb0: 6865 6172 7462 6561 7473 2e20 5468 6174  heartbeats. That
-00018bc0: 2069 732c 2061 206c 6561 6465 7220 7365   is, a leader se
-00018bd0: 6e64 7320 6865 6172 7462 6561 7420 6d65  nds heartbeat me
-00018be0: 7373 6167 6573 2074 6f20 6d61 696e 7461  ssages to mainta
-00018bf0: 696e 2069 7473 0a20 2020 2020 2020 206c  in its.        l
-00018c00: 6561 6465 7273 6869 7020 6576 6572 7920  eadership every 
-00018c10: 6865 6172 7462 6561 7420 7469 636b 732e  heartbeat ticks.
-00018c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00018c30: 2064 6566 2073 6574 5f68 6561 7274 6265   def set_heartbe
-00018c40: 6174 5f74 6963 6b28 7365 6c66 2c20 6865  at_tick(self, he
-00018c50: 6172 7462 6561 745f 7469 636b 3a20 696e  artbeat_tick: in
-00018c60: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00018c70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00018c80: 6068 6561 7274 6265 6174 5f74 6963 6b60  `heartbeat_tick`
-00018c90: 3a20 4865 6172 7462 6561 7454 6963 6b20  : HeartbeatTick 
-00018ca0: 6973 2074 6865 206e 756d 6265 7220 6f66  is the number of
-00018cb0: 206e 6f64 652e 7469 636b 2069 6e76 6f63   node.tick invoc
-00018cc0: 6174 696f 6e73 2074 6861 7420 6d75 7374  ations that must
-00018cd0: 2070 6173 7320 6265 7477 6565 6e0a 2020   pass between.  
-00018ce0: 2020 2020 2020 6865 6172 7462 6561 7473        heartbeats
-00018cf0: 2e20 5468 6174 2069 732c 2061 206c 6561  . That is, a lea
-00018d00: 6465 7220 7365 6e64 7320 6865 6172 7462  der sends heartb
-00018d10: 6561 7420 6d65 7373 6167 6573 2074 6f20  eat messages to 
-00018d20: 6d61 696e 7461 696e 2069 7473 0a20 2020  maintain its.   
-00018d30: 2020 2020 206c 6561 6465 7273 6869 7020       leadership 
-00018d40: 6576 6572 7920 6865 6172 7462 6561 7420  every heartbeat 
-00018d50: 7469 636b 732e 0a20 2020 2020 2020 2022  ticks..        "
-00018d60: 2222 0a20 2020 2064 6566 2067 6574 5f6d  "".    def get_m
-00018d70: 6178 5f73 697a 655f 7065 725f 6d73 6728  ax_size_per_msg(
-00018d80: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-00018d90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00018da0: 2020 606d 6178 5f73 697a 655f 7065 725f    `max_size_per_
-00018db0: 6d73 6760 3a20 4c69 6d69 7420 7468 6520  msg`: Limit the 
-00018dc0: 6d61 7820 7369 7a65 206f 6620 6561 6368  max size of each
-00018dd0: 2061 7070 656e 6420 6d65 7373 6167 652e   append message.
-00018de0: 2053 6d61 6c6c 6572 2076 616c 7565 206c   Smaller value l
-00018df0: 6f77 6572 730a 2020 2020 2020 2020 7468  owers.        th
-00018e00: 6520 7261 6674 2072 6563 6f76 6572 7920  e raft recovery 
-00018e10: 636f 7374 2869 6e69 7469 616c 2070 726f  cost(initial pro
-00018e20: 6269 6e67 2061 6e64 206d 6573 7361 6765  bing and message
-00018e30: 206c 6f73 7420 6475 7269 6e67 206e 6f72   lost during nor
-00018e40: 6d61 6c20 6f70 6572 6174 696f 6e29 2e0a  mal operation)..
-00018e50: 2020 2020 2020 2020 4f6e 2074 6865 206f          On the o
-00018e60: 7468 6572 2073 6964 652c 2069 7420 6d69  ther side, it mi
-00018e70: 6768 7420 6166 6665 6374 2074 6865 2074  ght affect the t
-00018e80: 6872 6f75 6768 7075 7420 6475 7269 6e67  hroughput during
-00018e90: 206e 6f72 6d61 6c20 7265 706c 6963 6174   normal replicat
-00018ea0: 696f 6e2e 0a20 2020 2020 2020 204e 6f74  ion..        Not
-00018eb0: 653a 206d 6174 682e 4d61 7855 7573 697a  e: math.MaxUusiz
-00018ec0: 6536 3420 666f 7220 756e 6c69 6d69 7465  e64 for unlimite
-00018ed0: 642c 2030 2066 6f72 2061 7420 6d6f 7374  d, 0 for at most
-00018ee0: 206f 6e65 2065 6e74 7279 2070 6572 206d   one entry per m
-00018ef0: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
-00018f00: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00018f10: 6d61 785f 7369 7a65 5f70 6572 5f6d 7367  max_size_per_msg
-00018f20: 2873 656c 662c 206d 6178 5f73 697a 655f  (self, max_size_
-00018f30: 7065 725f 6d73 673a 2069 6e74 2920 2d3e  per_msg: int) ->
-00018f40: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00018f50: 2222 0a20 2020 2020 2020 2060 6d61 785f  "".        `max_
-00018f60: 7369 7a65 5f70 6572 5f6d 7367 603a 204c  size_per_msg`: L
-00018f70: 696d 6974 2074 6865 206d 6178 2073 697a  imit the max siz
-00018f80: 6520 6f66 2065 6163 6820 6170 7065 6e64  e of each append
-00018f90: 206d 6573 7361 6765 2e20 536d 616c 6c65   message. Smalle
-00018fa0: 7220 7661 6c75 6520 6c6f 7765 7273 0a20  r value lowers. 
-00018fb0: 2020 2020 2020 2074 6865 2072 6166 7420         the raft 
-00018fc0: 7265 636f 7665 7279 2063 6f73 7428 696e  recovery cost(in
-00018fd0: 6974 6961 6c20 7072 6f62 696e 6720 616e  itial probing an
-00018fe0: 6420 6d65 7373 6167 6520 6c6f 7374 2064  d message lost d
-00018ff0: 7572 696e 6720 6e6f 726d 616c 206f 7065  uring normal ope
-00019000: 7261 7469 6f6e 292e 0a20 2020 2020 2020  ration)..       
-00019010: 204f 6e20 7468 6520 6f74 6865 7220 7369   On the other si
-00019020: 6465 2c20 6974 206d 6967 6874 2061 6666  de, it might aff
-00019030: 6563 7420 7468 6520 7468 726f 7567 6870  ect the throughp
-00019040: 7574 2064 7572 696e 6720 6e6f 726d 616c  ut during normal
-00019050: 2072 6570 6c69 6361 7469 6f6e 2e0a 2020   replication..  
-00019060: 2020 2020 2020 4e6f 7465 3a20 6d61 7468        Note: math
-00019070: 2e4d 6178 5575 7369 7a65 3634 2066 6f72  .MaxUusize64 for
-00019080: 2075 6e6c 696d 6974 6564 2c20 3020 666f   unlimited, 0 fo
-00019090: 7220 6174 206d 6f73 7420 6f6e 6520 656e  r at most one en
-000190a0: 7472 7920 7065 7220 6d65 7373 6167 652e  try per message.
-000190b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000190c0: 2064 6566 2067 6574 5f6d 6178 5f69 6e66   def get_max_inf
-000190d0: 6c69 6768 745f 6d73 6773 2873 656c 6629  light_msgs(self)
-000190e0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-000190f0: 2022 2222 0a20 2020 2020 2020 2060 6d61   """.        `ma
-00019100: 785f 696e 666c 6967 6874 5f6d 7367 7360  x_inflight_msgs`
-00019110: 3a20 4c69 6d69 7420 7468 6520 6d61 7820  : Limit the max 
-00019120: 6e75 6d62 6572 206f 6620 696e 2d66 6c69  number of in-fli
-00019130: 6768 7420 6170 7065 6e64 206d 6573 7361  ght append messa
-00019140: 6765 7320 6475 7269 6e67 206f 7074 696d  ges during optim
-00019150: 6973 7469 630a 2020 2020 2020 2020 7265  istic.        re
-00019160: 706c 6963 6174 696f 6e20 7068 6173 652e  plication phase.
-00019170: 2054 6865 2061 7070 6c69 6361 7469 6f6e   The application
-00019180: 2074 7261 6e73 706f 7274 6174 696f 6e20   transportation 
-00019190: 6c61 7965 7220 7573 7561 6c6c 7920 6861  layer usually ha
-000191a0: 7320 6974 7320 6f77 6e20 7365 6e64 696e  s its own sendin
-000191b0: 670a 2020 2020 2020 2020 6275 6666 6572  g.        buffer
-000191c0: 206f 7665 7220 5443 502f 5544 502e 2053   over TCP/UDP. S
-000191d0: 6574 2074 6f20 6176 6f69 6420 6f76 6572  et to avoid over
-000191e0: 666c 6f77 696e 6720 7468 6174 2073 656e  flowing that sen
-000191f0: 6469 6e67 2062 7566 6665 722e 0a20 2020  ding buffer..   
-00019200: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00019210: 2073 6574 5f6d 6178 5f69 6e66 6c69 6768   set_max_infligh
-00019220: 745f 6d73 6773 2873 656c 662c 206d 6178  t_msgs(self, max
-00019230: 5f69 6e66 6c69 6768 745f 6d73 6773 3a20  _inflight_msgs: 
-00019240: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00019250: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00019260: 2020 606d 6178 5f69 6e66 6c69 6768 745f    `max_inflight_
-00019270: 6d73 6773 603a 204c 696d 6974 2074 6865  msgs`: Limit the
-00019280: 206d 6178 206e 756d 6265 7220 6f66 2069   max number of i
-00019290: 6e2d 666c 6967 6874 2061 7070 656e 6420  n-flight append 
-000192a0: 6d65 7373 6167 6573 2064 7572 696e 6720  messages during 
-000192b0: 6f70 7469 6d69 7374 6963 0a20 2020 2020  optimistic.     
-000192c0: 2020 2072 6570 6c69 6361 7469 6f6e 2070     replication p
-000192d0: 6861 7365 2e20 5468 6520 6170 706c 6963  hase. The applic
-000192e0: 6174 696f 6e20 7472 616e 7370 6f72 7461  ation transporta
-000192f0: 7469 6f6e 206c 6179 6572 2075 7375 616c  tion layer usual
-00019300: 6c79 2068 6173 2069 7473 206f 776e 2073  ly has its own s
-00019310: 656e 6469 6e67 0a20 2020 2020 2020 2062  ending.        b
-00019320: 7566 6665 7220 6f76 6572 2054 4350 2f55  uffer over TCP/U
-00019330: 4450 2e20 5365 7420 746f 2061 766f 6964  DP. Set to avoid
-00019340: 206f 7665 7266 6c6f 7769 6e67 2074 6861   overflowing tha
-00019350: 7420 7365 6e64 696e 6720 6275 6666 6572  t sending buffer
-00019360: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00019370: 2020 6465 6620 6765 745f 6170 706c 6965    def get_applie
-00019380: 6428 7365 6c66 2920 2d3e 2069 6e74 3a0a  d(self) -> int:.
-00019390: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000193a0: 2020 2020 6061 7070 6c69 6564 603a 2041      `applied`: A
-000193b0: 7070 6c69 6564 2069 7320 7468 6520 6c61  pplied is the la
-000193c0: 7374 2061 7070 6c69 6564 2069 6e64 6578  st applied index
-000193d0: 2e20 4974 2073 686f 756c 6420 6f6e 6c79  . It should only
-000193e0: 2062 6520 7365 7420 7768 656e 2072 6573   be set when res
-000193f0: 7461 7274 696e 670a 2020 2020 2020 2020  tarting.        
-00019400: 7261 6674 2e20 7261 6674 2077 696c 6c20  raft. raft will 
-00019410: 6e6f 7420 7265 7475 726e 2065 6e74 7269  not return entri
-00019420: 6573 2074 6f20 7468 6520 6170 706c 6963  es to the applic
-00019430: 6174 696f 6e20 736d 616c 6c65 7220 6f72  ation smaller or
-00019440: 2065 7175 616c 2074 6f20 4170 706c 6965   equal to Applie
-00019450: 642e 0a20 2020 2020 2020 2049 6620 4170  d..        If Ap
-00019460: 706c 6965 6420 6973 2075 6e73 6574 2077  plied is unset w
-00019470: 6865 6e20 7265 7374 6172 7469 6e67 2c20  hen restarting, 
-00019480: 7261 6674 206d 6967 6874 2072 6574 7572  raft might retur
-00019490: 6e20 7072 6576 696f 7573 2061 7070 6c69  n previous appli
-000194a0: 6564 2065 6e74 7269 6573 2e0a 2020 2020  ed entries..    
-000194b0: 2020 2020 5468 6973 2069 7320 6120 7665      This is a ve
-000194c0: 7279 2061 7070 6c69 6361 7469 6f6e 2064  ry application d
-000194d0: 6570 656e 6465 6e74 2063 6f6e 6669 6775  ependent configu
-000194e0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-000194f0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00019500: 6170 706c 6965 6428 7365 6c66 2c20 6170  applied(self, ap
-00019510: 706c 6965 643a 2069 6e74 2920 2d3e 204e  plied: int) -> N
-00019520: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00019530: 0a20 2020 2020 2020 2060 6170 706c 6965  .        `applie
-00019540: 6460 3a20 4170 706c 6965 6420 6973 2074  d`: Applied is t
-00019550: 6865 206c 6173 7420 6170 706c 6965 6420  he last applied 
-00019560: 696e 6465 782e 2049 7420 7368 6f75 6c64  index. It should
-00019570: 206f 6e6c 7920 6265 2073 6574 2077 6865   only be set whe
-00019580: 6e20 7265 7374 6172 7469 6e67 0a20 2020  n restarting.   
-00019590: 2020 2020 2072 6166 742e 2072 6166 7420       raft. raft 
-000195a0: 7769 6c6c 206e 6f74 2072 6574 7572 6e20  will not return 
-000195b0: 656e 7472 6965 7320 746f 2074 6865 2061  entries to the a
-000195c0: 7070 6c69 6361 7469 6f6e 2073 6d61 6c6c  pplication small
-000195d0: 6572 206f 7220 6571 7561 6c20 746f 2041  er or equal to A
-000195e0: 7070 6c69 6564 2e0a 2020 2020 2020 2020  pplied..        
-000195f0: 4966 2041 7070 6c69 6564 2069 7320 756e  If Applied is un
-00019600: 7365 7420 7768 656e 2072 6573 7461 7274  set when restart
-00019610: 696e 672c 2072 6166 7420 6d69 6768 7420  ing, raft might 
-00019620: 7265 7475 726e 2070 7265 7669 6f75 7320  return previous 
-00019630: 6170 706c 6965 6420 656e 7472 6965 732e  applied entries.
-00019640: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
-00019650: 2061 2076 6572 7920 6170 706c 6963 6174   a very applicat
-00019660: 696f 6e20 6465 7065 6e64 656e 7420 636f  ion dependent co
-00019670: 6e66 6967 7572 6174 696f 6e2e 0a20 2020  nfiguration..   
-00019680: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00019690: 2067 6574 5f63 6865 636b 5f71 756f 7275   get_check_quoru
-000196a0: 6d28 7365 6c66 2920 2d3e 2062 6f6f 6c3a  m(self) -> bool:
-000196b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000196c0: 2020 2020 2060 6368 6563 6b5f 7175 6f72       `check_quor
-000196d0: 756d 603a 2053 7065 6369 6679 2069 6620  um`: Specify if 
-000196e0: 7468 6520 6c65 6164 6572 2073 686f 756c  the leader shoul
-000196f0: 6420 6368 6563 6b20 7175 6f72 756d 2061  d check quorum a
-00019700: 6374 6976 6974 792e 204c 6561 6465 7220  ctivity. Leader 
-00019710: 7374 6570 7320 646f 776e 2077 6865 6e0a  steps down when.
-00019720: 2020 2020 2020 2020 7175 6f72 756d 2069          quorum i
-00019730: 7320 6e6f 7420 6163 7469 7665 2066 6f72  s not active for
-00019740: 2061 6e20 656c 6563 7469 6f6e 5469 6d65   an electionTime
-00019750: 6f75 742e 0a20 2020 2020 2020 2022 2222  out..        """
-00019760: 0a20 2020 2064 6566 2073 6574 5f63 6865  .    def set_che
-00019770: 636b 5f71 756f 7275 6d28 7365 6c66 2c20  ck_quorum(self, 
-00019780: 6368 6563 6b5f 7175 6f72 756d 3a20 626f  check_quorum: bo
-00019790: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-000197a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000197b0: 2060 6368 6563 6b5f 7175 6f72 756d 603a   `check_quorum`:
-000197c0: 2053 7065 6369 6679 2069 6620 7468 6520   Specify if the 
-000197d0: 6c65 6164 6572 2073 686f 756c 6420 6368  leader should ch
-000197e0: 6563 6b20 7175 6f72 756d 2061 6374 6976  eck quorum activ
-000197f0: 6974 792e 204c 6561 6465 7220 7374 6570  ity. Leader step
-00019800: 7320 646f 776e 2077 6865 6e0a 2020 2020  s down when.    
-00019810: 2020 2020 7175 6f72 756d 2069 7320 6e6f      quorum is no
-00019820: 7420 6163 7469 7665 2066 6f72 2061 6e20  t active for an 
-00019830: 656c 6563 7469 6f6e 5469 6d65 6f75 742e  electionTimeout.
-00019840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019850: 2064 6566 2067 6574 5f70 7265 5f76 6f74   def get_pre_vot
-00019860: 6528 7365 6c66 2920 2d3e 2062 6f6f 6c3a  e(self) -> bool:
-00019870: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019880: 2020 2020 2060 7072 655f 766f 7465 603a       `pre_vote`:
-00019890: 2045 6e61 626c 6573 2074 6865 2050 7265   Enables the Pre
-000198a0: 2d56 6f74 6520 616c 676f 7269 7468 6d20  -Vote algorithm 
-000198b0: 6465 7363 7269 6265 6420 696e 2072 6166  described in raf
-000198c0: 7420 7468 6573 6973 2073 6563 7469 6f6e  t thesis section
-000198d0: 0a20 2020 2020 2020 2039 2e36 2e20 5468  .        9.6. Th
-000198e0: 6973 2070 7265 7665 6e74 7320 6469 7372  is prevents disr
-000198f0: 7570 7469 6f6e 2077 6865 6e20 6120 6e6f  uption when a no
-00019900: 6465 2074 6861 7420 6861 7320 6265 656e  de that has been
-00019910: 2070 6172 7469 7469 6f6e 6564 2061 7761   partitioned awa
-00019920: 790a 2020 2020 2020 2020 7265 6a6f 696e  y.        rejoin
-00019930: 7320 7468 6520 636c 7573 7465 722e 0a20  s the cluster.. 
-00019940: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00019950: 6566 2073 6574 5f70 7265 5f76 6f74 6528  ef set_pre_vote(
-00019960: 7365 6c66 2c20 7072 655f 766f 7465 3a20  self, pre_vote: 
-00019970: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-00019980: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00019990: 2020 2060 7072 655f 766f 7465 603a 2045     `pre_vote`: E
-000199a0: 6e61 626c 6573 2074 6865 2050 7265 2d56  nables the Pre-V
-000199b0: 6f74 6520 616c 676f 7269 7468 6d20 6465  ote algorithm de
-000199c0: 7363 7269 6265 6420 696e 2072 6166 7420  scribed in raft 
-000199d0: 7468 6573 6973 2073 6563 7469 6f6e 0a20  thesis section. 
-000199e0: 2020 2020 2020 2039 2e36 2e20 5468 6973         9.6. This
-000199f0: 2070 7265 7665 6e74 7320 6469 7372 7570   prevents disrup
-00019a00: 7469 6f6e 2077 6865 6e20 6120 6e6f 6465  tion when a node
-00019a10: 2074 6861 7420 6861 7320 6265 656e 2070   that has been p
-00019a20: 6172 7469 7469 6f6e 6564 2061 7761 790a  artitioned away.
-00019a30: 2020 2020 2020 2020 7265 6a6f 696e 7320          rejoins 
-00019a40: 7468 6520 636c 7573 7465 722e 0a20 2020  the cluster..   
-00019a50: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00019a60: 2067 6574 5f62 6174 6368 5f61 7070 656e   get_batch_appen
-00019a70: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
-00019a80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019a90: 2020 2020 2060 6261 7463 685f 6170 7065       `batch_appe
-00019aa0: 6e64 603a 2042 6174 6368 6573 2065 7665  nd`: Batches eve
-00019ab0: 7279 2061 7070 656e 6420 6d73 6720 6966  ry append msg if
-00019ac0: 2061 6e79 2061 7070 656e 6420 6d73 6720   any append msg 
-00019ad0: 616c 7265 6164 7920 6578 6973 7473 0a20  already exists. 
-00019ae0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00019af0: 6566 2073 6574 5f62 6174 6368 5f61 7070  ef set_batch_app
-00019b00: 656e 6428 7365 6c66 2c20 6261 7463 685f  end(self, batch_
-00019b10: 6170 7065 6e64 3a20 626f 6f6c 2920 2d3e  append: bool) ->
-00019b20: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00019b30: 2222 0a20 2020 2020 2020 2060 6261 7463  "".        `batc
-00019b40: 685f 6170 7065 6e64 603a 2042 6174 6368  h_append`: Batch
-00019b50: 6573 2065 7665 7279 2061 7070 656e 6420  es every append 
-00019b60: 6d73 6720 6966 2061 6e79 2061 7070 656e  msg if any appen
-00019b70: 6420 6d73 6720 616c 7265 6164 7920 6578  d msg already ex
-00019b80: 6973 7473 0a20 2020 2020 2020 2022 2222  ists.        """
-00019b90: 0a20 2020 2064 6566 2067 6574 5f73 6b69  .    def get_ski
-00019ba0: 705f 6263 6173 745f 636f 6d6d 6974 2873  p_bcast_commit(s
-00019bb0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-00019bc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00019bd0: 2020 6073 6b69 705f 6263 6173 745f 636f    `skip_bcast_co
-00019be0: 6d6d 6974 603a 2044 6f6e 2774 2062 726f  mmit`: Don't bro
-00019bf0: 6164 6361 7374 2061 6e20 656d 7074 7920  adcast an empty 
-00019c00: 7261 6674 2065 6e74 7279 2074 6f20 6e6f  raft entry to no
-00019c10: 7469 6679 2066 6f6c 6c6f 7765 7220 746f  tify follower to
-00019c20: 2063 6f6d 6d69 7420 616e 2065 6e74 7279   commit an entry
-00019c30: 2e0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
-00019c40: 6179 206d 616b 6520 666f 6c6c 6f77 6572  ay make follower
-00019c50: 2077 6169 7420 6120 6c6f 6e67 6572 2074   wait a longer t
-00019c60: 696d 6520 746f 2061 7070 6c79 2061 6e20  ime to apply an 
-00019c70: 656e 7472 792e 2054 6869 7320 636f 6e66  entry. This conf
-00019c80: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
-00019c90: 2020 4d61 7920 6166 6665 6374 2070 726f    May affect pro
-00019ca0: 706f 7361 6c20 666f 7277 6172 6469 6e67  posal forwarding
-00019cb0: 2061 6e64 2066 6f6c 6c6f 7765 7220 7265   and follower re
-00019cc0: 6164 2e0a 2020 2020 2020 2020 2222 220a  ad..        """.
-00019cd0: 2020 2020 6465 6620 7365 745f 736b 6970      def set_skip
-00019ce0: 5f62 6361 7374 5f63 6f6d 6d69 7428 7365  _bcast_commit(se
-00019cf0: 6c66 2c20 736b 6970 5f62 6361 7374 5f63  lf, skip_bcast_c
-00019d00: 6f6d 6d69 743a 2062 6f6f 6c29 202d 3e20  ommit: bool) -> 
-00019d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00019d20: 220a 2020 2020 2020 2020 6073 6b69 705f  ".        `skip_
-00019d30: 6263 6173 745f 636f 6d6d 6974 603a 2044  bcast_commit`: D
-00019d40: 6f6e 2774 2062 726f 6164 6361 7374 2061  on't broadcast a
-00019d50: 6e20 656d 7074 7920 7261 6674 2065 6e74  n empty raft ent
-00019d60: 7279 2074 6f20 6e6f 7469 6679 2066 6f6c  ry to notify fol
-00019d70: 6c6f 7765 7220 746f 2063 6f6d 6d69 7420  lower to commit 
-00019d80: 616e 2065 6e74 7279 2e0a 2020 2020 2020  an entry..      
-00019d90: 2020 5468 6973 206d 6179 206d 616b 6520    This may make 
-00019da0: 666f 6c6c 6f77 6572 2077 6169 7420 6120  follower wait a 
-00019db0: 6c6f 6e67 6572 2074 696d 6520 746f 2061  longer time to a
-00019dc0: 7070 6c79 2061 6e20 656e 7472 792e 2054  pply an entry. T
-00019dd0: 6869 7320 636f 6e66 6967 7572 6174 696f  his configuratio
-00019de0: 6e0a 2020 2020 2020 2020 4d61 7920 6166  n.        May af
-00019df0: 6665 6374 2070 726f 706f 7361 6c20 666f  fect proposal fo
-00019e00: 7277 6172 6469 6e67 2061 6e64 2066 6f6c  rwarding and fol
-00019e10: 6c6f 7765 7220 7265 6164 2e0a 2020 2020  lower read..    
-00019e20: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00019e30: 6765 745f 7072 696f 7269 7479 2873 656c  get_priority(sel
-00019e40: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00019e50: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00019e60: 7072 696f 7269 7479 603a 2054 6865 2065  priority`: The e
-00019e70: 6c65 6374 696f 6e20 7072 696f 7269 7479  lection priority
-00019e80: 206f 6620 7468 6973 206e 6f64 652e 0a20   of this node.. 
-00019e90: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00019ea0: 6566 2073 6574 5f70 7269 6f72 6974 7928  ef set_priority(
-00019eb0: 7365 6c66 2c20 7072 696f 7269 7479 3a20  self, priority: 
-00019ec0: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00019ed0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00019ee0: 2020 6070 7269 6f72 6974 7960 3a20 5468    `priority`: Th
-00019ef0: 6520 656c 6563 7469 6f6e 2070 7269 6f72  e election prior
-00019f00: 6974 7920 6f66 2074 6869 7320 6e6f 6465  ity of this node
-00019f10: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00019f20: 2020 6465 6620 6765 745f 6d61 785f 756e    def get_max_un
-00019f30: 636f 6d6d 6974 7465 645f 7369 7a65 2873  committed_size(s
-00019f40: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-00019f50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00019f60: 2060 6d61 785f 756e 636f 6d6d 6974 7465   `max_uncommitte
-00019f70: 645f 7369 7a65 603a 2053 7065 6369 6679  d_size`: Specify
-00019f80: 206d 6178 696d 756d 206f 6620 756e 636f   maximum of unco
-00019f90: 6d6d 6974 7465 6420 656e 7472 7920 7369  mmitted entry si
-00019fa0: 7a65 2e0a 2020 2020 2020 2020 5768 656e  ze..        When
-00019fb0: 2074 6869 7320 6c69 6d69 7420 6973 2072   this limit is r
-00019fc0: 6561 6368 6564 2c20 616c 6c20 7072 6f70  eached, all prop
-00019fd0: 6f73 616c 7320 746f 2061 7070 656e 6420  osals to append 
-00019fe0: 6e65 7720 6c6f 6720 7769 6c6c 2062 6520  new log will be 
-00019ff0: 6472 6f70 7065 640a 2020 2020 2020 2020  dropped.        
-0001a000: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-0001a010: 6d61 785f 756e 636f 6d6d 6974 7465 645f  max_uncommitted_
-0001a020: 7369 7a65 2873 656c 662c 206d 6178 5f75  size(self, max_u
-0001a030: 6e63 6f6d 6d69 7474 6564 5f73 697a 653a  ncommitted_size:
-0001a040: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-0001a050: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001a060: 2020 2060 6d61 785f 756e 636f 6d6d 6974     `max_uncommit
-0001a070: 7465 645f 7369 7a65 603a 2053 7065 6369  ted_size`: Speci
-0001a080: 6679 206d 6178 696d 756d 206f 6620 756e  fy maximum of un
-0001a090: 636f 6d6d 6974 7465 6420 656e 7472 7920  committed entry 
-0001a0a0: 7369 7a65 2e0a 2020 2020 2020 2020 5768  size..        Wh
-0001a0b0: 656e 2074 6869 7320 6c69 6d69 7420 6973  en this limit is
-0001a0c0: 2072 6561 6368 6564 2c20 616c 6c20 7072   reached, all pr
-0001a0d0: 6f70 6f73 616c 7320 746f 2061 7070 656e  oposals to appen
-0001a0e0: 6420 6e65 7720 6c6f 6720 7769 6c6c 2062  d new log will b
-0001a0f0: 6520 6472 6f70 7065 640a 2020 2020 2020  e dropped.      
-0001a100: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-0001a110: 745f 6d61 785f 636f 6d6d 6974 7465 645f  t_max_committed_
-0001a120: 7369 7a65 5f70 6572 5f72 6561 6479 2873  size_per_ready(s
-0001a130: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-0001a140: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001a150: 2060 6d61 785f 636f 6d6d 6974 7465 645f   `max_committed_
-0001a160: 7369 7a65 5f70 6572 5f72 6561 6479 603a  size_per_ready`:
-0001a170: 204d 6178 2073 697a 6520 666f 7220 636f   Max size for co
-0001a180: 6d6d 6974 7465 6420 656e 7472 6965 7320  mmitted entries 
-0001a190: 696e 2061 2060 5265 6164 7960 2e0a 2020  in a `Ready`..  
-0001a1a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0001a1b0: 6620 7365 745f 6d61 785f 636f 6d6d 6974  f set_max_commit
-0001a1c0: 7465 645f 7369 7a65 5f70 6572 5f72 6561  ted_size_per_rea
-0001a1d0: 6479 280a 2020 2020 2020 2020 7365 6c66  dy(.        self
-0001a1e0: 2c20 6d61 785f 636f 6d6d 6974 7465 645f  , max_committed_
-0001a1f0: 7369 7a65 5f70 6572 5f72 6561 6479 3a20  size_per_ready: 
-0001a200: 696e 740a 2020 2020 2920 2d3e 204e 6f6e  int.    ) -> Non
-0001a210: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00011140: 6973 206e 6f64 6520 746f 2061 2070 7265  is node to a pre
+00011150: 2d63 616e 6469 6461 7465 0a0a 2020 2020  -candidate..    
+00011160: 2020 2020 2320 5061 6e69 6373 0a0a 2020      # Panics..  
+00011170: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
+00011180: 6120 6c65 6164 6572 2061 6c72 6561 6479  a leader already
+00011190: 2065 7869 7374 732e 0a20 2020 2020 2020   exists..       
+000111a0: 2022 2222 0a20 2020 2064 6566 2062 6563   """.    def bec
+000111b0: 6f6d 655f 6361 6e64 6964 6174 6528 7365  ome_candidate(se
+000111c0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+000111d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000111e0: 2043 6f6e 7665 7274 7320 7468 6973 206e   Converts this n
+000111f0: 6f64 6520 746f 2061 2063 616e 6469 6461  ode to a candida
+00011200: 7465 0a0a 2020 2020 2020 2020 2320 5061  te..        # Pa
+00011210: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
+00011220: 6e69 6373 2069 6620 6120 6c65 6164 6572  nics if a leader
+00011230: 2061 6c72 6561 6479 2065 7869 7374 732e   already exists.
+00011240: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011250: 2064 6566 2068 6561 7274 6265 6174 5f74   def heartbeat_t
+00011260: 696d 656f 7574 2873 656c 6629 202d 3e20  imeout(self) -> 
+00011270: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+00011280: 0a20 2020 2020 2020 2046 6574 6368 2074  .        Fetch t
+00011290: 6865 206c 656e 6774 6820 6f66 2074 6865  he length of the
+000112a0: 2068 6561 7274 6265 6174 2074 696d 656f   heartbeat timeo
+000112b0: 7574 0a20 2020 2020 2020 2022 2222 0a20  ut.        """. 
+000112c0: 2020 2064 6566 2068 6561 7274 6265 6174     def heartbeat
+000112d0: 5f65 6c61 7073 6564 2873 656c 6629 202d  _elapsed(self) -
+000112e0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+000112f0: 2222 0a20 2020 2020 2020 2046 6574 6368  "".        Fetch
+00011300: 2074 6865 206e 756d 6265 7220 6f66 2074   the number of t
+00011310: 6963 6b73 2065 6c61 7073 6564 2073 696e  icks elapsed sin
+00011320: 6365 206c 6173 7420 6865 6172 7462 6561  ce last heartbea
+00011330: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+00011340: 2020 2064 6566 2065 6c65 6374 696f 6e5f     def election_
+00011350: 7469 6d65 6f75 7428 7365 6c66 2920 2d3e  timeout(self) ->
+00011360: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00011370: 220a 2020 2020 2020 2020 4665 7463 6820  ".        Fetch 
+00011380: 7468 6520 6c65 6e67 7468 206f 6620 7468  the length of th
+00011390: 6520 656c 6563 7469 6f6e 2074 696d 656f  e election timeo
+000113a0: 7574 2e0a 2020 2020 2020 2020 2222 220a  ut..        """.
+000113b0: 2020 2020 6465 6620 7261 6e64 6f6d 697a      def randomiz
+000113c0: 6564 5f65 6c65 6374 696f 6e5f 7469 6d65  ed_election_time
+000113d0: 6f75 7428 7365 6c66 2920 2d3e 2069 6e74  out(self) -> int
+000113e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000113f0: 2020 2020 2020 5265 7475 726e 2074 6865        Return the
+00011400: 206c 656e 6774 6820 6f66 2074 6865 2063   length of the c
+00011410: 7572 7265 6e74 2072 616e 646f 6d69 7a65  urrent randomize
+00011420: 6420 656c 6563 7469 6f6e 2074 696d 656f  d election timeo
+00011430: 7574 2e0a 2020 2020 2020 2020 2222 220a  ut..        """.
+00011440: 2020 2020 6465 6620 7365 745f 7261 6e64      def set_rand
+00011450: 6f6d 697a 6564 5f65 6c65 6374 696f 6e5f  omized_election_
+00011460: 7469 6d65 6f75 7428 7365 6c66 2c20 7261  timeout(self, ra
+00011470: 6e64 6f6d 697a 6564 5f65 6c65 6374 696f  ndomized_electio
+00011480: 6e5f 7469 6d65 6f75 743a 2069 6e74 2920  n_timeout: int) 
+00011490: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000114a0: 2022 2222 0a20 2020 2020 2020 2046 6f72   """.        For
+000114b0: 2074 6573 7469 6e67 206c 6561 6465 7220   testing leader 
+000114c0: 6c65 6173 650a 2020 2020 2020 2020 2222  lease.        ""
+000114d0: 220a 2020 2020 6465 6620 7265 7365 745f  ".    def reset_
+000114e0: 7261 6e64 6f6d 697a 6564 5f65 6c65 6374  randomized_elect
+000114f0: 696f 6e5f 7469 6d65 6f75 7428 7365 6c66  ion_timeout(self
+00011500: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00011510: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00011520: 6567 656e 6572 6174 6573 2061 6e64 2073  egenerates and s
+00011530: 746f 7265 7320 7468 6520 656c 6563 7469  tores the electi
+00011540: 6f6e 2074 696d 656f 7574 2e0a 2020 2020  on timeout..    
+00011550: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00011560: 7061 7373 5f65 6c65 6374 696f 6e5f 7469  pass_election_ti
+00011570: 6d65 6f75 7428 7365 6c66 2920 2d3e 2062  meout(self) -> b
+00011580: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00011590: 0a20 2020 2020 2020 2060 7061 7373 5f65  .        `pass_e
+000115a0: 6c65 6374 696f 6e5f 7469 6d65 6f75 7460  lection_timeout`
+000115b0: 2072 6574 7572 6e73 2074 7275 6520 6966   returns true if
+000115c0: 2060 656c 6563 7469 6f6e 5f65 6c61 7073   `election_elaps
+000115d0: 6564 6020 6973 2067 7265 6174 6572 0a20  ed` is greater. 
+000115e0: 2020 2020 2020 2074 6861 6e20 6f72 2065         than or e
+000115f0: 7175 616c 2074 6f20 7468 6520 7261 6e64  qual to the rand
+00011600: 6f6d 697a 6564 2065 6c65 6374 696f 6e20  omized election 
+00011610: 7469 6d65 6f75 7420 696e 0a20 2020 2020  timeout in.     
+00011620: 2020 205b 6065 6c65 6374 696f 6e5f 7469     [`election_ti
+00011630: 6d65 6f75 7460 2c20 3220 2a20 6065 6c65  meout`, 2 * `ele
+00011640: 6374 696f 6e5f 7469 6d65 6f75 7460 202d  ction_timeout` -
+00011650: 2031 5d2e 0a20 2020 2020 2020 2022 2222   1]..        """
+00011660: 0a20 2020 2064 6566 2073 656e 645f 7469  .    def send_ti
+00011670: 6d65 6f75 745f 6e6f 7728 7365 6c66 2c20  meout_now(self, 
+00011680: 746f 3a20 696e 7429 202d 3e20 4e6f 6e65  to: int) -> None
+00011690: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000116a0: 2020 2020 2020 4973 7375 6573 2061 206d        Issues a m
+000116b0: 6573 7361 6765 2074 6f20 7469 6d65 6f75  essage to timeou
+000116c0: 7420 696d 6d65 6469 6174 656c 792e 0a20  t immediately.. 
+000116d0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+000116e0: 6566 2072 6561 6479 5f72 6561 645f 636f  ef ready_read_co
+000116f0: 756e 7428 7365 6c66 2920 2d3e 2069 6e74  unt(self) -> int
+00011700: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00011710: 2020 2020 2020 5265 7475 726e 7320 686f        Returns ho
+00011720: 7720 6d61 6e79 2072 6561 6420 7374 6174  w many read stat
+00011730: 6573 2065 7869 7374 2e0a 2020 2020 2020  es exist..      
+00011740: 2020 2222 220a 2020 2020 6465 6620 7065    """.    def pe
+00011750: 6e64 696e 675f 7265 6164 5f63 6f75 6e74  nding_read_count
+00011760: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00011770: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011780: 2020 2052 6574 7572 6e73 2074 6865 206e     Returns the n
+00011790: 756d 6265 7220 6f66 2070 656e 6469 6e67  umber of pending
+000117a0: 2072 6561 642d 6f6e 6c79 206d 6573 7361   read-only messa
+000117b0: 6765 732e 0a20 2020 2020 2020 2022 2222  ges..        """
+000117c0: 0a20 2020 2064 6566 206c 6f61 645f 7374  .    def load_st
+000117d0: 6174 6528 7365 6c66 2c20 6873 3a20 2248  ate(self, hs: "H
+000117e0: 6172 6453 7461 7465 2220 7c20 2248 6172  ardState" | "Har
+000117f0: 6453 7461 7465 5265 6622 2920 2d3e 204e  dStateRef") -> N
+00011800: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00011810: 0a20 2020 2020 2020 2046 6f72 2061 2067  .        For a g
+00011820: 6976 656e 2068 6172 6473 7461 7465 2c20  iven hardstate, 
+00011830: 6c6f 6164 2074 6865 2073 7461 7465 2069  load the state i
+00011840: 6e74 6f20 7365 6c66 2e0a 2020 2020 2020  nto self..      
+00011850: 2020 2222 220a 2020 2020 6465 6620 736f    """.    def so
+00011860: 6674 5f73 7461 7465 2873 656c 6629 202d  ft_state(self) -
+00011870: 3e20 2253 6f66 7453 7461 7465 223a 0a20  > "SoftState":. 
+00011880: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011890: 2020 2052 6574 7572 6e73 2061 2076 616c     Returns a val
+000118a0: 7565 2072 6570 7265 7365 6e74 696e 6720  ue representing 
+000118b0: 7468 6520 736f 6674 7374 6174 6520 6174  the softstate at
+000118c0: 2074 6865 2074 696d 6520 6f66 2063 616c   the time of cal
+000118d0: 6c69 6e67 2e0a 2020 2020 2020 2020 2222  ling..        ""
+000118e0: 220a 2020 2020 6465 6620 6861 7264 5f73  ".    def hard_s
+000118f0: 7461 7465 2873 656c 6629 202d 3e20 2248  tate(self) -> "H
+00011900: 6172 6453 7461 7465 223a 0a20 2020 2020  ardState":.     
+00011910: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00011920: 6574 7572 6e73 2061 2076 616c 7565 2072  eturns a value r
+00011930: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00011940: 6861 7264 7374 6174 6520 6174 2074 6865  hardstate at the
+00011950: 2074 696d 6520 6f66 2063 616c 6c69 6e67   time of calling
+00011960: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00011970: 2020 6465 6620 7069 6e67 2873 656c 6629    def ping(self)
+00011980: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00011990: 2020 2222 220a 2020 2020 2020 2020 4272    """.        Br
+000119a0: 6f61 6463 6173 7473 2068 6561 7274 6265  oadcasts heartbe
+000119b0: 6174 7320 746f 2061 6c6c 2074 6865 2066  ats to all the f
+000119c0: 6f6c 6c6f 7765 7273 2069 6620 6974 2773  ollowers if it's
+000119d0: 206c 6561 6465 722e 0a20 2020 2020 2020   leader..       
+000119e0: 2022 2222 0a20 2020 2064 6566 2074 6963   """.    def tic
+000119f0: 6b28 7365 6c66 2920 2d3e 2062 6f6f 6c3a  k(self) -> bool:
+00011a00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011a10: 2020 2020 2052 6574 7572 6e73 2074 7275       Returns tru
+00011a20: 6520 746f 2069 6e64 6963 6174 6520 7468  e to indicate th
+00011a30: 6174 2074 6865 7265 2077 696c 6c20 7072  at there will pr
+00011a40: 6f62 6162 6c79 2062 6520 736f 6d65 2072  obably be some r
+00011a50: 6561 6469 6e65 7373 206e 6565 6420 746f  eadiness need to
+00011a60: 2062 6520 6861 6e64 6c65 642e 0a20 2020   be handled..   
+00011a70: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00011a80: 2074 6963 6b5f 656c 6563 7469 6f6e 2873   tick_election(s
+00011a90: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+00011aa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011ab0: 2020 5275 6e20 6279 2066 6f6c 6c6f 7765    Run by followe
+00011ac0: 7273 2061 6e64 2063 616e 6469 6461 7465  rs and candidate
+00011ad0: 7320 6166 7465 7220 7365 6c66 2e65 6c65  s after self.ele
+00011ae0: 6374 696f 6e5f 7469 6d65 6f75 742e 0a0a  ction_timeout...
+00011af0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+00011b00: 7472 7565 2074 6f20 696e 6469 6361 7465  true to indicate
+00011b10: 2074 6861 7420 7468 6572 6520 7769 6c6c   that there will
+00011b20: 2070 726f 6261 626c 7920 6265 2073 6f6d   probably be som
+00011b30: 6520 7265 6164 696e 6573 7320 6e65 6564  e readiness need
+00011b40: 2074 6f20 6265 2068 616e 646c 6564 2e0a   to be handled..
+00011b50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011b60: 6465 6620 7374 6570 2873 656c 662c 206d  def step(self, m
+00011b70: 7367 3a20 224d 6573 7361 6765 2220 7c20  sg: "Message" | 
+00011b80: 224d 6573 7361 6765 5265 6622 2920 2d3e  "MessageRef") ->
+00011b90: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00011ba0: 2222 0a20 2020 2020 2020 2053 7465 7073  "".        Steps
+00011bb0: 2074 6865 2072 6166 7420 616c 6f6e 6720   the raft along 
+00011bc0: 7669 6120 6120 6d65 7373 6167 652e 2054  via a message. T
+00011bd0: 6869 7320 7368 6f75 6c64 2062 6520 6361  his should be ca
+00011be0: 6c6c 6564 2065 7665 7279 7469 6d65 2079  lled everytime y
+00011bf0: 6f75 7220 7261 6674 2072 6563 6569 7665  our raft receive
+00011c00: 7320 610a 2020 2020 2020 2020 6d65 7373  s a.        mess
+00011c10: 6167 6520 6672 6f6d 2061 2070 6565 722e  age from a peer.
+00011c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011c30: 2064 6566 2068 6173 5f70 656e 6469 6e67   def has_pending
+00011c40: 5f63 6f6e 6628 7365 6c66 2920 2d3e 2062  _conf(self) -> b
+00011c50: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00011c60: 0a20 2020 2020 2020 2043 6865 636b 2069  .        Check i
+00011c70: 6620 7468 6572 6520 6973 2061 6e79 2070  f there is any p
+00011c80: 656e 6469 6e67 2063 6f6e 6663 6861 6e67  ending confchang
+00011c90: 652e 0a0a 2020 2020 2020 2020 5468 6973  e...        This
+00011ca0: 206d 6574 686f 6420 6361 6e20 6265 2066   method can be f
+00011cb0: 616c 7365 2070 6f73 6974 6976 652e 0a20  alse positive.. 
+00011cc0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00011cd0: 6566 2070 726f 6d6f 7461 626c 6528 7365  ef promotable(se
+00011ce0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00011cf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011d00: 2049 6e64 6963 6174 6573 2077 6865 7468   Indicates wheth
+00011d10: 6572 2073 7461 7465 206d 6163 6869 6e65  er state machine
+00011d20: 2063 616e 2062 6520 7072 6f6d 6f74 6564   can be promoted
+00011d30: 2074 6f20 6c65 6164 6572 2c0a 2020 2020   to leader,.    
+00011d40: 2020 2020 7768 6963 6820 6973 2074 7275      which is tru
+00011d50: 6520 7768 656e 2069 7427 7320 6120 766f  e when it's a vo
+00011d60: 7465 7220 616e 6420 6974 7320 6f77 6e20  ter and its own 
+00011d70: 6964 2069 7320 696e 2070 726f 6772 6573  id is in progres
+00011d80: 7320 6c69 7374 2e0a 2020 2020 2020 2020  s list..        
+00011d90: 2222 220a 2020 2020 6465 6620 706f 7374  """.    def post
+00011da0: 5f63 6f6e 665f 6368 616e 6765 2873 656c  _conf_change(sel
+00011db0: 6629 202d 3e20 2243 6f6e 6653 7461 7465  f) -> "ConfState
+00011dc0: 5265 6622 3a0a 2020 2020 2020 2020 2222  Ref":.        ""
+00011dd0: 220a 2020 2020 2020 2020 5570 6461 7465  ".        Update
+00011de0: 7320 7468 6520 696e 2d6d 656d 6f72 7920  s the in-memory 
+00011df0: 7374 6174 6520 616e 642c 2077 6865 6e20  state and, when 
+00011e00: 6e65 6365 7373 6172 792c 2063 6172 7269  necessary, carri
+00011e10: 6573 206f 7574 2061 6464 6974 696f 6e61  es out additiona
+00011e20: 6c20 6163 7469 6f6e 730a 2020 2020 2020  l actions.      
+00011e30: 2020 7375 6368 2061 7320 7265 6163 7469    such as reacti
+00011e40: 6e67 2074 6f20 7468 6520 7265 6d6f 7661  ng to the remova
+00011e50: 6c20 6f66 206e 6f64 6573 206f 7220 6368  l of nodes or ch
+00011e60: 616e 6765 6420 7175 6f72 756d 2072 6571  anged quorum req
+00011e70: 7569 7265 6d65 6e74 732e 0a20 2020 2020  uirements..     
+00011e80: 2020 2022 2222 0a20 2020 2064 6566 2069     """.    def i
+00011e90: 6e5f 6c65 6173 6528 7365 6c66 2920 2d3e  n_lease(self) ->
+00011ea0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00011eb0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+00011ec0: 6e73 2077 6865 7468 6572 2074 6865 2063  ns whether the c
+00011ed0: 7572 7265 6e74 2072 6166 7420 6973 2069  urrent raft is i
+00011ee0: 6e20 6c65 6173 652e 0a20 2020 2020 2020  n lease..       
+00011ef0: 2022 2222 0a20 2020 2064 6566 2068 616e   """.    def han
+00011f00: 646c 655f 6865 6172 7462 6561 7428 7365  dle_heartbeat(se
+00011f10: 6c66 2c20 6d73 673a 2022 4d65 7373 6167  lf, msg: "Messag
+00011f20: 6522 207c 2022 4d65 7373 6167 6552 6566  e" | "MessageRef
+00011f30: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
+00011f40: 2020 2020 2222 2246 6f72 2061 206d 6573      """For a mes
+00011f50: 7361 6765 2c20 636f 6d6d 6974 2061 6e64  sage, commit and
+00011f60: 2073 656e 6420 6f75 7420 6865 6172 7462   send out heartb
+00011f70: 6561 742e 2222 220a 2020 2020 6465 6620  eat.""".    def 
+00011f80: 6861 6e64 6c65 5f61 7070 656e 645f 656e  handle_append_en
+00011f90: 7472 6965 7328 7365 6c66 2c20 6d73 673a  tries(self, msg:
+00011fa0: 2022 4d65 7373 6167 6522 207c 2022 4d65   "Message" | "Me
+00011fb0: 7373 6167 6552 6566 2229 202d 3e20 4e6f  ssageRef") -> No
+00011fc0: 6e65 3a0a 2020 2020 2020 2020 2222 2246  ne:.        """F
+00011fd0: 6f72 2061 2067 6976 656e 206d 6573 7361  or a given messa
+00011fe0: 6765 2c20 6170 7065 6e64 2074 6865 2065  ge, append the e
+00011ff0: 6e74 7269 6573 2074 6f20 7468 6520 6c6f  ntries to the lo
+00012000: 672e 2222 220a 2020 2020 6465 6620 7265  g.""".    def re
+00012010: 7175 6573 745f 736e 6170 7368 6f74 2873  quest_snapshot(s
+00012020: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00012030: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012040: 2020 5265 7175 6573 7420 6120 736e 6170    Request a snap
+00012050: 7368 6f74 2066 726f 6d20 6120 6c65 6164  shot from a lead
+00012060: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
+00012070: 2020 2020 6465 6620 7072 7328 7365 6c66      def prs(self
+00012080: 2920 2d3e 2022 5072 6f67 7265 7373 5472  ) -> "ProgressTr
+00012090: 6163 6b65 7252 6566 223a 0a20 2020 2020  ackerRef":.     
+000120a0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+000120b0: 6574 7572 6e73 2061 2072 6561 642d 6f6e  eturns a read-on
+000120c0: 6c79 2072 6566 6572 656e 6365 2074 6f20  ly reference to 
+000120d0: 7468 6520 7072 6f67 7265 7373 2073 6574  the progress set
+000120e0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000120f0: 2020 6465 6620 7265 7365 7428 7365 6c66    def reset(self
+00012100: 2c20 7465 726d 3a20 696e 7429 202d 3e20  , term: int) -> 
+00012110: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00012120: 220a 2020 2020 2020 2020 5265 7365 7473  ".        Resets
+00012130: 2074 6865 2063 7572 7265 6e74 206e 6f64   the current nod
+00012140: 6520 746f 2061 2067 6976 656e 2074 6572  e to a given ter
+00012150: 6d2e 0a20 2020 2020 2020 2022 2222 0a20  m..        """. 
+00012160: 2020 2064 6566 2072 6573 746f 7265 2873     def restore(s
+00012170: 656c 662c 2073 6e61 7073 686f 743a 2022  elf, snapshot: "
+00012180: 536e 6170 7368 6f74 2220 7c20 2253 6e61  Snapshot" | "Sna
+00012190: 7073 686f 7452 6566 2229 202d 3e20 626f  pshotRef") -> bo
+000121a0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+000121b0: 2020 2020 2020 2020 5265 636f 7665 7273          Recovers
+000121c0: 2074 6865 2073 7461 7465 206d 6163 6869   the state machi
+000121d0: 6e65 2066 726f 6d20 6120 736e 6170 7368  ne from a snapsh
+000121e0: 6f74 2e20 4974 2072 6573 746f 7265 7320  ot. It restores 
+000121f0: 7468 6520 6c6f 6720 616e 6420 7468 650a  the log and the.
+00012200: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+00012210: 6174 696f 6e20 6f66 2073 7461 7465 206d  ation of state m
+00012220: 6163 6869 6e65 2e0a 2020 2020 2020 2020  achine..        
+00012230: 2222 220a 2020 2020 6465 6620 736e 6170  """.    def snap
+00012240: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00012250: 616c 5b22 536e 6170 7368 6f74 5265 6622  al["SnapshotRef"
+00012260: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+00012270: 2020 2020 2020 2047 7261 6273 2061 2072         Grabs a r
+00012280: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
+00012290: 736e 6170 7368 6f74 0a20 2020 2020 2020  snapshot.       
+000122a0: 2022 2222 0a20 2020 2064 6566 2073 746f   """.    def sto
+000122b0: 7265 2873 656c 6629 202d 3e20 224d 656d  re(self) -> "Mem
+000122c0: 5374 6f72 6167 6552 6566 223a 0a20 2020  StorageRef":.   
+000122d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000122e0: 2047 7261 6273 2061 6e20 696d 6d75 7461   Grabs an immuta
+000122f0: 626c 6520 7265 6665 7265 6e63 6520 746f  ble reference to
+00012300: 2074 6865 2073 746f 7265 2e0a 2020 2020   the store..    
+00012310: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00012320: 6f6e 5f70 6572 7369 7374 5f73 6e61 7028  on_persist_snap(
+00012330: 7365 6c66 2c20 696e 6465 783a 2069 6e74  self, index: int
+00012340: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012350: 2020 2022 2222 0a20 2020 2020 2020 204e     """.        N
+00012360: 6f74 6966 6965 7320 7468 6174 2074 6865  otifies that the
+00012370: 2073 6e61 7073 686f 7420 6861 7665 2062   snapshot have b
+00012380: 6565 6e20 7065 7273 6973 7465 642e 0a20  een persisted.. 
+00012390: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+000123a0: 6566 2061 626f 7274 5f6c 6561 6465 725f  ef abort_leader_
+000123b0: 7472 616e 7366 6572 2873 656c 6629 202d  transfer(self) -
+000123c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000123d0: 2222 220a 2020 2020 2020 2020 5374 6f70  """.        Stop
+000123e0: 7320 7468 6520 7472 616e 7366 6572 206f  s the transfer o
+000123f0: 6620 6120 6c65 6164 6572 2e0a 2020 2020  f a leader..    
+00012400: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00012410: 6361 6d70 6169 676e 2873 656c 662c 2074  campaign(self, t
+00012420: 7970 3a20 7374 7229 202d 3e20 4e6f 6e65  yp: str) -> None
+00012430: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012440: 2020 2020 2020 4361 6d70 6169 676e 2074        Campaign t
+00012450: 6f20 6174 7465 6d70 7420 746f 2062 6563  o attempt to bec
+00012460: 6f6d 6520 6120 6c65 6164 6572 2e0a 0a20  ome a leader... 
+00012470: 2020 2020 2020 2049 6620 7072 6576 6f74         If prevot
+00012480: 6520 6973 2065 6e61 626c 6564 2c20 7468  e is enabled, th
+00012490: 6973 2069 7320 6861 6e64 6c65 6420 6173  is is handled as
+000124a0: 2077 656c 6c2e 0a20 2020 2020 2020 2022   well..        "
+000124b0: 2222 0a20 2020 2064 6566 2067 6574 5f6c  "".    def get_l
+000124c0: 6561 645f 7472 616e 7366 6572 6565 2873  ead_transferee(s
+000124d0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+000124e0: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
+000124f0: 2222 0a20 2020 2020 2020 2060 6c65 6164  "".        `lead
+00012500: 5f74 7261 6e73 6665 7265 6560 3a20 4944  _transferee`: ID
+00012510: 206f 6620 7468 6520 6c65 6164 6572 2074   of the leader t
+00012520: 7261 6e73 6665 7220 7461 7267 6574 2077  ransfer target w
+00012530: 6865 6e20 6974 7320 7661 6c75 6520 6973  hen its value is
+00012540: 206e 6f74 204e 6f6e 652e 0a0a 2020 2020   not None...    
+00012550: 2020 2020 4966 2074 6869 7320 6973 2053      If this is S
+00012560: 6f6d 6528 6964 292c 2077 6520 666f 6c6c  ome(id), we foll
+00012570: 6f77 2074 6865 2070 726f 6365 6475 7265  ow the procedure
+00012580: 2064 6566 696e 6564 2069 6e20 7261 6674   defined in raft
+00012590: 2074 6865 7369 7320 332e 3130 2e0a 2020   thesis 3.10..  
+000125a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+000125b0: 6620 7365 745f 6c65 6164 5f74 7261 6e73  f set_lead_trans
+000125c0: 6665 7265 6528 7365 6c66 2c20 6c65 6164  feree(self, lead
+000125d0: 5f74 7261 6e73 6665 7265 653a 2069 6e74  _transferee: int
+000125e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000125f0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00012600: 6c65 6164 5f74 7261 6e73 6665 7265 6560  lead_transferee`
+00012610: 3a20 4944 206f 6620 7468 6520 6c65 6164  : ID of the lead
+00012620: 6572 2074 7261 6e73 6665 7220 7461 7267  er transfer targ
+00012630: 6574 2077 6865 6e20 6974 7320 7661 6c75  et when its valu
+00012640: 6520 6973 206e 6f74 204e 6f6e 652e 0a0a  e is not None...
+00012650: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
+00012660: 6973 2053 6f6d 6528 6964 292c 2077 6520  is Some(id), we 
+00012670: 666f 6c6c 6f77 2074 6865 2070 726f 6365  follow the proce
+00012680: 6475 7265 2064 6566 696e 6564 2069 6e20  dure defined in 
+00012690: 7261 6674 2074 6865 7369 7320 332e 3130  raft thesis 3.10
+000126a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000126b0: 2020 6465 6620 6765 745f 7465 726d 2873    def get_term(s
+000126c0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000126d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000126e0: 2060 7465 726d 603a 2054 6865 2063 7572   `term`: The cur
+000126f0: 7265 6e74 2065 6c65 6374 696f 6e20 7465  rent election te
+00012700: 726d 2e0a 2020 2020 2020 2020 2222 220a  rm..        """.
+00012710: 2020 2020 6465 6620 7365 745f 7465 726d      def set_term
+00012720: 2873 656c 662c 2074 6572 6d3a 2069 6e74  (self, term: int
+00012730: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00012740: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00012750: 7465 726d 603a 2054 6865 2063 7572 7265  term`: The curre
+00012760: 6e74 2065 6c65 6374 696f 6e20 7465 726d  nt election term
+00012770: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00012780: 2020 6465 6620 6765 745f 766f 7465 2873    def get_vote(s
+00012790: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000127a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000127b0: 2060 766f 7465 603a 2057 6869 6368 2070   `vote`: Which p
+000127c0: 6565 7220 7468 6973 2072 6166 7420 6973  eer this raft is
+000127d0: 2076 6f74 696e 6720 666f 722e 0a20 2020   voting for..   
+000127e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+000127f0: 2073 6574 5f76 6f74 6528 7365 6c66 2c20   set_vote(self, 
+00012800: 766f 7465 3a20 696e 7429 202d 3e20 4e6f  vote: int) -> No
+00012810: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00012820: 2020 2020 2020 2020 6076 6f74 6560 3a20          `vote`: 
+00012830: 5768 6963 6820 7065 6572 2074 6869 7320  Which peer this 
+00012840: 7261 6674 2069 7320 766f 7469 6e67 2066  raft is voting f
+00012850: 6f72 2e0a 2020 2020 2020 2020 2222 220a  or..        """.
+00012860: 2020 2020 6465 6620 6765 745f 7072 696f      def get_prio
+00012870: 7269 7479 2873 656c 6629 202d 3e20 696e  rity(self) -> in
+00012880: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+00012890: 2020 2020 2020 2060 7072 696f 7269 7479         `priority
+000128a0: 603a 2054 6865 2065 6c65 6374 696f 6e20  `: The election 
+000128b0: 7072 696f 7269 7479 206f 6620 7468 6973  priority of this
+000128c0: 206e 6f64 652e 0a20 2020 2020 2020 2022   node..        "
+000128d0: 2222 0a20 2020 2064 6566 2073 6574 5f70  "".    def set_p
+000128e0: 7269 6f72 6974 7928 7365 6c66 2c20 7072  riority(self, pr
+000128f0: 696f 7269 7479 3a20 696e 7429 202d 3e20  iority: int) -> 
+00012900: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00012910: 220a 2020 2020 2020 2020 6070 7269 6f72  ".        `prior
+00012920: 6974 7960 3a20 5468 6520 656c 6563 7469  ity`: The electi
+00012930: 6f6e 2070 7269 6f72 6974 7920 6f66 2074  on priority of t
+00012940: 6869 7320 6e6f 6465 2e0a 2020 2020 2020  his node..      
+00012950: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
+00012960: 745f 6c65 6164 6572 5f69 6428 7365 6c66  t_leader_id(self
+00012970: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+00012980: 2020 2222 220a 2020 2020 2020 2020 606c    """.        `l
+00012990: 6561 6465 725f 6964 603a 2054 6865 206c  eader_id`: The l
+000129a0: 6561 6465 7220 6964 0a20 2020 2020 2020  eader id.       
+000129b0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+000129c0: 5f6c 6561 6465 725f 6964 2873 656c 662c  _leader_id(self,
+000129d0: 206c 6561 6465 725f 6964 3a20 696e 7429   leader_id: int)
+000129e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000129f0: 2020 2222 220a 2020 2020 2020 2020 606c    """.        `l
+00012a00: 6561 6465 725f 6964 603a 2054 6865 206c  eader_id`: The l
+00012a10: 6561 6465 7220 6964 0a20 2020 2020 2020  eader id.       
+00012a20: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00012a30: 5f6d 6178 5f6d 7367 5f73 697a 6528 7365  _max_msg_size(se
+00012a40: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00012a50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012a60: 606d 6178 5f6d 7367 5f73 697a 6560 3a20  `max_msg_size`: 
+00012a70: 5468 6520 6d61 7869 6d75 6d20 6c65 6e67  The maximum leng
+00012a80: 7468 2028 696e 2062 7974 6573 2920 6f66  th (in bytes) of
+00012a90: 2061 6c6c 2074 6865 2065 6e74 7269 6573   all the entries
+00012aa0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00012ab0: 2020 6465 6620 7365 745f 6d61 785f 6d73    def set_max_ms
+00012ac0: 675f 7369 7a65 2873 656c 662c 206d 6178  g_size(self, max
+00012ad0: 5f6d 7367 5f73 697a 653a 2069 6e74 2920  _msg_size: int) 
+00012ae0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00012af0: 2022 2222 0a20 2020 2020 2020 2060 6d61   """.        `ma
+00012b00: 785f 6d73 675f 7369 7a65 603a 2054 6865  x_msg_size`: The
+00012b10: 206d 6178 696d 756d 206c 656e 6774 6820   maximum length 
+00012b20: 2869 6e20 6279 7465 7329 206f 6620 616c  (in bytes) of al
+00012b30: 6c20 7468 6520 656e 7472 6965 732e 0a20  l the entries.. 
+00012b40: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00012b50: 6566 2067 6574 5f70 656e 6469 6e67 5f63  ef get_pending_c
+00012b60: 6f6e 665f 696e 6465 7828 7365 6c66 2920  onf_index(self) 
+00012b70: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00012b80: 2222 220a 2020 2020 2020 2020 6070 656e  """.        `pen
+00012b90: 6469 6e67 5f63 6f6e 665f 696e 6465 7860  ding_conf_index`
+00012ba0: 3a20 4f6e 6c79 206f 6e65 2063 6f6e 6620  : Only one conf 
+00012bb0: 6368 616e 6765 206d 6179 2062 6520 7065  change may be pe
+00012bc0: 6e64 696e 6720 2869 6e20 7468 6520 6c6f  nding (in the lo
+00012bd0: 672c 2062 7574 206e 6f74 2079 6574 0a20  g, but not yet. 
+00012be0: 2020 2020 2020 2061 7070 6c69 6564 2920         applied) 
+00012bf0: 6174 2061 2074 696d 652e 2054 6869 7320  at a time. This 
+00012c00: 6973 2065 6e66 6f72 6365 6420 7669 6120  is enforced via 
+00012c10: 6070 656e 6469 6e67 5f63 6f6e 665f 696e  `pending_conf_in
+00012c20: 6465 7860 2c20 7768 6963 680a 2020 2020  dex`, which.    
+00012c30: 2020 2020 6973 2073 6574 2074 6f20 6120      is set to a 
+00012c40: 7661 6c75 6520 3e3d 2074 6865 206c 6f67  value >= the log
+00012c50: 2069 6e64 6578 206f 6620 7468 6520 6c61   index of the la
+00012c60: 7465 7374 2070 656e 6469 6e67 0a20 2020  test pending.   
+00012c70: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+00012c80: 6f6e 2063 6861 6e67 6520 2869 6620 616e  on change (if an
+00012c90: 7929 2e20 436f 6e66 6967 2063 6861 6e67  y). Config chang
+00012ca0: 6573 2061 7265 206f 6e6c 7920 616c 6c6f  es are only allo
+00012cb0: 7765 6420 746f 0a20 2020 2020 2020 2062  wed to.        b
+00012cc0: 6520 7072 6f70 6f73 6564 2069 6620 7468  e proposed if th
+00012cd0: 6520 6c65 6164 6572 2773 2061 7070 6c69  e leader's appli
+00012ce0: 6564 2069 6e64 6578 2069 7320 6772 6561  ed index is grea
+00012cf0: 7465 7220 7468 616e 2074 6869 730a 2020  ter than this.  
+00012d00: 2020 2020 2020 7661 6c75 652e 0a0a 2020        value...  
+00012d10: 2020 2020 2020 5468 6973 2076 616c 7565        This value
+00012d20: 2069 7320 636f 6e73 6572 7661 7469 7665   is conservative
+00012d30: 6c79 2073 6574 2069 6e20 6361 7365 7320  ly set in cases 
+00012d40: 7768 6572 6520 7468 6572 6520 6d61 7920  where there may 
+00012d50: 6265 2061 2063 6f6e 6669 6775 7261 7469  be a configurati
+00012d60: 6f6e 2063 6861 6e67 6520 7065 6e64 696e  on change pendin
+00012d70: 672c 0a20 2020 2020 2020 2062 7574 2073  g,.        but s
+00012d80: 6361 6e6e 696e 6720 7468 6520 6c6f 6720  canning the log 
+00012d90: 6973 2070 6f73 7369 626c 7920 6578 7065  is possibly expe
+00012da0: 6e73 6976 652e 2054 6869 7320 696d 706c  nsive. This impl
+00012db0: 6965 7320 7468 6174 2074 6865 2069 6e64  ies that the ind
+00012dc0: 6578 2073 7461 7465 6420 6865 7265 206d  ex stated here m
+00012dd0: 6179 206e 6f74 0a20 2020 2020 2020 206e  ay not.        n
+00012de0: 6563 6573 7361 7269 6c79 2062 6520 6120  ecessarily be a 
+00012df0: 636f 6e66 6967 2063 6861 6e67 6520 656e  config change en
+00012e00: 7472 792c 2061 6e64 2069 7420 6d61 7920  try, and it may 
+00012e10: 6e6f 7420 6265 2061 2060 4265 6769 6e4d  not be a `BeginM
+00012e20: 656d 6265 7273 6869 7043 6861 6e67 6560  embershipChange`
+00012e30: 2065 6e74 7279 2c20 6576 656e 2069 660a   entry, even if.
+00012e40: 2020 2020 2020 2020 7765 2073 6574 2074          we set t
+00012e50: 6869 7320 746f 206f 6e65 2e0a 2020 2020  his to one..    
+00012e60: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00012e70: 7365 745f 7065 6e64 696e 675f 636f 6e66  set_pending_conf
+00012e80: 5f69 6e64 6578 2873 656c 662c 2070 656e  _index(self, pen
+00012e90: 6469 6e67 5f63 6f6e 665f 696e 6465 783a  ding_conf_index:
+00012ea0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00012eb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012ec0: 2020 2060 7065 6e64 696e 675f 636f 6e66     `pending_conf
+00012ed0: 5f69 6e64 6578 603a 204f 6e6c 7920 6f6e  _index`: Only on
+00012ee0: 6520 636f 6e66 2063 6861 6e67 6520 6d61  e conf change ma
+00012ef0: 7920 6265 2070 656e 6469 6e67 2028 696e  y be pending (in
+00012f00: 2074 6865 206c 6f67 2c20 6275 7420 6e6f   the log, but no
+00012f10: 7420 7965 740a 2020 2020 2020 2020 6170  t yet.        ap
+00012f20: 706c 6965 6429 2061 7420 6120 7469 6d65  plied) at a time
+00012f30: 2e20 5468 6973 2069 7320 656e 666f 7263  . This is enforc
+00012f40: 6564 2076 6961 2060 7065 6e64 696e 675f  ed via `pending_
+00012f50: 636f 6e66 5f69 6e64 6578 602c 2077 6869  conf_index`, whi
+00012f60: 6368 0a20 2020 2020 2020 2069 7320 7365  ch.        is se
+00012f70: 7420 746f 2061 2076 616c 7565 203e 3d20  t to a value >= 
+00012f80: 7468 6520 6c6f 6720 696e 6465 7820 6f66  the log index of
+00012f90: 2074 6865 206c 6174 6573 7420 7065 6e64   the latest pend
+00012fa0: 696e 670a 2020 2020 2020 2020 636f 6e66  ing.        conf
+00012fb0: 6967 7572 6174 696f 6e20 6368 616e 6765  iguration change
+00012fc0: 2028 6966 2061 6e79 292e 2043 6f6e 6669   (if any). Confi
+00012fd0: 6720 6368 616e 6765 7320 6172 6520 6f6e  g changes are on
+00012fe0: 6c79 2061 6c6c 6f77 6564 2074 6f0a 2020  ly allowed to.  
+00012ff0: 2020 2020 2020 6265 2070 726f 706f 7365        be propose
+00013000: 6420 6966 2074 6865 206c 6561 6465 7227  d if the leader'
+00013010: 7320 6170 706c 6965 6420 696e 6465 7820  s applied index 
+00013020: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
+00013030: 7468 6973 0a20 2020 2020 2020 2076 616c  this.        val
+00013040: 7565 2e0a 0a20 2020 2020 2020 2054 6869  ue...        Thi
+00013050: 7320 7661 6c75 6520 6973 2063 6f6e 7365  s value is conse
+00013060: 7276 6174 6976 656c 7920 7365 7420 696e  rvatively set in
+00013070: 2063 6173 6573 2077 6865 7265 2074 6865   cases where the
+00013080: 7265 206d 6179 2062 6520 6120 636f 6e66  re may be a conf
+00013090: 6967 7572 6174 696f 6e20 6368 616e 6765  iguration change
+000130a0: 2070 656e 6469 6e67 2c0a 2020 2020 2020   pending,.      
+000130b0: 2020 6275 7420 7363 616e 6e69 6e67 2074    but scanning t
+000130c0: 6865 206c 6f67 2069 7320 706f 7373 6962  he log is possib
+000130d0: 6c79 2065 7870 656e 7369 7665 2e20 5468  ly expensive. Th
+000130e0: 6973 2069 6d70 6c69 6573 2074 6861 7420  is implies that 
+000130f0: 7468 6520 696e 6465 7820 7374 6174 6564  the index stated
+00013100: 2068 6572 6520 6d61 7920 6e6f 740a 2020   here may not.  
+00013110: 2020 2020 2020 6e65 6365 7373 6172 696c        necessaril
+00013120: 7920 6265 2061 2063 6f6e 6669 6720 6368  y be a config ch
+00013130: 616e 6765 2065 6e74 7279 2c20 616e 6420  ange entry, and 
+00013140: 6974 206d 6179 206e 6f74 2062 6520 6120  it may not be a 
+00013150: 6042 6567 696e 4d65 6d62 6572 7368 6970  `BeginMembership
+00013160: 4368 616e 6765 6020 656e 7472 792c 2065  Change` entry, e
+00013170: 7665 6e20 6966 0a20 2020 2020 2020 2077  ven if.        w
+00013180: 6520 7365 7420 7468 6973 2074 6f20 6f6e  e set this to on
+00013190: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+000131a0: 2020 2064 6566 2067 6574 5f70 656e 6469     def get_pendi
+000131b0: 6e67 5f72 6571 7565 7374 5f73 6e61 7073  ng_request_snaps
+000131c0: 686f 7428 7365 6c66 2920 2d3e 2069 6e74  hot(self) -> int
+000131d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000131e0: 2020 2020 2020 6070 656e 6469 6e67 5f72        `pending_r
+000131f0: 6571 7565 7374 5f73 6e61 7073 686f 7460  equest_snapshot`
+00013200: 3a20 5468 6520 7065 6572 2069 7320 7265  : The peer is re
+00013210: 7175 6573 7469 6e67 2073 6e61 7073 686f  questing snapsho
+00013220: 742c 2069 7420 6973 2074 6865 2069 6e64  t, it is the ind
+00013230: 6578 2074 6861 7420 7468 6520 666f 6c6c  ex that the foll
+00013240: 6f77 6572 0a20 2020 2020 2020 206e 6565  ower.        nee
+00013250: 6473 2069 7420 746f 2062 6520 696e 636c  ds it to be incl
+00013260: 7564 6564 2069 6e20 6120 736e 6170 7368  uded in a snapsh
+00013270: 6f74 2e0a 2020 2020 2020 2020 2222 220a  ot..        """.
+00013280: 2020 2020 6465 6620 7365 745f 7065 6e64      def set_pend
+00013290: 696e 675f 7265 7175 6573 745f 736e 6170  ing_request_snap
+000132a0: 7368 6f74 2873 656c 662c 2070 656e 6469  shot(self, pendi
+000132b0: 6e67 5f72 6571 7565 7374 5f73 6e61 7073  ng_request_snaps
+000132c0: 686f 743a 2069 6e74 2920 2d3e 204e 6f6e  hot: int) -> Non
+000132d0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000132e0: 2020 2020 2020 2060 7065 6e64 696e 675f         `pending_
+000132f0: 7265 7175 6573 745f 736e 6170 7368 6f74  request_snapshot
+00013300: 603a 2054 6865 2070 6565 7220 6973 2072  `: The peer is r
+00013310: 6571 7565 7374 696e 6720 736e 6170 7368  equesting snapsh
+00013320: 6f74 2c20 6974 2069 7320 7468 6520 696e  ot, it is the in
+00013330: 6465 7820 7468 6174 2074 6865 2066 6f6c  dex that the fol
+00013340: 6c6f 7765 720a 2020 2020 2020 2020 6e65  lower.        ne
+00013350: 6564 7320 6974 2074 6f20 6265 2069 6e63  eds it to be inc
+00013360: 6c75 6465 6420 696e 2061 2073 6e61 7073  luded in a snaps
+00013370: 686f 742e 0a20 2020 2020 2020 2022 2222  hot..        """
+00013380: 0a20 2020 2064 6566 2067 6574 5f69 6428  .    def get_id(
+00013390: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+000133a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000133b0: 2020 6069 6460 3a20 5468 6520 4944 206f    `id`: The ID o
+000133c0: 6620 7468 6973 206e 6f64 652e 0a20 2020  f this node..   
+000133d0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+000133e0: 2073 6574 5f69 6428 7365 6c66 2c20 6964   set_id(self, id
+000133f0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00013400: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013410: 2020 2020 6069 6460 3a20 5468 6520 4944      `id`: The ID
+00013420: 206f 6620 7468 6973 206e 6f64 652e 0a20   of this node.. 
+00013430: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00013440: 6566 2067 6574 5f6d 7367 7328 7365 6c66  ef get_msgs(self
+00013450: 2920 2d3e 204c 6973 745b 224d 6573 7361  ) -> List["Messa
+00013460: 6765 5265 6622 5d3a 0a20 2020 2020 2020  geRef"]:.       
+00013470: 2022 2222 0a20 2020 2020 2020 2060 6d73   """.        `ms
+00013480: 6773 603a 2054 6865 206c 6973 7420 6f66  gs`: The list of
+00013490: 206d 6573 7361 6765 732e 0a20 2020 2020   messages..     
+000134a0: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
+000134b0: 6574 5f6d 7367 7328 7365 6c66 2c20 6d73  et_msgs(self, ms
+000134c0: 6773 3a20 4c69 7374 5b22 4d65 7373 6167  gs: List["Messag
+000134d0: 6522 207c 2022 4d65 7373 6167 6552 6566  e" | "MessageRef
+000134e0: 225d 2920 2d3e 204e 6f6e 653a 0a20 2020  "]) -> None:.   
+000134f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013500: 2060 6d73 6773 603a 2054 6865 206c 6973   `msgs`: The lis
+00013510: 7420 6f66 206d 6573 7361 6765 732e 0a20  t of messages.. 
+00013520: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00013530: 6566 2074 616b 655f 6d73 6773 2873 656c  ef take_msgs(sel
+00013540: 6629 202d 3e20 4c69 7374 5b22 4d65 7373  f) -> List["Mess
+00013550: 6167 6522 5d3a 0a20 2020 2020 2020 2022  age"]:.        "
+00013560: 2222 0a20 2020 2020 2020 2060 6d73 6773  "".        `msgs
+00013570: 603a 2054 6865 206c 6973 7420 6f66 206d  `: The list of m
+00013580: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
+00013590: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+000135a0: 5f6d 6178 5f69 6e66 6c69 6768 7428 7365  _max_inflight(se
+000135b0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+000135c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000135d0: 606d 6178 5f69 6e66 6c69 6768 7460 3a20  `max_inflight`: 
+000135e0: 5468 6520 6d61 7869 6d75 6d20 6e75 6d62  The maximum numb
+000135f0: 6572 206f 6620 6d65 7373 6167 6573 2074  er of messages t
+00013600: 6861 7420 6361 6e20 6265 2069 6e66 6c69  hat can be infli
+00013610: 6768 742e 0a20 2020 2020 2020 2022 2222  ght..        """
+00013620: 0a20 2020 2064 6566 2073 6574 5f6d 6178  .    def set_max
+00013630: 5f69 6e66 6c69 6768 7428 7365 6c66 2c20  _inflight(self, 
+00013640: 6d61 785f 696e 666c 6967 6874 3a20 696e  max_inflight: in
+00013650: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+00013660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013670: 606d 6178 5f69 6e66 6c69 6768 7460 3a20  `max_inflight`: 
+00013680: 5468 6520 6d61 7869 6d75 6d20 6e75 6d62  The maximum numb
+00013690: 6572 206f 6620 6d65 7373 6167 6573 2074  er of messages t
+000136a0: 6861 7420 6361 6e20 6265 2069 6e66 6c69  hat can be infli
+000136b0: 6768 742e 0a20 2020 2020 2020 2022 2222  ght..        """
+000136c0: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
+000136d0: 7465 2873 656c 6629 202d 3e20 2253 7461  te(self) -> "Sta
+000136e0: 7465 526f 6c65 223a 0a20 2020 2020 2020  teRole":.       
+000136f0: 2022 2222 0a20 2020 2020 2020 2060 7374   """.        `st
+00013700: 6174 6560 3a20 5468 6520 6375 7272 656e  ate`: The curren
+00013710: 7420 726f 6c65 206f 6620 7468 6973 206e  t role of this n
+00013720: 6f64 652e 0a20 2020 2020 2020 2022 2222  ode..        """
+00013730: 0a20 2020 2064 6566 2073 6574 5f73 7461  .    def set_sta
+00013740: 7465 2873 656c 662c 2073 7461 7465 5f72  te(self, state_r
+00013750: 6f6c 653a 2022 5374 6174 6552 6f6c 6522  ole: "StateRole"
+00013760: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00013770: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00013780: 7374 6174 6560 3a20 5468 6520 6375 7272  state`: The curr
+00013790: 656e 7420 726f 6c65 206f 6620 7468 6973  ent role of this
+000137a0: 206e 6f64 652e 0a20 2020 2020 2020 2022   node..        "
+000137b0: 2222 0a20 2020 2064 6566 2067 6574 5f65  "".    def get_e
+000137c0: 6c65 6374 696f 6e5f 656c 6170 7365 6428  lection_elapsed(
+000137d0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+000137e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000137f0: 2020 6065 6c65 6374 696f 6e5f 656c 6170    `election_elap
+00013800: 7365 6460 3a20 5469 636b 7320 7369 6e63  sed`: Ticks sinc
+00013810: 6520 6974 2072 6561 6368 6564 206c 6173  e it reached las
+00013820: 7420 656c 6563 7469 6f6e 5469 6d65 6f75  t electionTimeou
+00013830: 7420 7768 656e 2069 7420 6973 206c 6561  t when it is lea
+00013840: 6465 7220 6f72 2063 616e 6469 6461 7465  der or candidate
+00013850: 2e0a 2020 2020 2020 2020 4e75 6d62 6572  ..        Number
+00013860: 206f 6620 7469 636b 7320 7369 6e63 6520   of ticks since 
+00013870: 6974 2072 6561 6368 6564 206c 6173 7420  it reached last 
+00013880: 656c 6563 7469 6f6e 5469 6d65 6f75 7420  electionTimeout 
+00013890: 6f72 2072 6563 6569 7665 6420 610a 2020  or received a.  
+000138a0: 2020 2020 2020 7661 6c69 6420 6d65 7373        valid mess
+000138b0: 6167 6520 6672 6f6d 2063 7572 7265 6e74  age from current
+000138c0: 206c 6561 6465 7220 7768 656e 2069 7420   leader when it 
+000138d0: 6973 2061 2066 6f6c 6c6f 7765 722e 0a20  is a follower.. 
+000138e0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+000138f0: 6566 2073 6574 5f65 6c65 6374 696f 6e5f  ef set_election_
+00013900: 656c 6170 7365 6428 7365 6c66 2c20 656c  elapsed(self, el
+00013910: 6563 7469 6f6e 5f65 6c61 7073 6564 3a20  ection_elapsed: 
+00013920: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00013930: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013940: 2020 6065 6c65 6374 696f 6e5f 656c 6170    `election_elap
+00013950: 7365 6460 3a20 5469 636b 7320 7369 6e63  sed`: Ticks sinc
+00013960: 6520 6974 2072 6561 6368 6564 206c 6173  e it reached las
+00013970: 7420 656c 6563 7469 6f6e 5469 6d65 6f75  t electionTimeou
+00013980: 7420 7768 656e 2069 7420 6973 206c 6561  t when it is lea
+00013990: 6465 7220 6f72 2063 616e 6469 6461 7465  der or candidate
+000139a0: 2e0a 2020 2020 2020 2020 4e75 6d62 6572  ..        Number
+000139b0: 206f 6620 7469 636b 7320 7369 6e63 6520   of ticks since 
+000139c0: 6974 2072 6561 6368 6564 206c 6173 7420  it reached last 
+000139d0: 656c 6563 7469 6f6e 5469 6d65 6f75 7420  electionTimeout 
+000139e0: 6f72 2072 6563 6569 7665 6420 610a 2020  or received a.  
+000139f0: 2020 2020 2020 7661 6c69 6420 6d65 7373        valid mess
+00013a00: 6167 6520 6672 6f6d 2063 7572 7265 6e74  age from current
+00013a10: 206c 6561 6465 7220 7768 656e 2069 7420   leader when it 
+00013a20: 6973 2061 2066 6f6c 6c6f 7765 722e 0a20  is a follower.. 
+00013a30: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00013a40: 6566 2067 6574 5f63 6865 636b 5f71 756f  ef get_check_quo
+00013a50: 7275 6d28 7365 6c66 2920 2d3e 2062 6f6f  rum(self) -> boo
+00013a60: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00013a70: 2020 2020 2020 2060 6368 6563 6b5f 7175         `check_qu
+00013a80: 6f72 756d 603a 2057 6865 7468 6572 2074  orum`: Whether t
+00013a90: 6f20 6368 6563 6b20 7468 6520 7175 6f72  o check the quor
+00013aa0: 756d 0a20 2020 2020 2020 2022 2222 0a20  um.        """. 
+00013ab0: 2020 2064 6566 2073 6574 5f63 6865 636b     def set_check
+00013ac0: 5f71 756f 7275 6d28 7365 6c66 2c20 6368  _quorum(self, ch
+00013ad0: 6563 6b5f 7175 6f72 756d 3a20 626f 6f6c  eck_quorum: bool
+00013ae0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00013af0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00013b00: 6368 6563 6b5f 7175 6f72 756d 603a 2057  check_quorum`: W
+00013b10: 6865 7468 6572 2074 6f20 6368 6563 6b20  hether to check 
+00013b20: 7468 6520 7175 6f72 756d 0a20 2020 2020  the quorum.     
+00013b30: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00013b40: 6574 5f70 7265 5f76 6f74 6528 7365 6c66  et_pre_vote(self
+00013b50: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00013b60: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00013b70: 7072 655f 766f 7465 603a 2045 6e61 626c  pre_vote`: Enabl
+00013b80: 6520 7468 6520 7072 6576 6f74 6520 616c  e the prevote al
+00013b90: 676f 7269 7468 6d2e 0a0a 2020 2020 2020  gorithm...      
+00013ba0: 2020 5468 6973 2065 6e61 626c 6573 2061    This enables a
+00013bb0: 2070 7265 2d65 6c65 6374 696f 6e20 766f   pre-election vo
+00013bc0: 7465 2072 6f75 6e64 206f 6e20 4361 6e64  te round on Cand
+00013bd0: 6964 6174 6573 2070 7269 6f72 2074 6f20  idates prior to 
+00013be0: 6469 7372 7570 7469 6e67 2074 6865 2063  disrupting the c
+00013bf0: 6c75 7374 6572 2e0a 0a20 2020 2020 2020  luster...       
+00013c00: 2045 6e61 626c 6520 7468 6973 2069 6620   Enable this if 
+00013c10: 6772 6561 7465 7220 636c 7573 7465 7220  greater cluster 
+00013c20: 7374 6162 696c 6974 7920 6973 2070 7265  stability is pre
+00013c30: 6665 7272 6564 206f 7665 7220 6661 7374  ferred over fast
+00013c40: 6572 2065 6c65 6374 696f 6e73 2e0a 2020  er elections..  
+00013c50: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00013c60: 6620 7365 745f 7072 655f 766f 7465 2873  f set_pre_vote(s
+00013c70: 656c 662c 2070 7265 5f76 6f74 653a 2062  elf, pre_vote: b
+00013c80: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
+00013c90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ca0: 2020 6070 7265 5f76 6f74 6560 3a20 456e    `pre_vote`: En
+00013cb0: 6162 6c65 2074 6865 2070 7265 766f 7465  able the prevote
+00013cc0: 2061 6c67 6f72 6974 686d 2e0a 0a20 2020   algorithm...   
+00013cd0: 2020 2020 2054 6869 7320 656e 6162 6c65       This enable
+00013ce0: 7320 6120 7072 652d 656c 6563 7469 6f6e  s a pre-election
+00013cf0: 2076 6f74 6520 726f 756e 6420 6f6e 2043   vote round on C
+00013d00: 616e 6469 6461 7465 7320 7072 696f 7220  andidates prior 
+00013d10: 746f 2064 6973 7275 7074 696e 6720 7468  to disrupting th
+00013d20: 6520 636c 7573 7465 722e 0a0a 2020 2020  e cluster...    
+00013d30: 2020 2020 456e 6162 6c65 2074 6869 7320      Enable this 
+00013d40: 6966 2067 7265 6174 6572 2063 6c75 7374  if greater clust
+00013d50: 6572 2073 7461 6269 6c69 7479 2069 7320  er stability is 
+00013d60: 7072 6566 6572 7265 6420 6f76 6572 2066  preferred over f
+00013d70: 6173 7465 7220 656c 6563 7469 6f6e 732e  aster elections.
+00013d80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013d90: 2064 6566 2061 7070 6c79 5f63 6f6e 665f   def apply_conf_
+00013da0: 6368 616e 6765 2873 656c 662c 2063 6f6e  change(self, con
+00013db0: 665f 6368 616e 6765 3a20 2243 6f6e 6643  f_change: "ConfC
+00013dc0: 6861 6e67 6556 3252 6566 2229 202d 3e20  hangeV2Ref") -> 
+00013dd0: 2243 6f6e 6643 6861 6e67 6552 6566 223a  "ConfChangeRef":
+00013de0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00013df0: 0a20 2020 2064 6566 2067 6574 5f72 6561  .    def get_rea
+00013e00: 645f 7374 6174 6573 2873 656c 6629 202d  d_states(self) -
+00013e10: 3e20 4c69 7374 5b22 5265 6164 5374 6174  > List["ReadStat
+00013e20: 6522 5d3a 0a20 2020 2020 2020 2022 2222  e"]:.        """
+00013e30: 0a20 2020 2020 2020 2060 7265 6164 5f73  .        `read_s
+00013e40: 7461 7465 7360 3a20 5468 6520 6375 7272  tates`: The curr
+00013e50: 656e 7420 7265 6164 2073 7461 7465 732e  ent read states.
+00013e60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013e70: 2064 6566 2073 6574 5f72 6561 645f 7374   def set_read_st
+00013e80: 6174 6573 280a 2020 2020 2020 2020 7365  ates(.        se
+00013e90: 6c66 2c20 7265 6164 5f73 7461 7465 733a  lf, read_states:
+00013ea0: 204c 6973 745b 2252 6561 6453 7461 7465   List["ReadState
+00013eb0: 225d 207c 204c 6973 745b 2252 6561 6453  "] | List["ReadS
+00013ec0: 7461 7465 5265 6622 5d0a 2020 2020 2920  tateRef"].    ) 
+00013ed0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00013ee0: 2022 2222 0a20 2020 2020 2020 2060 7265   """.        `re
+00013ef0: 6164 5f73 7461 7465 7360 3a20 5468 6520  ad_states`: The 
+00013f00: 6375 7272 656e 7420 7265 6164 2073 7461  current read sta
+00013f10: 7465 732e 0a20 2020 2020 2020 2022 2222  tes..        """
+00013f20: 0a20 2020 2064 6566 2067 6574 5f72 6561  .    def get_rea
+00013f30: 645f 6f6e 6c79 5f6f 7074 696f 6e28 7365  d_only_option(se
+00013f40: 6c66 2920 2d3e 2022 5265 6164 4f6e 6c79  lf) -> "ReadOnly
+00013f50: 4f70 7469 6f6e 223a 0a20 2020 2020 2020  Option":.       
+00013f60: 2022 2222 0a20 2020 2020 2020 2060 7265   """.        `re
+00013f70: 6164 5f6f 6e6c 795f 6f70 7469 6f6e 603a  ad_only_option`:
+00013f80: 2043 686f 6f73 6520 7468 6520 6c69 6e65   Choose the line
+00013f90: 6172 697a 6162 696c 6974 7920 6d6f 6465  arizability mode
+00013fa0: 206f 7220 7468 6520 6c65 6173 6520 6d6f   or the lease mo
+00013fb0: 6465 2074 6f20 7265 6164 2064 6174 612e  de to read data.
+00013fc0: 2049 6620 796f 7520 646f 6ee2 8099 7420   If you don...t 
+00013fd0: 6361 7265 2061 626f 7574 2074 6865 2072  care about the r
+00013fe0: 6561 6420 636f 6e73 6973 7465 6e63 7920  ead consistency 
+00013ff0: 616e 6420 7761 6e74 2061 2068 6967 6865  and want a highe
+00014000: 7220 7265 6164 2070 6572 666f 726d 616e  r read performan
+00014010: 6365 2c20 796f 7520 6361 6e20 7573 6520  ce, you can use 
+00014020: 7468 6520 6c65 6173 6520 6d6f 6465 2e0a  the lease mode..
+00014030: 2020 2020 2020 2020 5365 7474 696e 6720          Setting 
+00014040: 7468 6973 2074 6f20 604c 6561 7365 4261  this to `LeaseBa
+00014050: 7365 6460 2072 6571 7569 7265 7320 6063  sed` requires `c
+00014060: 6865 636b 5f71 756f 7275 6d20 3d20 7472  heck_quorum = tr
+00014070: 7565 602e 0a20 2020 2020 2020 2022 2222  ue`..        """
+00014080: 0a20 2020 2064 6566 2073 6574 5f72 6561  .    def set_rea
+00014090: 645f 6f6e 6c79 5f6f 7074 696f 6e28 7365  d_only_option(se
+000140a0: 6c66 2c20 6f70 7469 6f6e 3a20 2252 6561  lf, option: "Rea
+000140b0: 644f 6e6c 794f 7074 696f 6e22 2920 2d3e  dOnlyOption") ->
+000140c0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000140d0: 2222 0a20 2020 2020 2020 2060 7265 6164  "".        `read
+000140e0: 5f6f 6e6c 795f 6f70 7469 6f6e 603a 2043  _only_option`: C
+000140f0: 686f 6f73 6520 7468 6520 6c69 6e65 6172  hoose the linear
+00014100: 697a 6162 696c 6974 7920 6d6f 6465 206f  izability mode o
+00014110: 7220 7468 6520 6c65 6173 6520 6d6f 6465  r the lease mode
+00014120: 2074 6f20 7265 6164 2064 6174 612e 2049   to read data. I
+00014130: 6620 796f 7520 646f 6ee2 8099 7420 6361  f you don...t ca
+00014140: 7265 2061 626f 7574 2074 6865 2072 6561  re about the rea
+00014150: 6420 636f 6e73 6973 7465 6e63 7920 616e  d consistency an
+00014160: 6420 7761 6e74 2061 2068 6967 6865 7220  d want a higher 
+00014170: 7265 6164 2070 6572 666f 726d 616e 6365  read performance
+00014180: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
+00014190: 6520 6c65 6173 6520 6d6f 6465 2e0a 2020  e lease mode..  
+000141a0: 2020 2020 2020 5365 7474 696e 6720 7468        Setting th
+000141b0: 6973 2074 6f20 604c 6561 7365 4261 7365  is to `LeaseBase
+000141c0: 6460 2072 6571 7569 7265 7320 6063 6865  d` requires `che
+000141d0: 636b 5f71 756f 7275 6d20 3d20 7472 7565  ck_quorum = true
+000141e0: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
+000141f0: 2020 2064 6566 2069 6e66 6c69 6768 745f     def inflight_
+00014200: 6275 6666 6572 735f 7369 7a65 2873 656c  buffers_size(sel
+00014210: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00014220: 2020 2022 2222 4765 7420 7468 6520 696e     """Get the in
+00014230: 666c 6967 6874 2062 7566 6665 7220 7369  flight buffer si
+00014240: 7a65 2e22 2222 0a20 2020 2064 6566 206d  ze.""".    def m
+00014250: 6179 6265 5f66 7265 655f 696e 666c 6967  aybe_free_inflig
+00014260: 6874 5f62 7566 6665 7273 2873 656c 6629  ht_buffers(self)
+00014270: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00014280: 2020 2222 220a 2020 2020 2020 2020 4120    """.        A 
+00014290: 5261 6674 206c 6561 6465 7220 616c 6c6f  Raft leader allo
+000142a0: 6361 7465 7320 6120 7665 6374 6f72 2077  cates a vector w
+000142b0: 6974 6820 6361 7061 6369 7479 2060 6d61  ith capacity `ma
+000142c0: 785f 696e 666c 6967 6874 5f6d 7367 7360  x_inflight_msgs`
+000142d0: 2066 6f72 2065 7665 7279 2070 6565 722e   for every peer.
+000142e0: 0a20 2020 2020 2020 2049 7420 7461 6b65  .        It take
+000142f0: 7320 6120 6c6f 7420 6f66 206d 656d 6f72  s a lot of memor
+00014300: 7920 6966 2074 6865 7265 2061 7265 2074  y if there are t
+00014310: 6f6f 206d 616e 7920 5261 6674 2067 726f  oo many Raft gro
+00014320: 7570 732e 2060 6d61 7962 655f 6672 6565  ups. `maybe_free
+00014330: 5f69 6e66 6c69 6768 745f 6275 6666 6572  _inflight_buffer
+00014340: 7360 0a20 2020 2020 2020 2069 7320 7573  s`.        is us
+00014350: 6564 2074 6f20 6672 6565 206d 656d 6f72  ed to free memor
+00014360: 7920 6966 206e 6563 6573 7361 7279 2e0a  y if necessary..
+00014370: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014380: 6465 6620 6164 6a75 7374 5f6d 6178 5f69  def adjust_max_i
+00014390: 6e66 6c69 6768 745f 6d73 6773 2873 656c  nflight_msgs(sel
+000143a0: 662c 2074 6172 6765 743a 2069 6e74 2c20  f, target: int, 
+000143b0: 6361 703a 2069 6e74 2920 2d3e 204e 6f6e  cap: int) -> Non
+000143c0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000143d0: 2020 2020 2020 2054 6f20 6164 6a75 7374         To adjust
+000143e0: 2060 6d61 785f 696e 666c 6967 6874 5f6d   `max_inflight_m
+000143f0: 7367 7360 2066 6f72 2074 6865 2073 7065  sgs` for the spe
+00014400: 6369 6669 6564 2070 6565 722e 0a20 2020  cified peer..   
+00014410: 2020 2020 2053 6574 2074 6f20 6030 6020       Set to `0` 
+00014420: 7769 6c6c 2064 6973 6162 6c65 2074 6865  will disable the
+00014430: 2070 726f 6772 6573 732e 0a20 2020 2020   progress..     
+00014440: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00014450: 6574 5f72 6561 646f 6e6c 795f 7265 6164  et_readonly_read
+00014460: 5f69 6e64 6578 5f71 7565 7565 2873 656c  _index_queue(sel
+00014470: 6629 202d 3e20 4c69 7374 5b4c 6973 745b  f) -> List[List[
+00014480: 696e 745d 5d3a 0a20 2020 2020 2020 2022  int]]:.        "
+00014490: 2222 2022 2222 0a20 2020 2064 6566 2073  "" """.    def s
+000144a0: 6574 5f62 6174 6368 5f61 7070 656e 6428  et_batch_append(
+000144b0: 7365 6c66 2c20 6261 7463 685f 6170 7065  self, batch_appe
+000144c0: 6e64 3a20 626f 6f6c 2920 2d3e 204e 6f6e  nd: bool) -> Non
+000144d0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000144e0: 2020 2020 2020 2053 6574 2077 6865 7468         Set wheth
+000144f0: 6572 2062 6174 6368 2061 7070 656e 6420  er batch append 
+00014500: 6d73 6720 6174 2072 756e 7469 6d65 2e0a  msg at runtime..
+00014510: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014520: 6465 6620 7365 745f 6d61 785f 636f 6d6d  def set_max_comm
+00014530: 6974 7465 645f 7369 7a65 5f70 6572 5f72  itted_size_per_r
+00014540: 6561 6479 2873 656c 662c 2073 697a 653a  eady(self, size:
+00014550: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00014560: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014570: 2020 2053 6574 2060 6d61 785f 636f 6d6d     Set `max_comm
+00014580: 6974 7465 645f 7369 7a65 5f70 6572 5f72  itted_size_per_r
+00014590: 6561 6479 6020 746f 2060 7369 7a65 602e  eady` to `size`.
+000145a0: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+000145b0: 6173 7320 496e 4d65 6d6f 7279 5261 6674  ass InMemoryRaft
+000145c0: 285f 5f41 5049 5f52 6166 7429 3a0a 2020  (__API_Raft):.  
+000145d0: 2020 2222 220a 2020 2020 4120 7374 7275    """.    A stru
+000145e0: 6374 2074 6861 7420 7265 7072 6573 656e  ct that represen
+000145f0: 7473 2074 6865 2072 6166 7420 636f 6e73  ts the raft cons
+00014600: 656e 7375 7320 6974 7365 6c66 2e20 5374  ensus itself. St
+00014610: 6f72 6573 2064 6574 6169 6c73 2063 6f6e  ores details con
+00014620: 6365 726e 696e 6720 7468 6520 6375 7272  cerning the curr
+00014630: 656e 740a 2020 2020 616e 6420 706f 7373  ent.    and poss
+00014640: 6962 6c65 2073 7461 7465 2074 6865 2073  ible state the s
+00014650: 7973 7465 6d20 6361 6e20 7461 6b65 2e0a  ystem can take..
+00014660: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+00014670: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00014680: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00014690: 2063 6667 3a20 2243 6f6e 6669 6722 207c   cfg: "Config" |
+000146a0: 2022 436f 6e66 6967 5265 6622 2c0a 2020   "ConfigRef",.  
+000146b0: 2020 2020 2020 7374 6f72 653a 2022 4d65        store: "Me
+000146c0: 6d53 746f 7261 6765 2220 7c20 224d 656d  mStorage" | "Mem
+000146d0: 5374 6f72 6167 6552 6566 222c 0a20 2020  StorageRef",.   
+000146e0: 2020 2020 206c 6f67 6765 723a 2022 4c6f       logger: "Lo
+000146f0: 6767 6572 2220 7c20 224c 6f67 6765 7252  gger" | "LoggerR
+00014700: 6566 2220 7c20 2254 6872 6561 6453 6166  ef" | "ThreadSaf
+00014710: 654c 6f67 6765 7222 2c0a 2020 2020 2920  eLogger",.    ) 
+00014720: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+00014730: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
+00014740: 6c66 2920 2d3e 2022 496e 4d65 6d6f 7279  lf) -> "InMemory
+00014750: 5261 6674 5265 6622 3a20 2e2e 2e0a 2020  RaftRef": ....  
+00014760: 2020 6465 6620 6765 745f 7261 6674 5f6c    def get_raft_l
+00014770: 6f67 2873 656c 6629 202d 3e20 2249 6e4d  og(self) -> "InM
+00014780: 656d 6f72 7952 6166 744c 6f67 5265 6622  emoryRaftLogRef"
+00014790: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+000147a0: 220a 0a63 6c61 7373 2049 6e4d 656d 6f72  "..class InMemor
+000147b0: 7952 6166 7452 6566 285f 5f41 5049 5f52  yRaftRef(__API_R
+000147c0: 6166 7429 3a0a 2020 2020 2222 220a 2020  aft):.    """.  
+000147d0: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
+000147e0: 206f 6620 3a63 6c61 7373 3a60 496e 4d65   of :class:`InMe
+000147f0: 6d6f 7279 5261 6674 602e 0a20 2020 2022  moryRaft`..    "
+00014800: 2222 0a0a 2020 2020 6465 6620 6765 745f  ""..    def get_
+00014810: 7261 6674 5f6c 6f67 2873 656c 6629 202d  raft_log(self) -
+00014820: 3e20 2249 6e4d 656d 6f72 7952 6166 744c  > "InMemoryRaftL
+00014830: 6f67 5265 6622 3a0a 2020 2020 2020 2020  ogRef":.        
+00014840: 2222 2220 2222 220a 0a63 6c61 7373 2052  """ """..class R
+00014850: 6166 7428 5f5f 4150 495f 5261 6674 293a  aft(__API_Raft):
+00014860: 0a20 2020 2022 2222 0a20 2020 2041 2073  .    """.    A s
+00014870: 7472 7563 7420 7468 6174 2072 6570 7265  truct that repre
+00014880: 7365 6e74 7320 7468 6520 7261 6674 2063  sents the raft c
+00014890: 6f6e 7365 6e73 7573 2069 7473 656c 662e  onsensus itself.
+000148a0: 2053 746f 7265 7320 6465 7461 696c 7320   Stores details 
+000148b0: 636f 6e63 6572 6e69 6e67 2074 6865 2063  concerning the c
+000148c0: 7572 7265 6e74 0a20 2020 2061 6e64 2070  urrent.    and p
+000148d0: 6f73 7369 626c 6520 7374 6174 6520 7468  ossible state th
+000148e0: 6520 7379 7374 656d 2063 616e 2074 616b  e system can tak
+000148f0: 652e 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
+00014900: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00014910: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00014920: 2020 2020 6366 673a 2022 436f 6e66 6967      cfg: "Config
+00014930: 2220 7c20 2243 6f6e 6669 6752 6566 222c  " | "ConfigRef",
+00014940: 0a20 2020 2020 2020 2073 746f 7265 3a20  .        store: 
+00014950: 2253 746f 7261 6765 2220 7c20 2253 746f  "Storage" | "Sto
+00014960: 7261 6765 5265 6622 2c0a 2020 2020 2020  rageRef",.      
+00014970: 2020 6c6f 6767 6572 3a20 224c 6f67 6765    logger: "Logge
+00014980: 7222 207c 2022 4c6f 6767 6572 5265 6622  r" | "LoggerRef"
+00014990: 207c 2022 5468 7265 6164 5361 6665 4c6f   | "ThreadSafeLo
+000149a0: 6767 6572 222c 0a20 2020 2029 202d 3e20  gger",.    ) -> 
+000149b0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+000149c0: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+000149d0: 202d 3e20 2252 6166 7452 6566 223a 202e   -> "RaftRef": .
+000149e0: 2e2e 0a20 2020 2064 6566 2067 6574 5f72  ...    def get_r
+000149f0: 6166 745f 6c6f 6728 7365 6c66 2920 2d3e  aft_log(self) ->
+00014a00: 2022 5261 6674 4c6f 6752 6566 223a 0a20   "RaftLogRef":. 
+00014a10: 2020 2020 2020 2022 2222 2022 2222 0a0a         """ """..
+00014a20: 636c 6173 7320 5261 6674 5265 6628 5f5f  class RaftRef(__
+00014a30: 4150 495f 5261 6674 293a 0a20 2020 2022  API_Raft):.    "
+00014a40: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+00014a50: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+00014a60: 6052 6166 7460 2e0a 2020 2020 2222 220a  `Raft`..    """.
+00014a70: 0a20 2020 2064 6566 2067 6574 5f72 6166  .    def get_raf
+00014a80: 745f 6c6f 6728 7365 6c66 2920 2d3e 2022  t_log(self) -> "
+00014a90: 5261 6674 4c6f 6752 6566 223a 0a20 2020  RaftLogRef":.   
+00014aa0: 2020 2020 2022 2222 2022 2222 0a0a 636c       """ """..cl
+00014ab0: 6173 7320 5072 6f67 7265 7373 4d61 7049  ass ProgressMapI
+00014ac0: 7465 6d3a 0a20 2020 2064 6566 2069 6428  tem:.    def id(
+00014ad0: 7365 6c66 2920 2d3e 2069 6e74 3a20 2e2e  self) -> int: ..
+00014ae0: 2e0a 2020 2020 6465 6620 7072 6f67 7265  ..    def progre
+00014af0: 7373 2873 656c 6629 202d 3e20 2250 726f  ss(self) -> "Pro
+00014b00: 6772 6573 7322 3a20 2e2e 2e0a 0a63 6c61  gress": .....cla
+00014b10: 7373 205f 5f41 5049 5f50 726f 6772 6573  ss __API_Progres
+00014b20: 7354 7261 636b 6572 285f 5f43 6c6f 6e65  sTracker(__Clone
+00014b30: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
+00014b40: 6c6f 6e65 2873 656c 6629 202d 3e20 2250  lone(self) -> "P
+00014b50: 726f 6772 6573 7354 7261 636b 6572 223a  rogressTracker":
+00014b60: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+00014b70: 2873 656c 662c 2069 643a 2069 6e74 2920  (self, id: int) 
+00014b80: 2d3e 204f 7074 696f 6e61 6c5b 2250 726f  -> Optional["Pro
+00014b90: 6772 6573 7352 6566 225d 3a0a 2020 2020  gressRef"]:.    
+00014ba0: 2020 2020 2222 2222 2222 0a20 2020 2064      """""".    d
+00014bb0: 6566 2067 726f 7570 5f63 6f6d 6d69 7428  ef group_commit(
+00014bc0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+00014bd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014be0: 2020 2057 6865 7468 6572 2065 6e61 626c     Whether enabl
+00014bf0: 6520 6772 6f75 7020 636f 6d6d 6974 2e0a  e group commit..
+00014c00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014c10: 6465 6620 656e 6162 6c65 5f67 726f 7570  def enable_group
+00014c20: 5f63 6f6d 6d69 7428 7365 6c66 2c20 656e  _commit(self, en
+00014c30: 6162 6c65 3a20 626f 6f6c 2920 2d3e 204e  able: bool) -> N
+00014c40: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00014c50: 0a20 2020 2020 2020 2043 6f6e 6669 6775  .        Configu
+00014c60: 7265 7320 6772 6f75 7020 636f 6d6d 6974  res group commit
+00014c70: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00014c80: 2020 6465 6620 6861 735f 7175 6f72 756d    def has_quorum
+00014c90: 2873 656c 662c 2070 6f74 656e 7469 616c  (self, potential
+00014ca0: 5f71 756f 7275 6d3a 2053 6574 5b69 6e74  _quorum: Set[int
+00014cb0: 5d29 202d 3e20 626f 6f6c 3a0a 2020 2020  ]) -> bool:.    
+00014cc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014cd0: 4465 7465 726d 696e 6520 6966 2061 2071  Determine if a q
+00014ce0: 756f 7275 6d20 6973 2066 6f72 6d65 6420  uorum is formed 
+00014cf0: 6672 6f6d 2074 6865 2067 6976 656e 2073  from the given s
+00014d00: 6574 206f 6620 6e6f 6465 732e 0a0a 2020  et of nodes...  
+00014d10: 2020 2020 2020 5468 6973 2069 7320 7468        This is th
+00014d20: 6520 6f6e 6c79 2063 6f72 7265 6374 2077  e only correct w
+00014d30: 6179 2074 6f20 7665 7269 6679 2079 6f75  ay to verify you
+00014d40: 2068 6176 6520 7265 6163 6865 6420 6120   have reached a 
+00014d50: 7175 6f72 756d 2066 6f72 2074 6865 2077  quorum for the w
+00014d60: 686f 6c65 2067 726f 7570 2e0a 2020 2020  hole group..    
+00014d70: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00014d80: 6973 5f73 696e 676c 6574 6f6e 2873 656c  is_singleton(sel
+00014d90: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+00014da0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014db0: 5265 7475 726e 7320 7472 7565 2069 6620  Returns true if 
+00014dc0: 2861 6e64 206f 6e6c 7920 6966 2920 7468  (and only if) th
+00014dd0: 6572 6520 6973 206f 6e6c 7920 6f6e 6520  ere is only one 
+00014de0: 766f 7469 6e67 206d 656d 6265 720a 2020  voting member.  
+00014df0: 2020 2020 2020 2869 2e65 2e20 7468 6520        (i.e. the 
+00014e00: 6c65 6164 6572 2920 696e 2074 6865 2063  leader) in the c
+00014e10: 7572 7265 6e74 2063 6f6e 6669 6775 7261  urrent configura
+00014e20: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
+00014e30: 220a 2020 2020 6465 6620 7175 6f72 756d  ".    def quorum
+00014e40: 5f72 6563 656e 746c 795f 6163 7469 7665  _recently_active
+00014e50: 2873 656c 662c 2070 6572 7370 6563 7469  (self, perspecti
+00014e60: 7665 5f6f 663a 2069 6e74 2920 2d3e 2062  ve_of: int) -> b
+00014e70: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00014e80: 0a20 2020 2020 2020 2044 6574 6572 6d69  .        Determi
+00014e90: 6e65 7320 6966 2074 6865 2063 7572 7265  nes if the curre
+00014ea0: 6e74 2071 756f 7275 6d20 6973 2061 6374  nt quorum is act
+00014eb0: 6976 6520 6163 636f 7264 696e 6720 746f  ive according to
+00014ec0: 2074 6865 2074 6869 7320 7261 6674 206e   the this raft n
+00014ed0: 6f64 652e 0a20 2020 2020 2020 2044 6f69  ode..        Doi
+00014ee0: 6e67 2074 6869 7320 7769 6c6c 2073 6574  ng this will set
+00014ef0: 2074 6865 2060 7265 6365 6e74 5f61 6374   the `recent_act
+00014f00: 6976 6560 206f 6620 6561 6368 2070 6565  ive` of each pee
+00014f10: 7220 746f 2066 616c 7365 2e0a 0a20 2020  r to false...   
+00014f20: 2020 2020 2054 6869 7320 7368 6f75 6c64       This should
+00014f30: 206f 6e6c 7920 6265 2063 616c 6c65 6420   only be called 
+00014f40: 6279 2074 6865 206c 6561 6465 722e 0a20  by the leader.. 
+00014f50: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00014f60: 6566 206d 6178 696d 616c 5f63 6f6d 6d69  ef maximal_commi
+00014f70: 7474 6564 5f69 6e64 6578 2873 656c 6629  tted_index(self)
+00014f80: 202d 3e20 5475 706c 655b 696e 742c 2062   -> Tuple[int, b
+00014f90: 6f6f 6c5d 3a0a 2020 2020 2020 2020 2222  ool]:.        ""
+00014fa0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00014fb0: 7320 7468 6520 6d61 7869 6d61 6c20 636f  s the maximal co
+00014fc0: 6d6d 6974 7465 6420 696e 6465 7820 666f  mmitted index fo
+00014fd0: 7220 7468 6520 636c 7573 7465 722e 2054  r the cluster. T
+00014fe0: 6865 2062 6f6f 6c20 666c 6167 2069 6e64  he bool flag ind
+00014ff0: 6963 6174 6573 2077 6865 7468 6572 0a20  icates whether. 
+00015000: 2020 2020 2020 2074 6865 2069 6e64 6578         the index
+00015010: 2069 7320 636f 6d70 7574 6564 2062 7920   is computed by 
+00015020: 6772 6f75 7020 636f 6d6d 6974 2061 6c67  group commit alg
+00015030: 6f72 6974 686d 2073 7563 6365 7373 6675  orithm successfu
+00015040: 6c6c 790a 0a20 2020 2020 2020 2045 672e  lly..        Eg.
+00015050: 2049 6620 7468 6520 6d61 7463 6865 6420   If the matched 
+00015060: 696e 6465 7865 7320 6172 6520 605b 322c  indexes are `[2,
+00015070: 322c 322c 342c 355d 602c 2069 7420 7769  2,2,4,5]`, it wi
+00015080: 6c6c 2072 6574 7572 6e20 6032 602e 0a20  ll return `2`.. 
+00015090: 2020 2020 2020 2049 6620 7468 6520 6d61         If the ma
+000150a0: 7463 6865 6420 696e 6465 7865 7320 616e  tched indexes an
+000150b0: 6420 6772 6f75 7073 2061 7265 2060 5b28  d groups are `[(
+000150c0: 312c 2031 292c 2028 322c 2032 292c 2028  1, 1), (2, 2), (
+000150d0: 332c 2032 295d 602c 2069 7420 7769 6c6c  3, 2)]`, it will
+000150e0: 2072 6574 7572 6e20 6031 602e 0a20 2020   return `1`..   
+000150f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00015100: 2072 6563 6f72 645f 766f 7465 2873 656c   record_vote(sel
+00015110: 662c 2069 643a 2069 6e74 2c20 766f 7465  f, id: int, vote
+00015120: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
+00015130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015140: 2020 2020 2052 6563 6f72 6473 2074 6861       Records tha
+00015150: 7420 7468 6520 6e6f 6465 2077 6974 6820  t the node with 
+00015160: 7468 6520 6769 7665 6e20 6964 2076 6f74  the given id vot
+00015170: 6564 2066 6f72 2074 6869 7320 5261 6674  ed for this Raft
+00015180: 0a20 2020 2020 2020 2069 6e73 7461 6e63  .        instanc
+00015190: 6520 6966 2076 203d 3d20 7472 7565 2028  e if v == true (
+000151a0: 616e 6420 6465 636c 696e 6564 2069 7420  and declined it 
+000151b0: 6f74 6865 7277 6973 6529 2e0a 2020 2020  otherwise)..    
+000151c0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+000151d0: 7265 7365 745f 766f 7465 7328 7365 6c66  reset_votes(self
+000151e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000151f0: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+00015200: 7265 7061 7265 7320 666f 7220 6120 6e65  repares for a ne
+00015210: 7720 726f 756e 6420 6f66 2076 6f74 6520  w round of vote 
+00015220: 636f 756e 7469 6e67 2076 6961 2072 6563  counting via rec
+00015230: 6f72 6456 6f74 652e 0a20 2020 2020 2020  ordVote..       
+00015240: 2022 2222 0a20 2020 2064 6566 2063 6f6e   """.    def con
+00015250: 665f 766f 7465 7273 2873 656c 6629 202d  f_voters(self) -
+00015260: 3e20 224a 6f69 6e74 436f 6e66 6967 5265  > "JointConfigRe
+00015270: 6622 3a0a 2020 2020 2020 2020 2222 2220  f":.        """ 
+00015280: 2222 220a 2020 2020 6465 6620 636f 6e66  """.    def conf
+00015290: 5f6c 6561 726e 6572 7328 7365 6c66 2920  _learners(self) 
+000152a0: 2d3e 2053 6574 5b69 6e74 5d3a 0a20 2020  -> Set[int]:.   
+000152b0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+000152c0: 2064 6566 2063 6f6c 6c65 6374 2873 656c   def collect(sel
+000152d0: 6629 202d 3e20 4c69 7374 5b22 5072 6f67  f) -> List["Prog
+000152e0: 7265 7373 4d61 7049 7465 6d22 5d3a 0a20  ressMapItem"]:. 
+000152f0: 2020 2020 2020 2022 2222 2022 2222 0a0a         """ """..
+00015300: 636c 6173 7320 5072 6f67 7265 7373 5472  class ProgressTr
+00015310: 6163 6b65 7228 5f5f 4150 495f 5072 6f67  acker(__API_Prog
+00015320: 7265 7373 5472 6163 6b65 7229 3a0a 2020  ressTracker):.  
+00015330: 2020 2222 220a 2020 2020 6050 726f 6772    """.    `Progr
+00015340: 6573 7354 7261 636b 6572 6020 636f 6e74  essTracker` cont
+00015350: 6169 6e73 2073 6576 6572 616c 2060 5072  ains several `Pr
+00015360: 6f67 7265 7373 6065 732c 0a20 2020 2077  ogress`es,.    w
+00015370: 6869 6368 2063 6f75 6c64 2062 6520 604c  hich could be `L
+00015380: 6561 6465 7260 2c20 6046 6f6c 6c6f 7765  eader`, `Followe
+00015390: 7260 2061 6e64 2060 4c65 6172 6e65 7260  r` and `Learner`
+000153a0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+000153b0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000153c0: 2c20 6d61 785f 696e 666c 6967 6874 3a20  , max_inflight: 
+000153d0: 696e 7429 202d 3e20 4e6f 6e65 3a20 2e2e  int) -> None: ..
+000153e0: 2e0a 2020 2020 6465 6620 6d61 6b65 5f72  ..    def make_r
+000153f0: 6566 2873 656c 6629 202d 3e20 2250 726f  ef(self) -> "Pro
+00015400: 6772 6573 7354 7261 636b 6572 5265 6622  gressTrackerRef"
+00015410: 3a20 2e2e 2e0a 0a63 6c61 7373 2050 726f  : .....class Pro
+00015420: 6772 6573 7354 7261 636b 6572 5265 6628  gressTrackerRef(
+00015430: 5f5f 4150 495f 5072 6f67 7265 7373 5472  __API_ProgressTr
+00015440: 6163 6b65 7229 3a0a 2020 2020 2222 220a  acker):.    """.
+00015450: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
+00015460: 7065 206f 6620 3a63 6c61 7373 3a60 5072  pe of :class:`Pr
+00015470: 6f67 7265 7373 5472 6163 6b65 7260 2e0a  ogressTracker`..
+00015480: 2020 2020 2222 220a 0a63 6c61 7373 205f      """..class _
+00015490: 5f41 5049 5f50 726f 6772 6573 7328 5f5f  _API_Progress(__
+000154a0: 436c 6f6e 6561 626c 6529 3a0a 2020 2020  Cloneable):.    
+000154b0: 6465 6620 636c 6f6e 6528 7365 6c66 2920  def clone(self) 
+000154c0: 2d3e 2022 5072 6f67 7265 7373 223a 202e  -> "Progress": .
+000154d0: 2e2e 0a20 2020 2064 6566 2062 6563 6f6d  ...    def becom
+000154e0: 655f 7072 6f62 6528 7365 6c66 2920 2d3e  e_probe(self) ->
+000154f0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00015500: 2222 4368 616e 6765 7320 7468 6520 7072  ""Changes the pr
+00015510: 6f67 7265 7373 2074 6f20 6120 7072 6f62  ogress to a prob
+00015520: 652e 2222 220a 2020 2020 6465 6620 6265  e.""".    def be
+00015530: 636f 6d65 5f72 6570 6c69 6361 7465 2873  come_replicate(s
+00015540: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00015550: 2020 2020 2020 2222 2243 6861 6e67 6573        """Changes
+00015560: 2074 6865 2070 726f 6772 6573 7320 746f   the progress to
+00015570: 2061 2052 6570 6c69 6361 7465 2e22 2222   a Replicate."""
+00015580: 0a20 2020 2064 6566 2062 6563 6f6d 655f  .    def become_
+00015590: 736e 6170 7368 6f74 2873 656c 662c 2073  snapshot(self, s
+000155a0: 6e61 7073 686f 745f 6964 783a 2069 6e74  napshot_idx: int
+000155b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000155c0: 2020 2022 2222 4368 616e 6765 7320 7468     """Changes th
+000155d0: 6520 7072 6f67 7265 7373 2074 6f20 6120  e progress to a 
+000155e0: 736e 6170 7368 6f74 2e22 2222 0a20 2020  snapshot.""".   
+000155f0: 2064 6566 206d 6179 6265 5f75 7064 6174   def maybe_updat
+00015600: 6528 7365 6c66 2c20 6e3a 2069 6e74 2920  e(self, n: int) 
+00015610: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00015620: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00015630: 7572 6e73 2066 616c 7365 2069 6620 7468  urns false if th
+00015640: 6520 6769 7665 6e20 6e20 696e 6465 7820  e given n index 
+00015650: 636f 6d65 7320 6672 6f6d 2061 6e20 6f75  comes from an ou
+00015660: 7464 6174 6564 206d 6573 7361 6765 2e0a  tdated message..
+00015670: 2020 2020 2020 2020 4f74 6865 7277 6973          Otherwis
+00015680: 6520 6974 2075 7064 6174 6573 2074 6865  e it updates the
+00015690: 2070 726f 6772 6573 7320 616e 6420 7265   progress and re
+000156a0: 7475 726e 7320 7472 7565 2e0a 2020 2020  turns true..    
+000156b0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+000156c0: 6d61 7962 655f 6465 6372 5f74 6f28 0a20  maybe_decr_to(. 
+000156d0: 2020 2020 2020 2073 656c 662c 2072 656a         self, rej
+000156e0: 6563 7465 643a 2069 6e74 2c20 6d61 7463  ected: int, matc
+000156f0: 685f 6869 6e74 3a20 696e 742c 2072 6571  h_hint: int, req
+00015700: 7565 7374 5f73 6e61 7073 686f 743a 2069  uest_snapshot: i
+00015710: 6e74 0a20 2020 2029 202d 3e20 626f 6f6c  nt.    ) -> bool
+00015720: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00015730: 2020 2020 2020 5265 7475 726e 7320 6661        Returns fa
+00015740: 6c73 6520 6966 2074 6865 2067 6976 656e  lse if the given
+00015750: 2069 6e64 6578 2063 6f6d 6573 2066 726f   index comes fro
+00015760: 6d20 616e 206f 7574 206f 6620 6f72 6465  m an out of orde
+00015770: 7220 6d65 7373 6167 652e 0a20 2020 2020  r message..     
+00015780: 2020 204f 7468 6572 7769 7365 2069 7420     Otherwise it 
+00015790: 6465 6372 6561 7365 7320 7468 6520 7072  decreases the pr
+000157a0: 6f67 7265 7373 206e 6578 7420 696e 6465  ogress next inde
+000157b0: 7820 746f 206d 696e 2872 656a 6563 7465  x to min(rejecte
+000157c0: 642c 206c 6173 7429 0a20 2020 2020 2020  d, last).       
+000157d0: 2061 6e64 2072 6574 7572 6e73 2074 7275   and returns tru
+000157e0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+000157f0: 2020 2064 6566 2073 6e61 7073 686f 745f     def snapshot_
+00015800: 6661 696c 7572 6528 7365 6c66 2920 2d3e  failure(self) ->
+00015810: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00015820: 2222 0a20 2020 2020 2020 2053 6574 7320  "".        Sets 
+00015830: 7468 6520 736e 6170 7368 6f74 2074 6f20  the snapshot to 
+00015840: 6661 696c 7572 652e 0a20 2020 2020 2020  failure..       
+00015850: 2022 2222 0a20 2020 2064 6566 2070 6175   """.    def pau
+00015860: 7365 2873 656c 6629 202d 3e20 4e6f 6e65  se(self) -> None
+00015870: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00015880: 2020 2020 2020 5061 7573 6520 7072 6f67        Pause prog
+00015890: 7265 7373 2e0a 2020 2020 2020 2020 2222  ress..        ""
+000158a0: 220a 2020 2020 6465 6620 6973 5f70 6175  ".    def is_pau
+000158b0: 7365 6428 7365 6c66 2920 2d3e 2062 6f6f  sed(self) -> boo
+000158c0: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+000158d0: 2020 2020 2020 2044 6574 6572 6d69 6e65         Determine
+000158e0: 2077 6865 7468 6572 2070 726f 6772 6573   whether progres
+000158f0: 7320 6973 2070 6175 7365 642e 0a20 2020  s is paused..   
+00015900: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00015910: 2069 735f 736e 6170 7368 6f74 5f63 6175   is_snapshot_cau
+00015920: 6768 745f 7570 2873 656c 6629 202d 3e20  ght_up(self) -> 
+00015930: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00015940: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00015950: 7320 7472 7565 2069 6620 4d61 7463 6820  s true if Match 
+00015960: 6973 2065 7175 616c 206f 7220 6869 6768  is equal or high
+00015970: 6572 2074 6861 6e20 7468 6520 7065 6e64  er than the pend
+00015980: 696e 6753 6e61 7073 686f 742e 0a20 2020  ingSnapshot..   
+00015990: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+000159a0: 2072 6573 756d 6528 7365 6c66 2920 2d3e   resume(self) ->
+000159b0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000159c0: 2222 0a20 2020 2020 2020 2052 6573 756d  "".        Resum
+000159d0: 6520 7072 6f67 7265 7373 0a20 2020 2020  e progress.     
+000159e0: 2020 2022 2222 0a20 2020 2064 6566 2075     """.    def u
+000159f0: 7064 6174 655f 7374 6174 6528 7365 6c66  pdate_state(self
+00015a00: 2c20 6c61 7374 3a20 696e 7429 202d 3e20  , last: int) -> 
+00015a10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00015a20: 220a 2020 2020 2020 2020 5570 6461 7465  ".        Update
+00015a30: 2069 6e66 6c69 6768 7420 6d73 6773 2061   inflight msgs a
+00015a40: 6e64 206e 6578 745f 6964 780a 2020 2020  nd next_idx.    
+00015a50: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00015a60: 7570 6461 7465 5f63 6f6d 6d69 7474 6564  update_committed
+00015a70: 2873 656c 662c 2063 6f6d 6d69 7474 6564  (self, committed
+00015a80: 5f69 6e64 6578 3a20 696e 7429 202d 3e20  _index: int) -> 
+00015a90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00015aa0: 220a 2020 2020 2020 2020 5570 6461 7465  ".        Update
+00015ab0: 2063 6f6d 6d69 7474 6564 5f69 6e64 6578   committed_index
+00015ac0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00015ad0: 2020 6465 6620 6f70 7469 6d69 7374 6963    def optimistic
+00015ae0: 5f75 7064 6174 6528 7365 6c66 2c20 6e3a  _update(self, n:
+00015af0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00015b00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00015b10: 2020 204f 7074 696d 6973 7469 6361 6c6c     Optimisticall
+00015b20: 7920 6164 7661 6e63 6520 7468 6520 696e  y advance the in
+00015b30: 6465 780a 2020 2020 2020 2020 2222 220a  dex.        """.
+00015b40: 2020 2020 6465 6620 6765 745f 696e 7328      def get_ins(
+00015b50: 7365 6c66 2920 2d3e 2022 496e 666c 6967  self) -> "Inflig
+00015b60: 6874 7352 6566 223a 0a20 2020 2020 2020  htsRef":.       
+00015b70: 2022 2222 0a20 2020 2020 2020 2060 696e   """.        `in
+00015b80: 7360 3a20 496e 666c 6967 6874 7320 6973  s`: Inflights is
+00015b90: 2061 2073 6c69 6469 6e67 2077 696e 646f   a sliding windo
+00015ba0: 7720 666f 7220 7468 6520 696e 666c 6967  w for the inflig
+00015bb0: 6874 206d 6573 7361 6765 732e 0a20 2020  ht messages..   
+00015bc0: 2020 2020 2057 6865 6e20 696e 666c 6967       When inflig
+00015bd0: 6874 7320 6973 2066 756c 6c2c 206e 6f20  hts is full, no 
+00015be0: 6d6f 7265 206d 6573 7361 6765 2073 686f  more message sho
+00015bf0: 756c 6420 6265 2073 656e 742e 0a20 2020  uld be sent..   
+00015c00: 2020 2020 2057 6865 6e20 6120 6c65 6164       When a lead
+00015c10: 6572 2073 656e 6473 206f 7574 2061 206d  er sends out a m
+00015c20: 6573 7361 6765 2c20 7468 6520 696e 6465  essage, the inde
+00015c30: 7820 6f66 2074 6865 206c 6173 740a 2020  x of the last.  
+00015c40: 2020 2020 2020 656e 7472 7920 7368 6f75        entry shou
+00015c50: 6c64 2062 6520 6164 6465 6420 746f 2069  ld be added to i
+00015c60: 6e66 6c69 6768 7473 2e20 5468 6520 696e  nflights. The in
+00015c70: 6465 7820 4d55 5354 2062 6520 6164 6465  dex MUST be adde
+00015c80: 640a 2020 2020 2020 2020 696e 746f 2069  d.        into i
+00015c90: 6e66 6c69 6768 7473 2069 6e20 6f72 6465  nflights in orde
+00015ca0: 722e 0a20 2020 2020 2020 2057 6865 6e20  r..        When 
+00015cb0: 6120 6c65 6164 6572 2072 6563 6569 7665  a leader receive
+00015cc0: 7320 6120 7265 706c 792c 2074 6865 2070  s a reply, the p
+00015cd0: 7265 7669 6f75 7320 696e 666c 6967 6874  revious inflight
+00015ce0: 7320 7368 6f75 6c64 0a20 2020 2020 2020  s should.       
+00015cf0: 2062 6520 6672 6565 6420 6279 2063 616c   be freed by cal
+00015d00: 6c69 6e67 2069 6e66 6c69 6768 7473 2e66  ling inflights.f
+00015d10: 7265 6554 6f2e 0a20 2020 2020 2020 2022  reeTo..        "
+00015d20: 2222 0a20 2020 2064 6566 2073 6574 5f69  "".    def set_i
+00015d30: 6e73 2873 656c 662c 2069 6e66 6c69 6768  ns(self, infligh
+00015d40: 7473 3a20 2249 6e66 6c69 6768 7473 2220  ts: "Inflights" 
+00015d50: 7c20 2249 6e66 6c69 6768 7473 5265 6622  | "InflightsRef"
+00015d60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00015d70: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00015d80: 696e 7360 3a20 496e 666c 6967 6874 7320  ins`: Inflights 
+00015d90: 6973 2061 2073 6c69 6469 6e67 2077 696e  is a sliding win
+00015da0: 646f 7720 666f 7220 7468 6520 696e 666c  dow for the infl
+00015db0: 6967 6874 206d 6573 7361 6765 732e 0a20  ight messages.. 
+00015dc0: 2020 2020 2020 2057 6865 6e20 696e 666c         When infl
+00015dd0: 6967 6874 7320 6973 2066 756c 6c2c 206e  ights is full, n
+00015de0: 6f20 6d6f 7265 206d 6573 7361 6765 2073  o more message s
+00015df0: 686f 756c 6420 6265 2073 656e 742e 0a20  hould be sent.. 
+00015e00: 2020 2020 2020 2057 6865 6e20 6120 6c65         When a le
+00015e10: 6164 6572 2073 656e 6473 206f 7574 2061  ader sends out a
+00015e20: 206d 6573 7361 6765 2c20 7468 6520 696e   message, the in
+00015e30: 6465 7820 6f66 2074 6865 206c 6173 740a  dex of the last.
+00015e40: 2020 2020 2020 2020 656e 7472 7920 7368          entry sh
+00015e50: 6f75 6c64 2062 6520 6164 6465 6420 746f  ould be added to
+00015e60: 2069 6e66 6c69 6768 7473 2e20 5468 6520   inflights. The 
+00015e70: 696e 6465 7820 4d55 5354 2062 6520 6164  index MUST be ad
+00015e80: 6465 640a 2020 2020 2020 2020 696e 746f  ded.        into
+00015e90: 2069 6e66 6c69 6768 7473 2069 6e20 6f72   inflights in or
+00015ea0: 6465 722e 0a20 2020 2020 2020 2057 6865  der..        Whe
+00015eb0: 6e20 6120 6c65 6164 6572 2072 6563 6569  n a leader recei
+00015ec0: 7665 7320 6120 7265 706c 792c 2074 6865  ves a reply, the
+00015ed0: 2070 7265 7669 6f75 7320 696e 666c 6967   previous inflig
+00015ee0: 6874 7320 7368 6f75 6c64 0a20 2020 2020  hts should.     
+00015ef0: 2020 2062 6520 6672 6565 6420 6279 2063     be freed by c
+00015f00: 616c 6c69 6e67 2069 6e66 6c69 6768 7473  alling inflights
+00015f10: 2e66 7265 6554 6f2e 0a20 2020 2020 2020  .freeTo..       
+00015f20: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00015f30: 5f63 6f6d 6d69 745f 6772 6f75 705f 6964  _commit_group_id
+00015f40: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00015f50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00015f60: 2020 2060 636f 6d6d 6974 5f67 726f 7570     `commit_group
+00015f70: 5f69 6460 3a20 4f6e 6c79 206c 6f67 7320  _id`: Only logs 
+00015f80: 7265 706c 6963 6174 6564 2074 6f20 6469  replicated to di
+00015f90: 6666 6572 656e 7420 6772 6f75 7020 7769  fferent group wi
+00015fa0: 6c6c 2062 6520 636f 6d6d 6974 7465 6420  ll be committed 
+00015fb0: 6966 2061 6e79 2067 726f 7570 2069 7320  if any group is 
+00015fc0: 636f 6e66 6967 7572 6564 2e0a 2020 2020  configured..    
+00015fd0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00015fe0: 7365 745f 636f 6d6d 6974 5f67 726f 7570  set_commit_group
+00015ff0: 5f69 6428 7365 6c66 2c20 636f 6d6d 6974  _id(self, commit
+00016000: 5f67 726f 7570 5f69 643a 2069 6e74 2920  _group_id: int) 
+00016010: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00016020: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
+00016030: 6d6d 6974 5f67 726f 7570 5f69 6460 3a20  mmit_group_id`: 
+00016040: 4f6e 6c79 206c 6f67 7320 7265 706c 6963  Only logs replic
+00016050: 6174 6564 2074 6f20 6469 6666 6572 656e  ated to differen
+00016060: 7420 6772 6f75 7020 7769 6c6c 2062 6520  t group will be 
+00016070: 636f 6d6d 6974 7465 6420 6966 2061 6e79  committed if any
+00016080: 2067 726f 7570 2069 7320 636f 6e66 6967   group is config
+00016090: 7572 6564 2e0a 2020 2020 2020 2020 2222  ured..        ""
+000160a0: 220a 2020 2020 6465 6620 6765 745f 636f  ".    def get_co
+000160b0: 6d6d 6974 7465 645f 696e 6465 7828 7365  mmitted_index(se
+000160c0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+000160d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000160e0: 6063 6f6d 6d69 7474 6564 5f69 6e64 6578  `committed_index
+000160f0: 603a 2043 6f6d 6d69 7474 6564 2069 6e64  `: Committed ind
+00016100: 6578 2069 6e20 7261 6674 5f6c 6f67 0a20  ex in raft_log. 
+00016110: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00016120: 6566 2073 6574 5f63 6f6d 6d69 7474 6564  ef set_committed
+00016130: 5f69 6e64 6578 2873 656c 662c 2063 6f6d  _index(self, com
+00016140: 6d69 7474 6564 5f69 6e64 6578 3a20 696e  mitted_index: in
+00016150: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+00016160: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00016170: 6063 6f6d 6d69 7474 6564 5f69 6e64 6578  `committed_index
+00016180: 603a 2043 6f6d 6d69 7474 6564 2069 6e64  `: Committed ind
+00016190: 6578 2069 6e20 7261 6674 5f6c 6f67 0a20  ex in raft_log. 
+000161a0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+000161b0: 6566 2067 6574 5f6d 6174 6368 6564 2873  ef get_matched(s
+000161c0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000161d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000161e0: 2060 6d61 7463 6865 6460 3a20 486f 7720   `matched`: How 
+000161f0: 6d75 6368 2073 7461 7465 2069 7320 6d61  much state is ma
+00016200: 7463 6865 642e 0a20 2020 2020 2020 2022  tched..        "
+00016210: 2222 0a20 2020 2064 6566 2073 6574 5f6d  "".    def set_m
+00016220: 6174 6368 6564 2873 656c 662c 206d 6174  atched(self, mat
+00016230: 6368 6564 3a20 696e 7429 202d 3e20 4e6f  ched: int) -> No
+00016240: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00016250: 2020 2020 2020 2020 606d 6174 6368 6564          `matched
+00016260: 603a 2048 6f77 206d 7563 6820 7374 6174  `: How much stat
+00016270: 6520 6973 206d 6174 6368 6564 2e0a 2020  e is matched..  
+00016280: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00016290: 6620 6765 745f 6e65 7874 5f69 6478 2873  f get_next_idx(s
+000162a0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000162b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000162c0: 2060 6e65 7874 5f69 6478 603a 2054 6865   `next_idx`: The
+000162d0: 206e 6578 7420 696e 6465 7820 746f 2061   next index to a
+000162e0: 7070 6c79 0a20 2020 2020 2020 2022 2222  pply.        """
+000162f0: 0a20 2020 2064 6566 2073 6574 5f6e 6578  .    def set_nex
+00016300: 745f 6964 7828 7365 6c66 2c20 6e65 7874  t_idx(self, next
+00016310: 5f69 6478 3a20 696e 7429 202d 3e20 4e6f  _idx: int) -> No
+00016320: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00016330: 2020 2020 2020 2020 606e 6578 745f 6964          `next_id
+00016340: 7860 3a20 5468 6520 6e65 7874 2069 6e64  x`: The next ind
+00016350: 6578 2074 6f20 6170 706c 790a 2020 2020  ex to apply.    
+00016360: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00016370: 6765 745f 7065 6e64 696e 675f 736e 6170  get_pending_snap
+00016380: 7368 6f74 2873 656c 6629 202d 3e20 696e  shot(self) -> in
+00016390: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+000163a0: 2020 2020 2020 2060 7065 6e64 696e 675f         `pending_
+000163b0: 736e 6170 7368 6f74 603a 2054 6869 7320  snapshot`: This 
+000163c0: 6669 656c 6420 6973 2075 7365 6420 696e  field is used in
+000163d0: 2050 726f 6772 6573 7353 7461 7465 536e   ProgressStateSn
+000163e0: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
+000163f0: 4966 2074 6865 7265 2069 7320 6120 7065  If there is a pe
+00016400: 6e64 696e 6720 736e 6170 7368 6f74 2c20  nding snapshot, 
+00016410: 7468 6520 7065 6e64 696e 6753 6e61 7073  the pendingSnaps
+00016420: 686f 7420 7769 6c6c 2062 6520 7365 7420  hot will be set 
+00016430: 746f 2074 6865 0a20 2020 2020 2020 2069  to the.        i
+00016440: 6e64 6578 206f 6620 7468 6520 736e 6170  ndex of the snap
+00016450: 7368 6f74 2e20 4966 2070 656e 6469 6e67  shot. If pending
+00016460: 536e 6170 7368 6f74 2069 7320 7365 742c  Snapshot is set,
+00016470: 2074 6865 2072 6570 6c69 6361 7469 6f6e   the replication
+00016480: 2070 726f 6365 7373 206f 660a 2020 2020   process of.    
+00016490: 2020 2020 7468 6973 2050 726f 6772 6573      this Progres
+000164a0: 7320 7769 6c6c 2062 6520 7061 7573 6564  s will be paused
+000164b0: 2e20 7261 6674 2077 696c 6c20 6e6f 7420  . raft will not 
+000164c0: 7265 7365 6e64 2073 6e61 7073 686f 7420  resend snapshot 
+000164d0: 756e 7469 6c20 7468 6520 7065 6e64 696e  until the pendin
+000164e0: 6720 6f6e 650a 2020 2020 2020 2020 6973  g one.        is
+000164f0: 2072 6570 6f72 7465 6420 746f 2062 6520   reported to be 
+00016500: 6661 696c 6564 2e0a 2020 2020 2020 2020  failed..        
+00016510: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00016520: 7065 6e64 696e 675f 736e 6170 7368 6f74  pending_snapshot
+00016530: 2873 656c 662c 2070 656e 6469 6e67 5f73  (self, pending_s
+00016540: 6e61 7073 686f 743a 2069 6e74 2920 2d3e  napshot: int) ->
+00016550: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00016560: 2222 0a20 2020 2020 2020 2060 7065 6e64  "".        `pend
+00016570: 696e 675f 736e 6170 7368 6f74 603a 2054  ing_snapshot`: T
+00016580: 6869 7320 6669 656c 6420 6973 2075 7365  his field is use
+00016590: 6420 696e 2050 726f 6772 6573 7353 7461  d in ProgressSta
+000165a0: 7465 536e 6170 7368 6f74 2e0a 2020 2020  teSnapshot..    
+000165b0: 2020 2020 4966 2074 6865 7265 2069 7320      If there is 
+000165c0: 6120 7065 6e64 696e 6720 736e 6170 7368  a pending snapsh
+000165d0: 6f74 2c20 7468 6520 7065 6e64 696e 6753  ot, the pendingS
+000165e0: 6e61 7073 686f 7420 7769 6c6c 2062 6520  napshot will be 
+000165f0: 7365 7420 746f 2074 6865 0a20 2020 2020  set to the.     
+00016600: 2020 2069 6e64 6578 206f 6620 7468 6520     index of the 
+00016610: 736e 6170 7368 6f74 2e20 4966 2070 656e  snapshot. If pen
+00016620: 6469 6e67 536e 6170 7368 6f74 2069 7320  dingSnapshot is 
+00016630: 7365 742c 2074 6865 2072 6570 6c69 6361  set, the replica
+00016640: 7469 6f6e 2070 726f 6365 7373 206f 660a  tion process of.
+00016650: 2020 2020 2020 2020 7468 6973 2050 726f          this Pro
+00016660: 6772 6573 7320 7769 6c6c 2062 6520 7061  gress will be pa
+00016670: 7573 6564 2e20 7261 6674 2077 696c 6c20  used. raft will 
+00016680: 6e6f 7420 7265 7365 6e64 2073 6e61 7073  not resend snaps
+00016690: 686f 7420 756e 7469 6c20 7468 6520 7065  hot until the pe
+000166a0: 6e64 696e 6720 6f6e 650a 2020 2020 2020  nding one.      
+000166b0: 2020 6973 2072 6570 6f72 7465 6420 746f    is reported to
+000166c0: 2062 6520 6661 696c 6564 2e0a 2020 2020   be failed..    
+000166d0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+000166e0: 6765 745f 7065 6e64 696e 675f 7265 7175  get_pending_requ
+000166f0: 6573 745f 736e 6170 7368 6f74 2873 656c  est_snapshot(sel
+00016700: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00016710: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00016720: 7065 6e64 696e 675f 7265 7175 6573 745f  pending_request_
+00016730: 736e 6170 7368 6f74 603a 2054 6869 7320  snapshot`: This 
+00016740: 6669 656c 6420 6973 2075 7365 6420 696e  field is used in
+00016750: 2072 6571 7565 7374 2073 6e61 7073 686f   request snapsho
+00016760: 742e 0a20 2020 2020 2020 2049 6620 7468  t..        If th
+00016770: 6572 6520 6973 2061 2070 656e 6469 6e67  ere is a pending
+00016780: 2072 6571 7565 7374 2073 6e61 7073 686f   request snapsho
+00016790: 742c 2074 6869 7320 7769 6c6c 2062 6520  t, this will be 
+000167a0: 7365 7420 746f 2074 6865 2072 6571 7565  set to the reque
+000167b0: 7374 0a20 2020 2020 2020 2069 6e64 6578  st.        index
+000167c0: 206f 6620 7468 6520 736e 6170 7368 6f74   of the snapshot
+000167d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000167e0: 2020 6465 6620 7365 745f 7065 6e64 696e    def set_pendin
+000167f0: 675f 7265 7175 6573 745f 736e 6170 7368  g_request_snapsh
+00016800: 6f74 2873 656c 662c 2070 656e 6469 6e67  ot(self, pending
+00016810: 5f72 6571 7565 7374 5f73 6e61 7073 686f  _request_snapsho
+00016820: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
+00016830: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016840: 2020 2020 2060 7065 6e64 696e 675f 7265       `pending_re
+00016850: 7175 6573 745f 736e 6170 7368 6f74 603a  quest_snapshot`:
+00016860: 2054 6869 7320 6669 656c 6420 6973 2075   This field is u
+00016870: 7365 6420 696e 2072 6571 7565 7374 2073  sed in request s
+00016880: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
+00016890: 2049 6620 7468 6572 6520 6973 2061 2070   If there is a p
+000168a0: 656e 6469 6e67 2072 6571 7565 7374 2073  ending request s
+000168b0: 6e61 7073 686f 742c 2074 6869 7320 7769  napshot, this wi
+000168c0: 6c6c 2062 6520 7365 7420 746f 2074 6865  ll be set to the
+000168d0: 2072 6571 7565 7374 0a20 2020 2020 2020   request.       
+000168e0: 2069 6e64 6578 206f 6620 7468 6520 736e   index of the sn
+000168f0: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
+00016900: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00016910: 7265 6365 6e74 5f61 6374 6976 6528 7365  recent_active(se
+00016920: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00016930: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016940: 2060 7265 6365 6e74 5f61 6374 6976 6560   `recent_active`
+00016950: 3a20 5468 6973 2069 7320 7472 7565 2069  : This is true i
+00016960: 6620 7468 6520 7072 6f67 7265 7373 2069  f the progress i
+00016970: 7320 7265 6365 6e74 6c79 2061 6374 6976  s recently activ
+00016980: 652e 2052 6563 6569 7669 6e67 2061 6e79  e. Receiving any
+00016990: 206d 6573 7361 6765 730a 2020 2020 2020   messages.      
+000169a0: 2020 6672 6f6d 2074 6865 2063 6f72 7265    from the corre
+000169b0: 7370 6f6e 6469 6e67 2066 6f6c 6c6f 7765  sponding followe
+000169c0: 7220 696e 6469 6361 7465 7320 7468 6520  r indicates the 
+000169d0: 7072 6f67 7265 7373 2069 7320 6163 7469  progress is acti
+000169e0: 7665 2e0a 2020 2020 2020 2020 5265 6365  ve..        Rece
+000169f0: 6e74 4163 7469 7665 2063 616e 2062 6520  ntActive can be 
+00016a00: 7265 7365 7420 746f 2066 616c 7365 2061  reset to false a
+00016a10: 6674 6572 2061 6e20 656c 6563 7469 6f6e  fter an election
+00016a20: 2074 696d 656f 7574 2e0a 2020 2020 2020   timeout..      
+00016a30: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00016a40: 745f 7265 6365 6e74 5f61 6374 6976 6528  t_recent_active(
+00016a50: 7365 6c66 2c20 7265 6365 6e74 5f61 6374  self, recent_act
+00016a60: 6976 653a 2062 6f6f 6c29 202d 3e20 4e6f  ive: bool) -> No
+00016a70: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00016a80: 2020 2020 2020 2020 6072 6563 656e 745f          `recent_
+00016a90: 6163 7469 7665 603a 2054 6869 7320 6973  active`: This is
+00016aa0: 2074 7275 6520 6966 2074 6865 2070 726f   true if the pro
+00016ab0: 6772 6573 7320 6973 2072 6563 656e 746c  gress is recentl
+00016ac0: 7920 6163 7469 7665 2e20 5265 6365 6976  y active. Receiv
+00016ad0: 696e 6720 616e 7920 6d65 7373 6167 6573  ing any messages
+00016ae0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
+00016af0: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+00016b00: 666f 6c6c 6f77 6572 2069 6e64 6963 6174  follower indicat
+00016b10: 6573 2074 6865 2070 726f 6772 6573 7320  es the progress 
+00016b20: 6973 2061 6374 6976 652e 0a20 2020 2020  is active..     
+00016b30: 2020 2052 6563 656e 7441 6374 6976 6520     RecentActive 
+00016b40: 6361 6e20 6265 2072 6573 6574 2074 6f20  can be reset to 
+00016b50: 6661 6c73 6520 6166 7465 7220 616e 2065  false after an e
+00016b60: 6c65 6374 696f 6e20 7469 6d65 6f75 742e  lection timeout.
+00016b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016b80: 2064 6566 2067 6574 5f70 6175 7365 6428   def get_paused(
+00016b90: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+00016ba0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016bb0: 2020 2060 7061 7573 6564 603a 2050 6175     `paused`: Pau
+00016bc0: 7365 6420 6973 2075 7365 6420 696e 2050  sed is used in P
+00016bd0: 726f 6772 6573 7353 7461 7465 5072 6f62  rogressStateProb
+00016be0: 652e 0a20 2020 2020 2020 2057 6865 6e20  e..        When 
+00016bf0: 5061 7573 6564 2069 7320 7472 7565 2c20  Paused is true, 
+00016c00: 7261 6674 2073 686f 756c 6420 7061 7573  raft should paus
+00016c10: 6520 7365 6e64 696e 6720 7265 706c 6963  e sending replic
+00016c20: 6174 696f 6e20 6d65 7373 6167 6520 746f  ation message to
+00016c30: 2074 6869 7320 7065 6572 2e0a 2020 2020   this peer..    
+00016c40: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00016c50: 7365 745f 7061 7573 6564 2873 656c 662c  set_paused(self,
+00016c60: 2070 6175 7365 643a 2062 6f6f 6c29 202d   paused: bool) -
+00016c70: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00016c80: 2222 220a 2020 2020 2020 2020 6070 6175  """.        `pau
+00016c90: 7365 6460 3a20 5061 7573 6564 2069 7320  sed`: Paused is 
+00016ca0: 7573 6564 2069 6e20 5072 6f67 7265 7373  used in Progress
+00016cb0: 5374 6174 6550 726f 6265 2e0a 2020 2020  StateProbe..    
+00016cc0: 2020 2020 5768 656e 2050 6175 7365 6420      When Paused 
+00016cd0: 6973 2074 7275 652c 2072 6166 7420 7368  is true, raft sh
+00016ce0: 6f75 6c64 2070 6175 7365 2073 656e 6469  ould pause sendi
+00016cf0: 6e67 2072 6570 6c69 6361 7469 6f6e 206d  ng replication m
+00016d00: 6573 7361 6765 2074 6f20 7468 6973 2070  essage to this p
+00016d10: 6565 722e 0a20 2020 2020 2020 2022 2222  eer..        """
+00016d20: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
+00016d30: 7465 2873 656c 6629 202d 3e20 2250 726f  te(self) -> "Pro
+00016d40: 6772 6573 7353 7461 7465 223a 0a20 2020  gressState":.   
+00016d50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016d60: 2060 7374 6174 6560 3a20 5768 656e 2069   `state`: When i
+00016d70: 6e20 5072 6f67 7265 7373 5374 6174 6550  n ProgressStateP
+00016d80: 726f 6265 2c20 6c65 6164 6572 2073 656e  robe, leader sen
+00016d90: 6473 2061 7420 6d6f 7374 206f 6e65 2072  ds at most one r
+00016da0: 6570 6c69 6361 7469 6f6e 206d 6573 7361  eplication messa
+00016db0: 6765 0a20 2020 2020 2020 2070 6572 2068  ge.        per h
+00016dc0: 6561 7274 6265 6174 2069 6e74 6572 7661  eartbeat interva
+00016dd0: 6c2e 2049 7420 616c 736f 2070 726f 6265  l. It also probe
+00016de0: 7320 6163 7475 616c 2070 726f 6772 6573  s actual progres
+00016df0: 7320 6f66 2074 6865 2066 6f6c 6c6f 7765  s of the followe
+00016e00: 722e 0a0a 2020 2020 2020 2020 5768 656e  r...        When
+00016e10: 2069 6e20 5072 6f67 7265 7373 5374 6174   in ProgressStat
+00016e20: 6552 6570 6c69 6361 7465 2c20 6c65 6164  eReplicate, lead
+00016e30: 6572 206f 7074 696d 6973 7469 6361 6c6c  er optimisticall
+00016e40: 7920 696e 6372 6561 7365 7320 6e65 7874  y increases next
+00016e50: 0a20 2020 2020 2020 2074 6f20 7468 6520  .        to the 
+00016e60: 6c61 7465 7374 2065 6e74 7279 2073 656e  latest entry sen
+00016e70: 7420 6166 7465 7220 7365 6e64 696e 6720  t after sending 
+00016e80: 7265 706c 6963 6174 696f 6e20 6d65 7373  replication mess
+00016e90: 6167 652e 2054 6869 7320 6973 0a20 2020  age. This is.   
+00016ea0: 2020 2020 2061 6e20 6f70 7469 6d69 7a65       an optimize
+00016eb0: 6420 7374 6174 6520 666f 7220 6661 7374  d state for fast
+00016ec0: 2072 6570 6c69 6361 7469 6e67 206c 6f67   replicating log
+00016ed0: 2065 6e74 7269 6573 2074 6f20 7468 6520   entries to the 
+00016ee0: 666f 6c6c 6f77 6572 2e0a 0a20 2020 2020  follower...     
+00016ef0: 2020 2057 6865 6e20 696e 2050 726f 6772     When in Progr
+00016f00: 6573 7353 7461 7465 536e 6170 7368 6f74  essStateSnapshot
+00016f10: 2c20 6c65 6164 6572 2073 686f 756c 6420  , leader should 
+00016f20: 6861 7665 2073 656e 7420 6f75 7420 736e  have sent out sn
+00016f30: 6170 7368 6f74 0a20 2020 2020 2020 2062  apshot.        b
+00016f40: 6566 6f72 6520 616e 6420 7374 6f70 2073  efore and stop s
+00016f50: 656e 6469 6e67 2061 6e79 2072 6570 6c69  ending any repli
+00016f60: 6361 7469 6f6e 206d 6573 7361 6765 2e0a  cation message..
+00016f70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00016f80: 6465 6620 7365 745f 7374 6174 6528 7365  def set_state(se
+00016f90: 6c66 2c20 7374 6174 653a 2022 5072 6f67  lf, state: "Prog
+00016fa0: 7265 7373 5374 6174 6522 2920 2d3e 204e  ressState") -> N
+00016fb0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00016fc0: 0a20 2020 2020 2020 2060 7374 6174 6560  .        `state`
+00016fd0: 3a20 5768 656e 2069 6e20 5072 6f67 7265  : When in Progre
+00016fe0: 7373 5374 6174 6550 726f 6265 2c20 6c65  ssStateProbe, le
+00016ff0: 6164 6572 2073 656e 6473 2061 7420 6d6f  ader sends at mo
+00017000: 7374 206f 6e65 2072 6570 6c69 6361 7469  st one replicati
+00017010: 6f6e 206d 6573 7361 6765 0a20 2020 2020  on message.     
+00017020: 2020 2070 6572 2068 6561 7274 6265 6174     per heartbeat
+00017030: 2069 6e74 6572 7661 6c2e 2049 7420 616c   interval. It al
+00017040: 736f 2070 726f 6265 7320 6163 7475 616c  so probes actual
+00017050: 2070 726f 6772 6573 7320 6f66 2074 6865   progress of the
+00017060: 2066 6f6c 6c6f 7765 722e 0a0a 2020 2020   follower...    
+00017070: 2020 2020 5768 656e 2069 6e20 5072 6f67      When in Prog
+00017080: 7265 7373 5374 6174 6552 6570 6c69 6361  ressStateReplica
+00017090: 7465 2c20 6c65 6164 6572 206f 7074 696d  te, leader optim
+000170a0: 6973 7469 6361 6c6c 7920 696e 6372 6561  istically increa
+000170b0: 7365 7320 6e65 7874 0a20 2020 2020 2020  ses next.       
+000170c0: 2074 6f20 7468 6520 6c61 7465 7374 2065   to the latest e
+000170d0: 6e74 7279 2073 656e 7420 6166 7465 7220  ntry sent after 
+000170e0: 7365 6e64 696e 6720 7265 706c 6963 6174  sending replicat
+000170f0: 696f 6e20 6d65 7373 6167 652e 2054 6869  ion message. Thi
+00017100: 7320 6973 0a20 2020 2020 2020 2061 6e20  s is.        an 
+00017110: 6f70 7469 6d69 7a65 6420 7374 6174 6520  optimized state 
+00017120: 666f 7220 6661 7374 2072 6570 6c69 6361  for fast replica
+00017130: 7469 6e67 206c 6f67 2065 6e74 7269 6573  ting log entries
+00017140: 2074 6f20 7468 6520 666f 6c6c 6f77 6572   to the follower
+00017150: 2e0a 0a20 2020 2020 2020 2057 6865 6e20  ...        When 
+00017160: 696e 2050 726f 6772 6573 7353 7461 7465  in ProgressState
+00017170: 536e 6170 7368 6f74 2c20 6c65 6164 6572  Snapshot, leader
+00017180: 2073 686f 756c 6420 6861 7665 2073 656e   should have sen
+00017190: 7420 6f75 7420 736e 6170 7368 6f74 0a20  t out snapshot. 
+000171a0: 2020 2020 2020 2062 6566 6f72 6520 616e         before an
+000171b0: 6420 7374 6f70 2073 656e 6469 6e67 2061  d stop sending a
+000171c0: 6e79 2072 6570 6c69 6361 7469 6f6e 206d  ny replication m
+000171d0: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
+000171e0: 2222 220a 0a63 6c61 7373 2050 726f 6772  """..class Progr
+000171f0: 6573 7328 5f5f 4150 495f 5072 6f67 7265  ess(__API_Progre
+00017200: 7373 293a 0a20 2020 2022 2222 0a20 2020  ss):.    """.   
+00017210: 2054 6865 2070 726f 6772 6573 7320 6f66   The progress of
+00017220: 2063 6174 6368 696e 6720 7570 2066 726f   catching up fro
+00017230: 6d20 6120 7265 7374 6172 742e 0a20 2020  m a restart..   
+00017240: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00017250: 696e 6974 5f5f 2873 656c 662c 206e 6578  init__(self, nex
+00017260: 745f 6964 783a 2069 6e74 2c20 696e 735f  t_idx: int, ins_
+00017270: 7369 7a65 3a20 696e 7429 202d 3e20 4e6f  size: int) -> No
+00017280: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+00017290: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
+000172a0: 3e20 2250 726f 6772 6573 7352 6566 223a  > "ProgressRef":
+000172b0: 202e 2e2e 0a0a 636c 6173 7320 5072 6f67   .....class Prog
+000172c0: 7265 7373 5265 6628 5f5f 4150 495f 5072  ressRef(__API_Pr
+000172d0: 6f67 7265 7373 293a 0a20 2020 2022 2222  ogress):.    """
+000172e0: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
+000172f0: 7970 6520 6f66 203a 636c 6173 733a 6050  ype of :class:`P
+00017300: 726f 6772 6573 7360 2e0a 2020 2020 2222  rogress`..    ""
+00017310: 220a 0a63 6c61 7373 205f 5f41 5049 5f4a  "..class __API_J
+00017320: 6f69 6e74 436f 6e66 6967 285f 5f43 6c6f  ointConfig(__Clo
+00017330: 6e65 6162 6c65 293a 0a20 2020 2064 6566  neable):.    def
+00017340: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
+00017350: 224a 6f69 6e74 436f 6e66 6967 223a 202e  "JointConfig": .
+00017360: 2e2e 0a20 2020 2064 6566 2063 6c65 6172  ...    def clear
+00017370: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00017380: 2020 2020 2020 2020 2222 2243 6c65 6172          """Clear
+00017390: 7320 616c 6c20 4944 732e 2222 220a 2020  s all IDs.""".  
+000173a0: 2020 6465 6620 636f 6e74 6169 6e73 2873    def contains(s
+000173b0: 656c 662c 2069 643a 2069 6e74 2920 2d3e  elf, id: int) ->
+000173c0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+000173d0: 2222 4368 6563 6b20 6966 2061 6e20 6964  ""Check if an id
+000173e0: 2069 7320 6120 766f 7465 722e 2222 220a   is a voter.""".
+000173f0: 2020 2020 6465 6620 6964 7328 2920 2d3e      def ids() ->
+00017400: 2053 6574 5b69 6e74 5d3a 0a20 2020 2020   Set[int]:.     
+00017410: 2020 2022 2222 5265 7475 726e 7320 616e     """Returns an
+00017420: 2069 7465 7261 746f 7220 6f76 6572 2074   iterator over t
+00017430: 776f 2068 6173 6820 7365 7420 7769 7468  wo hash set with
+00017440: 6f75 7420 636c 6f6e 696e 672e 2222 220a  out cloning.""".
+00017450: 2020 2020 6465 6620 6973 5f73 696e 676c      def is_singl
+00017460: 6574 6f6e 2873 656c 6629 202d 3e20 626f  eton(self) -> bo
+00017470: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+00017480: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+00017490: 7472 7565 2069 6620 2861 6e64 206f 6e6c  true if (and onl
+000174a0: 7920 6966 2920 7468 6572 6520 6973 206f  y if) there is o
+000174b0: 6e6c 7920 6f6e 6520 766f 7469 6e67 206d  nly one voting m
+000174c0: 656d 6265 720a 2020 2020 2020 2020 2869  ember.        (i
+000174d0: 2e65 2e20 7468 6520 6c65 6164 6572 2920  .e. the leader) 
+000174e0: 696e 2074 6865 2063 7572 7265 6e74 2063  in the current c
+000174f0: 6f6e 6669 6775 7261 7469 6f6e 2e0a 2020  onfiguration..  
+00017500: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
+00017510: 204a 6f69 6e74 436f 6e66 6967 285f 5f41   JointConfig(__A
+00017520: 5049 5f4a 6f69 6e74 436f 6e66 6967 293a  PI_JointConfig):
+00017530: 0a20 2020 2022 2222 0a20 2020 2041 2063  .    """.    A c
+00017540: 6f6e 6669 6775 7261 7469 6f6e 206f 6620  onfiguration of 
+00017550: 7477 6f20 6772 6f75 7073 206f 6620 2870  two groups of (p
+00017560: 6f73 7369 626c 7920 6f76 6572 6c61 7070  ossibly overlapp
+00017570: 696e 6729 206d 616a 6f72 6974 7920 636f  ing) majority co
+00017580: 6e66 6967 7572 6174 696f 6e73 2e0a 2020  nfigurations..  
+00017590: 2020 4465 6369 7369 6f6e 7320 7265 7175    Decisions requ
+000175a0: 6972 6520 7468 6520 7375 7070 6f72 7420  ire the support 
+000175b0: 6f66 2062 6f74 6820 6d61 6a6f 7269 7469  of both majoriti
+000175c0: 6573 2e0a 2020 2020 2222 220a 0a20 2020  es..    """..   
+000175d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000175e0: 6c66 2c20 766f 7465 7273 3a20 5365 745b  lf, voters: Set[
+000175f0: 696e 745d 2920 2d3e 204e 6f6e 653a 202e  int]) -> None: .
+00017600: 2e2e 0a20 2020 2064 6566 206d 616b 655f  ...    def make_
+00017610: 7265 6628 7365 6c66 2920 2d3e 2022 4a6f  ref(self) -> "Jo
+00017620: 696e 7443 6f6e 6669 6752 6566 223a 202e  intConfigRef": .
+00017630: 2e2e 0a0a 636c 6173 7320 4a6f 696e 7443  ....class JointC
+00017640: 6f6e 6669 6752 6566 285f 5f41 5049 5f4a  onfigRef(__API_J
+00017650: 6f69 6e74 436f 6e66 6967 293a 0a20 2020  ointConfig):.   
+00017660: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
+00017670: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
+00017680: 733a 604a 6f69 6e74 436f 6e66 6967 602e  s:`JointConfig`.
+00017690: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+000176a0: 5f5f 4150 495f 4d61 6a6f 7269 7479 436f  __API_MajorityCo
+000176b0: 6e66 6967 285f 5f43 6c6f 6e65 6162 6c65  nfig(__Cloneable
+000176c0: 293a 0a20 2020 2064 6566 2063 6c6f 6e65  ):.    def clone
+000176d0: 2873 656c 6629 202d 3e20 224d 616a 6f72  (self) -> "Major
+000176e0: 6974 7943 6f6e 6669 6722 3a20 2e2e 2e0a  ityConfig": ....
+000176f0: 2020 2020 6465 6620 7261 775f 736c 6963      def raw_slic
+00017700: 6528 7365 6c66 2920 2d3e 204c 6973 745b  e(self) -> List[
+00017710: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
+00017720: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00017730: 7320 7468 6520 4d61 6a6f 7269 7479 436f  s the MajorityCo
+00017740: 6e66 6967 2061 7320 6120 736c 6963 652e  nfig as a slice.
+00017750: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017760: 2064 6566 2063 6170 6163 6974 7928 7365   def capacity(se
+00017770: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00017780: 2020 2020 2222 2222 2222 0a20 2020 2064      """""".    d
+00017790: 6566 2065 7874 656e 6428 7365 6c66 2c20  ef extend(self, 
+000177a0: 6f74 6865 725f 7365 743a 2053 6574 5b69  other_set: Set[i
+000177b0: 6e74 5d29 202d 3e20 4e6f 6e65 3a0a 2020  nt]) -> None:.  
+000177c0: 2020 2020 2020 2222 2222 2222 0a20 2020        """""".   
+000177d0: 2064 6566 2067 6574 2873 656c 662c 2069   def get(self, i
+000177e0: 6e64 6578 3a20 696e 7429 202d 3e20 4f70  ndex: int) -> Op
+000177f0: 7469 6f6e 616c 5b69 6e74 5d3a 0a20 2020  tional[int]:.   
+00017800: 2020 2020 2022 2222 2222 220a 2020 2020       """""".    
+00017810: 6465 6620 696e 7365 7274 2873 656c 662c  def insert(self,
+00017820: 2076 616c 7565 3a20 696e 7429 202d 3e20   value: int) -> 
+00017830: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00017840: 2222 2222 0a20 2020 2064 6566 2072 6570  """".    def rep
+00017850: 6c61 6365 2873 656c 662c 2076 616c 7565  lace(self, value
+00017860: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
+00017870: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
+00017880: 2020 6465 6620 6973 5f64 6973 6a6f 696e    def is_disjoin
+00017890: 7428 7365 6c66 2c20 6f74 6865 723a 2053  t(self, other: S
+000178a0: 6574 5b69 6e74 5d29 202d 3e20 626f 6f6c  et[int]) -> bool
+000178b0: 3a0a 2020 2020 2020 2020 2222 2222 2222  :.        """"""
+000178c0: 0a20 2020 2064 6566 2069 735f 7375 7065  .    def is_supe
+000178d0: 7273 6574 2873 656c 662c 206f 7468 6572  rset(self, other
+000178e0: 3a20 5365 745b 696e 745d 2920 2d3e 2062  : Set[int]) -> b
+000178f0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00017900: 2222 220a 2020 2020 6465 6620 6973 5f73  """.    def is_s
+00017910: 7562 7365 7428 7365 6c66 2c20 6f74 6865  ubset(self, othe
+00017920: 723a 2053 6574 5b69 6e74 5d29 202d 3e20  r: Set[int]) -> 
+00017930: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00017940: 2222 2222 0a20 2020 2064 6566 2072 6573  """".    def res
+00017950: 6572 7665 2873 656c 662c 2061 6464 6974  erve(self, addit
+00017960: 696f 6e61 6c3a 2069 6e74 2920 2d3e 204e  ional: int) -> N
+00017970: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00017980: 2222 220a 2020 2020 6465 6620 7265 6d6f  """.    def remo
+00017990: 7665 2873 656c 662c 2076 616c 7565 3a20  ve(self, value: 
+000179a0: 696e 7429 202d 3e20 626f 6f6c 3a0a 2020  int) -> bool:.  
+000179b0: 2020 2020 2020 2222 2222 2222 0a20 2020        """""".   
+000179c0: 2064 6566 2073 6872 696e 6b5f 746f 2873   def shrink_to(s
+000179d0: 656c 662c 206d 696e 5f63 6170 6163 6974  elf, min_capacit
+000179e0: 793a 2069 6e74 2920 2d3e 204e 6f6e 653a  y: int) -> None:
+000179f0: 0a20 2020 2020 2020 2022 2222 2222 220a  .        """""".
+00017a00: 2020 2020 6465 6620 7368 7269 6e6b 5f74      def shrink_t
+00017a10: 6f5f 6669 7428 7365 6c66 2920 2d3e 204e  o_fit(self) -> N
+00017a20: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00017a30: 2222 220a 2020 2020 6465 6620 7472 795f  """.    def try_
+00017a40: 7265 7365 7276 6528 7365 6c66 2c20 6164  reserve(self, ad
+00017a50: 6469 7469 6f6e 616c 3a20 696e 7429 202d  ditional: int) -
+00017a60: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00017a70: 2222 2222 2222 0a0a 636c 6173 7320 4d61  """"""..class Ma
+00017a80: 6a6f 7269 7479 436f 6e66 6967 285f 5f41  jorityConfig(__A
+00017a90: 5049 5f4d 616a 6f72 6974 7943 6f6e 6669  PI_MajorityConfi
+00017aa0: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
+00017ab0: 4120 7365 7420 6f66 2049 4473 2074 6861  A set of IDs tha
+00017ac0: 7420 7573 6573 206d 616a 6f72 6974 7920  t uses majority 
+00017ad0: 7175 6f72 756d 7320 746f 206d 616b 6520  quorums to make 
+00017ae0: 6465 6369 7369 6f6e 732e 0a20 2020 2022  decisions..    "
+00017af0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00017b00: 6974 5f5f 2873 656c 662c 2076 6f74 6572  it__(self, voter
+00017b10: 733a 2053 6574 5b69 6e74 5d29 202d 3e20  s: Set[int]) -> 
+00017b20: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+00017b30: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+00017b40: 202d 3e20 224d 616a 6f72 6974 7943 6f6e   -> "MajorityCon
+00017b50: 6669 6752 6566 223a 202e 2e2e 0a0a 636c  figRef": .....cl
+00017b60: 6173 7320 4d61 6a6f 7269 7479 436f 6e66  ass MajorityConf
+00017b70: 6967 5265 6628 5f5f 4150 495f 4d61 6a6f  igRef(__API_Majo
+00017b80: 7269 7479 436f 6e66 6967 293a 0a20 2020  rityConfig):.   
+00017b90: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
+00017ba0: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
+00017bb0: 733a 604d 616a 6f72 6974 7943 6f6e 6669  s:`MajorityConfi
+00017bc0: 6760 2e0a 2020 2020 2222 220a 0a63 6c61  g`..    """..cla
+00017bd0: 7373 205f 5f41 5049 5f49 6e66 6c69 6768  ss __API_Infligh
+00017be0: 7473 285f 5f43 6c6f 6e65 6162 6c65 293a  ts(__Cloneable):
+00017bf0: 0a20 2020 2064 6566 2063 6c6f 6e65 2873  .    def clone(s
+00017c00: 656c 6629 202d 3e20 2249 6e66 6c69 6768  elf) -> "Infligh
+00017c10: 7473 223a 202e 2e2e 0a20 2020 2064 6566  ts": ....    def
+00017c20: 2061 6464 2873 656c 662c 2069 6e66 6c69   add(self, infli
+00017c30: 6768 743a 2069 6e74 2920 2d3e 204e 6f6e  ght: int) -> Non
+00017c40: 653a 0a20 2020 2020 2020 2022 2222 4164  e:.        """Ad
+00017c50: 6473 2061 6e20 696e 666c 6967 6874 2069  ds an inflight i
+00017c60: 6e74 6f20 696e 666c 6967 6874 7322 2222  nto inflights"""
+00017c70: 0a20 2020 2064 6566 2066 756c 6c28 7365  .    def full(se
+00017c80: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00017c90: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
+00017ca0: 7472 7565 2069 6620 7468 6520 696e 666c  true if the infl
+00017cb0: 6967 6874 7320 6973 2066 756c 6c2e 2222  ights is full.""
+00017cc0: 220a 2020 2020 6465 6620 7265 7365 7428  ".    def reset(
+00017cd0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00017ce0: 2020 2020 2020 2022 2222 4672 6565 7320         """Frees 
+00017cf0: 616c 6c20 696e 666c 6967 6874 732e 2222  all inflights.""
+00017d00: 220a 2020 2020 6465 6620 6672 6565 5f74  ".    def free_t
+00017d10: 6f28 7365 6c66 2c20 746f 3a20 696e 7429  o(self, to: int)
+00017d20: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00017d30: 2020 2222 2246 7265 6573 2074 6865 2069    """Frees the i
+00017d40: 6e66 6c69 6768 7473 2073 6d61 6c6c 6572  nflights smaller
+00017d50: 206f 7220 6571 7561 6c20 746f 2074 6865   or equal to the
+00017d60: 2067 6976 656e 2060 746f 6020 666c 6967   given `to` flig
+00017d70: 6874 2e22 2222 0a20 2020 2064 6566 2066  ht.""".    def f
+00017d80: 7265 655f 6669 7273 745f 6f6e 6528 7365  ree_first_one(se
+00017d90: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00017da0: 2020 2020 2022 2222 4672 6565 7320 7468       """Frees th
+00017db0: 6520 6669 7273 7420 6275 6666 6572 2065  e first buffer e
+00017dc0: 6e74 7279 2e22 2222 0a20 2020 2064 6566  ntry.""".    def
+00017dd0: 206d 6179 6265 5f66 7265 655f 6275 6666   maybe_free_buff
+00017de0: 6572 2873 656c 6629 202d 3e20 4e6f 6e65  er(self) -> None
+00017df0: 3a0a 2020 2020 2020 2020 2222 2246 7265  :.        """Fre
+00017e00: 6520 756e 7573 6564 206d 656d 6f72 7922  e unused memory"
+00017e10: 2222 0a20 2020 2064 6566 2062 7566 6665  "".    def buffe
+00017e20: 725f 6361 7061 6369 7479 2873 656c 6629  r_capacity(self)
+00017e30: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00017e40: 2022 2222 4361 7061 6369 7479 206f 6620   """Capacity of 
+00017e50: 7468 6520 696e 7465 726e 616c 2062 7566  the internal buf
+00017e60: 6665 722e 2222 220a 2020 2020 6465 6620  fer.""".    def 
+00017e70: 6275 6666 6572 5f69 735f 616c 6c6f 6361  buffer_is_alloca
+00017e80: 7465 6428 7365 6c66 2920 2d3e 2062 6f6f  ted(self) -> boo
+00017e90: 6c3a 0a20 2020 2020 2020 2022 2222 5768  l:.        """Wh
+00017ea0: 6574 6865 7220 6275 6666 6572 2069 7320  ether buffer is 
+00017eb0: 616c 6c6f 6361 7465 6420 6f72 206e 6f74  allocated or not
+00017ec0: 2e20 4974 2773 2066 6f72 2074 6573 7473  . It's for tests
+00017ed0: 2e22 2222 0a20 2020 2064 6566 2063 6f75  .""".    def cou
+00017ee0: 6e74 2873 656c 6629 202d 3e20 696e 743a  nt(self) -> int:
+00017ef0: 0a20 2020 2020 2020 2022 2222 4e75 6d62  .        """Numb
+00017f00: 6572 206f 6620 696e 666c 6967 6874 206d  er of inflight m
+00017f10: 6573 7361 6765 732e 2049 7427 7320 666f  essages. It's fo
+00017f20: 7220 7465 7374 732e 2222 220a 2020 2020  r tests.""".    
+00017f30: 6465 6620 7365 745f 6361 7028 7365 6c66  def set_cap(self
+00017f40: 2c20 696e 636f 6d69 6e67 5f63 6170 3a20  , incoming_cap: 
+00017f50: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00017f60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00017f70: 2020 4164 6a75 7374 2069 6e66 6c69 6768    Adjust infligh
+00017f80: 7420 6275 6666 6572 2063 6170 6163 6974  t buffer capacit
+00017f90: 792e 2053 6574 2069 7420 746f 2060 3060  y. Set it to `0`
+00017fa0: 2077 696c 6c20 6469 7361 626c 6520 7468   will disable th
+00017fb0: 6520 7072 6f67 7265 7373 2e0a 2020 2020  e progress..    
+00017fc0: 2020 2020 4361 6c6c 696e 6720 6974 2062      Calling it b
+00017fd0: 6574 7765 656e 2060 7365 6c66 2e66 756c  etween `self.ful
+00017fe0: 6c28 2960 2061 6e64 2060 7365 6c66 2e61  l()` and `self.a
+00017ff0: 6464 2829 6020 6361 6e20 6361 7573 6520  dd()` can cause 
+00018000: 6120 7061 6e69 632e 0a20 2020 2020 2020  a panic..       
+00018010: 2022 2222 0a0a 636c 6173 7320 496e 666c   """..class Infl
+00018020: 6967 6874 7328 5f5f 4150 495f 496e 666c  ights(__API_Infl
+00018030: 6967 6874 7329 3a0a 2020 2020 2222 220a  ights):.    """.
+00018040: 2020 2020 4120 6275 6666 6572 206f 6620      A buffer of 
+00018050: 696e 666c 6967 6874 206d 6573 7361 6765  inflight message
+00018060: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
+00018070: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00018080: 662c 2063 6170 3a20 696e 7429 202d 3e20  f, cap: int) -> 
+00018090: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+000180a0: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+000180b0: 202d 3e20 2249 6e66 6c69 6768 7473 5265   -> "InflightsRe
+000180c0: 6622 3a20 2e2e 2e0a 0a63 6c61 7373 2049  f": .....class I
+000180d0: 6e66 6c69 6768 7473 5265 6628 5f5f 4150  nflightsRef(__AP
+000180e0: 495f 496e 666c 6967 6874 7329 3a0a 2020  I_Inflights):.  
+000180f0: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
+00018100: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
+00018110: 7373 3a60 496e 666c 6967 6874 7352 6566  ss:`InflightsRef
+00018120: 602e 0a20 2020 2022 2222 0a0a 636c 6173  `..    """..clas
+00018130: 7320 5f5f 4150 495f 436f 6e66 6967 285f  s __API_Config(_
+00018140: 5f43 6c6f 6e65 6162 6c65 293a 0a20 2020  _Cloneable):.   
+00018150: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
+00018160: 202d 3e20 2243 6f6e 6669 6722 3a20 2e2e   -> "Config": ..
+00018170: 2e0a 2020 2020 6465 6620 6d69 6e5f 656c  ..    def min_el
+00018180: 6563 7469 6f6e 5f74 6963 6b28 7365 6c66  ection_tick(self
+00018190: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+000181a0: 2020 2222 220a 2020 2020 2020 2020 606d    """.        `m
+000181b0: 696e 5f65 6c65 6374 696f 6e5f 7469 636b  in_election_tick
+000181c0: 603a 2054 6865 206d 696e 696d 756d 206e  `: The minimum n
+000181d0: 756d 6265 7220 6f66 2074 6963 6b73 2062  umber of ticks b
+000181e0: 6566 6f72 6520 616e 2065 6c65 6374 696f  efore an electio
+000181f0: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
+00018200: 2020 2064 6566 2073 6574 5f6d 696e 5f65     def set_min_e
+00018210: 6c65 6374 696f 6e5f 7469 636b 2873 656c  lection_tick(sel
+00018220: 662c 206d 696e 5f65 6c65 6374 696f 6e5f  f, min_election_
+00018230: 7469 636b 3a20 696e 7429 202d 3e20 4e6f  tick: int) -> No
+00018240: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00018250: 2020 2020 2020 2020 606d 696e 5f65 6c65          `min_ele
+00018260: 6374 696f 6e5f 7469 636b 603a 2054 6865  ction_tick`: The
+00018270: 206d 696e 696d 756d 206e 756d 6265 7220   minimum number 
+00018280: 6f66 2074 6963 6b73 2062 6566 6f72 6520  of ticks before 
+00018290: 616e 2065 6c65 6374 696f 6e2e 0a20 2020  an election..   
+000182a0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+000182b0: 206d 6178 5f65 6c65 6374 696f 6e5f 7469   max_election_ti
+000182c0: 636b 2873 656c 6629 202d 3e20 696e 743a  ck(self) -> int:
+000182d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000182e0: 2020 2020 2060 6d61 785f 656c 6563 7469       `max_electi
+000182f0: 6f6e 5f74 6963 6b60 3a20 5468 6520 6d61  on_tick`: The ma
+00018300: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
+00018310: 7469 636b 7320 6265 666f 7265 2061 6e20  ticks before an 
+00018320: 656c 6563 7469 6f6e 2e0a 2020 2020 2020  election..      
+00018330: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00018340: 745f 6d61 785f 656c 6563 7469 6f6e 5f74  t_max_election_t
+00018350: 6963 6b28 7365 6c66 2c20 6d61 785f 656c  ick(self, max_el
+00018360: 6563 7469 6f6e 5f74 6963 6b3a 2069 6e74  ection_tick: int
+00018370: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00018380: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00018390: 6d61 785f 656c 6563 7469 6f6e 5f74 6963  max_election_tic
+000183a0: 6b60 3a20 5468 6520 6d61 7869 6d75 6d20  k`: The maximum 
+000183b0: 6e75 6d62 6572 206f 6620 7469 636b 7320  number of ticks 
+000183c0: 6265 666f 7265 2061 6e20 656c 6563 7469  before an electi
+000183d0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
+000183e0: 2020 2020 6465 6620 6765 745f 7265 6164      def get_read
+000183f0: 5f6f 6e6c 795f 6f70 7469 6f6e 2873 656c  _only_option(sel
+00018400: 6629 202d 3e20 2252 6561 644f 6e6c 794f  f) -> "ReadOnlyO
+00018410: 7074 696f 6e22 3a0a 2020 2020 2020 2020  ption":.        
+00018420: 2222 220a 2020 2020 2020 2020 6072 6561  """.        `rea
+00018430: 645f 6f6e 6c79 5f6f 7074 696f 6e60 3a20  d_only_option`: 
+00018440: 4368 6f6f 7365 2074 6865 206c 696e 6561  Choose the linea
+00018450: 7269 7a61 6269 6c69 7479 206d 6f64 6520  rizability mode 
+00018460: 6f72 2074 6865 206c 6561 7365 206d 6f64  or the lease mod
+00018470: 6520 746f 2072 6561 6420 6461 7461 2e20  e to read data. 
+00018480: 4966 2079 6f75 2064 6f6e e280 9974 2063  If you don...t c
+00018490: 6172 6520 6162 6f75 7420 7468 6520 7265  are about the re
+000184a0: 6164 2063 6f6e 7369 7374 656e 6379 2061  ad consistency a
+000184b0: 6e64 2077 616e 7420 6120 6869 6768 6572  nd want a higher
+000184c0: 2072 6561 6420 7065 7266 6f72 6d61 6e63   read performanc
+000184d0: 652c 2079 6f75 2063 616e 2075 7365 2074  e, you can use t
+000184e0: 6865 206c 6561 7365 206d 6f64 652e 0a20  he lease mode.. 
+000184f0: 2020 2020 2020 2053 6574 7469 6e67 2074         Setting t
+00018500: 6869 7320 746f 2060 4c65 6173 6542 6173  his to `LeaseBas
+00018510: 6564 6020 7265 7175 6972 6573 2060 6368  ed` requires `ch
+00018520: 6563 6b5f 7175 6f72 756d 203d 2074 7275  eck_quorum = tru
+00018530: 6560 2e0a 2020 2020 2020 2020 2222 220a  e`..        """.
+00018540: 2020 2020 6465 6620 7365 745f 7265 6164      def set_read
+00018550: 5f6f 6e6c 795f 6f70 7469 6f6e 2873 656c  _only_option(sel
+00018560: 662c 2072 6561 645f 6f6e 6c79 5f6f 7074  f, read_only_opt
+00018570: 696f 6e3a 2022 5265 6164 4f6e 6c79 4f70  ion: "ReadOnlyOp
+00018580: 7469 6f6e 2229 202d 3e20 4e6f 6e65 3a0a  tion") -> None:.
+00018590: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000185a0: 2020 2020 6072 6561 645f 6f6e 6c79 5f6f      `read_only_o
+000185b0: 7074 696f 6e60 3a20 4368 6f6f 7365 2074  ption`: Choose t
+000185c0: 6865 206c 696e 6561 7269 7a61 6269 6c69  he linearizabili
+000185d0: 7479 206d 6f64 6520 6f72 2074 6865 206c  ty mode or the l
+000185e0: 6561 7365 206d 6f64 6520 746f 2072 6561  ease mode to rea
+000185f0: 6420 6461 7461 2e20 4966 2079 6f75 2064  d data. If you d
+00018600: 6f6e e280 9974 2063 6172 6520 6162 6f75  on...t care abou
+00018610: 7420 7468 6520 7265 6164 2063 6f6e 7369  t the read consi
+00018620: 7374 656e 6379 2061 6e64 2077 616e 7420  stency and want 
+00018630: 6120 6869 6768 6572 2072 6561 6420 7065  a higher read pe
+00018640: 7266 6f72 6d61 6e63 652c 2079 6f75 2063  rformance, you c
+00018650: 616e 2075 7365 2074 6865 206c 6561 7365  an use the lease
+00018660: 206d 6f64 652e 0a20 2020 2020 2020 2053   mode..        S
+00018670: 6574 7469 6e67 2074 6869 7320 746f 2060  etting this to `
+00018680: 4c65 6173 6542 6173 6564 6020 7265 7175  LeaseBased` requ
+00018690: 6972 6573 2060 6368 6563 6b5f 7175 6f72  ires `check_quor
+000186a0: 756d 203d 2074 7275 6560 2e0a 2020 2020  um = true`..    
+000186b0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+000186c0: 6765 745f 6964 2873 656c 6629 202d 3e20  get_id(self) -> 
+000186d0: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+000186e0: 0a20 2020 2020 2020 2060 6964 603a 2054  .        `id`: T
+000186f0: 6865 2069 6465 6e74 6974 7920 6f66 2074  he identity of t
+00018700: 6865 206c 6f63 616c 2072 6166 742e 2049  he local raft. I
+00018710: 7420 6361 6e6e 6f74 2062 6520 302c 2061  t cannot be 0, a
+00018720: 6e64 206d 7573 7420 6265 2075 6e69 7175  nd must be uniqu
+00018730: 6520 696e 2074 6865 2067 726f 7570 2e0a  e in the group..
+00018740: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00018750: 6465 6620 7365 745f 6964 2873 656c 662c  def set_id(self,
+00018760: 2069 643a 2069 6e74 2920 2d3e 204e 6f6e   id: int) -> Non
+00018770: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00018780: 2020 2020 2020 2060 6964 603a 2054 6865         `id`: The
+00018790: 2069 6465 6e74 6974 7920 6f66 2074 6865   identity of the
+000187a0: 206c 6f63 616c 2072 6166 742e 2049 7420   local raft. It 
+000187b0: 6361 6e6e 6f74 2062 6520 302c 2061 6e64  cannot be 0, and
+000187c0: 206d 7573 7420 6265 2075 6e69 7175 6520   must be unique 
+000187d0: 696e 2074 6865 2067 726f 7570 2e0a 2020  in the group..  
+000187e0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+000187f0: 6620 6765 745f 656c 6563 7469 6f6e 5f74  f get_election_t
+00018800: 6963 6b28 7365 6c66 2920 2d3e 2069 6e74  ick(self) -> int
+00018810: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00018820: 2020 2020 2020 6065 6c65 6374 696f 6e5f        `election_
+00018830: 7469 636b 603a 2054 6865 206e 756d 6265  tick`: The numbe
+00018840: 7220 6f66 206e 6f64 652e 7469 636b 2069  r of node.tick i
+00018850: 6e76 6f63 6174 696f 6e73 2074 6861 7420  nvocations that 
+00018860: 6d75 7374 2070 6173 7320 6265 7477 6565  must pass betwee
+00018870: 6e0a 2020 2020 2020 2020 656c 6563 7469  n.        electi
+00018880: 6f6e 732e 2054 6861 7420 6973 2c20 6966  ons. That is, if
+00018890: 2061 2066 6f6c 6c6f 7765 7220 646f 6573   a follower does
+000188a0: 206e 6f74 2072 6563 6569 7665 2061 6e79   not receive any
+000188b0: 206d 6573 7361 6765 2066 726f 6d20 7468   message from th
+000188c0: 650a 2020 2020 2020 2020 6c65 6164 6572  e.        leader
+000188d0: 206f 6620 6375 7272 656e 7420 7465 726d   of current term
+000188e0: 2062 6566 6f72 6520 456c 6563 7469 6f6e   before Election
+000188f0: 5469 636b 2068 6173 2065 6c61 7073 6564  Tick has elapsed
+00018900: 2c20 6974 2077 696c 6c20 6265 636f 6d65  , it will become
+00018910: 0a20 2020 2020 2020 2063 616e 6469 6461  .        candida
+00018920: 7465 2061 6e64 2073 7461 7274 2061 6e20  te and start an 
+00018930: 656c 6563 7469 6f6e 2e20 656c 6563 7469  election. electi
+00018940: 6f6e 5f74 6963 6b20 6d75 7374 2062 6520  on_tick must be 
+00018950: 6772 6561 7465 7220 7468 616e 0a20 2020  greater than.   
+00018960: 2020 2020 2048 6561 7274 6265 6174 5469       HeartbeatTi
+00018970: 636b 2e20 5765 2073 7567 6765 7374 2065  ck. We suggest e
+00018980: 6c65 6374 696f 6e5f 7469 636b 203d 2031  lection_tick = 1
+00018990: 3020 2a20 4865 6172 7462 6561 7454 6963  0 * HeartbeatTic
+000189a0: 6b20 746f 2061 766f 6964 0a20 2020 2020  k to avoid.     
+000189b0: 2020 2075 6e6e 6563 6573 7361 7279 206c     unnecessary l
+000189c0: 6561 6465 7220 7377 6974 6368 696e 670a  eader switching.
+000189d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000189e0: 6465 6620 7365 745f 656c 6563 7469 6f6e  def set_election
+000189f0: 5f74 6963 6b28 7365 6c66 2c20 656c 6563  _tick(self, elec
+00018a00: 7469 6f6e 5f74 6963 6b3a 2069 6e74 2920  tion_tick: int) 
+00018a10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00018a20: 2022 2222 0a20 2020 2020 2020 2060 656c   """.        `el
+00018a30: 6563 7469 6f6e 5f74 6963 6b60 3a20 5468  ection_tick`: Th
+00018a40: 6520 6e75 6d62 6572 206f 6620 6e6f 6465  e number of node
+00018a50: 2e74 6963 6b20 696e 766f 6361 7469 6f6e  .tick invocation
+00018a60: 7320 7468 6174 206d 7573 7420 7061 7373  s that must pass
+00018a70: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
+00018a80: 2065 6c65 6374 696f 6e73 2e20 5468 6174   elections. That
+00018a90: 2069 732c 2069 6620 6120 666f 6c6c 6f77   is, if a follow
+00018aa0: 6572 2064 6f65 7320 6e6f 7420 7265 6365  er does not rece
+00018ab0: 6976 6520 616e 7920 6d65 7373 6167 6520  ive any message 
+00018ac0: 6672 6f6d 2074 6865 0a20 2020 2020 2020  from the.       
+00018ad0: 206c 6561 6465 7220 6f66 2063 7572 7265   leader of curre
+00018ae0: 6e74 2074 6572 6d20 6265 666f 7265 2045  nt term before E
+00018af0: 6c65 6374 696f 6e54 6963 6b20 6861 7320  lectionTick has 
+00018b00: 656c 6170 7365 642c 2069 7420 7769 6c6c  elapsed, it will
+00018b10: 2062 6563 6f6d 650a 2020 2020 2020 2020   become.        
+00018b20: 6361 6e64 6964 6174 6520 616e 6420 7374  candidate and st
+00018b30: 6172 7420 616e 2065 6c65 6374 696f 6e2e  art an election.
+00018b40: 2065 6c65 6374 696f 6e5f 7469 636b 206d   election_tick m
+00018b50: 7573 7420 6265 2067 7265 6174 6572 2074  ust be greater t
+00018b60: 6861 6e0a 2020 2020 2020 2020 4865 6172  han.        Hear
+00018b70: 7462 6561 7454 6963 6b2e 2057 6520 7375  tbeatTick. We su
+00018b80: 6767 6573 7420 656c 6563 7469 6f6e 5f74  ggest election_t
+00018b90: 6963 6b20 3d20 3130 202a 2048 6561 7274  ick = 10 * Heart
+00018ba0: 6265 6174 5469 636b 2074 6f20 6176 6f69  beatTick to avoi
+00018bb0: 640a 2020 2020 2020 2020 756e 6e65 6365  d.        unnece
+00018bc0: 7373 6172 7920 6c65 6164 6572 2073 7769  ssary leader swi
+00018bd0: 7463 6869 6e67 0a20 2020 2020 2020 2022  tching.        "
+00018be0: 2222 0a20 2020 2064 6566 2067 6574 5f68  "".    def get_h
+00018bf0: 6561 7274 6265 6174 5f74 6963 6b28 7365  eartbeat_tick(se
+00018c00: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00018c10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00018c20: 6068 6561 7274 6265 6174 5f74 6963 6b60  `heartbeat_tick`
+00018c30: 3a20 4865 6172 7462 6561 7454 6963 6b20  : HeartbeatTick 
+00018c40: 6973 2074 6865 206e 756d 6265 7220 6f66  is the number of
+00018c50: 206e 6f64 652e 7469 636b 2069 6e76 6f63   node.tick invoc
+00018c60: 6174 696f 6e73 2074 6861 7420 6d75 7374  ations that must
+00018c70: 2070 6173 7320 6265 7477 6565 6e0a 2020   pass between.  
+00018c80: 2020 2020 2020 6865 6172 7462 6561 7473        heartbeats
+00018c90: 2e20 5468 6174 2069 732c 2061 206c 6561  . That is, a lea
+00018ca0: 6465 7220 7365 6e64 7320 6865 6172 7462  der sends heartb
+00018cb0: 6561 7420 6d65 7373 6167 6573 2074 6f20  eat messages to 
+00018cc0: 6d61 696e 7461 696e 2069 7473 0a20 2020  maintain its.   
+00018cd0: 2020 2020 206c 6561 6465 7273 6869 7020       leadership 
+00018ce0: 6576 6572 7920 6865 6172 7462 6561 7420  every heartbeat 
+00018cf0: 7469 636b 732e 0a20 2020 2020 2020 2022  ticks..        "
+00018d00: 2222 0a20 2020 2064 6566 2073 6574 5f68  "".    def set_h
+00018d10: 6561 7274 6265 6174 5f74 6963 6b28 7365  eartbeat_tick(se
+00018d20: 6c66 2c20 6865 6172 7462 6561 745f 7469  lf, heartbeat_ti
+00018d30: 636b 3a20 696e 7429 202d 3e20 4e6f 6e65  ck: int) -> None
+00018d40: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00018d50: 2020 2020 2020 6068 6561 7274 6265 6174        `heartbeat
+00018d60: 5f74 6963 6b60 3a20 4865 6172 7462 6561  _tick`: Heartbea
+00018d70: 7454 6963 6b20 6973 2074 6865 206e 756d  tTick is the num
+00018d80: 6265 7220 6f66 206e 6f64 652e 7469 636b  ber of node.tick
+00018d90: 2069 6e76 6f63 6174 696f 6e73 2074 6861   invocations tha
+00018da0: 7420 6d75 7374 2070 6173 7320 6265 7477  t must pass betw
+00018db0: 6565 6e0a 2020 2020 2020 2020 6865 6172  een.        hear
+00018dc0: 7462 6561 7473 2e20 5468 6174 2069 732c  tbeats. That is,
+00018dd0: 2061 206c 6561 6465 7220 7365 6e64 7320   a leader sends 
+00018de0: 6865 6172 7462 6561 7420 6d65 7373 6167  heartbeat messag
+00018df0: 6573 2074 6f20 6d61 696e 7461 696e 2069  es to maintain i
+00018e00: 7473 0a20 2020 2020 2020 206c 6561 6465  ts.        leade
+00018e10: 7273 6869 7020 6576 6572 7920 6865 6172  rship every hear
+00018e20: 7462 6561 7420 7469 636b 732e 0a20 2020  tbeat ticks..   
+00018e30: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00018e40: 2067 6574 5f6d 6178 5f73 697a 655f 7065   get_max_size_pe
+00018e50: 725f 6d73 6728 7365 6c66 2920 2d3e 2069  r_msg(self) -> i
+00018e60: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+00018e70: 2020 2020 2020 2020 606d 6178 5f73 697a          `max_siz
+00018e80: 655f 7065 725f 6d73 6760 3a20 4c69 6d69  e_per_msg`: Limi
+00018e90: 7420 7468 6520 6d61 7820 7369 7a65 206f  t the max size o
+00018ea0: 6620 6561 6368 2061 7070 656e 6420 6d65  f each append me
+00018eb0: 7373 6167 652e 2053 6d61 6c6c 6572 2076  ssage. Smaller v
+00018ec0: 616c 7565 206c 6f77 6572 730a 2020 2020  alue lowers.    
+00018ed0: 2020 2020 7468 6520 7261 6674 2072 6563      the raft rec
+00018ee0: 6f76 6572 7920 636f 7374 2869 6e69 7469  overy cost(initi
+00018ef0: 616c 2070 726f 6269 6e67 2061 6e64 206d  al probing and m
+00018f00: 6573 7361 6765 206c 6f73 7420 6475 7269  essage lost duri
+00018f10: 6e67 206e 6f72 6d61 6c20 6f70 6572 6174  ng normal operat
+00018f20: 696f 6e29 2e0a 2020 2020 2020 2020 4f6e  ion)..        On
+00018f30: 2074 6865 206f 7468 6572 2073 6964 652c   the other side,
+00018f40: 2069 7420 6d69 6768 7420 6166 6665 6374   it might affect
+00018f50: 2074 6865 2074 6872 6f75 6768 7075 7420   the throughput 
+00018f60: 6475 7269 6e67 206e 6f72 6d61 6c20 7265  during normal re
+00018f70: 706c 6963 6174 696f 6e2e 0a20 2020 2020  plication..     
+00018f80: 2020 204e 6f74 653a 206d 6174 682e 4d61     Note: math.Ma
+00018f90: 7855 7573 697a 6536 3420 666f 7220 756e  xUusize64 for un
+00018fa0: 6c69 6d69 7465 642c 2030 2066 6f72 2061  limited, 0 for a
+00018fb0: 7420 6d6f 7374 206f 6e65 2065 6e74 7279  t most one entry
+00018fc0: 2070 6572 206d 6573 7361 6765 2e0a 2020   per message..  
+00018fd0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00018fe0: 6620 7365 745f 6d61 785f 7369 7a65 5f70  f set_max_size_p
+00018ff0: 6572 5f6d 7367 2873 656c 662c 206d 6178  er_msg(self, max
+00019000: 5f73 697a 655f 7065 725f 6d73 673a 2069  _size_per_msg: i
+00019010: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00019020: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00019030: 2060 6d61 785f 7369 7a65 5f70 6572 5f6d   `max_size_per_m
+00019040: 7367 603a 204c 696d 6974 2074 6865 206d  sg`: Limit the m
+00019050: 6178 2073 697a 6520 6f66 2065 6163 6820  ax size of each 
+00019060: 6170 7065 6e64 206d 6573 7361 6765 2e20  append message. 
+00019070: 536d 616c 6c65 7220 7661 6c75 6520 6c6f  Smaller value lo
+00019080: 7765 7273 0a20 2020 2020 2020 2074 6865  wers.        the
+00019090: 2072 6166 7420 7265 636f 7665 7279 2063   raft recovery c
+000190a0: 6f73 7428 696e 6974 6961 6c20 7072 6f62  ost(initial prob
+000190b0: 696e 6720 616e 6420 6d65 7373 6167 6520  ing and message 
+000190c0: 6c6f 7374 2064 7572 696e 6720 6e6f 726d  lost during norm
+000190d0: 616c 206f 7065 7261 7469 6f6e 292e 0a20  al operation).. 
+000190e0: 2020 2020 2020 204f 6e20 7468 6520 6f74         On the ot
+000190f0: 6865 7220 7369 6465 2c20 6974 206d 6967  her side, it mig
+00019100: 6874 2061 6666 6563 7420 7468 6520 7468  ht affect the th
+00019110: 726f 7567 6870 7574 2064 7572 696e 6720  roughput during 
+00019120: 6e6f 726d 616c 2072 6570 6c69 6361 7469  normal replicati
+00019130: 6f6e 2e0a 2020 2020 2020 2020 4e6f 7465  on..        Note
+00019140: 3a20 6d61 7468 2e4d 6178 5575 7369 7a65  : math.MaxUusize
+00019150: 3634 2066 6f72 2075 6e6c 696d 6974 6564  64 for unlimited
+00019160: 2c20 3020 666f 7220 6174 206d 6f73 7420  , 0 for at most 
+00019170: 6f6e 6520 656e 7472 7920 7065 7220 6d65  one entry per me
+00019180: 7373 6167 652e 0a20 2020 2020 2020 2022  ssage..        "
+00019190: 2222 0a20 2020 2064 6566 2067 6574 5f6d  "".    def get_m
+000191a0: 6178 5f69 6e66 6c69 6768 745f 6d73 6773  ax_inflight_msgs
+000191b0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+000191c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000191d0: 2020 2060 6d61 785f 696e 666c 6967 6874     `max_inflight
+000191e0: 5f6d 7367 7360 3a20 4c69 6d69 7420 7468  _msgs`: Limit th
+000191f0: 6520 6d61 7820 6e75 6d62 6572 206f 6620  e max number of 
+00019200: 696e 2d66 6c69 6768 7420 6170 7065 6e64  in-flight append
+00019210: 206d 6573 7361 6765 7320 6475 7269 6e67   messages during
+00019220: 206f 7074 696d 6973 7469 630a 2020 2020   optimistic.    
+00019230: 2020 2020 7265 706c 6963 6174 696f 6e20      replication 
+00019240: 7068 6173 652e 2054 6865 2061 7070 6c69  phase. The appli
+00019250: 6361 7469 6f6e 2074 7261 6e73 706f 7274  cation transport
+00019260: 6174 696f 6e20 6c61 7965 7220 7573 7561  ation layer usua
+00019270: 6c6c 7920 6861 7320 6974 7320 6f77 6e20  lly has its own 
+00019280: 7365 6e64 696e 670a 2020 2020 2020 2020  sending.        
+00019290: 6275 6666 6572 206f 7665 7220 5443 502f  buffer over TCP/
+000192a0: 5544 502e 2053 6574 2074 6f20 6176 6f69  UDP. Set to avoi
+000192b0: 6420 6f76 6572 666c 6f77 696e 6720 7468  d overflowing th
+000192c0: 6174 2073 656e 6469 6e67 2062 7566 6665  at sending buffe
+000192d0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+000192e0: 2020 2064 6566 2073 6574 5f6d 6178 5f69     def set_max_i
+000192f0: 6e66 6c69 6768 745f 6d73 6773 2873 656c  nflight_msgs(sel
+00019300: 662c 206d 6178 5f69 6e66 6c69 6768 745f  f, max_inflight_
+00019310: 6d73 6773 3a20 696e 7429 202d 3e20 4e6f  msgs: int) -> No
+00019320: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00019330: 2020 2020 2020 2020 606d 6178 5f69 6e66          `max_inf
+00019340: 6c69 6768 745f 6d73 6773 603a 204c 696d  light_msgs`: Lim
+00019350: 6974 2074 6865 206d 6178 206e 756d 6265  it the max numbe
+00019360: 7220 6f66 2069 6e2d 666c 6967 6874 2061  r of in-flight a
+00019370: 7070 656e 6420 6d65 7373 6167 6573 2064  ppend messages d
+00019380: 7572 696e 6720 6f70 7469 6d69 7374 6963  uring optimistic
+00019390: 0a20 2020 2020 2020 2072 6570 6c69 6361  .        replica
+000193a0: 7469 6f6e 2070 6861 7365 2e20 5468 6520  tion phase. The 
+000193b0: 6170 706c 6963 6174 696f 6e20 7472 616e  application tran
+000193c0: 7370 6f72 7461 7469 6f6e 206c 6179 6572  sportation layer
+000193d0: 2075 7375 616c 6c79 2068 6173 2069 7473   usually has its
+000193e0: 206f 776e 2073 656e 6469 6e67 0a20 2020   own sending.   
+000193f0: 2020 2020 2062 7566 6665 7220 6f76 6572       buffer over
+00019400: 2054 4350 2f55 4450 2e20 5365 7420 746f   TCP/UDP. Set to
+00019410: 2061 766f 6964 206f 7665 7266 6c6f 7769   avoid overflowi
+00019420: 6e67 2074 6861 7420 7365 6e64 696e 6720  ng that sending 
+00019430: 6275 6666 6572 2e0a 2020 2020 2020 2020  buffer..        
+00019440: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00019450: 6170 706c 6965 6428 7365 6c66 2920 2d3e  applied(self) ->
+00019460: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00019470: 220a 2020 2020 2020 2020 6061 7070 6c69  ".        `appli
+00019480: 6564 603a 2041 7070 6c69 6564 2069 7320  ed`: Applied is 
+00019490: 7468 6520 6c61 7374 2061 7070 6c69 6564  the last applied
+000194a0: 2069 6e64 6578 2e20 4974 2073 686f 756c   index. It shoul
+000194b0: 6420 6f6e 6c79 2062 6520 7365 7420 7768  d only be set wh
+000194c0: 656e 2072 6573 7461 7274 696e 670a 2020  en restarting.  
+000194d0: 2020 2020 2020 7261 6674 2e20 7261 6674        raft. raft
+000194e0: 2077 696c 6c20 6e6f 7420 7265 7475 726e   will not return
+000194f0: 2065 6e74 7269 6573 2074 6f20 7468 6520   entries to the 
+00019500: 6170 706c 6963 6174 696f 6e20 736d 616c  application smal
+00019510: 6c65 7220 6f72 2065 7175 616c 2074 6f20  ler or equal to 
+00019520: 4170 706c 6965 642e 0a20 2020 2020 2020  Applied..       
+00019530: 2049 6620 4170 706c 6965 6420 6973 2075   If Applied is u
+00019540: 6e73 6574 2077 6865 6e20 7265 7374 6172  nset when restar
+00019550: 7469 6e67 2c20 7261 6674 206d 6967 6874  ting, raft might
+00019560: 2072 6574 7572 6e20 7072 6576 696f 7573   return previous
+00019570: 2061 7070 6c69 6564 2065 6e74 7269 6573   applied entries
+00019580: 2e0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+00019590: 7320 6120 7665 7279 2061 7070 6c69 6361  s a very applica
+000195a0: 7469 6f6e 2064 6570 656e 6465 6e74 2063  tion dependent c
+000195b0: 6f6e 6669 6775 7261 7469 6f6e 2e0a 2020  onfiguration..  
+000195c0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+000195d0: 6620 7365 745f 6170 706c 6965 6428 7365  f set_applied(se
+000195e0: 6c66 2c20 6170 706c 6965 643a 2069 6e74  lf, applied: int
+000195f0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00019600: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00019610: 6170 706c 6965 6460 3a20 4170 706c 6965  applied`: Applie
+00019620: 6420 6973 2074 6865 206c 6173 7420 6170  d is the last ap
+00019630: 706c 6965 6420 696e 6465 782e 2049 7420  plied index. It 
+00019640: 7368 6f75 6c64 206f 6e6c 7920 6265 2073  should only be s
+00019650: 6574 2077 6865 6e20 7265 7374 6172 7469  et when restarti
+00019660: 6e67 0a20 2020 2020 2020 2072 6166 742e  ng.        raft.
+00019670: 2072 6166 7420 7769 6c6c 206e 6f74 2072   raft will not r
+00019680: 6574 7572 6e20 656e 7472 6965 7320 746f  eturn entries to
+00019690: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+000196a0: 2073 6d61 6c6c 6572 206f 7220 6571 7561   smaller or equa
+000196b0: 6c20 746f 2041 7070 6c69 6564 2e0a 2020  l to Applied..  
+000196c0: 2020 2020 2020 4966 2041 7070 6c69 6564        If Applied
+000196d0: 2069 7320 756e 7365 7420 7768 656e 2072   is unset when r
+000196e0: 6573 7461 7274 696e 672c 2072 6166 7420  estarting, raft 
+000196f0: 6d69 6768 7420 7265 7475 726e 2070 7265  might return pre
+00019700: 7669 6f75 7320 6170 706c 6965 6420 656e  vious applied en
+00019710: 7472 6965 732e 0a20 2020 2020 2020 2054  tries..        T
+00019720: 6869 7320 6973 2061 2076 6572 7920 6170  his is a very ap
+00019730: 706c 6963 6174 696f 6e20 6465 7065 6e64  plication depend
+00019740: 656e 7420 636f 6e66 6967 7572 6174 696f  ent configuratio
+00019750: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
+00019760: 2020 2064 6566 2067 6574 5f63 6865 636b     def get_check
+00019770: 5f71 756f 7275 6d28 7365 6c66 2920 2d3e  _quorum(self) ->
+00019780: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00019790: 2222 0a20 2020 2020 2020 2060 6368 6563  "".        `chec
+000197a0: 6b5f 7175 6f72 756d 603a 2053 7065 6369  k_quorum`: Speci
+000197b0: 6679 2069 6620 7468 6520 6c65 6164 6572  fy if the leader
+000197c0: 2073 686f 756c 6420 6368 6563 6b20 7175   should check qu
+000197d0: 6f72 756d 2061 6374 6976 6974 792e 204c  orum activity. L
+000197e0: 6561 6465 7220 7374 6570 7320 646f 776e  eader steps down
+000197f0: 2077 6865 6e0a 2020 2020 2020 2020 7175   when.        qu
+00019800: 6f72 756d 2069 7320 6e6f 7420 6163 7469  orum is not acti
+00019810: 7665 2066 6f72 2061 6e20 656c 6563 7469  ve for an electi
+00019820: 6f6e 5469 6d65 6f75 742e 0a20 2020 2020  onTimeout..     
+00019830: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
+00019840: 6574 5f63 6865 636b 5f71 756f 7275 6d28  et_check_quorum(
+00019850: 7365 6c66 2c20 6368 6563 6b5f 7175 6f72  self, check_quor
+00019860: 756d 3a20 626f 6f6c 2920 2d3e 204e 6f6e  um: bool) -> Non
+00019870: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00019880: 2020 2020 2020 2060 6368 6563 6b5f 7175         `check_qu
+00019890: 6f72 756d 603a 2053 7065 6369 6679 2069  orum`: Specify i
+000198a0: 6620 7468 6520 6c65 6164 6572 2073 686f  f the leader sho
+000198b0: 756c 6420 6368 6563 6b20 7175 6f72 756d  uld check quorum
+000198c0: 2061 6374 6976 6974 792e 204c 6561 6465   activity. Leade
+000198d0: 7220 7374 6570 7320 646f 776e 2077 6865  r steps down whe
+000198e0: 6e0a 2020 2020 2020 2020 7175 6f72 756d  n.        quorum
+000198f0: 2069 7320 6e6f 7420 6163 7469 7665 2066   is not active f
+00019900: 6f72 2061 6e20 656c 6563 7469 6f6e 5469  or an electionTi
+00019910: 6d65 6f75 742e 0a20 2020 2020 2020 2022  meout..        "
+00019920: 2222 0a20 2020 2064 6566 2067 6574 5f70  "".    def get_p
+00019930: 7265 5f76 6f74 6528 7365 6c66 2920 2d3e  re_vote(self) ->
+00019940: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00019950: 2222 0a20 2020 2020 2020 2060 7072 655f  "".        `pre_
+00019960: 766f 7465 603a 2045 6e61 626c 6573 2074  vote`: Enables t
+00019970: 6865 2050 7265 2d56 6f74 6520 616c 676f  he Pre-Vote algo
+00019980: 7269 7468 6d20 6465 7363 7269 6265 6420  rithm described 
+00019990: 696e 2072 6166 7420 7468 6573 6973 2073  in raft thesis s
+000199a0: 6563 7469 6f6e 0a20 2020 2020 2020 2039  ection.        9
+000199b0: 2e36 2e20 5468 6973 2070 7265 7665 6e74  .6. This prevent
+000199c0: 7320 6469 7372 7570 7469 6f6e 2077 6865  s disruption whe
+000199d0: 6e20 6120 6e6f 6465 2074 6861 7420 6861  n a node that ha
+000199e0: 7320 6265 656e 2070 6172 7469 7469 6f6e  s been partition
+000199f0: 6564 2061 7761 790a 2020 2020 2020 2020  ed away.        
+00019a00: 7265 6a6f 696e 7320 7468 6520 636c 7573  rejoins the clus
+00019a10: 7465 722e 0a20 2020 2020 2020 2022 2222  ter..        """
+00019a20: 0a20 2020 2064 6566 2073 6574 5f70 7265  .    def set_pre
+00019a30: 5f76 6f74 6528 7365 6c66 2c20 7072 655f  _vote(self, pre_
+00019a40: 766f 7465 3a20 626f 6f6c 2920 2d3e 204e  vote: bool) -> N
+00019a50: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00019a60: 0a20 2020 2020 2020 2060 7072 655f 766f  .        `pre_vo
+00019a70: 7465 603a 2045 6e61 626c 6573 2074 6865  te`: Enables the
+00019a80: 2050 7265 2d56 6f74 6520 616c 676f 7269   Pre-Vote algori
+00019a90: 7468 6d20 6465 7363 7269 6265 6420 696e  thm described in
+00019aa0: 2072 6166 7420 7468 6573 6973 2073 6563   raft thesis sec
+00019ab0: 7469 6f6e 0a20 2020 2020 2020 2039 2e36  tion.        9.6
+00019ac0: 2e20 5468 6973 2070 7265 7665 6e74 7320  . This prevents 
+00019ad0: 6469 7372 7570 7469 6f6e 2077 6865 6e20  disruption when 
+00019ae0: 6120 6e6f 6465 2074 6861 7420 6861 7320  a node that has 
+00019af0: 6265 656e 2070 6172 7469 7469 6f6e 6564  been partitioned
+00019b00: 2061 7761 790a 2020 2020 2020 2020 7265   away.        re
+00019b10: 6a6f 696e 7320 7468 6520 636c 7573 7465  joins the cluste
+00019b20: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+00019b30: 2020 2064 6566 2067 6574 5f62 6174 6368     def get_batch
+00019b40: 5f61 7070 656e 6428 7365 6c66 2920 2d3e  _append(self) ->
+00019b50: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00019b60: 2222 0a20 2020 2020 2020 2060 6261 7463  "".        `batc
+00019b70: 685f 6170 7065 6e64 603a 2042 6174 6368  h_append`: Batch
+00019b80: 6573 2065 7665 7279 2061 7070 656e 6420  es every append 
+00019b90: 6d73 6720 6966 2061 6e79 2061 7070 656e  msg if any appen
+00019ba0: 6420 6d73 6720 616c 7265 6164 7920 6578  d msg already ex
+00019bb0: 6973 7473 0a20 2020 2020 2020 2022 2222  ists.        """
+00019bc0: 0a20 2020 2064 6566 2073 6574 5f62 6174  .    def set_bat
+00019bd0: 6368 5f61 7070 656e 6428 7365 6c66 2c20  ch_append(self, 
+00019be0: 6261 7463 685f 6170 7065 6e64 3a20 626f  batch_append: bo
+00019bf0: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
+00019c00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00019c10: 2060 6261 7463 685f 6170 7065 6e64 603a   `batch_append`:
+00019c20: 2042 6174 6368 6573 2065 7665 7279 2061   Batches every a
+00019c30: 7070 656e 6420 6d73 6720 6966 2061 6e79  ppend msg if any
+00019c40: 2061 7070 656e 6420 6d73 6720 616c 7265   append msg alre
+00019c50: 6164 7920 6578 6973 7473 0a20 2020 2020  ady exists.     
+00019c60: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00019c70: 6574 5f73 6b69 705f 6263 6173 745f 636f  et_skip_bcast_co
+00019c80: 6d6d 6974 2873 656c 6629 202d 3e20 626f  mmit(self) -> bo
+00019c90: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+00019ca0: 2020 2020 2020 2020 6073 6b69 705f 6263          `skip_bc
+00019cb0: 6173 745f 636f 6d6d 6974 603a 2044 6f6e  ast_commit`: Don
+00019cc0: 2774 2062 726f 6164 6361 7374 2061 6e20  't broadcast an 
+00019cd0: 656d 7074 7920 7261 6674 2065 6e74 7279  empty raft entry
+00019ce0: 2074 6f20 6e6f 7469 6679 2066 6f6c 6c6f   to notify follo
+00019cf0: 7765 7220 746f 2063 6f6d 6d69 7420 616e  wer to commit an
+00019d00: 2065 6e74 7279 2e0a 2020 2020 2020 2020   entry..        
+00019d10: 5468 6973 206d 6179 206d 616b 6520 666f  This may make fo
+00019d20: 6c6c 6f77 6572 2077 6169 7420 6120 6c6f  llower wait a lo
+00019d30: 6e67 6572 2074 696d 6520 746f 2061 7070  nger time to app
+00019d40: 6c79 2061 6e20 656e 7472 792e 2054 6869  ly an entry. Thi
+00019d50: 7320 636f 6e66 6967 7572 6174 696f 6e0a  s configuration.
+00019d60: 2020 2020 2020 2020 4d61 7920 6166 6665          May affe
+00019d70: 6374 2070 726f 706f 7361 6c20 666f 7277  ct proposal forw
+00019d80: 6172 6469 6e67 2061 6e64 2066 6f6c 6c6f  arding and follo
+00019d90: 7765 7220 7265 6164 2e0a 2020 2020 2020  wer read..      
+00019da0: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00019db0: 745f 736b 6970 5f62 6361 7374 5f63 6f6d  t_skip_bcast_com
+00019dc0: 6d69 7428 7365 6c66 2c20 736b 6970 5f62  mit(self, skip_b
+00019dd0: 6361 7374 5f63 6f6d 6d69 743a 2062 6f6f  cast_commit: boo
+00019de0: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+00019df0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00019e00: 6073 6b69 705f 6263 6173 745f 636f 6d6d  `skip_bcast_comm
+00019e10: 6974 603a 2044 6f6e 2774 2062 726f 6164  it`: Don't broad
+00019e20: 6361 7374 2061 6e20 656d 7074 7920 7261  cast an empty ra
+00019e30: 6674 2065 6e74 7279 2074 6f20 6e6f 7469  ft entry to noti
+00019e40: 6679 2066 6f6c 6c6f 7765 7220 746f 2063  fy follower to c
+00019e50: 6f6d 6d69 7420 616e 2065 6e74 7279 2e0a  ommit an entry..
+00019e60: 2020 2020 2020 2020 5468 6973 206d 6179          This may
+00019e70: 206d 616b 6520 666f 6c6c 6f77 6572 2077   make follower w
+00019e80: 6169 7420 6120 6c6f 6e67 6572 2074 696d  ait a longer tim
+00019e90: 6520 746f 2061 7070 6c79 2061 6e20 656e  e to apply an en
+00019ea0: 7472 792e 2054 6869 7320 636f 6e66 6967  try. This config
+00019eb0: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
+00019ec0: 4d61 7920 6166 6665 6374 2070 726f 706f  May affect propo
+00019ed0: 7361 6c20 666f 7277 6172 6469 6e67 2061  sal forwarding a
+00019ee0: 6e64 2066 6f6c 6c6f 7765 7220 7265 6164  nd follower read
+00019ef0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00019f00: 2020 6465 6620 6765 745f 7072 696f 7269    def get_priori
+00019f10: 7479 2873 656c 6629 202d 3e20 696e 743a  ty(self) -> int:
+00019f20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00019f30: 2020 2020 2060 7072 696f 7269 7479 603a       `priority`:
+00019f40: 2054 6865 2065 6c65 6374 696f 6e20 7072   The election pr
+00019f50: 696f 7269 7479 206f 6620 7468 6973 206e  iority of this n
+00019f60: 6f64 652e 0a20 2020 2020 2020 2022 2222  ode..        """
+00019f70: 0a20 2020 2064 6566 2073 6574 5f70 7269  .    def set_pri
+00019f80: 6f72 6974 7928 7365 6c66 2c20 7072 696f  ority(self, prio
+00019f90: 7269 7479 3a20 696e 7429 202d 3e20 4e6f  rity: int) -> No
+00019fa0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00019fb0: 2020 2020 2020 2020 6070 7269 6f72 6974          `priorit
+00019fc0: 7960 3a20 5468 6520 656c 6563 7469 6f6e  y`: The election
+00019fd0: 2070 7269 6f72 6974 7920 6f66 2074 6869   priority of thi
+00019fe0: 7320 6e6f 6465 2e0a 2020 2020 2020 2020  s node..        
+00019ff0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0001a000: 6d61 785f 756e 636f 6d6d 6974 7465 645f  max_uncommitted_
+0001a010: 7369 7a65 2873 656c 6629 202d 3e20 696e  size(self) -> in
+0001a020: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+0001a030: 2020 2020 2020 2060 6d61 785f 756e 636f         `max_unco
+0001a040: 6d6d 6974 7465 645f 7369 7a65 603a 2053  mmitted_size`: S
+0001a050: 7065 6369 6679 206d 6178 696d 756d 206f  pecify maximum o
+0001a060: 6620 756e 636f 6d6d 6974 7465 6420 656e  f uncommitted en
+0001a070: 7472 7920 7369 7a65 2e0a 2020 2020 2020  try size..      
+0001a080: 2020 5768 656e 2074 6869 7320 6c69 6d69    When this limi
+0001a090: 7420 6973 2072 6561 6368 6564 2c20 616c  t is reached, al
+0001a0a0: 6c20 7072 6f70 6f73 616c 7320 746f 2061  l proposals to a
+0001a0b0: 7070 656e 6420 6e65 7720 6c6f 6720 7769  ppend new log wi
+0001a0c0: 6c6c 2062 6520 6472 6f70 7065 640a 2020  ll be dropped.  
+0001a0d0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+0001a0e0: 6620 7365 745f 6d61 785f 756e 636f 6d6d  f set_max_uncomm
+0001a0f0: 6974 7465 645f 7369 7a65 2873 656c 662c  itted_size(self,
+0001a100: 206d 6178 5f75 6e63 6f6d 6d69 7474 6564   max_uncommitted
+0001a110: 5f73 697a 653a 2069 6e74 2920 2d3e 204e  _size: int) -> N
+0001a120: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0001a130: 0a20 2020 2020 2020 2060 6d61 785f 756e  .        `max_un
+0001a140: 636f 6d6d 6974 7465 645f 7369 7a65 603a  committed_size`:
+0001a150: 2053 7065 6369 6679 206d 6178 696d 756d   Specify maximum
+0001a160: 206f 6620 756e 636f 6d6d 6974 7465 6420   of uncommitted 
+0001a170: 656e 7472 7920 7369 7a65 2e0a 2020 2020  entry size..    
+0001a180: 2020 2020 5768 656e 2074 6869 7320 6c69      When this li
+0001a190: 6d69 7420 6973 2072 6561 6368 6564 2c20  mit is reached, 
+0001a1a0: 616c 6c20 7072 6f70 6f73 616c 7320 746f  all proposals to
+0001a1b0: 2061 7070 656e 6420 6e65 7720 6c6f 6720   append new log 
+0001a1c0: 7769 6c6c 2062 6520 6472 6f70 7065 640a  will be dropped.
+0001a1d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001a1e0: 6465 6620 6765 745f 6d61 785f 636f 6d6d  def get_max_comm
+0001a1f0: 6974 7465 645f 7369 7a65 5f70 6572 5f72  itted_size_per_r
+0001a200: 6561 6479 2873 656c 6629 202d 3e20 696e  eady(self) -> in
+0001a210: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
 0001a220: 2020 2020 2020 2060 6d61 785f 636f 6d6d         `max_comm
 0001a230: 6974 7465 645f 7369 7a65 5f70 6572 5f72  itted_size_per_r
 0001a240: 6561 6479 603a 204d 6178 2073 697a 6520  eady`: Max size 
 0001a250: 666f 7220 636f 6d6d 6974 7465 6420 656e  for committed en
 0001a260: 7472 6965 7320 696e 2061 2060 5265 6164  tries in a `Read
 0001a270: 7960 2e0a 2020 2020 2020 2020 2222 220a  y`..        """.
-0001a280: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0001a290: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-0001a2a0: 2020 2020 2020 2020 2222 2252 756e 7320          """Runs 
-0001a2b0: 7661 6c69 6461 7469 6f6e 7320 6167 6169  validations agai
-0001a2c0: 6e73 7420 7468 6520 636f 6e66 6967 2e22  nst the config."
-0001a2d0: 2222 0a0a 636c 6173 7320 436f 6e66 6967  ""..class Config
-0001a2e0: 285f 5f41 5049 5f43 6f6e 6669 6729 3a0a  (__API_Config):.
-0001a2f0: 2020 2020 2222 220a 2020 2020 436f 6e66      """.    Conf
-0001a300: 6967 2063 6f6e 7461 696e 7320 7468 6520  ig contains the 
-0001a310: 7061 7261 6d65 7465 7273 2074 6f20 7374  parameters to st
-0001a320: 6172 7420 6120 7261 6674 2e0a 2020 2020  art a raft..    
-0001a330: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-0001a340: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0001a350: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-0001a360: 2020 2020 2020 2020 6964 3a20 4f70 7469          id: Opti
-0001a370: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-0001a380: 2c0a 2020 2020 2020 2020 656c 6563 7469  ,.        electi
-0001a390: 6f6e 5f74 6963 6b3a 204f 7074 696f 6e61  on_tick: Optiona
-0001a3a0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
-0001a3b0: 2020 2020 2020 2068 6561 7274 6265 6174         heartbeat
-0001a3c0: 5f74 6963 6b3a 204f 7074 696f 6e61 6c5b  _tick: Optional[
-0001a3d0: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
-0001a3e0: 2020 2020 2061 7070 6c69 6564 3a20 4f70       applied: Op
-0001a3f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0001a400: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
-0001a410: 7369 7a65 5f70 6572 5f6d 7367 3a20 4f70  size_per_msg: Op
-0001a420: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0001a430: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
-0001a440: 696e 666c 6967 6874 5f6d 7367 733a 204f  inflight_msgs: O
-0001a450: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0001a460: 6f6e 652c 0a20 2020 2020 2020 2063 6865  one,.        che
-0001a470: 636b 5f71 756f 7275 6d3a 204f 7074 696f  ck_quorum: Optio
-0001a480: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-0001a490: 2c0a 2020 2020 2020 2020 7072 655f 766f  ,.        pre_vo
-0001a4a0: 7465 3a20 4f70 7469 6f6e 616c 5b62 6f6f  te: Optional[boo
-0001a4b0: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
-0001a4c0: 2020 206d 696e 5f65 6c65 6374 696f 6e5f     min_election_
-0001a4d0: 7469 636b 3a20 4f70 7469 6f6e 616c 5b69  tick: Optional[i
-0001a4e0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-0001a4f0: 2020 2020 6d61 785f 656c 6563 7469 6f6e      max_election
-0001a500: 5f74 6963 6b3a 204f 7074 696f 6e61 6c5b  _tick: Optional[
-0001a510: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
-0001a520: 2020 2020 2072 6561 645f 6f6e 6c79 5f6f       read_only_o
-0001a530: 7074 696f 6e3a 204f 7074 696f 6e61 6c5b  ption: Optional[
-0001a540: 2252 6561 644f 6e6c 794f 7074 696f 6e22  "ReadOnlyOption"
-0001a550: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0001a560: 2020 736b 6970 5f62 6361 7374 5f63 6f6d    skip_bcast_com
-0001a570: 6d69 743a 204f 7074 696f 6e61 6c5b 626f  mit: Optional[bo
-0001a580: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-0001a590: 2020 2020 6261 7463 685f 6170 7065 6e64      batch_append
-0001a5a0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
-0001a5b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0001a5c0: 2070 7269 6f72 6974 793a 204f 7074 696f   priority: Optio
-0001a5d0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0001a5e0: 0a20 2020 2020 2020 206d 6178 5f75 6e63  .        max_unc
-0001a5f0: 6f6d 6d69 7474 6564 5f73 697a 653a 204f  ommitted_size: O
-0001a600: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0001a610: 6f6e 652c 0a20 2020 2020 2020 206d 6178  one,.        max
-0001a620: 5f63 6f6d 6d69 7474 6564 5f73 697a 655f  _committed_size_
-0001a630: 7065 725f 7265 6164 793a 204f 7074 696f  per_ready: Optio
-0001a640: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0001a650: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
-0001a660: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001a670: 2020 2020 3a70 6172 616d 2069 643a 2054      :param id: T
-0001a680: 6865 2069 6465 6e74 6974 7920 6f66 2074  he identity of t
-0001a690: 6865 206c 6f63 616c 2072 6166 742e 2049  he local raft. I
-0001a6a0: 7420 6361 6e6e 6f74 2062 6520 302c 2061  t cannot be 0, a
-0001a6b0: 6e64 206d 7573 7420 6265 2075 6e69 7175  nd must be uniqu
-0001a6c0: 6520 696e 2074 6865 2067 726f 7570 2e0a  e in the group..
-0001a6d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0001a6e0: 656c 6563 7469 6f6e 5f74 6963 6b3a 2054  election_tick: T
-0001a6f0: 6865 206e 756d 6265 7220 6f66 206e 6f64  he number of nod
-0001a700: 652e 7469 636b 2069 6e76 6f63 6174 696f  e.tick invocatio
-0001a710: 6e73 2074 6861 7420 6d75 7374 2070 6173  ns that must pas
-0001a720: 7320 6265 7477 6565 6e0a 2020 2020 2020  s between.      
-0001a730: 2020 656c 6563 7469 6f6e 732e 2054 6861    elections. Tha
-0001a740: 7420 6973 2c20 6966 2061 2066 6f6c 6c6f  t is, if a follo
-0001a750: 7765 7220 646f 6573 206e 6f74 2072 6563  wer does not rec
-0001a760: 6569 7665 2061 6e79 206d 6573 7361 6765  eive any message
-0001a770: 2066 726f 6d20 7468 650a 2020 2020 2020   from the.      
-0001a780: 2020 6c65 6164 6572 206f 6620 6375 7272    leader of curr
-0001a790: 656e 7420 7465 726d 2062 6566 6f72 6520  ent term before 
-0001a7a0: 456c 6563 7469 6f6e 5469 636b 2068 6173  ElectionTick has
-0001a7b0: 2065 6c61 7073 6564 2c20 6974 2077 696c   elapsed, it wil
-0001a7c0: 6c20 6265 636f 6d65 0a20 2020 2020 2020  l become.       
-0001a7d0: 2063 616e 6469 6461 7465 2061 6e64 2073   candidate and s
-0001a7e0: 7461 7274 2061 6e20 656c 6563 7469 6f6e  tart an election
-0001a7f0: 2e20 656c 6563 7469 6f6e 5f74 6963 6b20  . election_tick 
-0001a800: 6d75 7374 2062 6520 6772 6561 7465 7220  must be greater 
-0001a810: 7468 616e 0a20 2020 2020 2020 2048 6561  than.        Hea
-0001a820: 7274 6265 6174 5469 636b 2e20 5765 2073  rtbeatTick. We s
-0001a830: 7567 6765 7374 2065 6c65 6374 696f 6e5f  uggest election_
-0001a840: 7469 636b 203d 2031 3020 2a20 4865 6172  tick = 10 * Hear
-0001a850: 7462 6561 7454 6963 6b20 746f 2061 766f  tbeatTick to avo
-0001a860: 6964 0a20 2020 2020 2020 2075 6e6e 6563  id.        unnec
-0001a870: 6573 7361 7279 206c 6561 6465 7220 7377  essary leader sw
-0001a880: 6974 6368 696e 670a 0a20 2020 2020 2020  itching..       
-0001a890: 203a 7061 7261 6d20 6865 6172 7462 6561   :param heartbea
-0001a8a0: 745f 7469 636b 3a20 4865 6172 7462 6561  t_tick: Heartbea
-0001a8b0: 7454 6963 6b20 6973 2074 6865 206e 756d  tTick is the num
-0001a8c0: 6265 7220 6f66 206e 6f64 652e 7469 636b  ber of node.tick
-0001a8d0: 2069 6e76 6f63 6174 696f 6e73 2074 6861   invocations tha
-0001a8e0: 7420 6d75 7374 2070 6173 7320 6265 7477  t must pass betw
-0001a8f0: 6565 6e0a 2020 2020 2020 2020 6865 6172  een.        hear
-0001a900: 7462 6561 7473 2e20 5468 6174 2069 732c  tbeats. That is,
-0001a910: 2061 206c 6561 6465 7220 7365 6e64 7320   a leader sends 
-0001a920: 6865 6172 7462 6561 7420 6d65 7373 6167  heartbeat messag
-0001a930: 6573 2074 6f20 6d61 696e 7461 696e 2069  es to maintain i
-0001a940: 7473 0a20 2020 2020 2020 206c 6561 6465  ts.        leade
-0001a950: 7273 6869 7020 6576 6572 7920 6865 6172  rship every hear
-0001a960: 7462 6561 7420 7469 636b 732e 0a0a 2020  tbeat ticks...  
-0001a970: 2020 2020 2020 3a70 6172 616d 2061 7070        :param app
-0001a980: 6c69 6564 3a20 4170 706c 6965 6420 6973  lied: Applied is
-0001a990: 2074 6865 206c 6173 7420 6170 706c 6965   the last applie
-0001a9a0: 6420 696e 6465 782e 2049 7420 7368 6f75  d index. It shou
-0001a9b0: 6c64 206f 6e6c 7920 6265 2073 6574 2077  ld only be set w
-0001a9c0: 6865 6e20 7265 7374 6172 7469 6e67 0a20  hen restarting. 
-0001a9d0: 2020 2020 2020 2072 6166 742e 2072 6166         raft. raf
-0001a9e0: 7420 7769 6c6c 206e 6f74 2072 6574 7572  t will not retur
-0001a9f0: 6e20 656e 7472 6965 7320 746f 2074 6865  n entries to the
-0001aa00: 2061 7070 6c69 6361 7469 6f6e 2073 6d61   application sma
-0001aa10: 6c6c 6572 206f 7220 6571 7561 6c20 746f  ller or equal to
-0001aa20: 2041 7070 6c69 6564 2e0a 2020 2020 2020   Applied..      
-0001aa30: 2020 4966 2041 7070 6c69 6564 2069 7320    If Applied is 
-0001aa40: 756e 7365 7420 7768 656e 2072 6573 7461  unset when resta
-0001aa50: 7274 696e 672c 2072 6166 7420 6d69 6768  rting, raft migh
-0001aa60: 7420 7265 7475 726e 2070 7265 7669 6f75  t return previou
-0001aa70: 7320 6170 706c 6965 6420 656e 7472 6965  s applied entrie
-0001aa80: 732e 0a20 2020 2020 2020 2054 6869 7320  s..        This 
-0001aa90: 6973 2061 2076 6572 7920 6170 706c 6963  is a very applic
-0001aaa0: 6174 696f 6e20 6465 7065 6e64 656e 7420  ation dependent 
-0001aab0: 636f 6e66 6967 7572 6174 696f 6e2e 0a0a  configuration...
-0001aac0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-0001aad0: 6178 5f73 697a 655f 7065 725f 6d73 673a  ax_size_per_msg:
-0001aae0: 204c 696d 6974 2074 6865 206d 6178 2073   Limit the max s
-0001aaf0: 697a 6520 6f66 2065 6163 6820 6170 7065  ize of each appe
-0001ab00: 6e64 206d 6573 7361 6765 2e20 536d 616c  nd message. Smal
-0001ab10: 6c65 7220 7661 6c75 6520 6c6f 7765 7273  ler value lowers
-0001ab20: 0a20 2020 2020 2020 2074 6865 2072 6166  .        the raf
-0001ab30: 7420 7265 636f 7665 7279 2063 6f73 7428  t recovery cost(
-0001ab40: 696e 6974 6961 6c20 7072 6f62 696e 6720  initial probing 
-0001ab50: 616e 6420 6d65 7373 6167 6520 6c6f 7374  and message lost
-0001ab60: 2064 7572 696e 6720 6e6f 726d 616c 206f   during normal o
-0001ab70: 7065 7261 7469 6f6e 292e 0a20 2020 2020  peration)..     
-0001ab80: 2020 204f 6e20 7468 6520 6f74 6865 7220     On the other 
-0001ab90: 7369 6465 2c20 6974 206d 6967 6874 2061  side, it might a
-0001aba0: 6666 6563 7420 7468 6520 7468 726f 7567  ffect the throug
-0001abb0: 6870 7574 2064 7572 696e 6720 6e6f 726d  hput during norm
-0001abc0: 616c 2072 6570 6c69 6361 7469 6f6e 2e0a  al replication..
-0001abd0: 2020 2020 2020 2020 4e6f 7465 3a20 6d61          Note: ma
-0001abe0: 7468 2e4d 6178 5575 7369 7a65 3634 2066  th.MaxUusize64 f
-0001abf0: 6f72 2075 6e6c 696d 6974 6564 2c20 3020  or unlimited, 0 
-0001ac00: 666f 7220 6174 206d 6f73 7420 6f6e 6520  for at most one 
-0001ac10: 656e 7472 7920 7065 7220 6d65 7373 6167  entry per messag
-0001ac20: 652e 0a0a 2020 2020 2020 2020 3a70 6172  e...        :par
-0001ac30: 616d 206d 6178 5f69 6e66 6c69 6768 745f  am max_inflight_
-0001ac40: 6d73 6773 3a20 4c69 6d69 7420 7468 6520  msgs: Limit the 
-0001ac50: 6d61 7820 6e75 6d62 6572 206f 6620 696e  max number of in
-0001ac60: 2d66 6c69 6768 7420 6170 7065 6e64 206d  -flight append m
-0001ac70: 6573 7361 6765 7320 6475 7269 6e67 206f  essages during o
-0001ac80: 7074 696d 6973 7469 630a 2020 2020 2020  ptimistic.      
-0001ac90: 2020 7265 706c 6963 6174 696f 6e20 7068    replication ph
-0001aca0: 6173 652e 2054 6865 2061 7070 6c69 6361  ase. The applica
-0001acb0: 7469 6f6e 2074 7261 6e73 706f 7274 6174  tion transportat
-0001acc0: 696f 6e20 6c61 7965 7220 7573 7561 6c6c  ion layer usuall
-0001acd0: 7920 6861 7320 6974 7320 6f77 6e20 7365  y has its own se
-0001ace0: 6e64 696e 670a 2020 2020 2020 2020 6275  nding.        bu
-0001acf0: 6666 6572 206f 7665 7220 5443 502f 5544  ffer over TCP/UD
-0001ad00: 502e 2053 6574 2074 6f20 6176 6f69 6420  P. Set to avoid 
-0001ad10: 6f76 6572 666c 6f77 696e 6720 7468 6174  overflowing that
-0001ad20: 2073 656e 6469 6e67 2062 7566 6665 722e   sending buffer.
-0001ad30: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0001ad40: 2063 6865 636b 5f71 756f 7275 6d3a 2053   check_quorum: S
-0001ad50: 7065 6369 6679 2069 6620 7468 6520 6c65  pecify if the le
-0001ad60: 6164 6572 2073 686f 756c 6420 6368 6563  ader should chec
-0001ad70: 6b20 7175 6f72 756d 2061 6374 6976 6974  k quorum activit
-0001ad80: 792e 204c 6561 6465 7220 7374 6570 7320  y. Leader steps 
-0001ad90: 646f 776e 2077 6865 6e0a 2020 2020 2020  down when.      
-0001ada0: 2020 7175 6f72 756d 2069 7320 6e6f 7420    quorum is not 
-0001adb0: 6163 7469 7665 2066 6f72 2061 6e20 656c  active for an el
-0001adc0: 6563 7469 6f6e 5469 6d65 6f75 742e 0a0a  ectionTimeout...
-0001add0: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0001ade0: 7265 5f76 6f74 653a 2045 6e61 626c 6573  re_vote: Enables
-0001adf0: 2074 6865 2050 7265 2d56 6f74 6520 616c   the Pre-Vote al
-0001ae00: 676f 7269 7468 6d20 6465 7363 7269 6265  gorithm describe
-0001ae10: 6420 696e 2072 6166 7420 7468 6573 6973  d in raft thesis
-0001ae20: 2073 6563 7469 6f6e 0a20 2020 2020 2020   section.       
-0001ae30: 2039 2e36 2e20 5468 6973 2070 7265 7665   9.6. This preve
-0001ae40: 6e74 7320 6469 7372 7570 7469 6f6e 2077  nts disruption w
-0001ae50: 6865 6e20 6120 6e6f 6465 2074 6861 7420  hen a node that 
-0001ae60: 6861 7320 6265 656e 2070 6172 7469 7469  has been partiti
-0001ae70: 6f6e 6564 2061 7761 790a 2020 2020 2020  oned away.      
-0001ae80: 2020 7265 6a6f 696e 7320 7468 6520 636c    rejoins the cl
-0001ae90: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
-0001aea0: 3a70 6172 616d 206d 696e 5f65 6c65 6374  :param min_elect
-0001aeb0: 696f 6e5f 7469 636b 3a20 5468 6520 7261  ion_tick: The ra
-0001aec0: 6e67 6520 6f66 2065 6c65 6374 696f 6e20  nge of election 
-0001aed0: 7469 6d65 6f75 742e 2049 6e20 736f 6d65  timeout. In some
-0001aee0: 2063 6173 6573 2c20 7765 2068 6f70 6520   cases, we hope 
-0001aef0: 736f 6d65 206e 6f64 6573 2068 6173 206c  some nodes has l
-0001af00: 6573 7320 706f 7373 6962 696c 6974 790a  ess possibility.
-0001af10: 2020 2020 2020 2020 746f 2062 6563 6f6d          to becom
-0001af20: 6520 6c65 6164 6572 2e20 5468 6973 2063  e leader. This c
-0001af30: 6f6e 6669 6775 7261 7469 6f6e 2065 6e73  onfiguration ens
-0001af40: 7572 6573 2074 6861 7420 7468 6520 7261  ures that the ra
-0001af50: 6e64 6f6d 697a 6564 2065 6c65 6374 696f  ndomized electio
-0001af60: 6e5f 7469 6d65 6f75 740a 2020 2020 2020  n_timeout.      
-0001af70: 2020 7769 6c6c 2061 6c77 6179 7320 6265    will always be
-0001af80: 2073 7569 7420 696e 205b 6d69 6e5f 656c   suit in [min_el
-0001af90: 6563 7469 6f6e 5f74 6963 6b2c 206d 6178  ection_tick, max
-0001afa0: 5f65 6c65 6374 696f 6e5f 7469 636b 292e  _election_tick).
-0001afb0: 0a20 2020 2020 2020 2049 6620 6974 2069  .        If it i
-0001afc0: 7320 302c 2074 6865 6e20 656c 6563 7469  s 0, then electi
-0001afd0: 6f6e 5f74 6963 6b20 7769 6c6c 2062 6520  on_tick will be 
-0001afe0: 6368 6f73 656e 2e0a 0a20 2020 2020 2020  chosen...       
-0001aff0: 203a 7061 7261 6d20 6d61 785f 656c 6563   :param max_elec
-0001b000: 7469 6f6e 5f74 6963 6b3a 2049 6620 6974  tion_tick: If it
-0001b010: 2069 7320 302c 2074 6865 6e20 3220 2a20   is 0, then 2 * 
-0001b020: 656c 6563 7469 6f6e 5f74 6963 6b20 7769  election_tick wi
-0001b030: 6c6c 2062 6520 6368 6f73 656e 2e0a 0a20  ll be chosen... 
-0001b040: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
-0001b050: 6164 5f6f 6e6c 795f 6f70 7469 6f6e 3a20  ad_only_option: 
-0001b060: 4368 6f6f 7365 2074 6865 206c 696e 6561  Choose the linea
-0001b070: 7269 7a61 6269 6c69 7479 206d 6f64 6520  rizability mode 
-0001b080: 6f72 2074 6865 206c 6561 7365 206d 6f64  or the lease mod
-0001b090: 6520 746f 2072 6561 6420 6461 7461 2e20  e to read data. 
-0001b0a0: 4966 2079 6f75 2064 6f6e e280 9974 2063  If you don...t c
-0001b0b0: 6172 6520 6162 6f75 7420 7468 6520 7265  are about the re
-0001b0c0: 6164 2063 6f6e 7369 7374 656e 6379 2061  ad consistency a
-0001b0d0: 6e64 2077 616e 7420 6120 6869 6768 6572  nd want a higher
-0001b0e0: 2072 6561 6420 7065 7266 6f72 6d61 6e63   read performanc
-0001b0f0: 652c 2079 6f75 2063 616e 2075 7365 2074  e, you can use t
-0001b100: 6865 206c 6561 7365 206d 6f64 652e 0a20  he lease mode.. 
-0001b110: 2020 2020 2020 2053 6574 7469 6e67 2074         Setting t
-0001b120: 6869 7320 746f 2060 4c65 6173 6542 6173  his to `LeaseBas
-0001b130: 6564 6020 7265 7175 6972 6573 2060 6368  ed` requires `ch
-0001b140: 6563 6b5f 7175 6f72 756d 203d 2074 7275  eck_quorum = tru
-0001b150: 6560 2e0a 0a20 2020 2020 2020 203a 7061  e`...        :pa
-0001b160: 7261 6d20 736b 6970 5f62 6361 7374 5f63  ram skip_bcast_c
-0001b170: 6f6d 6d69 743a 2044 6f6e 2774 2062 726f  ommit: Don't bro
-0001b180: 6164 6361 7374 2061 6e20 656d 7074 7920  adcast an empty 
-0001b190: 7261 6674 2065 6e74 7279 2074 6f20 6e6f  raft entry to no
-0001b1a0: 7469 6679 2066 6f6c 6c6f 7765 7220 746f  tify follower to
-0001b1b0: 2063 6f6d 6d69 7420 616e 2065 6e74 7279   commit an entry
-0001b1c0: 2e0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
-0001b1d0: 6179 206d 616b 6520 666f 6c6c 6f77 6572  ay make follower
-0001b1e0: 2077 6169 7420 6120 6c6f 6e67 6572 2074   wait a longer t
-0001b1f0: 696d 6520 746f 2061 7070 6c79 2061 6e20  ime to apply an 
-0001b200: 656e 7472 792e 2054 6869 7320 636f 6e66  entry. This conf
-0001b210: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
-0001b220: 2020 4d61 7920 6166 6665 6374 2070 726f    May affect pro
-0001b230: 706f 7361 6c20 666f 7277 6172 6469 6e67  posal forwarding
-0001b240: 2061 6e64 2066 6f6c 6c6f 7765 7220 7265   and follower re
-0001b250: 6164 2e0a 0a20 2020 2020 2020 203a 7061  ad...        :pa
-0001b260: 7261 6d20 6261 7463 685f 6170 7065 6e64  ram batch_append
-0001b270: 3a20 4261 7463 6865 7320 6576 6572 7920  : Batches every 
-0001b280: 6170 7065 6e64 206d 7367 2069 6620 616e  append msg if an
-0001b290: 7920 6170 7065 6e64 206d 7367 2061 6c72  y append msg alr
-0001b2a0: 6561 6479 2065 7869 7374 730a 0a20 2020  eady exists..   
-0001b2b0: 2020 2020 203a 7061 7261 6d20 7072 696f       :param prio
-0001b2c0: 7269 7479 3a20 5468 6520 656c 6563 7469  rity: The electi
-0001b2d0: 6f6e 2070 7269 6f72 6974 7920 6f66 2074  on priority of t
-0001b2e0: 6869 7320 6e6f 6465 2e0a 0a20 2020 2020  his node...     
-0001b2f0: 2020 203a 7061 7261 6d20 6d61 785f 756e     :param max_un
-0001b300: 636f 6d6d 6974 7465 645f 7369 7a65 3a20  committed_size: 
-0001b310: 5370 6563 6966 7920 6d61 7869 6d75 6d20  Specify maximum 
-0001b320: 6f66 2075 6e63 6f6d 6d69 7474 6564 2065  of uncommitted e
-0001b330: 6e74 7279 2073 697a 652e 0a20 2020 2020  ntry size..     
-0001b340: 2020 2057 6865 6e20 7468 6973 206c 696d     When this lim
-0001b350: 6974 2069 7320 7265 6163 6865 642c 2061  it is reached, a
-0001b360: 6c6c 2070 726f 706f 7361 6c73 2074 6f20  ll proposals to 
-0001b370: 6170 7065 6e64 206e 6577 206c 6f67 2077  append new log w
-0001b380: 696c 6c20 6265 2064 726f 7070 6564 0a0a  ill be dropped..
-0001b390: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-0001b3a0: 6178 5f63 6f6d 6d69 7474 6564 5f73 697a  ax_committed_siz
-0001b3b0: 655f 7065 725f 7265 6164 793a 204d 6178  e_per_ready: Max
-0001b3c0: 2073 697a 6520 666f 7220 636f 6d6d 6974   size for commit
-0001b3d0: 7465 6420 656e 7472 6965 7320 696e 2061  ted entries in a
-0001b3e0: 2060 5265 6164 7960 2e0a 2020 2020 2020   `Ready`..      
-0001b3f0: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
-0001b400: 6b65 5f72 6566 2873 656c 6629 202d 3e20  ke_ref(self) -> 
-0001b410: 2243 6f6e 6669 6752 6566 223a 202e 2e2e  "ConfigRef": ...
-0001b420: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0001b430: 6f64 0a20 2020 2064 6566 2064 6566 6175  od.    def defau
-0001b440: 6c74 2829 202d 3e20 2243 6f6e 6669 6722  lt() -> "Config"
-0001b450: 3a20 2e2e 2e0a 0a63 6c61 7373 2043 6f6e  : .....class Con
-0001b460: 6669 6752 6566 285f 5f41 5049 5f43 6f6e  figRef(__API_Con
-0001b470: 6669 6729 3a0a 2020 2020 2222 220a 2020  fig):.    """.  
-0001b480: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
-0001b490: 206f 6620 3a63 6c61 7373 3a60 496e 666c   of :class:`Infl
-0001b4a0: 6967 6874 7352 6566 602e 0a20 2020 2022  ightsRef`..    "
-0001b4b0: 2222 0a0a 2320 544f 444f 3a20 4164 6420  ""..# TODO: Add 
-0001b4c0: 6265 6c6f 7720 696d 706c 656d 656e 7461  below implementa
-0001b4d0: 7469 6f6e 2069 6620 6e65 6564 6564 2c20  tion if needed, 
-0001b4e0: 6f74 6865 7277 6973 6520 7265 6d6f 7665  otherwise remove
-0001b4f0: 2062 656c 6f77 2063 6f64 6573 2e0a 2320   below codes..# 
-0001b500: 636c 6173 7320 5f5f 4150 495f 5374 6174  class __API_Stat
-0001b510: 7573 3a0a 2320 2020 2020 6465 6620 6765  us:.#     def ge
-0001b520: 745f 6170 706c 6965 6428 7365 6c66 2920  t_applied(self) 
-0001b530: 2d3e 2069 6e74 3a0a 2320 2020 2020 2020  -> int:.#       
-0001b540: 2020 2222 2220 2222 220a 2320 2020 2020    """ """.#     
-0001b550: 6465 6620 7365 745f 6170 706c 6965 6428  def set_applied(
-0001b560: 7365 6c66 2c20 6170 706c 6965 643a 2069  self, applied: i
-0001b570: 6e74 2920 2d3e 204e 6f6e 653a 0a23 2020  nt) -> None:.#  
-0001b580: 2020 2020 2020 2022 2222 2022 2222 0a23         """ """.#
-0001b590: 2020 2020 2064 6566 2067 6574 5f69 6428       def get_id(
-0001b5a0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2320  self) -> int:.# 
-0001b5b0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0001b5c0: 2320 2020 2020 6465 6620 7365 745f 6964  #     def set_id
-0001b5d0: 2873 656c 662c 2069 643a 2069 6e74 2920  (self, id: int) 
-0001b5e0: 2d3e 204e 6f6e 653a 0a23 2020 2020 2020  -> None:.#      
-0001b5f0: 2020 2022 2222 2022 2222 0a23 2020 2020     """ """.#    
-0001b600: 2064 6566 2067 6574 5f68 7328 7365 6c66   def get_hs(self
-0001b610: 2920 2d3e 2048 6172 6453 7461 7465 5265  ) -> HardStateRe
-0001b620: 663a 0a23 2020 2020 2020 2020 2022 2222  f:.#         """
-0001b630: 2022 2222 0a23 2020 2020 2064 6566 2073   """.#     def s
-0001b640: 6574 5f68 7328 7365 6c66 2c20 6873 3a20  et_hs(self, hs: 
-0001b650: 4861 7264 5374 6174 6552 6566 2920 2d3e  HardStateRef) ->
-0001b660: 204e 6f6e 653a 0a23 2020 2020 2020 2020   None:.#        
-0001b670: 2022 2222 2022 2222 0a23 2020 2020 2064   """ """.#     d
-0001b680: 6566 2067 6574 5f73 7328 7365 6c66 2920  ef get_ss(self) 
-0001b690: 2d3e 2053 6f66 7453 7461 7465 5265 663a  -> SoftStateRef:
-0001b6a0: 0a23 2020 2020 2020 2020 2022 2222 2022  .#         """ "
-0001b6b0: 2222 0a23 2020 2020 2064 6566 2073 6574  "".#     def set
-0001b6c0: 5f73 7328 7365 6c66 2c20 7373 3a20 536f  _ss(self, ss: So
-0001b6d0: 6674 5374 6174 6552 6566 2920 2d3e 204e  ftStateRef) -> N
-0001b6e0: 6f6e 653a 0a23 2020 2020 2020 2020 2022  one:.#         "
-0001b6f0: 2222 2022 2222 0a23 2020 2020 2064 6566  "" """.#     def
-0001b700: 2067 6574 5f70 726f 6772 6573 7328 7365   get_progress(se
-0001b710: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
-0001b720: 5072 6f67 7265 7373 5472 6163 6b65 7252  ProgressTrackerR
-0001b730: 6566 5d3a 0a23 2020 2020 2020 2020 2022  ef]:.#         "
-0001b740: 2222 2022 2222 0a23 2020 2020 2064 6566  "" """.#     def
-0001b750: 2073 6574 5f70 726f 6772 6573 7328 0a23   set_progress(.#
-0001b760: 2020 2020 2020 2020 2073 656c 662c 2074           self, t
-0001b770: 7261 636b 6572 3a20 4f70 7469 6f6e 616c  racker: Optional
-0001b780: 5b50 726f 6772 6573 7354 7261 636b 6572  [ProgressTracker
-0001b790: 5d20 7c20 4f70 7469 6f6e 616c 5b50 726f  ] | Optional[Pro
-0001b7a0: 6772 6573 7354 7261 636b 6572 5265 665d  gressTrackerRef]
-0001b7b0: 0a23 2020 2020 2029 202d 3e20 4e6f 6e65  .#     ) -> None
-0001b7c0: 3a0a 2320 2020 2020 2020 2020 2222 2220  :.#         """ 
-0001b7d0: 2222 220a 0a23 2063 6c61 7373 2049 6e4d  """..# class InM
-0001b7e0: 656d 6f72 7953 7461 7475 7328 5f5f 4150  emoryStatus(__AP
-0001b7f0: 495f 5374 6174 7573 293a 0a23 2020 2020  I_Status):.#    
-0001b800: 2022 2222 0a23 2020 2020 2052 6570 7265   """.#     Repre
-0001b810: 7365 6e74 7320 7468 6520 6375 7272 656e  sents the curren
-0001b820: 7420 7374 6174 7573 206f 6620 7468 6520  t status of the 
-0001b830: 7261 6674 0a23 2020 2020 2022 2222 0a0a  raft.#     """..
-0001b840: 2320 2020 2020 6465 6620 5f5f 696e 6974  #     def __init
-0001b850: 5f5f 2873 656c 662c 2072 6166 743a 2049  __(self, raft: I
-0001b860: 6e4d 656d 6f72 7952 6166 7429 202d 3e20  nMemoryRaft) -> 
-0001b870: 4e6f 6e65 3a20 2e2e 2e0a 2320 2020 2020  None: ....#     
-0001b880: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
-0001b890: 6629 202d 3e20 5374 6174 7573 5f5f 4d65  f) -> Status__Me
-0001b8a0: 6d73 746f 7261 6765 5265 663a 202e 2e2e  mstorageRef: ...
-0001b8b0: 0a0a 2320 636c 6173 7320 496e 4d65 6d6f  ..# class InMemo
-0001b8c0: 7279 5374 6174 7573 5265 6628 5f5f 4150  ryStatusRef(__AP
-0001b8d0: 495f 5374 6174 7573 293a 0a23 2020 2020  I_Status):.#    
-0001b8e0: 2022 2222 0a23 2020 2020 2052 6566 6572   """.#     Refer
-0001b8f0: 656e 6365 2074 7970 6520 6f66 203a 636c  ence type of :cl
-0001b900: 6173 733a 6053 7461 7475 735f 5f4d 656d  ass:`Status__Mem
-0001b910: 7374 6f72 6167 6560 2e0a 2320 2020 2020  storage`..#     
-0001b920: 2222 220a 0a63 6c61 7373 2044 6573 7472  """..class Destr
-0001b930: 6f79 6564 5265 6655 7365 6445 7272 6f72  oyedRefUsedError
-0001b940: 2845 7863 6570 7469 6f6e 293a 0a20 2020  (Exception):.   
-0001b950: 2022 2222 2022 2222 0a0a 636c 6173 7320   """ """..class 
-0001b960: 5261 6674 4572 726f 7228 4578 6365 7074  RaftError(Except
-0001b970: 696f 6e29 3a0a 2020 2020 2222 2220 2222  ion):.    """ ""
-0001b980: 220a 0a63 6c61 7373 2045 7869 7374 7345  "..class ExistsE
-0001b990: 7272 6f72 2852 6166 7445 7272 6f72 293a  rror(RaftError):
-0001b9a0: 0a20 2020 2022 2222 0a20 2020 2054 6865  .    """.    The
-0001b9b0: 206e 6f64 6520 7b69 647d 2061 6c72 6561   node {id} alrea
-0001b9c0: 6479 2065 7869 7374 7320 696e 2074 6865  dy exists in the
-0001b9d0: 207b 7365 747d 2073 6574 2e0a 2020 2020   {set} set..    
-0001b9e0: 2222 220a 0a20 2020 2069 643a 2069 6e74  """..    id: int
-0001b9f0: 0a20 2020 2073 6574 3a20 7374 720a 0a63  .    set: str..c
-0001ba00: 6c61 7373 204e 6f74 4578 6973 7473 2852  lass NotExists(R
-0001ba10: 6166 7445 7272 6f72 293a 0a20 2020 2022  aftError):.    "
-0001ba20: 2222 0a20 2020 2054 6865 206e 6f64 6520  "".    The node 
-0001ba30: 7b69 647d 2069 7320 6e6f 7420 696e 2074  {id} is not in t
-0001ba40: 6865 207b 7365 747d 2073 6574 2e0a 2020  he {set} set..  
-0001ba50: 2020 2222 220a 0a20 2020 2069 643a 2069    """..    id: i
-0001ba60: 6e74 0a20 2020 2073 6574 3a20 7374 720a  nt.    set: str.
-0001ba70: 0a63 6c61 7373 2043 6f64 6563 4572 726f  .class CodecErro
-0001ba80: 7228 5261 6674 4572 726f 7229 3a0a 2020  r(RaftError):.  
-0001ba90: 2020 2222 220a 2020 2020 4120 7072 6f74    """.    A prot
-0001baa0: 6f62 7566 206d 6573 7361 6765 2063 6f64  obuf message cod
-0001bab0: 6563 2066 6169 6c65 6420 696e 2073 6f6d  ec failed in som
-0001bac0: 6520 6d61 6e6e 6572 2e0a 2020 2020 2222  e manner..    ""
-0001bad0: 220a 0a63 6c61 7373 2043 6f6e 6669 6749  "..class ConfigI
-0001bae0: 6e76 616c 6964 4572 726f 7228 5261 6674  nvalidError(Raft
-0001baf0: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
-0001bb00: 2020 2020 5468 6520 636f 6e66 6967 7572      The configur
-0001bb10: 6174 696f 6e20 6973 2069 6e76 616c 6964  ation is invalid
-0001bb20: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
-0001bb30: 2050 726f 706f 7361 6c44 726f 7070 6564   ProposalDropped
-0001bb40: 4572 726f 7228 5261 6674 4572 726f 7229  Error(RaftError)
-0001bb50: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-0001bb60: 6520 7072 6f70 6f73 616c 206f 6620 6368  e proposal of ch
-0001bb70: 616e 6765 7320 7761 7320 6472 6f70 7065  anges was droppe
-0001bb80: 642e 0a20 2020 2022 2222 0a0a 636c 6173  d..    """..clas
-0001bb90: 7320 5265 7175 6573 7453 6e61 7073 686f  s RequestSnapsho
-0001bba0: 7444 726f 7070 6564 4572 726f 7228 5261  tDroppedError(Ra
-0001bbb0: 6674 4572 726f 7229 3a0a 2020 2020 2222  ftError):.    ""
-0001bbc0: 220a 2020 2020 5468 6520 7265 7175 6573  ".    The reques
-0001bbd0: 7420 736e 6170 7368 6f74 2069 7320 6472  t snapshot is dr
-0001bbe0: 6f70 7065 642e 0a20 2020 2022 2222 0a0a  opped..    """..
-0001bbf0: 636c 6173 7320 436f 6e66 4368 616e 6765  class ConfChange
-0001bc00: 4572 726f 7228 5261 6674 4572 726f 7229  Error(RaftError)
-0001bc10: 3a0a 2020 2020 2222 220a 2020 2020 436f  :.    """.    Co
-0001bc20: 6e66 4368 616e 6765 2070 726f 706f 7361  nfChange proposa
-0001bc30: 6c20 6973 2069 6e76 616c 6964 2e0a 2020  l is invalid..  
-0001bc40: 2020 2222 220a 0a63 6c61 7373 2049 6f45    """..class IoE
-0001bc50: 7272 6f72 2852 6166 7445 7272 6f72 293a  rror(RaftError):
-0001bc60: 0a20 2020 2022 2222 0a20 2020 2041 6e20  .    """.    An 
-0001bc70: 494f 2065 7272 6f72 206f 6363 7572 7265  IO error occurre
-0001bc80: 642e 0a20 2020 2022 2222 0a0a 636c 6173  d..    """..clas
-0001bc90: 7320 5374 6f72 6545 7272 6f72 2852 6166  s StoreError(Raf
-0001bca0: 7445 7272 6f72 293a 0a20 2020 2022 2222  tError):.    """
-0001bcb0: 0a20 2020 2041 2073 746f 7261 6765 2065  .    A storage e
-0001bcc0: 7272 6f72 206f 6363 7572 7265 642e 0a20  rror occurred.. 
-0001bcd0: 2020 2022 2222 0a0a 636c 6173 7320 5374     """..class St
-0001bce0: 6570 4c6f 6361 6c4d 7367 2852 6166 7445  epLocalMsg(RaftE
-0001bcf0: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
-0001bd00: 2020 2052 6166 7420 6361 6e6e 6f74 2073     Raft cannot s
-0001bd10: 7465 7020 7468 6520 6c6f 6361 6c20 6d65  tep the local me
-0001bd20: 7373 6167 652e 0a20 2020 2022 2222 0a0a  ssage..    """..
-0001bd30: 636c 6173 7320 5374 6570 5065 6572 4e6f  class StepPeerNo
-0001bd40: 7446 6f75 6e64 2852 6166 7445 7272 6f72  tFound(RaftError
-0001bd50: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
-0001bd60: 6865 2072 6166 7420 7065 6572 2069 7320  he raft peer is 
-0001bd70: 6e6f 7420 666f 756e 6420 616e 6420 7468  not found and th
-0001bd80: 7573 2063 616e 6e6f 7420 7374 6570 2e0a  us cannot step..
-0001bd90: 2020 2020 2222 220a 0a63 6c61 7373 2052      """..class R
-0001bda0: 6166 7453 746f 7261 6765 4572 726f 7228  aftStorageError(
-0001bdb0: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
-0001bdc0: 2222 220a 2020 2020 416e 2065 7272 6f72  """.    An error
-0001bdd0: 2077 6974 6820 7468 6520 7374 6f72 6167   with the storag
-0001bde0: 652e 0a20 2020 2022 2222 0a0a 636c 6173  e..    """..clas
-0001bdf0: 7320 436f 6d70 6163 7465 6445 7272 6f72  s CompactedError
-0001be00: 2852 6166 7453 746f 7261 6765 4572 726f  (RaftStorageErro
-0001be10: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
-0001be20: 5468 6520 7374 6f72 6167 6520 7761 7320  The storage was 
-0001be30: 636f 6d70 6163 7465 6420 616e 6420 6e6f  compacted and no
-0001be40: 7420 6163 6365 7373 6962 6c65 0a20 2020  t accessible.   
-0001be50: 2022 2222 0a0a 636c 6173 7320 556e 6176   """..class Unav
-0001be60: 6169 6c61 626c 6545 7272 6f72 2852 6166  ailableError(Raf
-0001be70: 7453 746f 7261 6765 4572 726f 7229 3a0a  tStorageError):.
-0001be80: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
-0001be90: 6c6f 6720 6973 206e 6f74 2061 7661 696c  log is not avail
-0001bea0: 6162 6c65 2e0a 2020 2020 2222 220a 0a63  able..    """..c
-0001beb0: 6c61 7373 204c 6f67 5465 6d70 6f72 6172  lass LogTemporar
-0001bec0: 696c 7955 6e61 7661 696c 6162 6c65 4572  ilyUnavailableEr
-0001bed0: 726f 7228 5261 6674 5374 6f72 6167 6545  ror(RaftStorageE
-0001bee0: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
-0001bef0: 2020 2054 6865 206c 6f67 2069 7320 6265     The log is be
-0001bf00: 696e 6720 6665 7463 6865 642e 0a20 2020  ing fetched..   
-0001bf10: 2022 2222 0a0a 636c 6173 7320 536e 6170   """..class Snap
-0001bf20: 7368 6f74 4f75 744f 6644 6174 6545 7272  shotOutOfDateErr
-0001bf30: 6f72 2852 6166 7453 746f 7261 6765 4572  or(RaftStorageEr
-0001bf40: 726f 7229 3a0a 2020 2020 2222 220a 2020  ror):.    """.  
-0001bf50: 2020 5468 6520 736e 6170 7368 6f74 2069    The snapshot i
-0001bf60: 7320 6f75 7420 6f66 2064 6174 652e 0a20  s out of date.. 
-0001bf70: 2020 2022 2222 0a0a 636c 6173 7320 536e     """..class Sn
-0001bf80: 6170 7368 6f74 5465 6d70 6f72 6172 696c  apshotTemporaril
-0001bf90: 7955 6e61 7661 696c 6162 6c65 2852 6166  yUnavailable(Raf
-0001bfa0: 7453 746f 7261 6765 4572 726f 7229 3a0a  tStorageError):.
-0001bfb0: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
-0001bfc0: 736e 6170 7368 6f74 2069 7320 6265 696e  snapshot is bein
-0001bfd0: 6720 6372 6561 7465 642e 0a20 2020 2022  g created..    "
-0001bfe0: 2222 0a0a 636c 6173 7320 4f74 6865 7245  ""..class OtherE
-0001bff0: 7272 6f72 2852 6166 7453 746f 7261 6765  rror(RaftStorage
-0001c000: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
-0001c010: 2020 2020 536f 6d65 206f 7468 6572 2065      Some other e
-0001c020: 7272 6f72 206f 6363 7572 7265 642e 0a20  rror occurred.. 
-0001c030: 2020 2022 2222 0a                           """.
+0001a280: 2020 2020 6465 6620 7365 745f 6d61 785f      def set_max_
+0001a290: 636f 6d6d 6974 7465 645f 7369 7a65 5f70  committed_size_p
+0001a2a0: 6572 5f72 6561 6479 280a 2020 2020 2020  er_ready(.      
+0001a2b0: 2020 7365 6c66 2c20 6d61 785f 636f 6d6d    self, max_comm
+0001a2c0: 6974 7465 645f 7369 7a65 5f70 6572 5f72  itted_size_per_r
+0001a2d0: 6561 6479 3a20 696e 740a 2020 2020 2920  eady: int.    ) 
+0001a2e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0001a2f0: 2022 2222 0a20 2020 2020 2020 2060 6d61   """.        `ma
+0001a300: 785f 636f 6d6d 6974 7465 645f 7369 7a65  x_committed_size
+0001a310: 5f70 6572 5f72 6561 6479 603a 204d 6178  _per_ready`: Max
+0001a320: 2073 697a 6520 666f 7220 636f 6d6d 6974   size for commit
+0001a330: 7465 6420 656e 7472 6965 7320 696e 2061  ted entries in a
+0001a340: 2060 5265 6164 7960 2e0a 2020 2020 2020   `Ready`..      
+0001a350: 2020 2222 220a 2020 2020 6465 6620 7661    """.    def va
+0001a360: 6c69 6461 7465 2873 656c 6629 202d 3e20  lidate(self) -> 
+0001a370: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0001a380: 2252 756e 7320 7661 6c69 6461 7469 6f6e  "Runs validation
+0001a390: 7320 6167 6169 6e73 7420 7468 6520 636f  s against the co
+0001a3a0: 6e66 6967 2e22 2222 0a0a 636c 6173 7320  nfig."""..class 
+0001a3b0: 436f 6e66 6967 285f 5f41 5049 5f43 6f6e  Config(__API_Con
+0001a3c0: 6669 6729 3a0a 2020 2020 2222 220a 2020  fig):.    """.  
+0001a3d0: 2020 436f 6e66 6967 2063 6f6e 7461 696e    Config contain
+0001a3e0: 7320 7468 6520 7061 7261 6d65 7465 7273  s the parameters
+0001a3f0: 2074 6f20 7374 6172 7420 6120 7261 6674   to start a raft
+0001a400: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+0001a410: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0001a420: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0001a430: 2020 202a 2c0a 2020 2020 2020 2020 6964     *,.        id
+0001a440: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+0001a450: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0001a460: 656c 6563 7469 6f6e 5f74 6963 6b3a 204f  election_tick: O
+0001a470: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0001a480: 6f6e 652c 0a20 2020 2020 2020 2068 6561  one,.        hea
+0001a490: 7274 6265 6174 5f74 6963 6b3a 204f 7074  rtbeat_tick: Opt
+0001a4a0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0001a4b0: 652c 0a20 2020 2020 2020 2061 7070 6c69  e,.        appli
+0001a4c0: 6564 3a20 4f70 7469 6f6e 616c 5b69 6e74  ed: Optional[int
+0001a4d0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0001a4e0: 2020 6d61 785f 7369 7a65 5f70 6572 5f6d    max_size_per_m
+0001a4f0: 7367 3a20 4f70 7469 6f6e 616c 5b69 6e74  sg: Optional[int
+0001a500: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0001a510: 2020 6d61 785f 696e 666c 6967 6874 5f6d    max_inflight_m
+0001a520: 7367 733a 204f 7074 696f 6e61 6c5b 696e  sgs: Optional[in
+0001a530: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0001a540: 2020 2063 6865 636b 5f71 756f 7275 6d3a     check_quorum:
+0001a550: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
+0001a560: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0001a570: 7072 655f 766f 7465 3a20 4f70 7469 6f6e  pre_vote: Option
+0001a580: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 652c  al[bool] = None,
+0001a590: 0a20 2020 2020 2020 206d 696e 5f65 6c65  .        min_ele
+0001a5a0: 6374 696f 6e5f 7469 636b 3a20 4f70 7469  ction_tick: Opti
+0001a5b0: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001a5c0: 2c0a 2020 2020 2020 2020 6d61 785f 656c  ,.        max_el
+0001a5d0: 6563 7469 6f6e 5f74 6963 6b3a 204f 7074  ection_tick: Opt
+0001a5e0: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0001a5f0: 652c 0a20 2020 2020 2020 2072 6561 645f  e,.        read_
+0001a600: 6f6e 6c79 5f6f 7074 696f 6e3a 204f 7074  only_option: Opt
+0001a610: 696f 6e61 6c5b 2252 6561 644f 6e6c 794f  ional["ReadOnlyO
+0001a620: 7074 696f 6e22 5d20 3d20 4e6f 6e65 2c0a  ption"] = None,.
+0001a630: 2020 2020 2020 2020 736b 6970 5f62 6361          skip_bca
+0001a640: 7374 5f63 6f6d 6d69 743a 204f 7074 696f  st_commit: Optio
+0001a650: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001a660: 2c0a 2020 2020 2020 2020 6261 7463 685f  ,.        batch_
+0001a670: 6170 7065 6e64 3a20 4f70 7469 6f6e 616c  append: Optional
+0001a680: 5b62 6f6f 6c5d 203d 204e 6f6e 652c 0a20  [bool] = None,. 
+0001a690: 2020 2020 2020 2070 7269 6f72 6974 793a         priority:
+0001a6a0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0001a6b0: 204e 6f6e 652c 0a20 2020 2020 2020 206d   None,.        m
+0001a6c0: 6178 5f75 6e63 6f6d 6d69 7474 6564 5f73  ax_uncommitted_s
+0001a6d0: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+0001a6e0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0001a6f0: 2020 206d 6178 5f63 6f6d 6d69 7474 6564     max_committed
+0001a700: 5f73 697a 655f 7065 725f 7265 6164 793a  _size_per_ready:
+0001a710: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0001a720: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+0001a730: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0001a740: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+0001a750: 2069 643a 2054 6865 2069 6465 6e74 6974   id: The identit
+0001a760: 7920 6f66 2074 6865 206c 6f63 616c 2072  y of the local r
+0001a770: 6166 742e 2049 7420 6361 6e6e 6f74 2062  aft. It cannot b
+0001a780: 6520 302c 2061 6e64 206d 7573 7420 6265  e 0, and must be
+0001a790: 2075 6e69 7175 6520 696e 2074 6865 2067   unique in the g
+0001a7a0: 726f 7570 2e0a 0a20 2020 2020 2020 203a  roup...        :
+0001a7b0: 7061 7261 6d20 656c 6563 7469 6f6e 5f74  param election_t
+0001a7c0: 6963 6b3a 2054 6865 206e 756d 6265 7220  ick: The number 
+0001a7d0: 6f66 206e 6f64 652e 7469 636b 2069 6e76  of node.tick inv
+0001a7e0: 6f63 6174 696f 6e73 2074 6861 7420 6d75  ocations that mu
+0001a7f0: 7374 2070 6173 7320 6265 7477 6565 6e0a  st pass between.
+0001a800: 2020 2020 2020 2020 656c 6563 7469 6f6e          election
+0001a810: 732e 2054 6861 7420 6973 2c20 6966 2061  s. That is, if a
+0001a820: 2066 6f6c 6c6f 7765 7220 646f 6573 206e   follower does n
+0001a830: 6f74 2072 6563 6569 7665 2061 6e79 206d  ot receive any m
+0001a840: 6573 7361 6765 2066 726f 6d20 7468 650a  essage from the.
+0001a850: 2020 2020 2020 2020 6c65 6164 6572 206f          leader o
+0001a860: 6620 6375 7272 656e 7420 7465 726d 2062  f current term b
+0001a870: 6566 6f72 6520 456c 6563 7469 6f6e 5469  efore ElectionTi
+0001a880: 636b 2068 6173 2065 6c61 7073 6564 2c20  ck has elapsed, 
+0001a890: 6974 2077 696c 6c20 6265 636f 6d65 0a20  it will become. 
+0001a8a0: 2020 2020 2020 2063 616e 6469 6461 7465         candidate
+0001a8b0: 2061 6e64 2073 7461 7274 2061 6e20 656c   and start an el
+0001a8c0: 6563 7469 6f6e 2e20 656c 6563 7469 6f6e  ection. election
+0001a8d0: 5f74 6963 6b20 6d75 7374 2062 6520 6772  _tick must be gr
+0001a8e0: 6561 7465 7220 7468 616e 0a20 2020 2020  eater than.     
+0001a8f0: 2020 2048 6561 7274 6265 6174 5469 636b     HeartbeatTick
+0001a900: 2e20 5765 2073 7567 6765 7374 2065 6c65  . We suggest ele
+0001a910: 6374 696f 6e5f 7469 636b 203d 2031 3020  ction_tick = 10 
+0001a920: 2a20 4865 6172 7462 6561 7454 6963 6b20  * HeartbeatTick 
+0001a930: 746f 2061 766f 6964 0a20 2020 2020 2020  to avoid.       
+0001a940: 2075 6e6e 6563 6573 7361 7279 206c 6561   unnecessary lea
+0001a950: 6465 7220 7377 6974 6368 696e 670a 0a20  der switching.. 
+0001a960: 2020 2020 2020 203a 7061 7261 6d20 6865         :param he
+0001a970: 6172 7462 6561 745f 7469 636b 3a20 4865  artbeat_tick: He
+0001a980: 6172 7462 6561 7454 6963 6b20 6973 2074  artbeatTick is t
+0001a990: 6865 206e 756d 6265 7220 6f66 206e 6f64  he number of nod
+0001a9a0: 652e 7469 636b 2069 6e76 6f63 6174 696f  e.tick invocatio
+0001a9b0: 6e73 2074 6861 7420 6d75 7374 2070 6173  ns that must pas
+0001a9c0: 7320 6265 7477 6565 6e0a 2020 2020 2020  s between.      
+0001a9d0: 2020 6865 6172 7462 6561 7473 2e20 5468    heartbeats. Th
+0001a9e0: 6174 2069 732c 2061 206c 6561 6465 7220  at is, a leader 
+0001a9f0: 7365 6e64 7320 6865 6172 7462 6561 7420  sends heartbeat 
+0001aa00: 6d65 7373 6167 6573 2074 6f20 6d61 696e  messages to main
+0001aa10: 7461 696e 2069 7473 0a20 2020 2020 2020  tain its.       
+0001aa20: 206c 6561 6465 7273 6869 7020 6576 6572   leadership ever
+0001aa30: 7920 6865 6172 7462 6561 7420 7469 636b  y heartbeat tick
+0001aa40: 732e 0a0a 2020 2020 2020 2020 3a70 6172  s...        :par
+0001aa50: 616d 2061 7070 6c69 6564 3a20 4170 706c  am applied: Appl
+0001aa60: 6965 6420 6973 2074 6865 206c 6173 7420  ied is the last 
+0001aa70: 6170 706c 6965 6420 696e 6465 782e 2049  applied index. I
+0001aa80: 7420 7368 6f75 6c64 206f 6e6c 7920 6265  t should only be
+0001aa90: 2073 6574 2077 6865 6e20 7265 7374 6172   set when restar
+0001aaa0: 7469 6e67 0a20 2020 2020 2020 2072 6166  ting.        raf
+0001aab0: 742e 2072 6166 7420 7769 6c6c 206e 6f74  t. raft will not
+0001aac0: 2072 6574 7572 6e20 656e 7472 6965 7320   return entries 
+0001aad0: 746f 2074 6865 2061 7070 6c69 6361 7469  to the applicati
+0001aae0: 6f6e 2073 6d61 6c6c 6572 206f 7220 6571  on smaller or eq
+0001aaf0: 7561 6c20 746f 2041 7070 6c69 6564 2e0a  ual to Applied..
+0001ab00: 2020 2020 2020 2020 4966 2041 7070 6c69          If Appli
+0001ab10: 6564 2069 7320 756e 7365 7420 7768 656e  ed is unset when
+0001ab20: 2072 6573 7461 7274 696e 672c 2072 6166   restarting, raf
+0001ab30: 7420 6d69 6768 7420 7265 7475 726e 2070  t might return p
+0001ab40: 7265 7669 6f75 7320 6170 706c 6965 6420  revious applied 
+0001ab50: 656e 7472 6965 732e 0a20 2020 2020 2020  entries..       
+0001ab60: 2054 6869 7320 6973 2061 2076 6572 7920   This is a very 
+0001ab70: 6170 706c 6963 6174 696f 6e20 6465 7065  application depe
+0001ab80: 6e64 656e 7420 636f 6e66 6967 7572 6174  ndent configurat
+0001ab90: 696f 6e2e 0a0a 2020 2020 2020 2020 3a70  ion...        :p
+0001aba0: 6172 616d 206d 6178 5f73 697a 655f 7065  aram max_size_pe
+0001abb0: 725f 6d73 673a 204c 696d 6974 2074 6865  r_msg: Limit the
+0001abc0: 206d 6178 2073 697a 6520 6f66 2065 6163   max size of eac
+0001abd0: 6820 6170 7065 6e64 206d 6573 7361 6765  h append message
+0001abe0: 2e20 536d 616c 6c65 7220 7661 6c75 6520  . Smaller value 
+0001abf0: 6c6f 7765 7273 0a20 2020 2020 2020 2074  lowers.        t
+0001ac00: 6865 2072 6166 7420 7265 636f 7665 7279  he raft recovery
+0001ac10: 2063 6f73 7428 696e 6974 6961 6c20 7072   cost(initial pr
+0001ac20: 6f62 696e 6720 616e 6420 6d65 7373 6167  obing and messag
+0001ac30: 6520 6c6f 7374 2064 7572 696e 6720 6e6f  e lost during no
+0001ac40: 726d 616c 206f 7065 7261 7469 6f6e 292e  rmal operation).
+0001ac50: 0a20 2020 2020 2020 204f 6e20 7468 6520  .        On the 
+0001ac60: 6f74 6865 7220 7369 6465 2c20 6974 206d  other side, it m
+0001ac70: 6967 6874 2061 6666 6563 7420 7468 6520  ight affect the 
+0001ac80: 7468 726f 7567 6870 7574 2064 7572 696e  throughput durin
+0001ac90: 6720 6e6f 726d 616c 2072 6570 6c69 6361  g normal replica
+0001aca0: 7469 6f6e 2e0a 2020 2020 2020 2020 4e6f  tion..        No
+0001acb0: 7465 3a20 6d61 7468 2e4d 6178 5575 7369  te: math.MaxUusi
+0001acc0: 7a65 3634 2066 6f72 2075 6e6c 696d 6974  ze64 for unlimit
+0001acd0: 6564 2c20 3020 666f 7220 6174 206d 6f73  ed, 0 for at mos
+0001ace0: 7420 6f6e 6520 656e 7472 7920 7065 7220  t one entry per 
+0001acf0: 6d65 7373 6167 652e 0a0a 2020 2020 2020  message...      
+0001ad00: 2020 3a70 6172 616d 206d 6178 5f69 6e66    :param max_inf
+0001ad10: 6c69 6768 745f 6d73 6773 3a20 4c69 6d69  light_msgs: Limi
+0001ad20: 7420 7468 6520 6d61 7820 6e75 6d62 6572  t the max number
+0001ad30: 206f 6620 696e 2d66 6c69 6768 7420 6170   of in-flight ap
+0001ad40: 7065 6e64 206d 6573 7361 6765 7320 6475  pend messages du
+0001ad50: 7269 6e67 206f 7074 696d 6973 7469 630a  ring optimistic.
+0001ad60: 2020 2020 2020 2020 7265 706c 6963 6174          replicat
+0001ad70: 696f 6e20 7068 6173 652e 2054 6865 2061  ion phase. The a
+0001ad80: 7070 6c69 6361 7469 6f6e 2074 7261 6e73  pplication trans
+0001ad90: 706f 7274 6174 696f 6e20 6c61 7965 7220  portation layer 
+0001ada0: 7573 7561 6c6c 7920 6861 7320 6974 7320  usually has its 
+0001adb0: 6f77 6e20 7365 6e64 696e 670a 2020 2020  own sending.    
+0001adc0: 2020 2020 6275 6666 6572 206f 7665 7220      buffer over 
+0001add0: 5443 502f 5544 502e 2053 6574 2074 6f20  TCP/UDP. Set to 
+0001ade0: 6176 6f69 6420 6f76 6572 666c 6f77 696e  avoid overflowin
+0001adf0: 6720 7468 6174 2073 656e 6469 6e67 2062  g that sending b
+0001ae00: 7566 6665 722e 0a0a 2020 2020 2020 2020  uffer...        
+0001ae10: 3a70 6172 616d 2063 6865 636b 5f71 756f  :param check_quo
+0001ae20: 7275 6d3a 2053 7065 6369 6679 2069 6620  rum: Specify if 
+0001ae30: 7468 6520 6c65 6164 6572 2073 686f 756c  the leader shoul
+0001ae40: 6420 6368 6563 6b20 7175 6f72 756d 2061  d check quorum a
+0001ae50: 6374 6976 6974 792e 204c 6561 6465 7220  ctivity. Leader 
+0001ae60: 7374 6570 7320 646f 776e 2077 6865 6e0a  steps down when.
+0001ae70: 2020 2020 2020 2020 7175 6f72 756d 2069          quorum i
+0001ae80: 7320 6e6f 7420 6163 7469 7665 2066 6f72  s not active for
+0001ae90: 2061 6e20 656c 6563 7469 6f6e 5469 6d65   an electionTime
+0001aea0: 6f75 742e 0a0a 2020 2020 2020 2020 3a70  out...        :p
+0001aeb0: 6172 616d 2070 7265 5f76 6f74 653a 2045  aram pre_vote: E
+0001aec0: 6e61 626c 6573 2074 6865 2050 7265 2d56  nables the Pre-V
+0001aed0: 6f74 6520 616c 676f 7269 7468 6d20 6465  ote algorithm de
+0001aee0: 7363 7269 6265 6420 696e 2072 6166 7420  scribed in raft 
+0001aef0: 7468 6573 6973 2073 6563 7469 6f6e 0a20  thesis section. 
+0001af00: 2020 2020 2020 2039 2e36 2e20 5468 6973         9.6. This
+0001af10: 2070 7265 7665 6e74 7320 6469 7372 7570   prevents disrup
+0001af20: 7469 6f6e 2077 6865 6e20 6120 6e6f 6465  tion when a node
+0001af30: 2074 6861 7420 6861 7320 6265 656e 2070   that has been p
+0001af40: 6172 7469 7469 6f6e 6564 2061 7761 790a  artitioned away.
+0001af50: 2020 2020 2020 2020 7265 6a6f 696e 7320          rejoins 
+0001af60: 7468 6520 636c 7573 7465 722e 0a0a 2020  the cluster...  
+0001af70: 2020 2020 2020 3a70 6172 616d 206d 696e        :param min
+0001af80: 5f65 6c65 6374 696f 6e5f 7469 636b 3a20  _election_tick: 
+0001af90: 5468 6520 7261 6e67 6520 6f66 2065 6c65  The range of ele
+0001afa0: 6374 696f 6e20 7469 6d65 6f75 742e 2049  ction timeout. I
+0001afb0: 6e20 736f 6d65 2063 6173 6573 2c20 7765  n some cases, we
+0001afc0: 2068 6f70 6520 736f 6d65 206e 6f64 6573   hope some nodes
+0001afd0: 2068 6173 206c 6573 7320 706f 7373 6962   has less possib
+0001afe0: 696c 6974 790a 2020 2020 2020 2020 746f  ility.        to
+0001aff0: 2062 6563 6f6d 6520 6c65 6164 6572 2e20   become leader. 
+0001b000: 5468 6973 2063 6f6e 6669 6775 7261 7469  This configurati
+0001b010: 6f6e 2065 6e73 7572 6573 2074 6861 7420  on ensures that 
+0001b020: 7468 6520 7261 6e64 6f6d 697a 6564 2065  the randomized e
+0001b030: 6c65 6374 696f 6e5f 7469 6d65 6f75 740a  lection_timeout.
+0001b040: 2020 2020 2020 2020 7769 6c6c 2061 6c77          will alw
+0001b050: 6179 7320 6265 2073 7569 7420 696e 205b  ays be suit in [
+0001b060: 6d69 6e5f 656c 6563 7469 6f6e 5f74 6963  min_election_tic
+0001b070: 6b2c 206d 6178 5f65 6c65 6374 696f 6e5f  k, max_election_
+0001b080: 7469 636b 292e 0a20 2020 2020 2020 2049  tick)..        I
+0001b090: 6620 6974 2069 7320 302c 2074 6865 6e20  f it is 0, then 
+0001b0a0: 656c 6563 7469 6f6e 5f74 6963 6b20 7769  election_tick wi
+0001b0b0: 6c6c 2062 6520 6368 6f73 656e 2e0a 0a20  ll be chosen... 
+0001b0c0: 2020 2020 2020 203a 7061 7261 6d20 6d61         :param ma
+0001b0d0: 785f 656c 6563 7469 6f6e 5f74 6963 6b3a  x_election_tick:
+0001b0e0: 2049 6620 6974 2069 7320 302c 2074 6865   If it is 0, the
+0001b0f0: 6e20 3220 2a20 656c 6563 7469 6f6e 5f74  n 2 * election_t
+0001b100: 6963 6b20 7769 6c6c 2062 6520 6368 6f73  ick will be chos
+0001b110: 656e 2e0a 0a20 2020 2020 2020 203a 7061  en...        :pa
+0001b120: 7261 6d20 7265 6164 5f6f 6e6c 795f 6f70  ram read_only_op
+0001b130: 7469 6f6e 3a20 4368 6f6f 7365 2074 6865  tion: Choose the
+0001b140: 206c 696e 6561 7269 7a61 6269 6c69 7479   linearizability
+0001b150: 206d 6f64 6520 6f72 2074 6865 206c 6561   mode or the lea
+0001b160: 7365 206d 6f64 6520 746f 2072 6561 6420  se mode to read 
+0001b170: 6461 7461 2e20 4966 2079 6f75 2064 6f6e  data. If you don
+0001b180: e280 9974 2063 6172 6520 6162 6f75 7420  ...t care about 
+0001b190: 7468 6520 7265 6164 2063 6f6e 7369 7374  the read consist
+0001b1a0: 656e 6379 2061 6e64 2077 616e 7420 6120  ency and want a 
+0001b1b0: 6869 6768 6572 2072 6561 6420 7065 7266  higher read perf
+0001b1c0: 6f72 6d61 6e63 652c 2079 6f75 2063 616e  ormance, you can
+0001b1d0: 2075 7365 2074 6865 206c 6561 7365 206d   use the lease m
+0001b1e0: 6f64 652e 0a20 2020 2020 2020 2053 6574  ode..        Set
+0001b1f0: 7469 6e67 2074 6869 7320 746f 2060 4c65  ting this to `Le
+0001b200: 6173 6542 6173 6564 6020 7265 7175 6972  aseBased` requir
+0001b210: 6573 2060 6368 6563 6b5f 7175 6f72 756d  es `check_quorum
+0001b220: 203d 2074 7275 6560 2e0a 0a20 2020 2020   = true`...     
+0001b230: 2020 203a 7061 7261 6d20 736b 6970 5f62     :param skip_b
+0001b240: 6361 7374 5f63 6f6d 6d69 743a 2044 6f6e  cast_commit: Don
+0001b250: 2774 2062 726f 6164 6361 7374 2061 6e20  't broadcast an 
+0001b260: 656d 7074 7920 7261 6674 2065 6e74 7279  empty raft entry
+0001b270: 2074 6f20 6e6f 7469 6679 2066 6f6c 6c6f   to notify follo
+0001b280: 7765 7220 746f 2063 6f6d 6d69 7420 616e  wer to commit an
+0001b290: 2065 6e74 7279 2e0a 2020 2020 2020 2020   entry..        
+0001b2a0: 5468 6973 206d 6179 206d 616b 6520 666f  This may make fo
+0001b2b0: 6c6c 6f77 6572 2077 6169 7420 6120 6c6f  llower wait a lo
+0001b2c0: 6e67 6572 2074 696d 6520 746f 2061 7070  nger time to app
+0001b2d0: 6c79 2061 6e20 656e 7472 792e 2054 6869  ly an entry. Thi
+0001b2e0: 7320 636f 6e66 6967 7572 6174 696f 6e0a  s configuration.
+0001b2f0: 2020 2020 2020 2020 4d61 7920 6166 6665          May affe
+0001b300: 6374 2070 726f 706f 7361 6c20 666f 7277  ct proposal forw
+0001b310: 6172 6469 6e67 2061 6e64 2066 6f6c 6c6f  arding and follo
+0001b320: 7765 7220 7265 6164 2e0a 0a20 2020 2020  wer read...     
+0001b330: 2020 203a 7061 7261 6d20 6261 7463 685f     :param batch_
+0001b340: 6170 7065 6e64 3a20 4261 7463 6865 7320  append: Batches 
+0001b350: 6576 6572 7920 6170 7065 6e64 206d 7367  every append msg
+0001b360: 2069 6620 616e 7920 6170 7065 6e64 206d   if any append m
+0001b370: 7367 2061 6c72 6561 6479 2065 7869 7374  sg already exist
+0001b380: 730a 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+0001b390: 6d20 7072 696f 7269 7479 3a20 5468 6520  m priority: The 
+0001b3a0: 656c 6563 7469 6f6e 2070 7269 6f72 6974  election priorit
+0001b3b0: 7920 6f66 2074 6869 7320 6e6f 6465 2e0a  y of this node..
+0001b3c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0001b3d0: 6d61 785f 756e 636f 6d6d 6974 7465 645f  max_uncommitted_
+0001b3e0: 7369 7a65 3a20 5370 6563 6966 7920 6d61  size: Specify ma
+0001b3f0: 7869 6d75 6d20 6f66 2075 6e63 6f6d 6d69  ximum of uncommi
+0001b400: 7474 6564 2065 6e74 7279 2073 697a 652e  tted entry size.
+0001b410: 0a20 2020 2020 2020 2057 6865 6e20 7468  .        When th
+0001b420: 6973 206c 696d 6974 2069 7320 7265 6163  is limit is reac
+0001b430: 6865 642c 2061 6c6c 2070 726f 706f 7361  hed, all proposa
+0001b440: 6c73 2074 6f20 6170 7065 6e64 206e 6577  ls to append new
+0001b450: 206c 6f67 2077 696c 6c20 6265 2064 726f   log will be dro
+0001b460: 7070 6564 0a0a 2020 2020 2020 2020 3a70  pped..        :p
+0001b470: 6172 616d 206d 6178 5f63 6f6d 6d69 7474  aram max_committ
+0001b480: 6564 5f73 697a 655f 7065 725f 7265 6164  ed_size_per_read
+0001b490: 793a 204d 6178 2073 697a 6520 666f 7220  y: Max size for 
+0001b4a0: 636f 6d6d 6974 7465 6420 656e 7472 6965  committed entrie
+0001b4b0: 7320 696e 2061 2060 5265 6164 7960 2e0a  s in a `Ready`..
+0001b4c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001b4d0: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
+0001b4e0: 6629 202d 3e20 2243 6f6e 6669 6752 6566  f) -> "ConfigRef
+0001b4f0: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
+0001b500: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0001b510: 2064 6566 6175 6c74 2829 202d 3e20 2243   default() -> "C
+0001b520: 6f6e 6669 6722 3a20 2e2e 2e0a 0a63 6c61  onfig": .....cla
+0001b530: 7373 2043 6f6e 6669 6752 6566 285f 5f41  ss ConfigRef(__A
+0001b540: 5049 5f43 6f6e 6669 6729 3a0a 2020 2020  PI_Config):.    
+0001b550: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
+0001b560: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
+0001b570: 3a60 496e 666c 6967 6874 7352 6566 602e  :`InflightsRef`.
+0001b580: 0a20 2020 2022 2222 0a0a 2320 544f 444f  .    """..# TODO
+0001b590: 3a20 4164 6420 6265 6c6f 7720 696d 706c  : Add below impl
+0001b5a0: 656d 656e 7461 7469 6f6e 2069 6620 6e65  ementation if ne
+0001b5b0: 6564 6564 2c20 6f74 6865 7277 6973 6520  eded, otherwise 
+0001b5c0: 7265 6d6f 7665 2062 656c 6f77 2063 6f64  remove below cod
+0001b5d0: 6573 2e0a 2320 636c 6173 7320 5f5f 4150  es..# class __AP
+0001b5e0: 495f 5374 6174 7573 3a0a 2320 2020 2020  I_Status:.#     
+0001b5f0: 6465 6620 6765 745f 6170 706c 6965 6428  def get_applied(
+0001b600: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2320  self) -> int:.# 
+0001b610: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0001b620: 2320 2020 2020 6465 6620 7365 745f 6170  #     def set_ap
+0001b630: 706c 6965 6428 7365 6c66 2c20 6170 706c  plied(self, appl
+0001b640: 6965 643a 2069 6e74 2920 2d3e 204e 6f6e  ied: int) -> Non
+0001b650: 653a 0a23 2020 2020 2020 2020 2022 2222  e:.#         """
+0001b660: 2022 2222 0a23 2020 2020 2064 6566 2067   """.#     def g
+0001b670: 6574 5f69 6428 7365 6c66 2920 2d3e 2069  et_id(self) -> i
+0001b680: 6e74 3a0a 2320 2020 2020 2020 2020 2222  nt:.#         ""
+0001b690: 2220 2222 220a 2320 2020 2020 6465 6620  " """.#     def 
+0001b6a0: 7365 745f 6964 2873 656c 662c 2069 643a  set_id(self, id:
+0001b6b0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a23   int) -> None:.#
+0001b6c0: 2020 2020 2020 2020 2022 2222 2022 2222           """ """
+0001b6d0: 0a23 2020 2020 2064 6566 2067 6574 5f68  .#     def get_h
+0001b6e0: 7328 7365 6c66 2920 2d3e 2048 6172 6453  s(self) -> HardS
+0001b6f0: 7461 7465 5265 663a 0a23 2020 2020 2020  tateRef:.#      
+0001b700: 2020 2022 2222 2022 2222 0a23 2020 2020     """ """.#    
+0001b710: 2064 6566 2073 6574 5f68 7328 7365 6c66   def set_hs(self
+0001b720: 2c20 6873 3a20 4861 7264 5374 6174 6552  , hs: HardStateR
+0001b730: 6566 2920 2d3e 204e 6f6e 653a 0a23 2020  ef) -> None:.#  
+0001b740: 2020 2020 2020 2022 2222 2022 2222 0a23         """ """.#
+0001b750: 2020 2020 2064 6566 2067 6574 5f73 7328       def get_ss(
+0001b760: 7365 6c66 2920 2d3e 2053 6f66 7453 7461  self) -> SoftSta
+0001b770: 7465 5265 663a 0a23 2020 2020 2020 2020  teRef:.#        
+0001b780: 2022 2222 2022 2222 0a23 2020 2020 2064   """ """.#     d
+0001b790: 6566 2073 6574 5f73 7328 7365 6c66 2c20  ef set_ss(self, 
+0001b7a0: 7373 3a20 536f 6674 5374 6174 6552 6566  ss: SoftStateRef
+0001b7b0: 2920 2d3e 204e 6f6e 653a 0a23 2020 2020  ) -> None:.#    
+0001b7c0: 2020 2020 2022 2222 2022 2222 0a23 2020       """ """.#  
+0001b7d0: 2020 2064 6566 2067 6574 5f70 726f 6772     def get_progr
+0001b7e0: 6573 7328 7365 6c66 2920 2d3e 204f 7074  ess(self) -> Opt
+0001b7f0: 696f 6e61 6c5b 5072 6f67 7265 7373 5472  ional[ProgressTr
+0001b800: 6163 6b65 7252 6566 5d3a 0a23 2020 2020  ackerRef]:.#    
+0001b810: 2020 2020 2022 2222 2022 2222 0a23 2020       """ """.#  
+0001b820: 2020 2064 6566 2073 6574 5f70 726f 6772     def set_progr
+0001b830: 6573 7328 0a23 2020 2020 2020 2020 2073  ess(.#         s
+0001b840: 656c 662c 2074 7261 636b 6572 3a20 4f70  elf, tracker: Op
+0001b850: 7469 6f6e 616c 5b50 726f 6772 6573 7354  tional[ProgressT
+0001b860: 7261 636b 6572 5d20 7c20 4f70 7469 6f6e  racker] | Option
+0001b870: 616c 5b50 726f 6772 6573 7354 7261 636b  al[ProgressTrack
+0001b880: 6572 5265 665d 0a23 2020 2020 2029 202d  erRef].#     ) -
+0001b890: 3e20 4e6f 6e65 3a0a 2320 2020 2020 2020  > None:.#       
+0001b8a0: 2020 2222 2220 2222 220a 0a23 2063 6c61    """ """..# cla
+0001b8b0: 7373 2049 6e4d 656d 6f72 7953 7461 7475  ss InMemoryStatu
+0001b8c0: 7328 5f5f 4150 495f 5374 6174 7573 293a  s(__API_Status):
+0001b8d0: 0a23 2020 2020 2022 2222 0a23 2020 2020  .#     """.#    
+0001b8e0: 2052 6570 7265 7365 6e74 7320 7468 6520   Represents the 
+0001b8f0: 6375 7272 656e 7420 7374 6174 7573 206f  current status o
+0001b900: 6620 7468 6520 7261 6674 0a23 2020 2020  f the raft.#    
+0001b910: 2022 2222 0a0a 2320 2020 2020 6465 6620   """..#     def 
+0001b920: 5f5f 696e 6974 5f5f 2873 656c 662c 2072  __init__(self, r
+0001b930: 6166 743a 2049 6e4d 656d 6f72 7952 6166  aft: InMemoryRaf
+0001b940: 7429 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  t) -> None: ....
+0001b950: 2320 2020 2020 6465 6620 6d61 6b65 5f72  #     def make_r
+0001b960: 6566 2873 656c 6629 202d 3e20 5374 6174  ef(self) -> Stat
+0001b970: 7573 5f5f 4d65 6d73 746f 7261 6765 5265  us__MemstorageRe
+0001b980: 663a 202e 2e2e 0a0a 2320 636c 6173 7320  f: .....# class 
+0001b990: 496e 4d65 6d6f 7279 5374 6174 7573 5265  InMemoryStatusRe
+0001b9a0: 6628 5f5f 4150 495f 5374 6174 7573 293a  f(__API_Status):
+0001b9b0: 0a23 2020 2020 2022 2222 0a23 2020 2020  .#     """.#    
+0001b9c0: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+0001b9d0: 6f66 203a 636c 6173 733a 6053 7461 7475  of :class:`Statu
+0001b9e0: 735f 5f4d 656d 7374 6f72 6167 6560 2e0a  s__Memstorage`..
+0001b9f0: 2320 2020 2020 2222 220a 0a63 6c61 7373  #     """..class
+0001ba00: 2044 6573 7472 6f79 6564 5265 6655 7365   DestroyedRefUse
+0001ba10: 6445 7272 6f72 2845 7863 6570 7469 6f6e  dError(Exception
+0001ba20: 293a 0a20 2020 2022 2222 2022 2222 0a0a  ):.    """ """..
+0001ba30: 636c 6173 7320 5261 6674 4572 726f 7228  class RaftError(
+0001ba40: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+0001ba50: 2222 2220 2222 220a 0a63 6c61 7373 2045  """ """..class E
+0001ba60: 7869 7374 7345 7272 6f72 2852 6166 7445  xistsError(RaftE
+0001ba70: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
+0001ba80: 2020 2054 6865 206e 6f64 6520 7b69 647d     The node {id}
+0001ba90: 2061 6c72 6561 6479 2065 7869 7374 7320   already exists 
+0001baa0: 696e 2074 6865 207b 7365 747d 2073 6574  in the {set} set
+0001bab0: 2e0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
+0001bac0: 643a 2069 6e74 0a20 2020 2073 6574 3a20  d: int.    set: 
+0001bad0: 7374 720a 0a63 6c61 7373 204e 6f74 4578  str..class NotEx
+0001bae0: 6973 7473 2852 6166 7445 7272 6f72 293a  ists(RaftError):
+0001baf0: 0a20 2020 2022 2222 0a20 2020 2054 6865  .    """.    The
+0001bb00: 206e 6f64 6520 7b69 647d 2069 7320 6e6f   node {id} is no
+0001bb10: 7420 696e 2074 6865 207b 7365 747d 2073  t in the {set} s
+0001bb20: 6574 2e0a 2020 2020 2222 220a 0a20 2020  et..    """..   
+0001bb30: 2069 643a 2069 6e74 0a20 2020 2073 6574   id: int.    set
+0001bb40: 3a20 7374 720a 0a63 6c61 7373 2043 6f64  : str..class Cod
+0001bb50: 6563 4572 726f 7228 5261 6674 4572 726f  ecError(RaftErro
+0001bb60: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
+0001bb70: 4120 7072 6f74 6f62 7566 206d 6573 7361  A protobuf messa
+0001bb80: 6765 2063 6f64 6563 2066 6169 6c65 6420  ge codec failed 
+0001bb90: 696e 2073 6f6d 6520 6d61 6e6e 6572 2e0a  in some manner..
+0001bba0: 2020 2020 2222 220a 0a63 6c61 7373 2043      """..class C
+0001bbb0: 6f6e 6669 6749 6e76 616c 6964 4572 726f  onfigInvalidErro
+0001bbc0: 7228 5261 6674 4572 726f 7229 3a0a 2020  r(RaftError):.  
+0001bbd0: 2020 2222 220a 2020 2020 5468 6520 636f    """.    The co
+0001bbe0: 6e66 6967 7572 6174 696f 6e20 6973 2069  nfiguration is i
+0001bbf0: 6e76 616c 6964 2e0a 2020 2020 2222 220a  nvalid..    """.
+0001bc00: 0a63 6c61 7373 2050 726f 706f 7361 6c44  .class ProposalD
+0001bc10: 726f 7070 6564 4572 726f 7228 5261 6674  roppedError(Raft
+0001bc20: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
+0001bc30: 2020 2020 5468 6520 7072 6f70 6f73 616c      The proposal
+0001bc40: 206f 6620 6368 616e 6765 7320 7761 7320   of changes was 
+0001bc50: 6472 6f70 7065 642e 0a20 2020 2022 2222  dropped..    """
+0001bc60: 0a0a 636c 6173 7320 5265 7175 6573 7453  ..class RequestS
+0001bc70: 6e61 7073 686f 7444 726f 7070 6564 4572  napshotDroppedEr
+0001bc80: 726f 7228 5261 6674 4572 726f 7229 3a0a  ror(RaftError):.
+0001bc90: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
+0001bca0: 7265 7175 6573 7420 736e 6170 7368 6f74  request snapshot
+0001bcb0: 2069 7320 6472 6f70 7065 642e 0a20 2020   is dropped..   
+0001bcc0: 2022 2222 0a0a 636c 6173 7320 436f 6e66   """..class Conf
+0001bcd0: 4368 616e 6765 4572 726f 7228 5261 6674  ChangeError(Raft
+0001bce0: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
+0001bcf0: 2020 2020 436f 6e66 4368 616e 6765 2070      ConfChange p
+0001bd00: 726f 706f 7361 6c20 6973 2069 6e76 616c  roposal is inval
+0001bd10: 6964 2e0a 2020 2020 2222 220a 0a63 6c61  id..    """..cla
+0001bd20: 7373 2049 6f45 7272 6f72 2852 6166 7445  ss IoError(RaftE
+0001bd30: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
+0001bd40: 2020 2041 6e20 494f 2065 7272 6f72 206f     An IO error o
+0001bd50: 6363 7572 7265 642e 0a20 2020 2022 2222  ccurred..    """
+0001bd60: 0a0a 636c 6173 7320 5374 6f72 6545 7272  ..class StoreErr
+0001bd70: 6f72 2852 6166 7445 7272 6f72 293a 0a20  or(RaftError):. 
+0001bd80: 2020 2022 2222 0a20 2020 2041 2073 746f     """.    A sto
+0001bd90: 7261 6765 2065 7272 6f72 206f 6363 7572  rage error occur
+0001bda0: 7265 642e 0a20 2020 2022 2222 0a0a 636c  red..    """..cl
+0001bdb0: 6173 7320 5374 6570 4c6f 6361 6c4d 7367  ass StepLocalMsg
+0001bdc0: 2852 6166 7445 7272 6f72 293a 0a20 2020  (RaftError):.   
+0001bdd0: 2022 2222 0a20 2020 2052 6166 7420 6361   """.    Raft ca
+0001bde0: 6e6e 6f74 2073 7465 7020 7468 6520 6c6f  nnot step the lo
+0001bdf0: 6361 6c20 6d65 7373 6167 652e 0a20 2020  cal message..   
+0001be00: 2022 2222 0a0a 636c 6173 7320 5374 6570   """..class Step
+0001be10: 5065 6572 4e6f 7446 6f75 6e64 2852 6166  PeerNotFound(Raf
+0001be20: 7445 7272 6f72 293a 0a20 2020 2022 2222  tError):.    """
+0001be30: 0a20 2020 2054 6865 2072 6166 7420 7065  .    The raft pe
+0001be40: 6572 2069 7320 6e6f 7420 666f 756e 6420  er is not found 
+0001be50: 616e 6420 7468 7573 2063 616e 6e6f 7420  and thus cannot 
+0001be60: 7374 6570 2e0a 2020 2020 2222 220a 0a63  step..    """..c
+0001be70: 6c61 7373 2052 6166 7453 746f 7261 6765  lass RaftStorage
+0001be80: 4572 726f 7228 4578 6365 7074 696f 6e29  Error(Exception)
+0001be90: 3a0a 2020 2020 2222 220a 2020 2020 416e  :.    """.    An
+0001bea0: 2065 7272 6f72 2077 6974 6820 7468 6520   error with the 
+0001beb0: 7374 6f72 6167 652e 0a20 2020 2022 2222  storage..    """
+0001bec0: 0a0a 636c 6173 7320 436f 6d70 6163 7465  ..class Compacte
+0001bed0: 6445 7272 6f72 2852 6166 7453 746f 7261  dError(RaftStora
+0001bee0: 6765 4572 726f 7229 3a0a 2020 2020 2222  geError):.    ""
+0001bef0: 220a 2020 2020 5468 6520 7374 6f72 6167  ".    The storag
+0001bf00: 6520 7761 7320 636f 6d70 6163 7465 6420  e was compacted 
+0001bf10: 616e 6420 6e6f 7420 6163 6365 7373 6962  and not accessib
+0001bf20: 6c65 0a20 2020 2022 2222 0a0a 636c 6173  le.    """..clas
+0001bf30: 7320 556e 6176 6169 6c61 626c 6545 7272  s UnavailableErr
+0001bf40: 6f72 2852 6166 7453 746f 7261 6765 4572  or(RaftStorageEr
+0001bf50: 726f 7229 3a0a 2020 2020 2222 220a 2020  ror):.    """.  
+0001bf60: 2020 5468 6520 6c6f 6720 6973 206e 6f74    The log is not
+0001bf70: 2061 7661 696c 6162 6c65 2e0a 2020 2020   available..    
+0001bf80: 2222 220a 0a63 6c61 7373 204c 6f67 5465  """..class LogTe
+0001bf90: 6d70 6f72 6172 696c 7955 6e61 7661 696c  mporarilyUnavail
+0001bfa0: 6162 6c65 4572 726f 7228 5261 6674 5374  ableError(RaftSt
+0001bfb0: 6f72 6167 6545 7272 6f72 293a 0a20 2020  orageError):.   
+0001bfc0: 2022 2222 0a20 2020 2054 6865 206c 6f67   """.    The log
+0001bfd0: 2069 7320 6265 696e 6720 6665 7463 6865   is being fetche
+0001bfe0: 642e 0a20 2020 2022 2222 0a0a 636c 6173  d..    """..clas
+0001bff0: 7320 536e 6170 7368 6f74 4f75 744f 6644  s SnapshotOutOfD
+0001c000: 6174 6545 7272 6f72 2852 6166 7453 746f  ateError(RaftSto
+0001c010: 7261 6765 4572 726f 7229 3a0a 2020 2020  rageError):.    
+0001c020: 2222 220a 2020 2020 5468 6520 736e 6170  """.    The snap
+0001c030: 7368 6f74 2069 7320 6f75 7420 6f66 2064  shot is out of d
+0001c040: 6174 652e 0a20 2020 2022 2222 0a0a 636c  ate..    """..cl
+0001c050: 6173 7320 536e 6170 7368 6f74 5465 6d70  ass SnapshotTemp
+0001c060: 6f72 6172 696c 7955 6e61 7661 696c 6162  orarilyUnavailab
+0001c070: 6c65 2852 6166 7453 746f 7261 6765 4572  le(RaftStorageEr
+0001c080: 726f 7229 3a0a 2020 2020 2222 220a 2020  ror):.    """.  
+0001c090: 2020 5468 6520 736e 6170 7368 6f74 2069    The snapshot i
+0001c0a0: 7320 6265 696e 6720 6372 6561 7465 642e  s being created.
+0001c0b0: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+0001c0c0: 4f74 6865 7245 7272 6f72 2852 6166 7453  OtherError(RaftS
+0001c0d0: 746f 7261 6765 4572 726f 7229 3a0a 2020  torageError):.  
+0001c0e0: 2020 2222 220a 2020 2020 536f 6d65 206f    """.    Some o
+0001c0f0: 7468 6572 2065 7272 6f72 206f 6363 7572  ther error occur
+0001c100: 7265 642e 0a20 2020 2022 2222 0a         red..    """.
```

### Comparing `rraft_py-0.1.2/src/bindings/config.rs` & `rraft_py-0.1.3/src/bindings/config.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/get_entries_context.rs` & `rraft_py-0.1.3/src/bindings/get_entries_context.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/global.rs` & `rraft_py-0.1.3/src/bindings/global.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/inflights.rs` & `rraft_py-0.1.3/src/bindings/inflights.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/joint_config.rs` & `rraft_py-0.1.3/src/bindings/joint_config.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/light_ready.rs` & `rraft_py-0.1.3/src/bindings/light_ready.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/majority_config.rs` & `rraft_py-0.1.3/src/bindings/majority_config.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/peer.rs` & `rraft_py-0.1.3/src/bindings/peer.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/progress.rs` & `rraft_py-0.1.3/src/bindings/progress.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/progress_state.rs` & `rraft_py-0.1.3/src/bindings/progress_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/progress_tracker.rs` & `rraft_py-0.1.3/src/bindings/progress_tracker.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/raft_state.rs` & `rraft_py-0.1.3/src/bindings/raft_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/read_state.rs` & `rraft_py-0.1.3/src/bindings/read_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/readonly_option.rs` & `rraft_py-0.1.3/src/bindings/readonly_option.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/ready.rs` & `rraft_py-0.1.3/src/bindings/ready.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/snapshot_status.rs` & `rraft_py-0.1.3/src/bindings/snapshot_status.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/soft_state.rs` & `rraft_py-0.1.3/src/bindings/soft_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/state_role.rs` & `rraft_py-0.1.3/src/bindings/state_role.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/bindings/unstable.rs` & `rraft_py-0.1.3/src/bindings/unstable.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/external_bindings/slog.rs` & `rraft_py-0.1.3/src/external_bindings/slog.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/external_bindings/thread_safe_slog.rs` & `rraft_py-0.1.3/src/external_bindings/thread_safe_slog.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/lib.rs` & `rraft_py-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/mem_storage_bindings/mem_storage.rs` & `rraft_py-0.1.3/src/mem_storage_bindings/mem_storage.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/mem_storage_bindings/mem_storage_core.rs` & `rraft_py-0.1.3/src/mem_storage_bindings/mem_storage_core.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/mem_storage_bindings/raft.rs` & `rraft_py-0.1.3/src/mem_storage_bindings/raft.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/mem_storage_bindings/raft_log.rs` & `rraft_py-0.1.3/src/mem_storage_bindings/raft_log.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/mem_storage_bindings/raw_node.rs` & `rraft_py-0.1.3/src/mem_storage_bindings/raw_node.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/py_storage_bindings/py_storage.rs` & `rraft_py-0.1.3/src/py_storage_bindings/py_storage.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/py_storage_bindings/raft.rs` & `rraft_py-0.1.3/src/py_storage_bindings/raft.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/py_storage_bindings/raft_log.rs` & `rraft_py-0.1.3/src/py_storage_bindings/raft_log.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/py_storage_bindings/raw_node.rs` & `rraft_py-0.1.3/src/py_storage_bindings/raw_node.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/conf_change.rs` & `rraft_py-0.1.3/src/raftpb_bindings/conf_change.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/conf_change_single.rs` & `rraft_py-0.1.3/src/raftpb_bindings/conf_change_single.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/conf_change_transition.rs` & `rraft_py-0.1.3/src/raftpb_bindings/conf_change_transition.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/conf_change_type.rs` & `rraft_py-0.1.3/src/raftpb_bindings/conf_change_type.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/conf_change_v2.rs` & `rraft_py-0.1.3/src/raftpb_bindings/conf_change_v2.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/conf_state.rs` & `rraft_py-0.1.3/src/raftpb_bindings/conf_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/entry.rs` & `rraft_py-0.1.3/src/raftpb_bindings/entry.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/entry_type.rs` & `rraft_py-0.1.3/src/raftpb_bindings/entry_type.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/hard_state.rs` & `rraft_py-0.1.3/src/raftpb_bindings/hard_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/message.rs` & `rraft_py-0.1.3/src/raftpb_bindings/message.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/message_type.rs` & `rraft_py-0.1.3/src/raftpb_bindings/message_type.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/snapshot.rs` & `rraft_py-0.1.3/src/raftpb_bindings/snapshot.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/raftpb_bindings/snapshot_metadata.rs` & `rraft_py-0.1.3/src/raftpb_bindings/snapshot_metadata.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/utils/errors.rs` & `rraft_py-0.1.3/src/utils/errors.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/src/utils/reference.rs` & `rraft_py-0.1.3/src/utils/reference.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.2/Cargo.lock` & `rraft_py-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "rraft-py"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "bincode",
  "fxhash",
  "prost",
  "protobuf",
  "pyo3",
  "raft",
```

### Comparing `rraft_py-0.1.2/PKG-INFO` & `rraft_py-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rraft-py
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE
 Summary: Unofficial Python Binding of the tikv/raft-rs
 Keywords: raft,distributed-systems,consensus-algorithm,replication,distributed-database
 Home-Page: https://github.com/lablup/rraft-py
 Author: Lablup Inc.
```


# Comparing `tmp/rraft_py-0.1.1.tar.gz` & `tmp/rraft_py-0.1.2.tar.gz`

## Comparing `rraft_py-0.1.1.tar` & `rraft_py-0.1.2.tar`

### file list

```diff
@@ -1,84 +1,85 @@
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 rraft_py-0.1.1/Cargo.toml
--rw-r--r--   0      501       20      206 2023-02-27 06:56:36.000000 rraft_py-0.1.1/.editorconfig
--rw-r--r--   0      501       20      788 2023-07-31 07:01:16.000000 rraft_py-0.1.1/.github/workflows/test.yml
--rw-r--r--   0      501       20      700 2023-04-06 07:12:36.000000 rraft_py-0.1.1/.gitignore
--rw-r--r--   0      501       20        7 2023-08-09 02:53:53.000000 rraft_py-0.1.1/.python-version
--rw-r--r--   0      501       20    11345 2023-07-31 07:01:16.000000 rraft_py-0.1.1/LICENSE
--rw-r--r--   0      501       20      573 2023-07-31 07:01:16.000000 rraft_py-0.1.1/Makefile
--rw-r--r--   0      501       20     3061 2023-08-08 00:51:37.000000 rraft_py-0.1.1/README.md
--rw-r--r--   0      501       20      223 2023-07-31 07:01:16.000000 rraft_py-0.1.1/benches/suites/progress.py
--rw-r--r--   0      501       20     4467 2023-07-31 07:01:16.000000 rraft_py-0.1.1/benches/suites/raft.py
--rw-r--r--   0      501       20        0 2023-07-31 07:01:16.000000 rraft_py-0.1.1/benches/suites/raw_node.py
--rw-r--r--   0      501       20    12446 2023-07-31 07:01:34.000000 rraft_py-0.1.1/example/multi_mem_node/main.py
--rw-r--r--   0      501       20     6010 2023-07-31 07:01:16.000000 rraft_py-0.1.1/example/single_mem_node/use_coroutine.py
--rw-r--r--   0      501       20     6293 2023-07-31 07:01:16.000000 rraft_py-0.1.1/example/single_mem_node/use_threading.py
--rw-r--r--   0      501       20      150 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/README.md
--rw-r--r--   0      501       20     2290 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/src/interface.py
--rw-r--r--   0      501       20     6835 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/src/network.py
--rw-r--r--   0      501       20     1004 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/tests/test_failpoints.py
--rw-r--r--   0      501       20   186320 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/tests/test_raft.py
--rw-r--r--   0      501       20     7732 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/tests/test_raft_flow_control.py
--rw-r--r--   0      501       20    34562 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/tests/test_raft_paper.py
--rw-r--r--   0      501       20     6467 2023-08-04 03:36:56.000000 rraft_py-0.1.1/harness/tests/test_raft_snap.py
--rw-r--r--   0      501       20    59741 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/tests/test_raw_node.py
--rw-r--r--   0      501       20     5874 2023-07-31 07:01:16.000000 rraft_py-0.1.1/harness/utils.py
--rw-r--r--   0      501       20        0 2023-01-26 07:03:57.000000 rraft_py-0.1.1/py.typed
--rw-r--r--   0      501       20      287 2023-07-31 07:01:16.000000 rraft_py-0.1.1/pyproject.toml
--rw-r--r--   0      501       20       36 2023-07-31 07:01:16.000000 rraft_py-0.1.1/pytest.ini
--rw-r--r--   0      501       20       52 2023-08-09 02:54:19.000000 rraft_py-0.1.1/requirements.txt
--rw-r--r--   0      501       20   114587 2023-08-08 05:40:33.000000 rraft_py-0.1.1/rraft.pyi
--rw-r--r--   0      501       20     9790 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/config.rs
--rw-r--r--   0      501       20     1332 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/get_entries_context.rs
--rw-r--r--   0      501       20     1906 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/global.rs
--rw-r--r--   0      501       20     3547 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/inflights.rs
--rw-r--r--   0      501       20     3716 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/joint_config.rs
--rw-r--r--   0      501       20     2989 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/light_ready.rs
--rw-r--r--   0      501       20     5194 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/majority_config.rs
--rw-r--r--   0      501       20      393 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/mod.rs
--rw-r--r--   0      501       20     1652 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/peer.rs
--rw-r--r--   0      501       20     6960 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/progress.rs
--rw-r--r--   0      501       20     1612 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/progress_state.rs
--rw-r--r--   0      501       20     5916 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/progress_tracker.rs
--rw-r--r--   0      501       20     2715 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/raft_state.rs
--rw-r--r--   0      501       20     3069 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/read_state.rs
--rw-r--r--   0      501       20     1388 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/readonly_option.rs
--rw-r--r--   0      501       20     6371 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/ready.rs
--rw-r--r--   0      501       20     1382 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/snapshot_status.rs
--rw-r--r--   0      501       20     2572 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/soft_state.rs
--rw-r--r--   0      501       20     1731 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/state_role.rs
--rw-r--r--   0      501       20     5229 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/bindings/unstable.rs
--rw-r--r--   0      501       20       14 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/external_bindings/mod.rs
--rw-r--r--   0      501       20     3571 2023-08-09 02:36:39.000000 rraft_py-0.1.1/src/external_bindings/slog.rs
--rw-r--r--   0      501       20     7929 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/lib.rs
--rw-r--r--   0      501       20     4789 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/mem_storage_bindings/mem_storage.rs
--rw-r--r--   0      501       20     4031 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/mem_storage_bindings/mem_storage_core.rs
--rw-r--r--   0      501       20       97 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/mem_storage_bindings/mod.rs
--rw-r--r--   0      501       20    19404 2023-08-09 02:47:04.000000 rraft_py-0.1.1/src/mem_storage_bindings/raft.rs
--rw-r--r--   0      501       20    11619 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/mem_storage_bindings/raft_log.rs
--rw-r--r--   0      501       20     8415 2023-08-08 09:59:49.000000 rraft_py-0.1.1/src/mem_storage_bindings/raw_node.rs
--rw-r--r--   0      501       20       70 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/py_storage_bindings/mod.rs
--rw-r--r--   0      501       20    12837 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/py_storage_bindings/py_storage.rs
--rw-r--r--   0      501       20    19208 2023-08-09 02:48:07.000000 rraft_py-0.1.1/src/py_storage_bindings/raft.rs
--rw-r--r--   0      501       20    11469 2023-08-08 05:35:51.000000 rraft_py-0.1.1/src/py_storage_bindings/raft_log.rs
--rw-r--r--   0      501       20     8271 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/py_storage_bindings/raw_node.rs
--rw-r--r--   0      501       20     6870 2023-08-08 07:53:52.000000 rraft_py-0.1.1/src/raftpb_bindings/conf_change.rs
--rw-r--r--   0      501       20     4026 2023-08-08 05:33:36.000000 rraft_py-0.1.1/src/raftpb_bindings/conf_change_single.rs
--rw-r--r--   0      501       20     2239 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/conf_change_transition.rs
--rw-r--r--   0      501       20     2051 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/conf_change_type.rs
--rw-r--r--   0      501       20     6846 2023-08-08 08:33:58.000000 rraft_py-0.1.1/src/raftpb_bindings/conf_change_v2.rs
--rw-r--r--   0      501       20     6511 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/conf_state.rs
--rw-r--r--   0      501       20     6038 2023-08-08 10:20:16.000000 rraft_py-0.1.1/src/raftpb_bindings/entry.rs
--rw-r--r--   0      501       20     1977 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/entry_type.rs
--rw-r--r--   0      501       20     4025 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/hard_state.rs
--rw-r--r--   0      501       20    11400 2023-08-08 07:54:25.000000 rraft_py-0.1.1/src/raftpb_bindings/message.rs
--rw-r--r--   0      501       20     7115 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/message_type.rs
--rw-r--r--   0      501       20      290 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/mod.rs
--rw-r--r--   0      501       20     4634 2023-08-09 02:55:14.000000 rraft_py-0.1.1/src/raftpb_bindings/snapshot.rs
--rw-r--r--   0      501       20     4570 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/raftpb_bindings/snapshot_metadata.rs
--rw-r--r--   0      501       20      475 2023-08-09 02:36:39.000000 rraft_py-0.1.1/src/utils/deserializer.rs
--rw-r--r--   0      501       20     9258 2023-08-04 00:35:31.000000 rraft_py-0.1.1/src/utils/errors.rs
--rw-r--r--   0      501       20       78 2023-08-08 05:00:26.000000 rraft_py-0.1.1/src/utils/mod.rs
--rw-r--r--   0      501       20     4407 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/utils/reference.rs
--rw-r--r--   0      501       20      409 2023-07-31 07:01:16.000000 rraft_py-0.1.1/src/utils/unsafe_cast.rs
--rw-r--r--   0      501       20    27236 2023-08-09 02:55:01.000000 rraft_py-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 rraft_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 rraft_py-0.1.2/Cargo.toml
+-rw-r--r--   0      501       20      206 2023-02-27 06:56:36.000000 rraft_py-0.1.2/.editorconfig
+-rw-r--r--   0      501       20      788 2023-07-31 07:01:16.000000 rraft_py-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0      501       20      700 2023-04-06 07:12:36.000000 rraft_py-0.1.2/.gitignore
+-rw-r--r--   0      501       20        7 2023-08-09 02:53:53.000000 rraft_py-0.1.2/.python-version
+-rw-r--r--   0      501       20    11345 2023-07-31 07:01:16.000000 rraft_py-0.1.2/LICENSE
+-rw-r--r--   0      501       20      599 2023-08-09 04:47:38.000000 rraft_py-0.1.2/Makefile
+-rw-r--r--   0      501       20     3061 2023-08-08 00:51:37.000000 rraft_py-0.1.2/README.md
+-rw-r--r--   0      501       20      223 2023-07-31 07:01:16.000000 rraft_py-0.1.2/benches/suites/progress.py
+-rw-r--r--   0      501       20     4467 2023-07-31 07:01:16.000000 rraft_py-0.1.2/benches/suites/raft.py
+-rw-r--r--   0      501       20        0 2023-07-31 07:01:16.000000 rraft_py-0.1.2/benches/suites/raw_node.py
+-rw-r--r--   0      501       20    12446 2023-07-31 07:01:34.000000 rraft_py-0.1.2/example/multi_mem_node/main.py
+-rw-r--r--   0      501       20     6010 2023-07-31 07:01:16.000000 rraft_py-0.1.2/example/single_mem_node/use_coroutine.py
+-rw-r--r--   0      501       20     6293 2023-08-09 04:43:12.000000 rraft_py-0.1.2/example/single_mem_node/use_threading.py
+-rw-r--r--   0      501       20      150 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/README.md
+-rw-r--r--   0      501       20     2290 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/src/interface.py
+-rw-r--r--   0      501       20     6835 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/src/network.py
+-rw-r--r--   0      501       20     1004 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_failpoints.py
+-rw-r--r--   0      501       20   186320 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raft.py
+-rw-r--r--   0      501       20     7732 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raft_flow_control.py
+-rw-r--r--   0      501       20    34562 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raft_paper.py
+-rw-r--r--   0      501       20     6467 2023-08-04 03:36:56.000000 rraft_py-0.1.2/harness/tests/test_raft_snap.py
+-rw-r--r--   0      501       20    59741 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/tests/test_raw_node.py
+-rw-r--r--   0      501       20     5874 2023-07-31 07:01:16.000000 rraft_py-0.1.2/harness/utils.py
+-rw-r--r--   0      501       20        0 2023-01-26 07:03:57.000000 rraft_py-0.1.2/py.typed
+-rw-r--r--   0      501       20      400 2023-08-09 03:08:57.000000 rraft_py-0.1.2/pyproject.toml
+-rw-r--r--   0      501       20       36 2023-07-31 07:01:16.000000 rraft_py-0.1.2/pytest.ini
+-rw-r--r--   0      501       20       52 2023-08-09 02:54:19.000000 rraft_py-0.1.2/requirements.txt
+-rw-r--r--   0      501       20   114743 2023-08-09 04:46:38.000000 rraft_py-0.1.2/rraft.pyi
+-rw-r--r--   0      501       20     9790 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/config.rs
+-rw-r--r--   0      501       20     1332 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/get_entries_context.rs
+-rw-r--r--   0      501       20     1906 2023-08-09 04:41:47.000000 rraft_py-0.1.2/src/bindings/global.rs
+-rw-r--r--   0      501       20     3547 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/inflights.rs
+-rw-r--r--   0      501       20     3716 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/joint_config.rs
+-rw-r--r--   0      501       20     2989 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/light_ready.rs
+-rw-r--r--   0      501       20     5194 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/majority_config.rs
+-rw-r--r--   0      501       20      393 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/mod.rs
+-rw-r--r--   0      501       20     1652 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/peer.rs
+-rw-r--r--   0      501       20     6960 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/progress.rs
+-rw-r--r--   0      501       20     1612 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/progress_state.rs
+-rw-r--r--   0      501       20     5916 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/progress_tracker.rs
+-rw-r--r--   0      501       20     2715 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/raft_state.rs
+-rw-r--r--   0      501       20     3069 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/read_state.rs
+-rw-r--r--   0      501       20     1388 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/readonly_option.rs
+-rw-r--r--   0      501       20     6371 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/ready.rs
+-rw-r--r--   0      501       20     1382 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/snapshot_status.rs
+-rw-r--r--   0      501       20     2572 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/soft_state.rs
+-rw-r--r--   0      501       20     1731 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/state_role.rs
+-rw-r--r--   0      501       20     5229 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/bindings/unstable.rs
+-rw-r--r--   0      501       20       40 2023-08-09 04:38:46.000000 rraft_py-0.1.2/src/external_bindings/mod.rs
+-rw-r--r--   0      501       20     3571 2023-08-09 04:28:59.000000 rraft_py-0.1.2/src/external_bindings/slog.rs
+-rw-r--r--   0      501       20     1844 2023-08-09 04:44:33.000000 rraft_py-0.1.2/src/external_bindings/thread_safe_slog.rs
+-rw-r--r--   0      501       20     8008 2023-08-09 04:40:34.000000 rraft_py-0.1.2/src/lib.rs
+-rw-r--r--   0      501       20     4789 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/mem_storage.rs
+-rw-r--r--   0      501       20     4031 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/mem_storage_core.rs
+-rw-r--r--   0      501       20       97 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/mod.rs
+-rw-r--r--   0      501       20    19404 2023-08-09 02:47:04.000000 rraft_py-0.1.2/src/mem_storage_bindings/raft.rs
+-rw-r--r--   0      501       20    11619 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/mem_storage_bindings/raft_log.rs
+-rw-r--r--   0      501       20     8415 2023-08-08 09:59:49.000000 rraft_py-0.1.2/src/mem_storage_bindings/raw_node.rs
+-rw-r--r--   0      501       20       70 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/py_storage_bindings/mod.rs
+-rw-r--r--   0      501       20    12837 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/py_storage_bindings/py_storage.rs
+-rw-r--r--   0      501       20    19208 2023-08-09 02:48:07.000000 rraft_py-0.1.2/src/py_storage_bindings/raft.rs
+-rw-r--r--   0      501       20    11469 2023-08-08 05:35:51.000000 rraft_py-0.1.2/src/py_storage_bindings/raft_log.rs
+-rw-r--r--   0      501       20     8271 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/py_storage_bindings/raw_node.rs
+-rw-r--r--   0      501       20     6870 2023-08-08 07:53:52.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change.rs
+-rw-r--r--   0      501       20     4026 2023-08-08 05:33:36.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_single.rs
+-rw-r--r--   0      501       20     2239 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_transition.rs
+-rw-r--r--   0      501       20     2051 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_type.rs
+-rw-r--r--   0      501       20     6846 2023-08-08 08:33:58.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_change_v2.rs
+-rw-r--r--   0      501       20     6511 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/conf_state.rs
+-rw-r--r--   0      501       20     6038 2023-08-08 10:20:16.000000 rraft_py-0.1.2/src/raftpb_bindings/entry.rs
+-rw-r--r--   0      501       20     1977 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/entry_type.rs
+-rw-r--r--   0      501       20     4025 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/hard_state.rs
+-rw-r--r--   0      501       20    11400 2023-08-08 07:54:25.000000 rraft_py-0.1.2/src/raftpb_bindings/message.rs
+-rw-r--r--   0      501       20     7115 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/message_type.rs
+-rw-r--r--   0      501       20      290 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/mod.rs
+-rw-r--r--   0      501       20     4634 2023-08-09 02:55:14.000000 rraft_py-0.1.2/src/raftpb_bindings/snapshot.rs
+-rw-r--r--   0      501       20     4570 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/raftpb_bindings/snapshot_metadata.rs
+-rw-r--r--   0      501       20      475 2023-08-09 02:36:39.000000 rraft_py-0.1.2/src/utils/deserializer.rs
+-rw-r--r--   0      501       20     9258 2023-08-04 00:35:31.000000 rraft_py-0.1.2/src/utils/errors.rs
+-rw-r--r--   0      501       20       78 2023-08-08 05:00:26.000000 rraft_py-0.1.2/src/utils/mod.rs
+-rw-r--r--   0      501       20     4407 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/utils/reference.rs
+-rw-r--r--   0      501       20      409 2023-07-31 07:01:16.000000 rraft_py-0.1.2/src/utils/unsafe_cast.rs
+-rw-r--r--   0      501       20    27236 2023-08-09 04:45:25.000000 rraft_py-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     3632 1970-01-01 00:00:00.000000 rraft_py-0.1.2/PKG-INFO
```

### Comparing `rraft_py-0.1.1/Cargo.toml` & `rraft_py-0.1.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rraft-py"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Lablup Inc."]
 license = "Apache-2.0"
 repository = "https://github.com/lablup/rraft-py"
 readme = "./README.md"
 homepage = "https://github.com/lablup/rraft-py"
 description = """
 Unofficial Python Binding of the tikv/raft-rs
```

### Comparing `rraft_py-0.1.1/.github/workflows/test.yml` & `rraft_py-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/.gitignore` & `rraft_py-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/LICENSE` & `rraft_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/README.md` & `rraft_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/benches/suites/raft.py` & `rraft_py-0.1.2/benches/suites/raft.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/example/multi_mem_node/main.py` & `rraft_py-0.1.2/example/multi_mem_node/main.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/example/single_mem_node/use_coroutine.py` & `rraft_py-0.1.2/example/single_mem_node/use_coroutine.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/example/single_mem_node/use_threading.py` & `rraft_py-0.1.2/example/single_mem_node/use_threading.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/src/interface.py` & `rraft_py-0.1.2/harness/src/interface.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/src/network.py` & `rraft_py-0.1.2/harness/src/network.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/tests/test_failpoints.py` & `rraft_py-0.1.2/harness/tests/test_failpoints.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/tests/test_raft.py` & `rraft_py-0.1.2/harness/tests/test_raft.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/tests/test_raft_flow_control.py` & `rraft_py-0.1.2/harness/tests/test_raft_flow_control.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/tests/test_raft_paper.py` & `rraft_py-0.1.2/harness/tests/test_raft_paper.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/tests/test_raft_snap.py` & `rraft_py-0.1.2/harness/tests/test_raft_snap.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/tests/test_raw_node.py` & `rraft_py-0.1.2/harness/tests/test_raw_node.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/harness/utils.py` & `rraft_py-0.1.2/harness/utils.py`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/rraft.pyi` & `rraft_py-0.1.2/rraft.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -379,6784 +379,6794 @@
 000017a0: 6f77 5374 7261 7465 6779 220a 2020 2020  owStrategy".    
 000017b0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
 000017c0: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
 000017d0: 7365 6c66 2920 2d3e 2022 4c6f 6767 6572  self) -> "Logger
 000017e0: 5265 6622 3a20 2e2e 2e0a 0a63 6c61 7373  Ref": .....class
 000017f0: 204c 6f67 6765 7252 6566 285f 5f41 5049   LoggerRef(__API
 00001800: 5f4c 6f67 6765 7229 3a0a 2020 2020 2222  _Logger):.    ""
-00001810: 2220 2222 220a 0a63 6c61 7373 205f 5f41  " """..class __A
-00001820: 5049 5f52 6166 7453 7461 7465 285f 5f43  PI_RaftState(__C
-00001830: 6c6f 6e65 6162 6c65 293a 0a20 2020 2064  loneable):.    d
-00001840: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-00001850: 3e20 2252 6166 7453 7461 7465 223a 202e  > "RaftState": .
-00001860: 2e2e 0a20 2020 2064 6566 2069 6e69 7469  ...    def initi
-00001870: 616c 697a 6564 2873 656c 6629 202d 3e20  alized(self) -> 
-00001880: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00001890: 220a 2020 2020 2020 2020 496e 6469 6361  ".        Indica
-000018a0: 7465 7320 7468 6520 6052 6166 7453 7461  tes the `RaftSta
-000018b0: 7465 6020 6973 2069 6e69 7469 616c 697a  te` is initializ
-000018c0: 6564 206f 7220 6e6f 742e 0a20 2020 2020  ed or not..     
-000018d0: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-000018e0: 6574 5f63 6f6e 665f 7374 6174 6528 7365  et_conf_state(se
-000018f0: 6c66 2920 2d3e 2022 436f 6e66 5374 6174  lf) -> "ConfStat
-00001900: 6552 6566 223a 0a20 2020 2020 2020 2022  eRef":.        "
-00001910: 2222 0a20 2020 2020 2020 2060 636f 6e66  "".        `conf
-00001920: 5f73 7461 7465 603a 2052 6563 6f72 6473  _state`: Records
-00001930: 2074 6865 2063 7572 7265 6e74 206e 6f64   the current nod
-00001940: 6520 4944 7320 6c69 6b65 2060 5b31 2c20  e IDs like `[1, 
-00001950: 322c 2033 5d60 2069 6e20 7468 6520 636c  2, 3]` in the cl
-00001960: 7573 7465 722e 2045 7665 7279 2052 6166  uster. Every Raf
-00001970: 7420 6e6f 6465 206d 7573 7420 6861 7665  t node must have
-00001980: 2061 0a20 2020 2020 2020 2075 6e69 7175   a.        uniqu
-00001990: 6520 4944 2069 6e20 7468 6520 636c 7573  e ID in the clus
-000019a0: 7465 723b 0a20 2020 2020 2020 2022 2222  ter;.        """
-000019b0: 0a20 2020 2064 6566 2073 6574 5f63 6f6e  .    def set_con
-000019c0: 665f 7374 6174 6528 7365 6c66 2c20 6373  f_state(self, cs
-000019d0: 3a20 2243 6f6e 6653 7461 7465 5265 6622  : "ConfStateRef"
-000019e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000019f0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00001a00: 636f 6e66 5f73 7461 7465 603a 2052 6563  conf_state`: Rec
-00001a10: 6f72 6473 2074 6865 2063 7572 7265 6e74  ords the current
-00001a20: 206e 6f64 6520 4944 7320 6c69 6b65 2060   node IDs like `
-00001a30: 5b31 2c20 322c 2033 5d60 2069 6e20 7468  [1, 2, 3]` in th
-00001a40: 6520 636c 7573 7465 722e 2045 7665 7279  e cluster. Every
-00001a50: 2052 6166 7420 6e6f 6465 206d 7573 7420   Raft node must 
-00001a60: 6861 7665 2061 0a20 2020 2020 2020 2075  have a.        u
-00001a70: 6e69 7175 6520 4944 2069 6e20 7468 6520  nique ID in the 
-00001a80: 636c 7573 7465 723b 0a20 2020 2020 2020  cluster;.       
-00001a90: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00001aa0: 5f68 6172 645f 7374 6174 6528 7365 6c66  _hard_state(self
-00001ab0: 2920 2d3e 2022 4861 7264 5374 6174 6552  ) -> "HardStateR
-00001ac0: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-00001ad0: 0a20 2020 2020 2020 2060 6861 7264 5f73  .        `hard_s
-00001ae0: 7461 7465 603a 2043 6f6e 7461 696e 7320  tate`: Contains 
-00001af0: 7468 6520 6c61 7374 206d 6574 6120 696e  the last meta in
-00001b00: 666f 726d 6174 696f 6e20 696e 636c 7564  formation includ
-00001b10: 696e 6720 636f 6d6d 6974 2069 6e64 6578  ing commit index
-00001b20: 2c20 7468 6520 766f 7465 206c 6561 6465  , the vote leade
-00001b30: 722c 2061 6e64 2074 6865 2076 6f74 6520  r, and the vote 
-00001b40: 7465 726d 2e0a 2020 2020 2020 2020 2222  term..        ""
-00001b50: 220a 2020 2020 6465 6620 7365 745f 6861  ".    def set_ha
-00001b60: 7264 5f73 7461 7465 2873 656c 662c 2068  rd_state(self, h
-00001b70: 733a 2022 4861 7264 5374 6174 6552 6566  s: "HardStateRef
-00001b80: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
-00001b90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00001ba0: 6068 6172 645f 7374 6174 6560 3a20 436f  `hard_state`: Co
-00001bb0: 6e74 6169 6e73 2074 6865 206c 6173 7420  ntains the last 
-00001bc0: 6d65 7461 2069 6e66 6f72 6d61 7469 6f6e  meta information
-00001bd0: 2069 6e63 6c75 6469 6e67 2063 6f6d 6d69   including commi
-00001be0: 7420 696e 6465 782c 2074 6865 2076 6f74  t index, the vot
-00001bf0: 6520 6c65 6164 6572 2c20 616e 6420 7468  e leader, and th
-00001c00: 6520 766f 7465 2074 6572 6d2e 0a20 2020  e vote term..   
-00001c10: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-00001c20: 5261 6674 5374 6174 6528 5f5f 4150 495f  RaftState(__API_
-00001c30: 5261 6674 5374 6174 6529 3a0a 2020 2020  RaftState):.    
-00001c40: 2222 220a 2020 2020 486f 6c64 7320 626f  """.    Holds bo
-00001c50: 7468 2074 6865 2068 6172 6420 7374 6174  th the hard stat
-00001c60: 6520 2863 6f6d 6d69 7420 696e 6465 782c  e (commit index,
-00001c70: 2076 6f74 6520 6c65 6164 6572 2c20 7465   vote leader, te
-00001c80: 726d 2920 616e 6420 7468 6520 636f 6e66  rm) and the conf
-00001c90: 6967 7572 6174 696f 6e20 7374 6174 650a  iguration state.
-00001ca0: 2020 2020 2843 7572 7265 6e74 206e 6f64      (Current nod
-00001cb0: 6520 4944 7329 0a20 2020 2022 2222 0a0a  e IDs).    """..
-00001cc0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001cd0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a20  (self) -> None: 
-00001ce0: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-00001cf0: 5f72 6566 2873 656c 6629 202d 3e20 2252  _ref(self) -> "R
-00001d00: 6166 7453 7461 7465 5265 6622 3a20 2e2e  aftStateRef": ..
-00001d10: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00001d20: 686f 640a 2020 2020 6465 6620 6465 6661  hod.    def defa
-00001d30: 756c 7428 2920 2d3e 2022 5261 6674 5374  ult() -> "RaftSt
-00001d40: 6174 6522 3a20 2e2e 2e0a 0a63 6c61 7373  ate": .....class
-00001d50: 2052 6166 7453 7461 7465 5265 6628 5f5f   RaftStateRef(__
-00001d60: 4150 495f 5261 6674 5374 6174 6529 3a0a  API_RaftState):.
-00001d70: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
-00001d80: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
-00001d90: 6c61 7373 3a60 5261 6674 5374 6174 6560  lass:`RaftState`
-00001da0: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
-00001db0: 205f 5f41 5049 5f53 746f 7261 6765 436f   __API_StorageCo
-00001dc0: 7265 3a0a 2020 2020 6465 6620 6170 7065  re:.    def appe
-00001dd0: 6e64 2873 656c 662c 2065 6e74 733a 204c  nd(self, ents: L
-00001de0: 6973 745b 2245 6e74 7279 225d 207c 204c  ist["Entry"] | L
-00001df0: 6973 745b 2245 6e74 7279 5265 6622 5d29  ist["EntryRef"])
-00001e00: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00001e10: 2020 2222 220a 2020 2020 2020 2020 4170    """.        Ap
-00001e20: 7065 6e64 2074 6865 206e 6577 2065 6e74  pend the new ent
-00001e30: 7269 6573 2074 6f20 7374 6f72 6167 652e  ries to storage.
-00001e40: 0a0a 2020 2020 2020 2020 2320 5061 6e69  ..        # Pani
-00001e50: 6373 0a0a 2020 2020 2020 2020 5061 6e69  cs..        Pani
-00001e60: 6373 2069 6620 6065 6e74 7360 2063 6f6e  cs if `ents` con
-00001e70: 7461 696e 7320 636f 6d70 6163 7465 6420  tains compacted 
-00001e80: 656e 7472 6965 732c 206f 7220 7468 6572  entries, or ther
-00001e90: 6527 7320 6120 6761 7020 6265 7477 6565  e's a gap betwee
-00001ea0: 6e20 6065 6e74 7360 2061 6e64 2074 6865  n `ents` and the
-00001eb0: 206c 6173 740a 2020 2020 2020 2020 7265   last.        re
-00001ec0: 6365 6976 6564 2065 6e74 7279 2069 6e20  ceived entry in 
-00001ed0: 7468 6520 7374 6f72 6167 652e 0a20 2020  the storage..   
-00001ee0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00001ef0: 2061 7070 6c79 5f73 6e61 7073 686f 7428   apply_snapshot(
-00001f00: 7365 6c66 2c20 736e 6170 7368 6f74 3a20  self, snapshot: 
-00001f10: 2253 6e61 7073 686f 7422 207c 2022 536e  "Snapshot" | "Sn
-00001f20: 6170 7368 6f74 5265 6622 2920 2d3e 204e  apshotRef") -> N
-00001f30: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00001f40: 0a20 2020 2020 2020 204f 7665 7277 7269  .        Overwri
-00001f50: 7465 7320 7468 6520 636f 6e74 656e 7473  tes the contents
-00001f60: 206f 6620 7468 6973 2053 746f 7261 6765   of this Storage
-00001f70: 206f 626a 6563 7420 7769 7468 2074 686f   object with tho
-00001f80: 7365 206f 6620 7468 6520 6769 7665 6e20  se of the given 
-00001f90: 736e 6170 7368 6f74 2e0a 0a20 2020 2020  snapshot...     
-00001fa0: 2020 2023 2050 616e 6963 730a 0a20 2020     # Panics..   
-00001fb0: 2020 2020 2050 616e 6963 7320 6966 2074       Panics if t
-00001fc0: 6865 2073 6e61 7073 686f 7420 696e 6465  he snapshot inde
-00001fd0: 7820 6973 206c 6573 7320 7468 616e 2074  x is less than t
-00001fe0: 6865 2073 746f 7261 6765 2773 2066 6972  he storage's fir
-00001ff0: 7374 2069 6e64 6578 2e0a 2020 2020 2020  st index..      
-00002000: 2020 2222 220a 2020 2020 6465 6620 636f    """.    def co
-00002010: 6d70 6163 7428 7365 6c66 2c20 636f 6d70  mpact(self, comp
-00002020: 6163 745f 696e 6465 783a 2069 6e74 2920  act_index: int) 
-00002030: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00002040: 2022 2222 0a20 2020 2020 2020 2044 6973   """.        Dis
-00002050: 6361 7264 7320 616c 6c20 6c6f 6720 656e  cards all log en
-00002060: 7472 6965 7320 7072 696f 7220 746f 2063  tries prior to c
-00002070: 6f6d 7061 6374 5f69 6e64 6578 2e0a 2020  ompact_index..  
-00002080: 2020 2020 2020 4974 2069 7320 7468 6520        It is the 
-00002090: 6170 706c 6963 6174 696f 6e27 7320 7265  application's re
-000020a0: 7370 6f6e 7369 6269 6c69 7479 2074 6f20  sponsibility to 
-000020b0: 6e6f 7420 6174 7465 6d70 7420 746f 2063  not attempt to c
-000020c0: 6f6d 7061 6374 2061 6e20 696e 6465 780a  ompact an index.
-000020d0: 2020 2020 2020 2020 6772 6561 7465 7220          greater 
-000020e0: 7468 616e 2052 6166 744c 6f67 2e61 7070  than RaftLog.app
-000020f0: 6c69 6564 2e0a 0a20 2020 2020 2020 2023  lied...        #
-00002100: 2050 616e 6963 730a 0a20 2020 2020 2020   Panics..       
-00002110: 2050 616e 6963 7320 6966 2060 636f 6d70   Panics if `comp
-00002120: 6163 745f 696e 6465 7860 2069 7320 6869  act_index` is hi
-00002130: 6768 6572 2074 6861 6e20 6053 746f 7261  gher than `Stora
-00002140: 6765 3a3a 6c61 7374 5f69 6e64 6578 2826  ge::last_index(&
-00002150: 7365 6c66 2920 2b20 3160 2e0a 2020 2020  self) + 1`..    
-00002160: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00002170: 636f 6d6d 6974 5f74 6f28 7365 6c66 2c20  commit_to(self, 
-00002180: 696e 6465 783a 2069 6e74 2920 2d3e 204e  index: int) -> N
-00002190: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000021a0: 0a20 2020 2020 2020 2043 6f6d 6d69 7420  .        Commit 
-000021b0: 746f 2061 6e20 696e 6465 782e 0a0a 2020  to an index...  
-000021c0: 2020 2020 2020 2320 5061 6e69 6373 0a0a        # Panics..
-000021d0: 2020 2020 2020 2020 5061 6e69 6373 2069          Panics i
-000021e0: 6620 7468 6572 6520 6973 206e 6f20 7375  f there is no su
-000021f0: 6368 2065 6e74 7279 2069 6e20 7261 6674  ch entry in raft
-00002200: 206c 6f67 732e 0a20 2020 2020 2020 2022   logs..        "
-00002210: 2222 0a20 2020 2064 6566 2063 6f6d 6d69  "".    def commi
-00002220: 745f 746f 5f61 6e64 5f73 6574 5f63 6f6e  t_to_and_set_con
-00002230: 665f 7374 6174 6573 280a 2020 2020 2020  f_states(.      
-00002240: 2020 7365 6c66 2c20 6964 783a 2069 6e74    self, idx: int
-00002250: 2c20 6373 3a20 4f70 7469 6f6e 616c 5b22  , cs: Optional["
-00002260: 436f 6e66 5374 6174 6522 5d20 7c20 4f70  ConfState"] | Op
-00002270: 7469 6f6e 616c 5b22 436f 6e66 5374 6174  tional["ConfStat
-00002280: 6552 6566 225d 0a20 2020 2029 202d 3e20  eRef"].    ) -> 
-00002290: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000022a0: 220a 2020 2020 2020 2020 436f 6d6d 6974  ".        Commit
-000022b0: 2074 6f20 6069 6478 6020 616e 6420 7365   to `idx` and se
-000022c0: 7420 636f 6e66 6967 7572 6174 696f 6e20  t configuration 
-000022d0: 746f 2074 6865 2067 6976 656e 2073 7461  to the given sta
-000022e0: 7465 732e 204f 6e6c 7920 7573 6564 2066  tes. Only used f
-000022f0: 6f72 2074 6573 7473 2e0a 2020 2020 2020  or tests..      
-00002300: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00002310: 745f 636f 6e66 5f73 7461 7465 2873 656c  t_conf_state(sel
-00002320: 662c 2063 733a 2022 436f 6e66 5374 6174  f, cs: "ConfStat
-00002330: 6522 207c 2022 436f 6e66 5374 6174 6552  e" | "ConfStateR
-00002340: 6566 2229 202d 3e20 4e6f 6e65 3a0a 2020  ef") -> None:.  
-00002350: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00002360: 2020 5361 7665 7320 7468 6520 6375 7272    Saves the curr
-00002370: 656e 7420 636f 6e66 2073 7461 7465 2e0a  ent conf state..
-00002380: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00002390: 6465 6620 6861 7264 5f73 7461 7465 2873  def hard_state(s
-000023a0: 656c 6629 202d 3e20 2248 6172 6453 7461  elf) -> "HardSta
-000023b0: 7465 5265 6622 3a0a 2020 2020 2020 2020  teRef":.        
-000023c0: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
-000023d0: 7468 6520 6861 7264 2073 7461 7465 2e0a  the hard state..
-000023e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000023f0: 6465 6620 7365 745f 6861 7264 7374 6174  def set_hardstat
-00002400: 6528 7365 6c66 2c20 6873 3a20 2248 6172  e(self, hs: "Har
-00002410: 6453 7461 7465 2220 7c20 2248 6172 6453  dState" | "HardS
-00002420: 7461 7465 5265 6622 2920 2d3e 204e 6f6e  tateRef") -> Non
-00002430: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00002440: 2020 2020 2020 2053 6176 6573 2074 6865         Saves the
-00002450: 2063 7572 7265 6e74 2048 6172 6453 7461   current HardSta
-00002460: 7465 2e0a 2020 2020 2020 2020 2222 220a  te..        """.
-00002470: 2020 2020 6465 6620 7472 6967 6765 725f      def trigger_
-00002480: 736e 6170 5f75 6e61 7661 696c 6162 6c65  snap_unavailable
-00002490: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000024a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000024b0: 2020 2020 5472 6967 6765 7220 6120 536e      Trigger a Sn
-000024c0: 6170 7368 6f74 5465 6d70 6f72 6172 696c  apshotTemporaril
-000024d0: 7955 6e61 7661 696c 6162 6c65 2065 7272  yUnavailable err
-000024e0: 6f72 2e0a 2020 2020 2020 2020 2222 220a  or..        """.
-000024f0: 2020 2020 6465 6620 7472 6967 6765 725f      def trigger_
-00002500: 6c6f 675f 756e 6176 6169 6c61 626c 6528  log_unavailable(
-00002510: 7365 6c66 2c20 763a 2062 6f6f 6c29 202d  self, v: bool) -
-00002520: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00002530: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
-00002540: 6120 4c6f 6754 656d 706f 7261 7269 6c79  a LogTemporarily
-00002550: 556e 6176 6169 6c61 626c 6520 6572 726f  Unavailable erro
-00002560: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-00002570: 2020 2064 6566 2074 616b 655f 6765 745f     def take_get_
-00002580: 656e 7472 6965 735f 636f 6e74 6578 7428  entries_context(
-00002590: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-000025a0: 6c5b 2247 6574 456e 7472 6965 7343 6f6e  l["GetEntriesCon
-000025b0: 7465 7874 225d 3a0a 2020 2020 2020 2020  text"]:.        
-000025c0: 2222 220a 2020 2020 2020 2020 5461 6b65  """.        Take
-000025d0: 2067 6574 2065 6e74 7269 6573 2063 6f6e   get entries con
-000025e0: 7465 7874 2e0a 2020 2020 2020 2020 2222  text..        ""
-000025f0: 220a 0a63 6c61 7373 204d 656d 5374 6f72  "..class MemStor
-00002600: 6167 6543 6f72 6528 5f5f 4150 495f 5374  ageCore(__API_St
-00002610: 6f72 6167 6543 6f72 6529 3a0a 2020 2020  orageCore):.    
-00002620: 2222 220a 2020 2020 5468 6520 4d65 6d6f  """.    The Memo
-00002630: 7279 2053 746f 7261 6765 2043 6f72 6520  ry Storage Core 
-00002640: 696e 7374 616e 6365 2068 6f6c 6473 2074  instance holds t
-00002650: 6865 2061 6374 7561 6c20 7374 6174 6520  he actual state 
-00002660: 6f66 2074 6865 2073 746f 7261 6765 2073  of the storage s
-00002670: 7472 7563 742e 2054 6f20 6163 6365 7373  truct. To access
-00002680: 2074 6869 730a 2020 2020 7661 6c75 652c   this.    value,
-00002690: 2075 7365 2074 6865 2060 726c 6020 616e   use the `rl` an
-000026a0: 6420 6077 6c60 2066 756e 6374 696f 6e73  d `wl` functions
-000026b0: 206f 6e20 7468 6520 6d61 696e 204d 656d   on the main Mem
-000026c0: 5374 6f72 6167 6520 696d 706c 656d 656e  Storage implemen
-000026d0: 7461 7469 6f6e 2e0a 2020 2020 2222 220a  tation..    """.
-000026e0: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
-000026f0: 6628 7365 6c66 2920 2d3e 2022 4d65 6d53  f(self) -> "MemS
-00002700: 746f 7261 6765 436f 7265 5265 6622 3a20  torageCoreRef": 
-00002710: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
-00002720: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
-00002730: 6661 756c 7428 2920 2d3e 2022 4d65 6d53  fault() -> "MemS
-00002740: 746f 7261 6765 436f 7265 223a 202e 2e2e  torageCore": ...
-00002750: 0a0a 636c 6173 7320 4d65 6d53 746f 7261  ..class MemStora
-00002760: 6765 436f 7265 5265 6628 5f5f 4150 495f  geCoreRef(__API_
-00002770: 5374 6f72 6167 6543 6f72 6529 3a0a 2020  StorageCore):.  
-00002780: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
-00002790: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
-000027a0: 7373 3a60 4d65 6d53 746f 7261 6765 602e  ss:`MemStorage`.
-000027b0: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-000027c0: 5374 6f72 6167 6543 6f72 6528 5f5f 4150  StorageCore(__AP
-000027d0: 495f 5374 6f72 6167 6543 6f72 6529 3a0a  I_StorageCore):.
-000027e0: 2020 2020 2222 2220 2222 220a 0a20 2020      """ """..   
-000027f0: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
-00002800: 6c66 2920 2d3e 2022 5374 6f72 6167 6543  lf) -> "StorageC
-00002810: 6f72 6552 6566 223a 202e 2e2e 0a20 2020  oreRef": ....   
-00002820: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00002830: 2020 2064 6566 2064 6566 6175 6c74 2829     def default()
-00002840: 202d 3e20 2253 746f 7261 6765 436f 7265   -> "StorageCore
-00002850: 223a 202e 2e2e 0a0a 636c 6173 7320 5374  ": .....class St
-00002860: 6f72 6167 6543 6f72 6552 6566 285f 5f41  orageCoreRef(__A
-00002870: 5049 5f53 746f 7261 6765 436f 7265 293a  PI_StorageCore):
-00002880: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
-00002890: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
-000028a0: 636c 6173 733a 6053 746f 7261 6765 436f  class:`StorageCo
-000028b0: 7265 602e 0a20 2020 2022 2222 0a0a 636c  re`..    """..cl
-000028c0: 6173 7320 5f5f 4150 495f 5374 6f72 6167  ass __API_Storag
-000028d0: 6528 5f5f 436c 6f6e 6561 626c 6529 3a0a  e(__Cloneable):.
-000028e0: 2020 2020 6465 6620 636c 6f6e 6528 7365      def clone(se
-000028f0: 6c66 2920 2d3e 2041 6e79 3a20 2e2e 2e0a  lf) -> Any: ....
-00002900: 2020 2020 6465 6620 696e 6974 6961 6c69      def initiali
-00002910: 7a65 5f77 6974 685f 636f 6e66 5f73 7461  ze_with_conf_sta
-00002920: 7465 280a 2020 2020 2020 2020 7365 6c66  te(.        self
-00002930: 2c20 636f 6e66 5f73 7461 7465 3a20 2243  , conf_state: "C
-00002940: 6f6e 6653 7461 7465 2220 7c20 2243 6f6e  onfState" | "Con
-00002950: 6653 7461 7465 5265 6622 0a20 2020 2029  fStateRef".    )
-00002960: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00002970: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
-00002980: 6974 6961 6c69 7a65 2061 2060 4d65 6d53  itialize a `MemS
-00002990: 746f 7261 6765 6020 7769 7468 2061 2067  torage` with a g
-000029a0: 6976 656e 2060 436f 6e66 6967 602e 0a0a  iven `Config`...
-000029b0: 2020 2020 2020 2020 596f 7520 7368 6f75          You shou
-000029c0: 6c64 2075 7365 2074 6865 2073 616d 6520  ld use the same 
-000029d0: 696e 7075 7420 746f 2069 6e69 7469 616c  input to initial
-000029e0: 697a 6520 616c 6c20 6e6f 6465 732e 0a20  ize all nodes.. 
-000029f0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00002a00: 6566 2069 6e69 7469 616c 5f73 7461 7465  ef initial_state
-00002a10: 2873 656c 6629 202d 3e20 5261 6674 5374  (self) -> RaftSt
-00002a20: 6174 653a 0a20 2020 2020 2020 2022 2222  ate:.        """
-00002a30: 0a20 2020 2020 2020 2049 6d70 6c65 6d65  .        Impleme
-00002a40: 6e74 7320 7468 6520 5374 6f72 6167 6520  nts the Storage 
-00002a50: 7472 6169 742e 0a20 2020 2020 2020 2022  trait..        "
-00002a60: 2222 0a20 2020 2064 6566 2065 6e74 7269  "".    def entri
-00002a70: 6573 280a 2020 2020 2020 2020 7365 6c66  es(.        self
-00002a80: 2c0a 2020 2020 2020 2020 6c6f 773a 2069  ,.        low: i
-00002a90: 6e74 2c0a 2020 2020 2020 2020 6869 6768  nt,.        high
-00002aa0: 3a20 696e 742c 0a20 2020 2020 2020 2063  : int,.        c
-00002ab0: 6f6e 7465 7874 3a20 2247 6574 456e 7472  ontext: "GetEntr
-00002ac0: 6965 7343 6f6e 7465 7874 5265 6622 2c0a  iesContextRef",.
-00002ad0: 2020 2020 2020 2020 6d61 785f 7369 7a65          max_size
-00002ae0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d2c  : Optional[int],
-00002af0: 0a20 2020 2029 202d 3e20 4c69 7374 5b22  .    ) -> List["
-00002b00: 456e 7472 7922 5d3a 0a20 2020 2020 2020  Entry"]:.       
-00002b10: 2022 2222 0a20 2020 2020 2020 2049 6d70   """.        Imp
-00002b20: 6c65 6d65 6e74 7320 7468 6520 5374 6f72  lements the Stor
-00002b30: 6167 6520 7472 6169 742e 0a20 2020 2020  age trait..     
-00002b40: 2020 2022 2222 0a20 2020 2064 6566 2074     """.    def t
-00002b50: 6572 6d28 7365 6c66 2c20 6964 783a 2069  erm(self, idx: i
-00002b60: 6e74 2920 2d3e 2069 6e74 3a0a 2020 2020  nt) -> int:.    
-00002b70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002b80: 496d 706c 656d 656e 7473 2074 6865 2053  Implements the S
-00002b90: 746f 7261 6765 2074 7261 6974 2e0a 2020  torage trait..  
-00002ba0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00002bb0: 6620 6669 7273 745f 696e 6465 7828 7365  f first_index(se
-00002bc0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00002bd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002be0: 496d 706c 656d 656e 7473 2074 6865 2053  Implements the S
-00002bf0: 746f 7261 6765 2074 7261 6974 2e0a 2020  torage trait..  
-00002c00: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00002c10: 6620 6c61 7374 5f69 6e64 6578 2873 656c  f last_index(sel
-00002c20: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00002c30: 2020 2022 2222 0a20 2020 2020 2020 2049     """.        I
-00002c40: 6d70 6c65 6d65 6e74 7320 7468 6520 5374  mplements the St
-00002c50: 6f72 6167 6520 7472 6169 742e 0a20 2020  orage trait..   
-00002c60: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00002c70: 2073 6e61 7073 686f 7428 7365 6c66 2c20   snapshot(self, 
-00002c80: 7265 7175 6573 745f 696e 6465 783a 2069  request_index: i
-00002c90: 6e74 2c20 746f 3a20 696e 7429 202d 3e20  nt, to: int) -> 
-00002ca0: 2253 6e61 7073 686f 7422 3a0a 2020 2020  "Snapshot":.    
-00002cb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00002cc0: 496d 706c 656d 656e 7473 2074 6865 2053  Implements the S
-00002cd0: 746f 7261 6765 2074 7261 6974 2e0a 2020  torage trait..  
-00002ce0: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
-00002cf0: 204d 656d 5374 6f72 6167 6528 5f5f 4150   MemStorage(__AP
-00002d00: 495f 5374 6f72 6167 6529 3a0a 2020 2020  I_Storage):.    
-00002d10: 2222 220a 2020 2020 604d 656d 5374 6f72  """.    `MemStor
-00002d20: 6167 6560 2069 7320 6120 7468 7265 6164  age` is a thread
-00002d30: 2d73 6166 6520 6275 7420 696e 636f 6d70  -safe but incomp
-00002d40: 6c65 7465 2069 6d70 6c65 6d65 6e74 6174  lete implementat
-00002d50: 696f 6e20 6f66 2060 5374 6f72 6167 6560  ion of `Storage`
-00002d60: 2c20 6d61 696e 6c79 2066 6f72 2074 6573  , mainly for tes
-00002d70: 7473 2e0a 0a20 2020 2041 2072 6561 6c20  ts...    A real 
-00002d80: 6053 746f 7261 6765 6020 7368 6f75 6c64  `Storage` should
-00002d90: 2073 6176 6520 626f 7468 2072 6166 7420   save both raft 
-00002da0: 6c6f 6773 2061 6e64 2061 7070 6c69 6564  logs and applied
-00002db0: 2064 6174 612e 2048 6f77 6576 6572 2060   data. However `
-00002dc0: 4d65 6d53 746f 7261 6765 6020 6f6e 6c79  MemStorage` only
-00002dd0: 0a20 2020 2063 6f6e 7461 696e 7320 7261  .    contains ra
-00002de0: 6674 206c 6f67 732e 2053 6f20 796f 7520  ft logs. So you 
-00002df0: 6361 6e20 6361 6c6c 2060 4d65 6d53 746f  can call `MemSto
-00002e00: 7261 6765 3a3a 6170 7065 6e64 6020 746f  rage::append` to
-00002e10: 2070 6572 7369 7374 206e 6577 2072 6563   persist new rec
-00002e20: 6569 7665 6420 756e 7374 6162 6c65 2072  eived unstable r
-00002e30: 6166 740a 2020 2020 6c6f 6773 2061 6e64  aft.    logs and
-00002e40: 2074 6865 6e20 6163 6365 7373 2074 6865   then access the
-00002e50: 6d20 7769 7468 2060 5374 6f72 6167 6560  m with `Storage`
-00002e60: 2041 5049 732e 2054 6865 206f 6e6c 7920   APIs. The only 
-00002e70: 6578 6365 7074 696f 6e20 6973 2060 5374  exception is `St
-00002e80: 6f72 6167 653a 3a73 6e61 7073 686f 7460  orage::snapshot`
-00002e90: 2e20 5468 6572 650a 2020 2020 6973 206e  . There.    is n
-00002ea0: 6f20 6461 7461 2069 6e20 6053 6e61 7073  o data in `Snaps
-00002eb0: 686f 7460 2072 6574 7572 6e65 6420 6279  hot` returned by
-00002ec0: 2060 4d65 6d53 746f 7261 6765 3a3a 736e   `MemStorage::sn
-00002ed0: 6170 7368 6f74 6020 6265 6361 7573 6520  apshot` because 
-00002ee0: 6170 706c 6965 6420 6461 7461 2069 7320  applied data is 
-00002ef0: 6e6f 7420 7374 6f72 6564 0a20 2020 2069  not stored.    i
-00002f00: 6e20 604d 656d 5374 6f72 6167 6560 2e0a  n `MemStorage`..
-00002f10: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00002f20: 205f 5f69 6e69 745f 5f28 7365 6c66 2920   __init__(self) 
-00002f30: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-00002f40: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
-00002f50: 6c66 2920 2d3e 2022 4d65 6d53 746f 7261  lf) -> "MemStora
-00002f60: 6765 5265 6622 3a20 2e2e 2e0a 2020 2020  geRef": ....    
-00002f70: 6465 6620 636c 6f6e 6528 7365 6c66 2920  def clone(self) 
-00002f80: 2d3e 2022 4d65 6d53 746f 7261 6765 223a  -> "MemStorage":
-00002f90: 202e 2e2e 0a20 2020 2040 7374 6174 6963   ....    @static
-00002fa0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-00002fb0: 6566 6175 6c74 2829 202d 3e20 224d 656d  efault() -> "Mem
-00002fc0: 5374 6f72 6167 6522 3a20 2e2e 2e0a 2020  Storage": ....  
-00002fd0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-00002fe0: 2020 2020 6465 6620 6e65 775f 7769 7468      def new_with
-00002ff0: 5f63 6f6e 665f 7374 6174 6528 0a20 2020  _conf_state(.   
-00003000: 2020 2020 2063 6f6e 665f 7374 6174 653a       conf_state:
-00003010: 2022 436f 6e66 5374 6174 6522 207c 2022   "ConfState" | "
-00003020: 436f 6e66 5374 6174 6552 6566 222c 0a20  ConfStateRef",. 
-00003030: 2020 2029 202d 3e20 224d 656d 5374 6f72     ) -> "MemStor
-00003040: 6167 6522 3a0a 2020 2020 2020 2020 2222  age":.        ""
-00003050: 220a 2020 2020 2020 2020 4372 6561 7465  ".        Create
-00003060: 2061 206e 6577 2060 4d65 6d53 746f 7261   a new `MemStora
-00003070: 6765 6020 7769 7468 2061 2067 6976 656e  ge` with a given
-00003080: 2060 436f 6e66 6967 602e 2054 6865 2067   `Config`. The g
-00003090: 6976 656e 2060 436f 6e66 6967 6020 7769  iven `Config` wi
-000030a0: 6c6c 2062 6520 7573 6564 2074 6f0a 2020  ll be used to.  
-000030b0: 2020 2020 2020 696e 6974 6961 6c69 7a65        initialize
-000030c0: 2074 6865 2073 746f 7261 6765 2e0a 0a20   the storage... 
-000030d0: 2020 2020 2020 2059 6f75 2073 686f 756c         You shoul
-000030e0: 6420 7573 6520 7468 6520 7361 6d65 2069  d use the same i
-000030f0: 6e70 7574 2074 6f20 696e 6974 6961 6c69  nput to initiali
-00003100: 7a65 2061 6c6c 206e 6f64 6573 2e0a 2020  ze all nodes..  
-00003110: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00003120: 6620 776c 2873 656c 6629 202d 3e20 224d  f wl(self) -> "M
-00003130: 656d 5374 6f72 6167 6543 6f72 6552 6566  emStorageCoreRef
-00003140: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-00003150: 2020 2020 2020 204f 7065 6e73 2075 7020         Opens up 
-00003160: 6120 7772 6974 6520 6c6f 636b 206f 6e20  a write lock on 
-00003170: 7468 6520 7374 6f72 6167 6520 616e 6420  the storage and 
-00003180: 7265 7475 726e 7320 6775 6172 6420 6861  returns guard ha
-00003190: 6e64 6c65 2e20 5573 6520 7468 6973 0a20  ndle. Use this. 
-000031a0: 2020 2020 2020 2077 6974 6820 6675 6e63         with func
-000031b0: 7469 6f6e 7320 7468 6174 2074 616b 6520  tions that take 
-000031c0: 6120 6d75 7461 626c 6520 7265 6665 7265  a mutable refere
-000031d0: 6e63 6520 746f 2073 656c 662e 0a20 2020  nce to self..   
-000031e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-000031f0: 2072 6c28 7365 6c66 2920 2d3e 2022 4d65   rl(self) -> "Me
-00003200: 6d53 746f 7261 6765 436f 7265 5265 6622  mStorageCoreRef"
-00003210: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00003220: 2020 2020 2020 4f70 656e 7320 7570 2061        Opens up a
-00003230: 2072 6561 6420 6c6f 636b 206f 6e20 7468   read lock on th
-00003240: 6520 7374 6f72 6167 6520 616e 6420 7265  e storage and re
-00003250: 7475 726e 7320 6120 6775 6172 6420 6861  turns a guard ha
-00003260: 6e64 6c65 2e20 5573 6520 7468 6973 0a20  ndle. Use this. 
-00003270: 2020 2020 2020 2077 6974 6820 6675 6e63         with func
-00003280: 7469 6f6e 7320 7468 6174 2064 6f6e 2774  tions that don't
-00003290: 2072 6571 7569 7265 206d 7574 6174 696f   require mutatio
-000032a0: 6e2e 0a20 2020 2020 2020 2022 2222 0a0a  n..        """..
-000032b0: 636c 6173 7320 4d65 6d53 746f 7261 6765  class MemStorage
-000032c0: 5265 6628 5f5f 4150 495f 5374 6f72 6167  Ref(__API_Storag
-000032d0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-000032e0: 5265 6665 7265 6e63 6520 7479 7065 206f  Reference type o
-000032f0: 6620 3a63 6c61 7373 3a60 4d65 6d53 746f  f :class:`MemSto
-00003300: 7261 6765 602e 0a20 2020 2022 2222 0a0a  rage`..    """..
-00003310: 2020 2020 6465 6620 636c 6f6e 6528 7365      def clone(se
-00003320: 6c66 2920 2d3e 2022 4d65 6d53 746f 7261  lf) -> "MemStora
-00003330: 6765 223a 202e 2e2e 0a20 2020 2064 6566  ge": ....    def
-00003340: 2077 6c28 7365 6c66 2920 2d3e 2022 4d65   wl(self) -> "Me
-00003350: 6d53 746f 7261 6765 436f 7265 5265 6622  mStorageCoreRef"
-00003360: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00003370: 2020 2020 2020 4f70 656e 7320 7570 2061        Opens up a
-00003380: 2077 7269 7465 206c 6f63 6b20 6f6e 2074   write lock on t
-00003390: 6865 2073 746f 7261 6765 2061 6e64 2072  he storage and r
-000033a0: 6574 7572 6e73 2067 7561 7264 2068 616e  eturns guard han
-000033b0: 646c 652e 2055 7365 2074 6869 730a 2020  dle. Use this.  
-000033c0: 2020 2020 2020 7769 7468 2066 756e 6374        with funct
-000033d0: 696f 6e73 2074 6861 7420 7461 6b65 2061  ions that take a
-000033e0: 206d 7574 6162 6c65 2072 6566 6572 656e   mutable referen
-000033f0: 6365 2074 6f20 7365 6c66 2e0a 2020 2020  ce to self..    
-00003400: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00003410: 726c 2873 656c 6629 202d 3e20 224d 656d  rl(self) -> "Mem
-00003420: 5374 6f72 6167 6543 6f72 6552 6566 223a  StorageCoreRef":
-00003430: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003440: 2020 2020 204f 7065 6e73 2075 7020 6120       Opens up a 
-00003450: 7265 6164 206c 6f63 6b20 6f6e 2074 6865  read lock on the
-00003460: 2073 746f 7261 6765 2061 6e64 2072 6574   storage and ret
-00003470: 7572 6e73 2061 2067 7561 7264 2068 616e  urns a guard han
-00003480: 646c 652e 2055 7365 2074 6869 730a 2020  dle. Use this.  
-00003490: 2020 2020 2020 7769 7468 2066 756e 6374        with funct
-000034a0: 696f 6e73 2074 6861 7420 646f 6e27 7420  ions that don't 
-000034b0: 7265 7175 6972 6520 6d75 7461 7469 6f6e  require mutation
-000034c0: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
-000034d0: 6c61 7373 2053 746f 7261 6765 285f 5f41  lass Storage(__A
-000034e0: 5049 5f53 746f 7261 6765 293a 0a20 2020  PI_Storage):.   
-000034f0: 2022 2222 0a20 2020 2053 746f 7261 6765   """.    Storage
-00003500: 2073 6176 6573 2061 6c6c 2074 6865 2069   saves all the i
-00003510: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00003520: 2074 6865 2063 7572 7265 6e74 2052 6166   the current Raf
-00003530: 7420 696d 706c 656d 656e 7461 7469 6f6e  t implementation
-00003540: 2c20 696e 636c 7564 696e 6720 5261 6674  , including Raft
-00003550: 204c 6f67 2c0a 2020 2020 636f 6d6d 6974   Log,.    commit
-00003560: 2069 6e64 6578 2c20 7468 6520 6c65 6164   index, the lead
-00003570: 6572 2074 6f20 766f 7465 2066 6f72 2c20  er to vote for, 
-00003580: 6574 632e 0a0a 2020 2020 4966 2061 6e79  etc...    If any
-00003590: 2053 746f 7261 6765 206d 6574 686f 6420   Storage method 
-000035a0: 7265 7475 726e 7320 616e 2065 7272 6f72  returns an error
-000035b0: 2c20 7468 6520 7261 6674 2069 6e73 7461  , the raft insta
-000035c0: 6e63 6520 7769 6c6c 0a20 2020 2062 6563  nce will.    bec
-000035d0: 6f6d 6520 696e 6f70 6572 6162 6c65 2061  ome inoperable a
-000035e0: 6e64 2072 6566 7573 6520 746f 2070 6172  nd refuse to par
-000035f0: 7469 6369 7061 7465 2069 6e20 656c 6563  ticipate in elec
-00003600: 7469 6f6e 733b 2074 6865 0a20 2020 2061  tions; the.    a
-00003610: 7070 6c69 6361 7469 6f6e 2069 7320 7265  pplication is re
-00003620: 7370 6f6e 7369 626c 6520 666f 7220 636c  sponsible for cl
-00003630: 6561 6e75 7020 616e 6420 7265 636f 7665  eanup and recove
-00003640: 7279 2069 6e20 7468 6973 2063 6173 652e  ry in this case.
-00003650: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-00003660: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-00003670: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-00003680: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
-00003690: 656c 6629 202d 3e20 2253 746f 7261 6765  elf) -> "Storage
-000036a0: 5265 6622 3a20 2e2e 2e0a 2020 2020 6465  Ref": ....    de
-000036b0: 6620 636c 6f6e 6528 7365 6c66 2920 2d3e  f clone(self) ->
-000036c0: 2022 5374 6f72 6167 6522 3a20 2e2e 2e0a   "Storage": ....
-000036d0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-000036e0: 640a 2020 2020 6465 6620 6465 6661 756c  d.    def defaul
-000036f0: 7428 2920 2d3e 2022 5374 6f72 6167 6522  t() -> "Storage"
-00003700: 3a20 2e2e 2e0a 2020 2020 4073 7461 7469  : ....    @stati
-00003710: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-00003720: 6e65 775f 7769 7468 5f63 6f6e 665f 7374  new_with_conf_st
-00003730: 6174 6528 0a20 2020 2020 2020 2063 6f6e  ate(.        con
-00003740: 665f 7374 6174 653a 2022 436f 6e66 5374  f_state: "ConfSt
-00003750: 6174 6522 207c 2022 436f 6e66 5374 6174  ate" | "ConfStat
-00003760: 6552 6566 222c 0a20 2020 2029 202d 3e20  eRef",.    ) -> 
-00003770: 2253 746f 7261 6765 223a 0a20 2020 2020  "Storage":.     
-00003780: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00003790: 6566 2077 6c28 7365 6c66 2920 2d3e 2041  ef wl(self) -> A
-000037a0: 6e79 3a0a 2020 2020 2020 2020 2222 220a  ny:.        """.
-000037b0: 2020 2020 2020 2020 4f70 656e 7320 7570          Opens up
-000037c0: 2061 2077 7269 7465 206c 6f63 6b20 6f6e   a write lock on
-000037d0: 2074 6865 2073 746f 7261 6765 2061 6e64   the storage and
-000037e0: 2072 6574 7572 6e73 2067 7561 7264 2068   returns guard h
-000037f0: 616e 646c 652e 2055 7365 2074 6869 730a  andle. Use this.
-00003800: 2020 2020 2020 2020 7769 7468 2066 756e          with fun
-00003810: 6374 696f 6e73 2074 6861 7420 7461 6b65  ctions that take
-00003820: 2061 206d 7574 6162 6c65 2072 6566 6572   a mutable refer
-00003830: 656e 6365 2074 6f20 7365 6c66 2e0a 2020  ence to self..  
-00003840: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00003850: 6620 726c 2873 656c 6629 202d 3e20 416e  f rl(self) -> An
-00003860: 793a 0a20 2020 2020 2020 2022 2222 0a20  y:.        """. 
-00003870: 2020 2020 2020 204f 7065 6e73 2075 7020         Opens up 
-00003880: 6120 7265 6164 206c 6f63 6b20 6f6e 2074  a read lock on t
-00003890: 6865 2073 746f 7261 6765 2061 6e64 2072  he storage and r
-000038a0: 6574 7572 6e73 2061 2067 7561 7264 2068  eturns a guard h
-000038b0: 616e 646c 652e 2055 7365 2074 6869 730a  andle. Use this.
-000038c0: 2020 2020 2020 2020 7769 7468 2066 756e          with fun
-000038d0: 6374 696f 6e73 2074 6861 7420 646f 6e27  ctions that don'
-000038e0: 7420 7265 7175 6972 6520 6d75 7461 7469  t require mutati
-000038f0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-00003900: 0a63 6c61 7373 2053 746f 7261 6765 5265  .class StorageRe
-00003910: 6628 5f5f 4150 495f 5374 6f72 6167 6529  f(__API_Storage)
-00003920: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00003930: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
-00003940: 3a63 6c61 7373 3a60 5374 6f72 6167 6560  :class:`Storage`
-00003950: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00003960: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-00003970: 3e20 2253 746f 7261 6765 223a 202e 2e2e  > "Storage": ...
-00003980: 0a20 2020 2064 6566 2077 6c28 7365 6c66  .    def wl(self
-00003990: 2920 2d3e 2041 6e79 3a0a 2020 2020 2020  ) -> Any:.      
-000039a0: 2020 2222 220a 2020 2020 2020 2020 4f70    """.        Op
-000039b0: 656e 7320 7570 2061 2077 7269 7465 206c  ens up a write l
-000039c0: 6f63 6b20 6f6e 2074 6865 2073 746f 7261  ock on the stora
-000039d0: 6765 2061 6e64 2072 6574 7572 6e73 2067  ge and returns g
-000039e0: 7561 7264 2068 616e 646c 652e 2055 7365  uard handle. Use
-000039f0: 2074 6869 730a 2020 2020 2020 2020 7769   this.        wi
-00003a00: 7468 2066 756e 6374 696f 6e73 2074 6861  th functions tha
-00003a10: 7420 7461 6b65 2061 206d 7574 6162 6c65  t take a mutable
-00003a20: 2072 6566 6572 656e 6365 2074 6f20 7365   reference to se
-00003a30: 6c66 2e0a 2020 2020 2020 2020 2222 220a  lf..        """.
-00003a40: 2020 2020 6465 6620 726c 2873 656c 6629      def rl(self)
-00003a50: 202d 3e20 416e 793a 0a20 2020 2020 2020   -> Any:.       
-00003a60: 2022 2222 0a20 2020 2020 2020 204f 7065   """.        Ope
-00003a70: 6e73 2075 7020 6120 7265 6164 206c 6f63  ns up a read loc
-00003a80: 6b20 6f6e 2074 6865 2073 746f 7261 6765  k on the storage
-00003a90: 2061 6e64 2072 6574 7572 6e73 2061 2067   and returns a g
-00003aa0: 7561 7264 2068 616e 646c 652e 2055 7365  uard handle. Use
-00003ab0: 2074 6869 730a 2020 2020 2020 2020 7769   this.        wi
-00003ac0: 7468 2066 756e 6374 696f 6e73 2074 6861  th functions tha
-00003ad0: 7420 646f 6e27 7420 7265 7175 6972 6520  t don't require 
-00003ae0: 6d75 7461 7469 6f6e 2e0a 2020 2020 2020  mutation..      
-00003af0: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-00003b00: 5049 5f52 6561 6479 3a0a 2020 2020 6465  PI_Ready:.    de
-00003b10: 6620 6873 2873 656c 6629 202d 3e20 4f70  f hs(self) -> Op
-00003b20: 7469 6f6e 616c 5b22 4861 7264 5374 6174  tional["HardStat
-00003b30: 6552 6566 225d 3a0a 2020 2020 2020 2020  eRef"]:.        
-00003b40: 2222 220a 2020 2020 2020 2020 5468 6520  """.        The 
-00003b50: 6375 7272 656e 7420 7374 6174 6520 6f66  current state of
-00003b60: 2061 204e 6f64 6520 746f 2062 6520 7361   a Node to be sa
-00003b70: 7665 6420 746f 2073 7461 626c 6520 7374  ved to stable st
-00003b80: 6f72 6167 652e 0a20 2020 2020 2020 2048  orage..        H
-00003b90: 6172 6453 7461 7465 2077 696c 6c20 6265  ardState will be
-00003ba0: 204e 6f6e 6520 7374 6174 6520 6966 2074   None state if t
-00003bb0: 6865 7265 2069 7320 6e6f 2075 7064 6174  here is no updat
-00003bc0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00003bd0: 2020 2064 6566 2073 7328 7365 6c66 2920     def ss(self) 
-00003be0: 2d3e 204f 7074 696f 6e61 6c5b 2253 6f66  -> Optional["Sof
-00003bf0: 7453 7461 7465 5265 6622 5d3a 0a20 2020  tStateRef"]:.   
-00003c00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003c10: 2054 6865 2063 7572 7265 6e74 2076 6f6c   The current vol
-00003c20: 6174 696c 6520 7374 6174 6520 6f66 2061  atile state of a
-00003c30: 204e 6f64 652e 0a20 2020 2020 2020 2053   Node..        S
-00003c40: 6f66 7453 7461 7465 2077 696c 6c20 6265  oftState will be
-00003c50: 204e 6f6e 6520 6966 2074 6865 7265 2069   None if there i
-00003c60: 7320 6e6f 2075 7064 6174 652e 0a20 2020  s no update..   
-00003c70: 2020 2020 2049 7420 6973 206e 6f74 2072       It is not r
-00003c80: 6571 7569 7265 6420 746f 2063 6f6e 7375  equired to consu
-00003c90: 6d65 206f 7220 7374 6f72 6520 536f 6674  me or store Soft
-00003ca0: 5374 6174 652e 0a20 2020 2020 2020 2022  State..        "
-00003cb0: 2222 0a20 2020 2064 6566 206d 7573 745f  "".    def must_
-00003cc0: 7379 6e63 2873 656c 6629 202d 3e20 626f  sync(self) -> bo
-00003cd0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-00003ce0: 2020 2020 2020 2020 4d75 7374 5379 6e63          MustSync
-00003cf0: 2069 7320 6661 6c73 6520 6966 2061 6e64   is false if and
-00003d00: 206f 6e6c 7920 6966 0a20 2020 2020 2020   only if.       
-00003d10: 2031 2e20 6e6f 2048 6172 6453 7461 7465   1. no HardState
-00003d20: 206f 7220 6f6e 6c79 2069 7473 2063 6f6d   or only its com
-00003d30: 6d69 7420 6973 2064 6966 6665 7265 6e74  mit is different
-00003d40: 2066 726f 6d20 6265 666f 7265 0a20 2020   from before.   
-00003d50: 2020 2020 2032 2e20 6e6f 2045 6e74 7269       2. no Entri
-00003d60: 6573 2061 6e64 2053 6e61 7073 686f 740a  es and Snapshot.
-00003d70: 2020 2020 2020 2020 4966 2069 7427 7320          If it's 
-00003d80: 6661 6c73 652c 2061 6e20 6173 796e 6368  false, an asynch
-00003d90: 726f 6e6f 7573 2077 7269 7465 206f 6620  ronous write of 
-00003da0: 4861 7264 5374 6174 6520 6973 2070 6572  HardState is per
-00003db0: 6d69 7373 6962 6c65 2062 6566 6f72 6520  missible before 
-00003dc0: 6361 6c6c 696e 670a 2020 2020 2020 2020  calling.        
-00003dd0: 5b60 5261 774e 6f64 653a 3a6f 6e5f 7065  [`RawNode::on_pe
-00003de0: 7273 6973 745f 7265 6164 7960 5d20 6f72  rsist_ready`] or
-00003df0: 205b 6052 6177 4e6f 6465 3a3a 6164 7661   [`RawNode::adva
-00003e00: 6e63 6560 5d20 6f72 2069 7473 2066 616d  nce`] or its fam
-00003e10: 696c 6965 732e 0a20 2020 2020 2020 2022  ilies..        "
-00003e20: 2222 0a20 2020 2064 6566 206e 756d 6265  "".    def numbe
-00003e30: 7228 7365 6c66 2920 2d3e 2069 6e74 3a0a  r(self) -> int:.
-00003e40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003e50: 2020 2020 5468 6520 6e75 6d62 6572 206f      The number o
-00003e60: 6620 6375 7272 656e 7420 5265 6164 792e  f current Ready.
-00003e70: 0a20 2020 2020 2020 2049 7420 6973 2075  .        It is u
-00003e80: 7365 6420 666f 7220 6964 656e 7469 6679  sed for identify
-00003e90: 696e 6720 7468 6520 6469 6666 6572 656e  ing the differen
-00003ea0: 7420 5265 6164 7920 616e 6420 5265 6164  t Ready and Read
-00003eb0: 7952 6563 6f72 642e 0a20 2020 2020 2020  yRecord..       
-00003ec0: 2022 2222 0a20 2020 2064 6566 2073 6e61   """.    def sna
-00003ed0: 7073 686f 7428 7365 6c66 2920 2d3e 2022  pshot(self) -> "
-00003ee0: 536e 6170 7368 6f74 5265 6622 3a0a 2020  SnapshotRef":.  
-00003ef0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003f00: 2020 536e 6170 7368 6f74 2073 7065 6369    Snapshot speci
-00003f10: 6669 6573 2074 6865 2073 6e61 7073 686f  fies the snapsho
-00003f20: 7420 746f 2062 6520 7361 7665 6420 746f  t to be saved to
-00003f30: 2073 7461 626c 6520 7374 6f72 6167 652e   stable storage.
-00003f40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003f50: 2064 6566 2063 6f6d 6d69 7474 6564 5f65   def committed_e
-00003f60: 6e74 7269 6573 2873 656c 6629 202d 3e20  ntries(self) -> 
-00003f70: 4c69 7374 5b22 456e 7472 7952 6566 225d  List["EntryRef"]
-00003f80: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00003f90: 2020 2020 2020 436f 6d6d 6974 7465 6445        CommittedE
-00003fa0: 6e74 7269 6573 2073 7065 6369 6669 6573  ntries specifies
-00003fb0: 2065 6e74 7269 6573 2074 6f20 6265 2063   entries to be c
-00003fc0: 6f6d 6d69 7474 6564 2074 6f20 610a 2020  ommitted to a.  
-00003fd0: 2020 2020 2020 7374 6f72 652f 7374 6174        store/stat
-00003fe0: 652d 6d61 6368 696e 652e 2054 6865 7365  e-machine. These
-00003ff0: 2068 6176 6520 7072 6576 696f 7573 6c79   have previously
-00004000: 2062 6565 6e20 636f 6d6d 6974 7465 6420   been committed 
-00004010: 746f 2073 7461 626c 650a 2020 2020 2020  to stable.      
-00004020: 2020 7374 6f72 652e 0a20 2020 2020 2020    store..       
-00004030: 2022 2222 0a20 2020 2064 6566 2074 616b   """.    def tak
-00004040: 655f 636f 6d6d 6974 7465 645f 656e 7472  e_committed_entr
-00004050: 6965 7328 7365 6c66 2920 2d3e 204c 6973  ies(self) -> Lis
-00004060: 745b 2245 6e74 7279 225d 3a0a 2020 2020  t["Entry"]:.    
-00004070: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004080: 5461 6b65 2074 6865 2043 6f6d 6d69 7445  Take the CommitE
-00004090: 6e74 7269 6573 2e0a 2020 2020 2020 2020  ntries..        
-000040a0: 2222 220a 2020 2020 6465 6620 656e 7472  """.    def entr
-000040b0: 6965 7328 7365 6c66 2920 2d3e 204c 6973  ies(self) -> Lis
-000040c0: 745b 2245 6e74 7279 5265 6622 5d3a 0a20  t["EntryRef"]:. 
-000040d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000040e0: 2020 2045 6e74 7269 6573 2073 7065 6369     Entries speci
-000040f0: 6669 6573 2065 6e74 7269 6573 2074 6f20  fies entries to 
-00004100: 6265 2073 6176 6564 2074 6f20 7374 6162  be saved to stab
-00004110: 6c65 2073 746f 7261 6765 2e0a 2020 2020  le storage..    
-00004120: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00004130: 7461 6b65 5f65 6e74 7269 6573 2873 656c  take_entries(sel
-00004140: 6629 202d 3e20 4c69 7374 5b22 456e 7472  f) -> List["Entr
-00004150: 7922 5d3a 0a20 2020 2020 2020 2022 2222  y"]:.        """
-00004160: 0a20 2020 2020 2020 2054 616b 6520 7468  .        Take th
-00004170: 6520 456e 7472 6965 732e 0a20 2020 2020  e Entries..     
-00004180: 2020 2022 2222 0a20 2020 2064 6566 206d     """.    def m
-00004190: 6573 7361 6765 7328 7365 6c66 2920 2d3e  essages(self) ->
-000041a0: 204c 6973 745b 224d 6573 7361 6765 5265   List["MessageRe
-000041b0: 6622 5d3a 0a20 2020 2020 2020 2022 2222  f"]:.        """
-000041c0: 0a20 2020 2020 2020 204d 6573 7361 6765  .        Message
-000041d0: 7320 7370 6563 6966 6965 7320 6f75 7462  s specifies outb
-000041e0: 6f75 6e64 206d 6573 7361 6765 7320 746f  ound messages to
-000041f0: 2062 6520 7365 6e74 2e0a 2020 2020 2020   be sent..      
-00004200: 2020 4966 2069 7420 636f 6e74 6169 6e73    If it contains
-00004210: 2061 204d 7367 536e 6170 206d 6573 7361   a MsgSnap messa
-00004220: 6765 2c20 7468 6520 6170 706c 6963 6174  ge, the applicat
-00004230: 696f 6e20 4d55 5354 2072 6570 6f72 7420  ion MUST report 
-00004240: 6261 636b 2074 6f20 7261 6674 0a20 2020  back to raft.   
-00004250: 2020 2020 2077 6865 6e20 7468 6520 736e       when the sn
-00004260: 6170 7368 6f74 2068 6173 2062 6565 6e20  apshot has been 
-00004270: 7265 6365 6976 6564 206f 7220 6861 7320  received or has 
-00004280: 6661 696c 6564 2062 7920 6361 6c6c 696e  failed by callin
-00004290: 6720 5265 706f 7274 536e 6170 7368 6f74  g ReportSnapshot
-000042a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000042b0: 2020 6465 6620 7461 6b65 5f6d 6573 7361    def take_messa
-000042c0: 6765 7328 7365 6c66 2920 2d3e 204c 6973  ges(self) -> Lis
-000042d0: 745b 224d 6573 7361 6765 225d 3a0a 2020  t["Message"]:.  
-000042e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000042f0: 2020 5461 6b65 2074 6865 204d 6573 7361    Take the Messa
-00004300: 6765 732e 0a20 2020 2020 2020 2022 2222  ges..        """
-00004310: 0a20 2020 2064 6566 2070 6572 7369 7374  .    def persist
-00004320: 6564 5f6d 6573 7361 6765 7328 7365 6c66  ed_messages(self
-00004330: 2920 2d3e 204c 6973 745b 224d 6573 7361  ) -> List["Messa
-00004340: 6765 5265 6622 5d3a 0a20 2020 2020 2020  geRef"]:.       
-00004350: 2022 2222 0a20 2020 2020 2020 2050 6572   """.        Per
-00004360: 7369 7374 6564 204d 6573 7361 6765 7320  sisted Messages 
-00004370: 7370 6563 6966 6965 7320 6f75 7462 6f75  specifies outbou
-00004380: 6e64 206d 6573 7361 6765 7320 746f 2062  nd messages to b
-00004390: 6520 7365 6e74 2041 4654 4552 2074 6865  e sent AFTER the
-000043a0: 2048 6172 6453 7461 7465 2c0a 2020 2020   HardState,.    
-000043b0: 2020 2020 456e 7472 6965 7320 616e 6420      Entries and 
-000043c0: 536e 6170 7368 6f74 2061 7265 2070 6572  Snapshot are per
-000043d0: 7369 7374 6564 2074 6f20 7374 6162 6c65  sisted to stable
-000043e0: 2073 746f 7261 6765 2e0a 2020 2020 2020   storage..      
-000043f0: 2020 2222 220a 2020 2020 6465 6620 7461    """.    def ta
-00004400: 6b65 5f70 6572 7369 7374 6564 5f6d 6573  ke_persisted_mes
-00004410: 7361 6765 7328 7365 6c66 2920 2d3e 204c  sages(self) -> L
-00004420: 6973 745b 224d 6573 7361 6765 225d 3a0a  ist["Message"]:.
-00004430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004440: 2020 2020 5461 6b65 2074 6865 2050 6572      Take the Per
-00004450: 7369 7374 6564 204d 6573 7361 6765 732e  sisted Messages.
-00004460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004470: 2064 6566 2072 6561 645f 7374 6174 6573   def read_states
-00004480: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
-00004490: 5265 6164 5374 6174 6552 6566 225d 3a0a  ReadStateRef"]:.
-000044a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000044b0: 2020 2020 5265 6164 5374 6174 6573 2073      ReadStates s
-000044c0: 7065 6369 6669 6573 2074 6865 2073 7461  pecifies the sta
-000044d0: 7465 2066 6f72 2072 6561 6420 6f6e 6c79  te for read only
-000044e0: 2071 7565 7279 2e0a 2020 2020 2020 2020   query..        
-000044f0: 2222 220a 2020 2020 6465 6620 7461 6b65  """.    def take
-00004500: 5f72 6561 645f 7374 6174 6573 2873 656c  _read_states(sel
-00004510: 6629 202d 3e20 4c69 7374 5b22 5265 6164  f) -> List["Read
-00004520: 5374 6174 6522 5d3a 0a20 2020 2020 2020  State"]:.       
-00004530: 2022 2222 0a20 2020 2020 2020 2052 6561   """.        Rea
-00004540: 6453 7461 7465 7320 7370 6563 6966 6965  dStates specifie
-00004550: 7320 7468 6520 7374 6174 6520 666f 7220  s the state for 
-00004560: 7265 6164 206f 6e6c 7920 7175 6572 792e  read only query.
-00004570: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
-00004580: 6173 7320 5265 6164 7928 5f5f 4150 495f  ass Ready(__API_
-00004590: 5265 6164 7929 3a0a 2020 2020 2222 220a  Ready):.    """.
-000045a0: 2020 2020 5265 6164 7920 656e 6361 7073      Ready encaps
-000045b0: 756c 6174 6573 2074 6865 2065 6e74 7269  ulates the entri
-000045c0: 6573 2061 6e64 206d 6573 7361 6765 7320  es and messages 
-000045d0: 7468 6174 2061 7265 2072 6561 6479 2074  that are ready t
-000045e0: 6f20 7265 6164 2c0a 2020 2020 6265 2073  o read,.    be s
-000045f0: 6176 6564 2074 6f20 7374 6162 6c65 2073  aved to stable s
-00004600: 746f 7261 6765 2c20 636f 6d6d 6974 7465  torage, committe
-00004610: 6420 6f72 2073 656e 7420 746f 206f 7468  d or sent to oth
-00004620: 6572 2070 6565 7273 2e0a 2020 2020 2222  er peers..    ""
-00004630: 220a 0a20 2020 2064 6566 206d 616b 655f  "..    def make_
-00004640: 7265 6628 7365 6c66 2920 2d3e 2022 5265  ref(self) -> "Re
-00004650: 6164 7952 6566 223a 202e 2e2e 0a20 2020  adyRef": ....   
-00004660: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00004670: 2020 2064 6566 2064 6566 6175 6c74 2829     def default()
-00004680: 202d 3e20 2252 6561 6479 223a 202e 2e2e   -> "Ready": ...
-00004690: 0a0a 636c 6173 7320 5265 6164 7952 6566  ..class ReadyRef
-000046a0: 285f 5f41 5049 5f52 6561 6479 293a 0a20  (__API_Ready):. 
-000046b0: 2020 2022 2222 0a20 2020 2052 6566 6572     """.    Refer
-000046c0: 656e 6365 2074 7970 6520 6f66 203a 636c  ence type of :cl
-000046d0: 6173 733a 6052 6561 6479 602e 0a20 2020  ass:`Ready`..   
-000046e0: 2022 2222 0a0a 636c 6173 7320 5f5f 4150   """..class __AP
-000046f0: 495f 5261 774e 6f64 653a 0a20 2020 2064  I_RawNode:.    d
-00004700: 6566 2061 6476 616e 6365 5f61 7070 6c79  ef advance_apply
-00004710: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00004720: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004730: 2020 2020 4164 7661 6e63 6520 6170 706c      Advance appl
-00004740: 7920 746f 2074 6865 2069 6e64 6578 206f  y to the index o
-00004750: 6620 7468 6520 6c61 7374 2063 6f6d 6d69  f the last commi
-00004760: 7474 6564 2065 6e74 7269 6573 2067 6976  tted entries giv
-00004770: 656e 2062 6566 6f72 652e 0a20 2020 2020  en before..     
-00004780: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
-00004790: 6476 616e 6365 5f61 7070 6c79 5f74 6f28  dvance_apply_to(
-000047a0: 7365 6c66 2c20 6170 706c 6965 643a 2069  self, applied: i
-000047b0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-000047c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000047d0: 2041 6476 616e 6365 2061 7070 6c79 2074   Advance apply t
-000047e0: 6f20 7468 6520 7061 7373 6564 2069 6e64  o the passed ind
-000047f0: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
-00004800: 2020 2020 6465 6620 6164 7661 6e63 6528      def advance(
-00004810: 7365 6c66 2c20 7264 3a20 2252 6561 6479  self, rd: "Ready
-00004820: 5265 6622 2920 2d3e 2022 4c69 6768 7452  Ref") -> "LightR
-00004830: 6561 6479 223a 0a20 2020 2020 2020 2022  eady":.        "
-00004840: 2222 0a20 2020 2020 2020 2041 6476 616e  "".        Advan
-00004850: 6365 7320 7468 6520 7265 6164 7920 6166  ces the ready af
-00004860: 7465 7220 6675 6c6c 7920 7072 6f63 6573  ter fully proces
-00004870: 7369 6e67 2069 742e 0a0a 2020 2020 2020  sing it...      
-00004880: 2020 4675 6c6c 7920 7072 6f63 6573 7369    Fully processi
-00004890: 6e67 2061 2072 6561 6479 2072 6571 7569  ng a ready requi
-000048a0: 7265 7320 746f 2070 6572 7369 7374 2073  res to persist s
-000048b0: 6e61 7073 686f 742c 2065 6e74 7269 6573  napshot, entries
-000048c0: 2061 6e64 2068 6172 6420 7374 6174 6573   and hard states
-000048d0: 2c20 6170 706c 7920 616c 6c0a 2020 2020  , apply all.    
-000048e0: 2020 2020 636f 6d6d 6974 7465 6420 656e      committed en
-000048f0: 7472 6965 732c 2073 656e 6420 616c 6c20  tries, send all 
-00004900: 6d65 7373 6167 6573 2e0a 0a20 2020 2020  messages...     
-00004910: 2020 2052 6574 7572 6e73 2074 6865 204c     Returns the L
-00004920: 6967 6874 5265 6164 7920 7468 6174 2063  ightReady that c
-00004930: 6f6e 7461 696e 7320 636f 6d6d 6974 2069  ontains commit i
-00004940: 6e64 6578 2c20 636f 6d6d 6974 7465 6420  ndex, committed 
-00004950: 656e 7472 6965 7320 616e 6420 6d65 7373  entries and mess
-00004960: 6167 6573 2e20 5b60 4c69 6768 7452 6561  ages. [`LightRea
-00004970: 6479 605d 0a20 2020 2020 2020 2063 6f6e  dy`].        con
-00004980: 7461 696e 7320 7570 6461 7465 7320 7468  tains updates th
-00004990: 6174 206f 6e6c 7920 7661 6c69 6420 6166  at only valid af
-000049a0: 7465 7220 7065 7273 6973 7469 6e67 206c  ter persisting l
-000049b0: 6173 7420 7265 6164 792e 2049 7420 7368  ast ready. It sh
-000049c0: 6f75 6c64 2061 6c73 6f20 6265 2066 756c  ould also be ful
-000049d0: 6c79 2070 726f 6365 7373 6564 2e0a 2020  ly processed..  
-000049e0: 2020 2020 2020 5468 656e 205b 6053 656c        Then [`Sel
-000049f0: 663a 3a61 6476 616e 6365 5f61 7070 6c79  f::advance_apply
-00004a00: 605d 206f 7220 5b60 5365 6c66 3a3a 6164  `] or [`Self::ad
-00004a10: 7661 6e63 655f 6170 706c 795f 746f 605d  vance_apply_to`]
-00004a20: 2073 686f 756c 6420 6265 2075 7365 6420   should be used 
-00004a30: 6c61 7465 7220 746f 2075 7064 6174 6520  later to update 
-00004a40: 6170 706c 7969 6e67 0a20 2020 2020 2020  applying.       
-00004a50: 2070 726f 6772 6573 732e 0a20 2020 2020   progress..     
-00004a60: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
-00004a70: 6476 616e 6365 5f61 7070 656e 6428 7365  dvance_append(se
-00004a80: 6c66 2c20 7264 3a20 2252 6561 6479 5265  lf, rd: "ReadyRe
-00004a90: 6622 2920 2d3e 2022 4c69 6768 7452 6561  f") -> "LightRea
-00004aa0: 6479 223a 0a20 2020 2020 2020 2022 2222  dy":.        """
-00004ab0: 0a20 2020 2020 2020 2041 6476 616e 6365  .        Advance
-00004ac0: 7320 7468 6520 7265 6164 7920 7769 7468  s the ready with
-00004ad0: 6f75 7420 6170 706c 7969 6e67 2063 6f6d  out applying com
-00004ae0: 6d69 7474 6564 2065 6e74 7269 6573 2e20  mitted entries. 
-00004af0: 5b60 5365 6c66 3a3a 6164 7661 6e63 655f  [`Self::advance_
-00004b00: 6170 706c 7960 5d20 6f72 0a20 2020 2020  apply`] or.     
-00004b10: 2020 205b 6053 656c 663a 3a61 6476 616e     [`Self::advan
-00004b20: 6365 5f61 7070 6c79 5f74 6f60 5d20 7368  ce_apply_to`] sh
-00004b30: 6f75 6c64 2062 6520 7573 6564 206c 6174  ould be used lat
-00004b40: 6572 2074 6f20 7570 6461 7465 2061 7070  er to update app
-00004b50: 6c79 696e 6720 7072 6f67 7265 7373 2e0a  lying progress..
-00004b60: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004b70: 2074 6865 204c 6967 6874 5265 6164 7920   the LightReady 
-00004b80: 7468 6174 2063 6f6e 7461 696e 7320 636f  that contains co
-00004b90: 6d6d 6974 2069 6e64 6578 2c20 636f 6d6d  mmit index, comm
-00004ba0: 6974 7465 6420 656e 7472 6965 7320 616e  itted entries an
-00004bb0: 6420 6d65 7373 6167 6573 2e0a 0a20 2020  d messages...   
-00004bc0: 2020 2020 2053 696e 6365 2052 6561 6479       Since Ready
-00004bd0: 206d 7573 7420 6265 2070 6572 7369 7374   must be persist
-00004be0: 6564 2069 6e20 6f72 6465 722c 2063 616c  ed in order, cal
-00004bf0: 6c69 6e67 2074 6869 7320 6675 6e63 7469  ling this functi
-00004c00: 6f6e 2069 6d70 6c69 6369 746c 7920 6d65  on implicitly me
-00004c10: 616e 730a 2020 2020 2020 2020 616c 6c20  ans.        all 
-00004c20: 7265 6164 7920 636f 6c6c 6563 7465 6420  ready collected 
-00004c30: 6265 666f 7265 2068 6176 6520 6265 656e  before have been
-00004c40: 2070 6572 7369 7374 6564 2e0a 2020 2020   persisted..    
-00004c50: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00004c60: 6164 7661 6e63 655f 6170 7065 6e64 5f61  advance_append_a
-00004c70: 7379 6e63 2873 656c 662c 2072 643a 2022  sync(self, rd: "
-00004c80: 5265 6164 7952 6566 2229 202d 3e20 4e6f  ReadyRef") -> No
-00004c90: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00004ca0: 2020 2020 2020 2020 5361 6d65 2061 7320          Same as 
-00004cb0: 5b60 5365 6c66 3a3a 6164 7661 6e63 655f  [`Self::advance_
-00004cc0: 6170 7065 6e64 605d 2065 7863 6570 7420  append`] except 
-00004cd0: 7468 6174 2069 7420 616c 6c6f 7773 2074  that it allows t
-00004ce0: 6f20 6f6e 6c79 2073 746f 7265 2074 6865  o only store the
-00004cf0: 2075 7064 6174 6573 2069 6e20 6361 6368   updates in cach
-00004d00: 652e 0a20 2020 2020 2020 205b 6053 656c  e..        [`Sel
-00004d10: 663a 3a6f 6e5f 7065 7273 6973 745f 7265  f::on_persist_re
-00004d20: 6164 7960 5d20 7368 6f75 6c64 2062 6520  ady`] should be 
-00004d30: 7573 6564 206c 6174 6572 2074 6f20 7570  used later to up
-00004d40: 6461 7465 2074 6865 2070 6572 7369 7374  date the persist
-00004d50: 696e 6720 7072 6f67 7265 7373 2e0a 0a20  ing progress... 
-00004d60: 2020 2020 2020 2052 6166 7420 776f 726b         Raft work
-00004d70: 7320 6f6e 2061 6e20 6173 7375 6d70 7469  s on an assumpti
-00004d80: 6f6e 2070 6572 7369 7374 6564 2075 7064  on persisted upd
-00004d90: 6174 6573 2073 686f 756c 6420 6e6f 7420  ates should not 
-00004da0: 6265 206c 6f73 742c 2077 6869 6368 2075  be lost, which u
-00004db0: 7375 616c 6c79 2072 6571 7569 7265 7320  sually requires 
-00004dc0: 6578 7065 6e73 6976 650a 2020 2020 2020  expensive.      
-00004dd0: 2020 6f70 6572 6174 696f 6e73 206c 696b    operations lik
-00004de0: 6520 6066 7379 6e63 602e 2060 6164 7661  e `fsync`. `adva
-00004df0: 6e63 655f 6170 7065 6e64 5f61 7379 6e63  nce_append_async
-00004e00: 6020 616c 6c6f 7773 2079 6f75 2074 6f20  ` allows you to 
-00004e10: 636f 6e74 726f 6c20 7468 6520 7261 7465  control the rate
-00004e20: 206f 6620 7375 6368 206f 7065 7261 7469   of such operati
-00004e30: 6f6e 7320 616e 640a 2020 2020 2020 2020  ons and.        
-00004e40: 6765 7420 6120 7265 6173 6f6e 6162 6c65  get a reasonable
-00004e50: 2062 6174 6368 2073 697a 652e 2048 6f77   batch size. How
-00004e60: 6576 6572 2c20 6974 2773 2073 7469 6c6c  ever, it's still
-00004e70: 2072 6571 7569 7265 6420 7468 6174 2074   required that t
-00004e80: 6865 2075 7064 6174 6573 2063 616e 2062  he updates can b
-00004e90: 6520 7265 6164 2062 7920 7261 6674 2066  e read by raft f
-00004ea0: 726f 6d20 7468 650a 2020 2020 2020 2020  rom the.        
-00004eb0: 6053 746f 7261 6765 6020 7472 6169 7420  `Storage` trait 
-00004ec0: 6265 666f 7265 2063 616c 6c69 6e67 2060  before calling `
-00004ed0: 6164 7661 6e63 655f 6170 7065 6e64 5f61  advance_append_a
-00004ee0: 7379 6e63 602e 0a20 2020 2020 2020 2022  sync`..        "
-00004ef0: 2222 0a20 2020 2064 6566 2068 6173 5f72  "".    def has_r
-00004f00: 6561 6479 2873 656c 6629 202d 3e20 626f  eady(self) -> bo
-00004f10: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-00004f20: 2020 2020 2020 2020 4861 7352 6561 6479          HasReady
-00004f30: 2063 616c 6c65 6420 7768 656e 2052 6177   called when Raw
-00004f40: 4e6f 6465 2075 7365 7220 6e65 6564 2074  Node user need t
-00004f50: 6f20 6368 6563 6b20 6966 2061 6e79 2052  o check if any R
-00004f60: 6561 6479 2070 656e 6469 6e67 2e0a 2020  eady pending..  
-00004f70: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00004f80: 6620 7469 636b 2873 656c 6629 202d 3e20  f tick(self) -> 
-00004f90: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00004fa0: 220a 2020 2020 2020 2020 5469 636b 2061  ".        Tick a
-00004fb0: 6476 616e 6365 7320 7468 6520 696e 7465  dvances the inte
-00004fc0: 726e 616c 206c 6f67 6963 616c 2063 6c6f  rnal logical clo
-00004fd0: 636b 2062 7920 6120 7369 6e67 6c65 2074  ck by a single t
-00004fe0: 6963 6b2e 0a0a 2020 2020 2020 2020 5265  ick...        Re
-00004ff0: 7475 726e 7320 7472 7565 2074 6f20 696e  turns true to in
-00005000: 6469 6361 7465 2074 6861 7420 7468 6572  dicate that ther
-00005010: 6520 7769 6c6c 2070 726f 6261 626c 7920  e will probably 
-00005020: 6265 2073 6f6d 6520 7265 6164 696e 6573  be some readines
-00005030: 7320 7768 6963 680a 2020 2020 2020 2020  s which.        
-00005040: 6e65 6564 7320 746f 2062 6520 6861 6e64  needs to be hand
-00005050: 6c65 642e 0a20 2020 2020 2020 2022 2222  led..        """
-00005060: 0a20 2020 2064 6566 2073 6574 5f62 6174  .    def set_bat
-00005070: 6368 5f61 7070 656e 6428 7365 6c66 2c20  ch_append(self, 
-00005080: 6261 7463 685f 6170 7065 6e64 3a20 626f  batch_append: bo
-00005090: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-000050a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000050b0: 2053 6574 2077 6865 7468 6572 2074 6f20   Set whether to 
-000050c0: 6261 7463 6820 6170 7065 6e64 206d 7367  batch append msg
-000050d0: 2061 7420 7275 6e74 696d 652e 0a20 2020   at runtime..   
-000050e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-000050f0: 2073 6574 5f70 7269 6f72 6974 7928 7365   set_priority(se
-00005100: 6c66 2c20 7072 696f 7269 7479 3a20 696e  lf, priority: in
-00005110: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00005120: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005130: 5365 7473 2070 7269 6f72 6974 7920 6f66  Sets priority of
-00005140: 206e 6f64 652e 0a20 2020 2020 2020 2022   node..        "
-00005150: 2222 0a20 2020 2064 6566 2072 6570 6f72  "".    def repor
-00005160: 745f 736e 6170 7368 6f74 2873 656c 662c  t_snapshot(self,
-00005170: 2069 643a 2069 6e74 2c20 736e 6170 7368   id: int, snapsh
-00005180: 6f74 3a20 2253 6e61 7073 686f 7453 7461  ot: "SnapshotSta
-00005190: 7475 7322 2920 2d3e 204e 6f6e 653a 0a20  tus") -> None:. 
-000051a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000051b0: 2020 2052 6570 6f72 7453 6e61 7073 686f     ReportSnapsho
-000051c0: 7420 7265 706f 7274 7320 7468 6520 7374  t reports the st
-000051d0: 6174 7573 206f 6620 7468 6520 7365 6e74  atus of the sent
-000051e0: 2073 6e61 7073 686f 742e 0a20 2020 2020   snapshot..     
-000051f0: 2020 2022 2222 0a20 2020 2064 6566 2072     """.    def r
-00005200: 6570 6f72 745f 756e 7265 6163 6861 626c  eport_unreachabl
-00005210: 6528 7365 6c66 2c20 6964 3a20 696e 7429  e(self, id: int)
-00005220: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00005230: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00005240: 706f 7274 556e 7265 6163 6861 626c 6520  portUnreachable 
-00005250: 7265 706f 7274 7320 7468 6520 6769 7665  reports the give
-00005260: 6e20 6e6f 6465 2069 7320 6e6f 7420 7265  n node is not re
-00005270: 6163 6861 626c 6520 666f 7220 7468 6520  achable for the 
-00005280: 6c61 7374 2073 656e 642e 0a20 2020 2020  last send..     
-00005290: 2020 2022 2222 0a20 2020 2064 6566 2074     """.    def t
-000052a0: 7261 6e73 6665 725f 6c65 6164 6572 2873  ransfer_leader(s
-000052b0: 656c 662c 2074 7261 6e73 6665 7265 653a  elf, transferee:
-000052c0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-000052d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000052e0: 2020 2054 7261 6e73 6665 724c 6561 6465     TransferLeade
-000052f0: 7220 7472 6965 7320 746f 2074 7261 6e73  r tries to trans
-00005300: 6665 7220 6c65 6164 6572 7368 6970 2074  fer leadership t
-00005310: 6f20 7468 6520 6769 7665 6e20 7472 616e  o the given tran
-00005320: 7366 6572 6565 2e0a 2020 2020 2020 2020  sferee..        
-00005330: 2222 220a 2020 2020 6465 6620 736e 6170  """.    def snap
-00005340: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
-00005350: 616c 5b22 536e 6170 7368 6f74 5265 6622  al["SnapshotRef"
-00005360: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-00005370: 2020 2020 2020 2047 7261 6273 2074 6865         Grabs the
-00005380: 2073 6e61 7073 686f 7420 6672 6f6d 2074   snapshot from t
-00005390: 6865 2072 6166 7420 6966 2061 7661 696c  he raft if avail
-000053a0: 6162 6c65 2e0a 2020 2020 2020 2020 2222  able..        ""
-000053b0: 220a 2020 2020 6465 6620 7374 6570 2873  ".    def step(s
-000053c0: 656c 662c 206d 7367 3a20 224d 6573 7361  elf, msg: "Messa
-000053d0: 6765 2220 7c20 224d 6573 7361 6765 5265  ge" | "MessageRe
-000053e0: 6622 2920 2d3e 204e 6f6e 653a 0a20 2020  f") -> None:.   
-000053f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005400: 2053 7465 7020 6164 7661 6e63 6573 2074   Step advances t
-00005410: 6865 2073 7461 7465 206d 6163 6869 6e65  he state machine
-00005420: 2075 7369 6e67 2074 6865 2067 6976 656e   using the given
-00005430: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
-00005440: 2020 2222 220a 2020 2020 6465 6620 736b    """.    def sk
-00005450: 6970 5f62 6361 7374 5f63 6f6d 6d69 7428  ip_bcast_commit(
-00005460: 7365 6c66 2c20 736b 6970 3a20 626f 6f6c  self, skip: bool
-00005470: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00005480: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00005490: 6574 2077 6865 7468 6572 2073 6b69 7020  et whether skip 
-000054a0: 6272 6f61 6463 6173 7420 656d 7074 7920  broadcast empty 
-000054b0: 636f 6d6d 6974 206d 6573 7361 6765 7320  commit messages 
-000054c0: 6174 2072 756e 7469 6d65 2e0a 2020 2020  at runtime..    
-000054d0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-000054e0: 6361 6d70 6169 676e 2873 656c 6629 202d  campaign(self) -
-000054f0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00005500: 2222 220a 2020 2020 2020 2020 4361 6d70  """.        Camp
-00005510: 6169 676e 2063 6175 7365 7320 7468 6973  aign causes this
-00005520: 2052 6177 4e6f 6465 2074 6f20 7472 616e   RawNode to tran
-00005530: 7369 7469 6f6e 2074 6f20 6361 6e64 6964  sition to candid
-00005540: 6174 6520 7374 6174 652e 0a20 2020 2020  ate state..     
-00005550: 2020 2022 2222 0a20 2020 2064 6566 2070     """.    def p
-00005560: 726f 706f 7365 2873 656c 662c 2063 6f6e  ropose(self, con
-00005570: 7465 7874 3a20 6279 7465 732c 2064 6174  text: bytes, dat
-00005580: 613a 2062 7974 6573 2920 2d3e 204e 6f6e  a: bytes) -> Non
-00005590: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000055a0: 2020 2020 2020 2050 726f 706f 7365 2070         Propose p
-000055b0: 726f 706f 7365 7320 6461 7461 2062 6520  roposes data be 
-000055c0: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
-000055d0: 7261 6674 206c 6f67 2e0a 2020 2020 2020  raft log..      
-000055e0: 2020 2222 220a 2020 2020 6465 6620 7072    """.    def pr
-000055f0: 6f70 6f73 655f 636f 6e66 5f63 6861 6e67  opose_conf_chang
-00005600: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-00005610: 2063 6f6e 7465 7874 3a20 6279 7465 732c   context: bytes,
-00005620: 2063 633a 2022 436f 6e66 4368 616e 6765   cc: "ConfChange
-00005630: 2220 7c20 2243 6f6e 6643 6861 6e67 6552  " | "ConfChangeR
-00005640: 6566 220a 2020 2020 2920 2d3e 204e 6f6e  ef".    ) -> Non
-00005650: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00005660: 2020 2020 2020 2050 726f 706f 7365 436f         ProposeCo
-00005670: 6e66 4368 616e 6765 2070 726f 706f 7365  nfChange propose
-00005680: 7320 6120 636f 6e66 6967 2063 6861 6e67  s a config chang
-00005690: 652e 0a0a 2020 2020 2020 2020 4966 2074  e...        If t
-000056a0: 6865 206e 6f64 6520 656e 7465 7273 206a  he node enters j
-000056b0: 6f69 6e74 2073 7461 7465 2077 6974 6820  oint state with 
-000056c0: 6061 7574 6f5f 6c65 6176 6560 2073 6574  `auto_leave` set
-000056d0: 2074 6f20 7472 7565 2c20 6974 2773 0a20   to true, it's. 
-000056e0: 2020 2020 2020 2063 616c 6c65 7227 7320         caller's 
-000056f0: 7265 7370 6f6e 7369 6269 6c69 7479 2074  responsibility t
-00005700: 6f20 7072 6f70 6f73 6520 616e 2065 6d70  o propose an emp
-00005710: 7479 2063 6f6e 6620 6368 616e 6765 2061  ty conf change a
-00005720: 6761 696e 2074 6f20 666f 7263 650a 2020  gain to force.  
-00005730: 2020 2020 2020 6c65 6176 696e 6720 6a6f        leaving jo
-00005740: 696e 7420 7374 6174 652e 0a20 2020 2020  int state..     
-00005750: 2020 2022 2222 0a20 2020 2064 6566 2070     """.    def p
-00005760: 726f 706f 7365 5f63 6f6e 665f 6368 616e  ropose_conf_chan
-00005770: 6765 5f76 3228 0a20 2020 2020 2020 2073  ge_v2(.        s
-00005780: 656c 662c 2063 6f6e 7465 7874 3a20 6279  elf, context: by
-00005790: 7465 732c 2063 633a 2022 436f 6e66 4368  tes, cc: "ConfCh
-000057a0: 616e 6765 5632 2220 7c20 2243 6f6e 6643  angeV2" | "ConfC
-000057b0: 6861 6e67 6556 3252 6566 220a 2020 2020  hangeV2Ref".    
-000057c0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000057d0: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-000057e0: 726f 706f 7365 436f 6e66 4368 616e 6765  roposeConfChange
-000057f0: 2070 726f 706f 7365 7320 6120 636f 6e66   proposes a conf
-00005800: 6967 2063 6861 6e67 652e 0a0a 2020 2020  ig change...    
-00005810: 2020 2020 4966 2074 6865 206e 6f64 6520      If the node 
-00005820: 656e 7465 7273 206a 6f69 6e74 2073 7461  enters joint sta
-00005830: 7465 2077 6974 6820 6061 7574 6f5f 6c65  te with `auto_le
-00005840: 6176 6560 2073 6574 2074 6f20 7472 7565  ave` set to true
-00005850: 2c20 6974 2773 0a20 2020 2020 2020 2063  , it's.        c
-00005860: 616c 6c65 7227 7320 7265 7370 6f6e 7369  aller's responsi
-00005870: 6269 6c69 7479 2074 6f20 7072 6f70 6f73  bility to propos
-00005880: 6520 616e 2065 6d70 7479 2063 6f6e 6620  e an empty conf 
-00005890: 6368 616e 6765 2061 6761 696e 2074 6f20  change again to 
-000058a0: 666f 7263 650a 2020 2020 2020 2020 6c65  force.        le
-000058b0: 6176 696e 6720 6a6f 696e 7420 7374 6174  aving joint stat
-000058c0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-000058d0: 2020 2064 6566 2061 7070 6c79 5f63 6f6e     def apply_con
-000058e0: 665f 6368 616e 6765 2873 656c 662c 2063  f_change(self, c
-000058f0: 633a 2022 436f 6e66 4368 616e 6765 2220  c: "ConfChange" 
-00005900: 7c20 2243 6f6e 6643 6861 6e67 6552 6566  | "ConfChangeRef
-00005910: 2229 202d 3e20 436f 6e66 5374 6174 653a  ") -> ConfState:
-00005920: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00005930: 2020 2020 2041 7070 6c69 6573 2061 2063       Applies a c
-00005940: 6f6e 6669 6720 6368 616e 6765 2074 6f20  onfig change to 
-00005950: 7468 6520 6c6f 6361 6c20 6e6f 6465 2e20  the local node. 
-00005960: 5468 6520 6170 7020 6d75 7374 2063 616c  The app must cal
-00005970: 6c20 7468 6973 2077 6865 6e20 6974 0a20  l this when it. 
-00005980: 2020 2020 2020 2061 7070 6c69 6573 2061         applies a
-00005990: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
-000059a0: 6861 6e67 652c 2065 7863 6570 7420 7768  hange, except wh
-000059b0: 656e 2069 7420 6465 6369 6465 7320 746f  en it decides to
-000059c0: 2072 656a 6563 7420 7468 650a 2020 2020   reject the.    
-000059d0: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
-000059e0: 6e20 6368 616e 6765 2c20 696e 2077 6869  n change, in whi
-000059f0: 6368 2063 6173 6520 6e6f 2063 616c 6c20  ch case no call 
-00005a00: 6d75 7374 2074 616b 6520 706c 6163 652e  must take place.
-00005a10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00005a20: 2064 6566 2061 7070 6c79 5f63 6f6e 665f   def apply_conf_
-00005a30: 6368 616e 6765 5f76 3228 0a20 2020 2020  change_v2(.     
-00005a40: 2020 2073 656c 662c 2063 633a 2022 436f     self, cc: "Co
-00005a50: 6e66 4368 616e 6765 5632 2220 7c20 2243  nfChangeV2" | "C
-00005a60: 6f6e 6643 6861 6e67 6556 3252 6566 220a  onfChangeV2Ref".
-00005a70: 2020 2020 2920 2d3e 2022 436f 6e66 5374      ) -> "ConfSt
-00005a80: 6174 6522 3a0a 2020 2020 2020 2020 2222  ate":.        ""
-00005a90: 220a 2020 2020 2020 2020 4170 706c 6965  ".        Applie
-00005aa0: 7320 6120 636f 6e66 6967 2063 6861 6e67  s a config chang
-00005ab0: 6520 746f 2074 6865 206c 6f63 616c 206e  e to the local n
-00005ac0: 6f64 652e 2054 6865 2061 7070 206d 7573  ode. The app mus
-00005ad0: 7420 6361 6c6c 2074 6869 7320 7768 656e  t call this when
-00005ae0: 2069 740a 2020 2020 2020 2020 6170 706c   it.        appl
-00005af0: 6965 7320 6120 636f 6e66 6967 7572 6174  ies a configurat
-00005b00: 696f 6e20 6368 616e 6765 2c20 6578 6365  ion change, exce
-00005b10: 7074 2077 6865 6e20 6974 2064 6563 6964  pt when it decid
-00005b20: 6573 2074 6f20 7265 6a65 6374 2074 6865  es to reject the
-00005b30: 0a20 2020 2020 2020 2063 6f6e 6669 6775  .        configu
-00005b40: 7261 7469 6f6e 2063 6861 6e67 652c 2069  ration change, i
-00005b50: 6e20 7768 6963 6820 6361 7365 206e 6f20  n which case no 
-00005b60: 6361 6c6c 206d 7573 7420 7461 6b65 2070  call must take p
-00005b70: 6c61 6365 2e0a 2020 2020 2020 2020 2222  lace..        ""
-00005b80: 220a 2020 2020 6465 6620 7069 6e67 2873  ".    def ping(s
-00005b90: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00005ba0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005bb0: 2020 4272 6f61 6463 6173 7420 6865 6172    Broadcast hear
-00005bc0: 7462 6561 7473 2074 6f20 616c 6c20 7468  tbeats to all th
-00005bd0: 6520 666f 6c6c 6f77 6572 732e 0a0a 2020  e followers...  
-00005be0: 2020 2020 2020 4966 2069 7427 7320 6e6f        If it's no
-00005bf0: 7420 6c65 6164 6572 2c20 6e6f 7468 696e  t leader, nothin
-00005c00: 6720 7769 6c6c 2068 6170 7065 6e2e 0a20  g will happen.. 
-00005c10: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00005c20: 6566 206f 6e5f 7065 7273 6973 745f 7265  ef on_persist_re
-00005c30: 6164 7928 7365 6c66 2c20 6e75 6d62 6572  ady(self, number
-00005c40: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00005c50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005c60: 2020 2020 4e6f 7469 6669 6573 2074 6861      Notifies tha
-00005c70: 7420 7468 6520 7265 6164 7920 6f66 2074  t the ready of t
-00005c80: 6869 7320 6e75 6d62 6572 2068 6173 2062  his number has b
-00005c90: 6565 6e20 7065 7273 6973 7465 642e 0a0a  een persisted...
-00005ca0: 2020 2020 2020 2020 5369 6e63 6520 5265          Since Re
-00005cb0: 6164 7920 6d75 7374 2062 6520 7065 7273  ady must be pers
-00005cc0: 6973 7465 6420 696e 206f 7264 6572 2c20  isted in order, 
-00005cd0: 6361 6c6c 696e 6720 7468 6973 2066 756e  calling this fun
-00005ce0: 6374 696f 6e20 696d 706c 6963 6974 6c79  ction implicitly
-00005cf0: 206d 6561 6e73 0a20 2020 2020 2020 2061   means.        a
-00005d00: 6c6c 2072 6561 6469 6573 2077 6974 6820  ll readies with 
-00005d10: 6e75 6d62 6572 7320 736d 616c 6c65 7220  numbers smaller 
-00005d20: 7468 616e 2074 6869 7320 6f6e 6520 6861  than this one ha
-00005d30: 7665 2062 6565 6e20 7065 7273 6973 7465  ve been persiste
-00005d40: 642e 0a0a 2020 2020 2020 2020 5b60 5365  d...        [`Se
-00005d50: 6c66 3a3a 6861 735f 7265 6164 7960 5d20  lf::has_ready`] 
-00005d60: 616e 6420 5b60 5365 6c66 3a3a 7265 6164  and [`Self::read
-00005d70: 7960 5d20 7368 6f75 6c64 2062 6520 6361  y`] should be ca
-00005d80: 6c6c 6564 206c 6174 6572 2074 6f20 6861  lled later to ha
-00005d90: 6e64 6c65 2066 7572 7468 6572 0a20 2020  ndle further.   
-00005da0: 2020 2020 2075 7064 6174 6573 2074 6861       updates tha
-00005db0: 7420 6265 636f 6d65 2076 616c 6964 2061  t become valid a
-00005dc0: 6674 6572 2072 6561 6479 2062 6569 6e67  fter ready being
-00005dd0: 2070 6572 7369 7374 6564 2e0a 2020 2020   persisted..    
-00005de0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00005df0: 7265 6164 5f69 6e64 6578 2873 656c 662c  read_index(self,
-00005e00: 2072 6374 783a 2062 7974 6573 2920 2d3e   rctx: bytes) ->
-00005e10: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00005e20: 2222 0a20 2020 2020 2020 2052 6561 6449  "".        ReadI
-00005e30: 6e64 6578 2072 6571 7565 7374 7320 6120  ndex requests a 
-00005e40: 7265 6164 2073 7461 7465 2e20 5468 6520  read state. The 
-00005e50: 7265 6164 2073 7461 7465 2077 696c 6c20  read state will 
-00005e60: 6265 2073 6574 2069 6e20 7265 6164 792e  be set in ready.
-00005e70: 0a20 2020 2020 2020 2052 6561 6420 5374  .        Read St
-00005e80: 6174 6520 6861 7320 6120 7265 6164 2069  ate has a read i
-00005e90: 6e64 6578 2e20 4f6e 6365 2074 6865 2061  ndex. Once the a
-00005ea0: 7070 6c69 6361 7469 6f6e 2061 6476 616e  pplication advan
-00005eb0: 6365 7320 6675 7274 6865 7220 7468 616e  ces further than
-00005ec0: 2074 6865 2072 6561 640a 2020 2020 2020   the read.      
-00005ed0: 2020 696e 6465 782c 2061 6e79 206c 696e    index, any lin
-00005ee0: 6561 7269 7a61 626c 6520 7265 6164 2072  earizable read r
-00005ef0: 6571 7565 7374 7320 6973 7375 6564 2062  equests issued b
-00005f00: 6566 6f72 6520 7468 6520 7265 6164 2072  efore the read r
-00005f10: 6571 7565 7374 2063 616e 2062 650a 2020  equest can be.  
-00005f20: 2020 2020 2020 7072 6f63 6573 7365 6420        processed 
-00005f30: 7361 6665 6c79 2e20 5468 6520 7265 6164  safely. The read
-00005f40: 2073 7461 7465 2077 696c 6c20 6861 7665   state will have
-00005f50: 2074 6865 2073 616d 6520 7263 7478 2061   the same rctx a
-00005f60: 7474 6163 6865 642e 0a20 2020 2020 2020  ttached..       
-00005f70: 2022 2222 0a20 2020 2064 6566 2072 6561   """.    def rea
-00005f80: 6479 2873 656c 6629 202d 3e20 5265 6164  dy(self) -> Read
-00005f90: 793a 0a20 2020 2020 2020 2022 2222 0a20  y:.        """. 
-00005fa0: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
-00005fb0: 6865 206f 7574 7374 616e 6469 6e67 2077  he outstanding w
-00005fc0: 6f72 6b20 7468 6174 2074 6865 2061 7070  ork that the app
-00005fd0: 6c69 6361 7469 6f6e 206e 6565 6473 2074  lication needs t
-00005fe0: 6f20 6861 6e64 6c65 2e0a 0a20 2020 2020  o handle...     
-00005ff0: 2020 2054 6869 7320 696e 636c 7564 6573     This includes
-00006000: 2061 7070 656e 6469 6e67 2061 6e64 2061   appending and a
-00006010: 7070 6c79 696e 6720 656e 7472 6965 7320  pplying entries 
-00006020: 6f72 2061 2073 6e61 7073 686f 742c 2075  or a snapshot, u
-00006030: 7064 6174 696e 6720 7468 6520 4861 7264  pdating the Hard
-00006040: 5374 6174 652c 0a20 2020 2020 2020 2061  State,.        a
-00006050: 6e64 2073 656e 6469 6e67 206d 6573 7361  nd sending messa
-00006060: 6765 732e 2054 6865 2072 6574 7572 6e65  ges. The returne
-00006070: 6420 6052 6561 6479 6020 2a4d 5553 542a  d `Ready` *MUST*
-00006080: 2062 6520 6861 6e64 6c65 6420 616e 6420   be handled and 
-00006090: 7375 6273 6571 7565 6e74 6c79 0a20 2020  subsequently.   
-000060a0: 2020 2020 2070 6173 7365 6420 6261 636b       passed back
-000060b0: 2076 6961 2060 6164 7661 6e63 6560 206f   via `advance` o
-000060c0: 7220 6974 7320 6661 6d69 6c69 6573 2e20  r its families. 
-000060d0: 4265 666f 7265 2074 6861 742c 202a 444f  Before that, *DO
-000060e0: 204e 4f54 2a20 6361 6c6c 2061 6e79 2066   NOT* call any f
-000060f0: 756e 6374 696f 6e20 6c69 6b65 0a20 2020  unction like.   
-00006100: 2020 2020 2060 7374 6570 602c 2060 7072       `step`, `pr
-00006110: 6f70 6f73 6560 2c20 6063 616d 7061 6967  opose`, `campaig
-00006120: 6e60 2074 6f20 6368 616e 6765 2069 6e74  n` to change int
-00006130: 6572 6e61 6c20 7374 6174 652e 0a0a 2020  ernal state...  
-00006140: 2020 2020 2020 5b60 5365 6c66 3a3a 6861        [`Self::ha
-00006150: 735f 7265 6164 7960 5d20 7368 6f75 6c64  s_ready`] should
-00006160: 2062 6520 6361 6c6c 6564 2066 6972 7374   be called first
-00006170: 2074 6f20 6368 6563 6b20 6966 2069 7427   to check if it'
-00006180: 7320 6e65 6365 7373 6172 7920 746f 2068  s necessary to h
-00006190: 616e 646c 6520 7468 6520 7265 6164 792e  andle the ready.
-000061a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000061b0: 2064 6566 2072 6571 7565 7374 5f73 6e61   def request_sna
-000061c0: 7073 686f 7428 7365 6c66 2920 2d3e 2022  pshot(self) -> "
-000061d0: 5265 6164 7922 3a0a 2020 2020 2020 2020  Ready":.        
-000061e0: 2222 220a 2020 2020 2020 2020 5265 7175  """.        Requ
-000061f0: 6573 7420 6120 736e 6170 7368 6f74 2066  est a snapshot f
-00006200: 726f 6d20 6120 6c65 6164 6572 2e0a 2020  rom a leader..  
-00006210: 2020 2020 2020 5468 6520 736e 6170 7368        The snapsh
-00006220: 6f74 2773 2069 6e64 6578 206d 7573 7420  ot's index must 
-00006230: 6265 2067 7265 6174 6572 206f 7220 6571  be greater or eq
-00006240: 7561 6c20 746f 2074 6865 2072 6571 7565  ual to the reque
-00006250: 7374 5f69 6e64 6578 2028 6c61 7374 5f69  st_index (last_i
-00006260: 6e64 6578 2920 6f72 0a20 2020 2020 2020  ndex) or.       
-00006270: 2074 6865 206c 6561 6465 7227 7320 7465   the leader's te
-00006280: 726d 206d 7573 7420 6265 2067 7265 6174  rm must be great
-00006290: 6572 2074 6861 6e20 7468 6520 7265 7175  er than the requ
-000062a0: 6573 7420 7465 726d 2028 6c61 7374 5f69  est term (last_i
-000062b0: 6e64 6578 2773 2074 6572 6d29 2e0a 2020  ndex's term)..  
-000062c0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000062d0: 6620 6f6e 5f65 6e74 7269 6573 5f66 6574  f on_entries_fet
-000062e0: 6368 6564 2873 656c 6629 202d 3e20 4e6f  ched(self) -> No
-000062f0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00006300: 2020 2020 2020 2020 4120 6361 6c6c 6261          A callba
-00006310: 636b 2077 6865 6e20 656e 7472 6965 7320  ck when entries 
-00006320: 6172 6520 6665 7463 6865 6420 6173 796e  are fetched asyn
-00006330: 6368 726f 6e6f 7573 6c79 2e0a 2020 2020  chronously..    
-00006340: 2020 2020 5468 6520 636f 6e74 6578 7420      The context 
-00006350: 7368 6f75 6c64 2070 726f 7669 6465 2074  should provide t
-00006360: 6865 2063 6f6e 7465 7874 2070 6173 7365  he context passe
-00006370: 6420 6672 6f6d 2053 746f 7261 6765 2e65  d from Storage.e
-00006380: 6e74 6972 6573 2829 2e0a 2020 2020 2020  ntires()..      
-00006390: 2020 5365 6520 6d6f 7265 2069 6e20 7468    See more in th
-000063a0: 6520 636f 6d6d 656e 7420 6f66 2053 746f  e comment of Sto
-000063b0: 7261 6765 2e65 6e74 6972 6573 2829 2e0a  rage.entires()..
-000063c0: 0a20 2020 2020 2020 2023 2050 616e 6963  .        # Panic
-000063d0: 730a 0a20 2020 2020 2020 2050 616e 6963  s..        Panic
-000063e0: 7320 6966 2070 6173 7365 6420 7769 7468  s if passed with
-000063f0: 2074 6865 2063 6f6e 7465 7874 206f 6620   the context of 
-00006400: 636f 6e74 6578 742e 6361 6e5f 6173 796e  context.can_asyn
-00006410: 6328 2920 3d3d 2066 616c 7365 0a20 2020  c() == false.   
-00006420: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-00006430: 496e 4d65 6d6f 7279 5261 774e 6f64 6528  InMemoryRawNode(
-00006440: 5f5f 4150 495f 5261 774e 6f64 6529 3a0a  __API_RawNode):.
-00006450: 2020 2020 2222 220a 2020 2020 5261 774e      """.    RawN
-00006460: 6f64 6520 6973 2061 2074 6872 6561 642d  ode is a thread-
-00006470: 756e 7361 6665 204e 6f64 652e 0a20 2020  unsafe Node..   
-00006480: 2054 6865 206d 6574 686f 6473 206f 6620   The methods of 
-00006490: 7468 6973 2073 7472 7563 7420 636f 7272  this struct corr
-000064a0: 6573 706f 6e64 2074 6f20 7468 6520 6d65  espond to the me
-000064b0: 7468 6f64 7320 6f66 204e 6f64 6520 616e  thods of Node an
-000064c0: 6420 6172 6520 6465 7363 7269 6265 640a  d are described.
-000064d0: 2020 2020 6d6f 7265 2066 756c 6c79 2074      more fully t
-000064e0: 6865 7265 2e0a 2020 2020 2222 220a 0a20  here..    """.. 
-000064f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00006500: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00006510: 2020 2020 2020 2063 6667 3a20 2243 6f6e         cfg: "Con
-00006520: 6669 6722 207c 2022 436f 6e66 6967 5265  fig" | "ConfigRe
-00006530: 6622 2c0a 2020 2020 2020 2020 7374 6f72  f",.        stor
-00006540: 653a 2022 4d65 6d53 746f 7261 6765 2220  e: "MemStorage" 
-00006550: 7c20 224d 656d 5374 6f72 6167 6552 6566  | "MemStorageRef
-00006560: 222c 0a20 2020 2020 2020 206c 6f67 6765  ",.        logge
-00006570: 723a 2022 4c6f 6767 6572 2220 7c20 224c  r: "Logger" | "L
-00006580: 6f67 6765 7252 6566 222c 0a20 2020 2029  oggerRef",.    )
-00006590: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-000065a0: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
-000065b0: 656c 6629 202d 3e20 2249 6e4d 656d 6f72  elf) -> "InMemor
-000065c0: 7952 6177 4e6f 6465 5265 6622 3a20 2e2e  yRawNodeRef": ..
-000065d0: 2e0a 2020 2020 6465 6620 6765 745f 7261  ..    def get_ra
-000065e0: 6674 2873 656c 6629 202d 3e20 2249 6e4d  ft(self) -> "InM
-000065f0: 656d 6f72 7952 6166 7452 6566 223a 0a20  emoryRaftRef":. 
-00006600: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00006610: 2020 2064 6566 2073 746f 7265 2873 656c     def store(sel
-00006620: 6629 202d 3e20 224d 656d 5374 6f72 6167  f) -> "MemStorag
-00006630: 6552 6566 223a 0a20 2020 2020 2020 2022  eRef":.        "
-00006640: 2222 5265 7475 726e 7320 7468 6520 7374  ""Returns the st
-00006650: 6f72 6520 6173 2061 206d 7574 6162 6c65  ore as a mutable
-00006660: 2072 6566 6572 656e 6365 2e22 2222 0a0a   reference."""..
-00006670: 636c 6173 7320 496e 4d65 6d6f 7279 5261  class InMemoryRa
-00006680: 774e 6f64 6552 6566 285f 5f41 5049 5f52  wNodeRef(__API_R
-00006690: 6177 4e6f 6465 293a 0a20 2020 2022 2222  awNode):.    """
-000066a0: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
-000066b0: 7970 6520 6f66 203a 636c 6173 733a 6049  ype of :class:`I
-000066c0: 6e4d 656d 6f72 7952 6177 4e6f 6465 602e  nMemoryRawNode`.
-000066d0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-000066e0: 6620 6765 745f 7261 6674 2873 656c 6629  f get_raft(self)
-000066f0: 202d 3e20 2249 6e4d 656d 6f72 7952 6166   -> "InMemoryRaf
-00006700: 7452 6566 223a 0a20 2020 2020 2020 2022  tRef":.        "
-00006710: 2222 2022 2222 0a20 2020 2064 6566 2073  "" """.    def s
-00006720: 746f 7265 2873 656c 6629 202d 3e20 224d  tore(self) -> "M
-00006730: 656d 5374 6f72 6167 6552 6566 223a 0a20  emStorageRef":. 
-00006740: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00006750: 7320 7468 6520 7374 6f72 6520 6173 2061  s the store as a
-00006760: 206d 7574 6162 6c65 2072 6566 6572 656e   mutable referen
-00006770: 6365 2e22 2222 0a20 2020 2023 2064 6566  ce.""".    # def
-00006780: 2073 7461 7475 7328 7365 6c66 2920 2d3e   status(self) ->
-00006790: 2049 6e4d 656d 6f72 7953 7461 7475 733a   InMemoryStatus:
-000067a0: 0a20 2020 2023 2020 2020 2022 2222 0a20  .    #     """. 
-000067b0: 2020 2023 2020 2020 2053 7461 7475 7320     #     Status 
-000067c0: 7265 7475 726e 7320 7468 6520 6375 7272  returns the curr
-000067d0: 656e 7420 7374 6174 7573 206f 6620 7468  ent status of th
-000067e0: 6520 6769 7665 6e20 6772 6f75 702e 0a20  e given group.. 
-000067f0: 2020 2023 2020 2020 2022 2222 0a0a 636c     #     """..cl
-00006800: 6173 7320 5261 774e 6f64 6528 5f5f 4150  ass RawNode(__AP
-00006810: 495f 5261 774e 6f64 6529 3a0a 2020 2020  I_RawNode):.    
-00006820: 2222 220a 2020 2020 5261 774e 6f64 6520  """.    RawNode 
-00006830: 6973 2061 2074 6872 6561 642d 756e 7361  is a thread-unsa
-00006840: 6665 204e 6f64 652e 0a20 2020 2054 6865  fe Node..    The
-00006850: 206d 6574 686f 6473 206f 6620 7468 6973   methods of this
-00006860: 2073 7472 7563 7420 636f 7272 6573 706f   struct correspo
-00006870: 6e64 2074 6f20 7468 6520 6d65 7468 6f64  nd to the method
-00006880: 7320 6f66 204e 6f64 6520 616e 6420 6172  s of Node and ar
-00006890: 6520 6465 7363 7269 6265 640a 2020 2020  e described.    
-000068a0: 6d6f 7265 2066 756c 6c79 2074 6865 7265  more fully there
-000068b0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-000068c0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000068d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000068e0: 2020 2063 6667 3a20 2243 6f6e 6669 6722     cfg: "Config"
-000068f0: 207c 2022 436f 6e66 6967 5265 6622 2c0a   | "ConfigRef",.
-00006900: 2020 2020 2020 2020 7374 6f72 653a 2022          store: "
-00006910: 5374 6f72 6167 6522 207c 2022 5374 6f72  Storage" | "Stor
-00006920: 6167 6552 6566 222c 0a20 2020 2020 2020  ageRef",.       
-00006930: 206c 6f67 6765 723a 2022 4c6f 6767 6572   logger: "Logger
-00006940: 2220 7c20 224c 6f67 6765 7252 6566 222c  " | "LoggerRef",
-00006950: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
-00006960: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
-00006970: 5f72 6566 2873 656c 6629 202d 3e20 2252  _ref(self) -> "R
-00006980: 6177 4e6f 6465 5265 6622 3a20 2e2e 2e0a  awNodeRef": ....
-00006990: 2020 2020 6465 6620 6765 745f 7261 6674      def get_raft
-000069a0: 2873 656c 6629 202d 3e20 2252 6166 7452  (self) -> "RaftR
-000069b0: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-000069c0: 2022 2222 0a20 2020 2064 6566 2073 746f   """.    def sto
-000069d0: 7265 2873 656c 6629 202d 3e20 2253 746f  re(self) -> "Sto
-000069e0: 7261 6765 5265 6622 3a0a 2020 2020 2020  rageRef":.      
-000069f0: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
-00006a00: 2073 746f 7265 2061 7320 6120 6d75 7461   store as a muta
-00006a10: 626c 6520 7265 6665 7265 6e63 652e 2222  ble reference.""
-00006a20: 220a 2020 2020 2320 6465 6620 7374 6174  ".    # def stat
-00006a30: 7573 2873 656c 6629 202d 3e20 5374 6174  us(self) -> Stat
-00006a40: 7573 3a0a 2020 2020 2320 2020 2020 2222  us:.    #     ""
-00006a50: 220a 2020 2020 2320 2020 2020 5374 6174  ".    #     Stat
-00006a60: 7573 2072 6574 7572 6e73 2074 6865 2063  us returns the c
-00006a70: 7572 7265 6e74 2073 7461 7475 7320 6f66  urrent status of
-00006a80: 2074 6865 2067 6976 656e 2067 726f 7570   the given group
-00006a90: 2e0a 2020 2020 2320 2020 2020 2222 220a  ..    #     """.
-00006aa0: 0a63 6c61 7373 2052 6177 4e6f 6465 5265  .class RawNodeRe
-00006ab0: 6628 5f5f 4150 495f 5261 774e 6f64 6529  f(__API_RawNode)
-00006ac0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00006ad0: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
-00006ae0: 3a63 6c61 7373 3a60 5261 774e 6f64 6560  :class:`RawNode`
-00006af0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00006b00: 6566 2067 6574 5f72 6166 7428 7365 6c66  ef get_raft(self
-00006b10: 2920 2d3e 2022 5261 6674 5265 6622 3a0a  ) -> "RaftRef":.
-00006b20: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00006b30: 2020 2020 6465 6620 7374 6f72 6528 7365      def store(se
-00006b40: 6c66 2920 2d3e 2022 5374 6f72 6167 6552  lf) -> "StorageR
-00006b50: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-00006b60: 5265 7475 726e 7320 7468 6520 7374 6f72  Returns the stor
-00006b70: 6520 6173 2061 206d 7574 6162 6c65 2072  e as a mutable r
-00006b80: 6566 6572 656e 6365 2e22 2222 0a20 2020  eference.""".   
-00006b90: 2023 2064 6566 2073 7461 7475 7328 7365   # def status(se
-00006ba0: 6c66 2920 2d3e 2049 6e4d 656d 6f72 7953  lf) -> InMemoryS
-00006bb0: 7461 7475 733a 0a20 2020 2023 2020 2020  tatus:.    #    
-00006bc0: 2022 2222 0a20 2020 2023 2020 2020 2053   """.    #     S
-00006bd0: 7461 7475 7320 7265 7475 726e 7320 7468  tatus returns th
-00006be0: 6520 6375 7272 656e 7420 7374 6174 7573  e current status
-00006bf0: 206f 6620 7468 6520 6769 7665 6e20 6772   of the given gr
-00006c00: 6f75 702e 0a20 2020 2023 2020 2020 2022  oup..    #     "
-00006c10: 2222 0a0a 636c 6173 7320 5f5f 4150 495f  ""..class __API_
-00006c20: 5065 6572 3a0a 2020 2020 6465 6620 6765  Peer:.    def ge
-00006c30: 745f 6964 2873 656c 6629 202d 3e20 696e  t_id(self) -> in
-00006c40: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-00006c50: 2020 2020 2020 2060 6964 603a 2054 6865         `id`: The
-00006c60: 2049 4420 6f66 2074 6865 2070 6565 722e   ID of the peer.
-00006c70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006c80: 2064 6566 2073 6574 5f69 6428 7365 6c66   def set_id(self
-00006c90: 2c20 6964 3a20 696e 7429 202d 3e20 4e6f  , id: int) -> No
-00006ca0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00006cb0: 2020 2020 2020 2020 6069 6460 3a20 5468          `id`: Th
-00006cc0: 6520 4944 206f 6620 7468 6520 7065 6572  e ID of the peer
-00006cd0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00006ce0: 2020 6465 6620 6765 745f 636f 6e74 6578    def get_contex
-00006cf0: 7428 7365 6c66 2920 2d3e 2062 7974 6573  t(self) -> bytes
-00006d00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00006d10: 2020 2020 2020 6063 6f6e 7465 7874 603a        `context`:
-00006d20: 2049 6620 7468 6572 6520 6973 2063 6f6e   If there is con
-00006d30: 7465 7874 2061 7373 6f63 6961 7465 6420  text associated 
-00006d40: 7769 7468 2074 6865 2070 6565 7220 286c  with the peer (l
-00006d50: 696b 6520 636f 6e6e 6563 7469 6f6e 2069  ike connection i
-00006d60: 6e66 6f72 6d61 7469 6f6e 292c 2069 7420  nformation), it 
-00006d70: 6361 6e20 6265 0a20 2020 2020 2020 2073  can be.        s
-00006d80: 6572 6961 6c69 7a65 6420 616e 6420 7374  erialized and st
-00006d90: 6f72 6564 2068 6572 652e 0a20 2020 2020  ored here..     
-00006da0: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
-00006db0: 6574 5f63 6f6e 7465 7874 2873 656c 662c  et_context(self,
-00006dc0: 2063 6f6e 7465 7874 3a20 6279 7465 7329   context: bytes)
-00006dd0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00006de0: 2020 2222 220a 2020 2020 2020 2020 6063    """.        `c
-00006df0: 6f6e 7465 7874 603a 2049 6620 7468 6572  ontext`: If ther
-00006e00: 6520 6973 2063 6f6e 7465 7874 2061 7373  e is context ass
-00006e10: 6f63 6961 7465 6420 7769 7468 2074 6865  ociated with the
-00006e20: 2070 6565 7220 286c 696b 6520 636f 6e6e   peer (like conn
-00006e30: 6563 7469 6f6e 2069 6e66 6f72 6d61 7469  ection informati
-00006e40: 6f6e 292c 2069 7420 6361 6e20 6265 0a20  on), it can be. 
-00006e50: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
-00006e60: 6420 616e 6420 7374 6f72 6564 2068 6572  d and stored her
-00006e70: 652e 0a20 2020 2020 2020 2022 2222 0a0a  e..        """..
-00006e80: 636c 6173 7320 5065 6572 285f 5f41 5049  class Peer(__API
-00006e90: 5f50 6565 7229 3a0a 2020 2020 2222 220a  _Peer):.    """.
-00006ea0: 2020 2020 5265 7072 6573 656e 7473 2061      Represents a
-00006eb0: 2050 6565 7220 6e6f 6465 2069 6e20 7468   Peer node in th
-00006ec0: 6520 636c 7573 7465 722e 0a20 2020 2022  e cluster..    "
-00006ed0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-00006ee0: 6974 5f5f 2873 656c 6629 202d 3e20 4e6f  it__(self) -> No
-00006ef0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00006f00: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-00006f10: 3e20 2250 6565 7252 6566 223a 202e 2e2e  > "PeerRef": ...
-00006f20: 0a0a 636c 6173 7320 5065 6572 5265 6628  ..class PeerRef(
-00006f30: 5f5f 4150 495f 5065 6572 293a 0a20 2020  __API_Peer):.   
-00006f40: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
-00006f50: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
-00006f60: 733a 6050 6565 7260 2e0a 2020 2020 2222  s:`Peer`..    ""
-00006f70: 220a 0a63 6c61 7373 205f 5f41 5049 5f4c  "..class __API_L
-00006f80: 6967 6874 5265 6164 793a 0a20 2020 2064  ightReady:.    d
-00006f90: 6566 2063 6f6d 6d69 745f 696e 6465 7828  ef commit_index(
-00006fa0: 7365 6c66 2920 2d3e 204f 7074 696f 6e61  self) -> Optiona
-00006fb0: 6c5b 696e 745d 3a0a 2020 2020 2020 2020  l[int]:.        
-00006fc0: 2222 220a 2020 2020 2020 2020 5468 6520  """.        The 
-00006fd0: 6375 7272 656e 7420 636f 6d6d 6974 2069  current commit i
-00006fe0: 6e64 6578 2e0a 2020 2020 2020 2020 4974  ndex..        It
-00006ff0: 2077 696c 6c20 6265 204e 6f6e 6520 7374   will be None st
-00007000: 6174 6520 6966 2074 6865 7265 2069 7320  ate if there is 
-00007010: 6e6f 2075 7064 6174 652e 0a20 2020 2020  no update..     
-00007020: 2020 2049 7420 6973 206e 6f74 2072 6571     It is not req
-00007030: 7569 7265 6420 746f 2073 6176 6520 6974  uired to save it
-00007040: 2074 6f20 7374 6162 6c65 2073 746f 7261   to stable stora
-00007050: 6765 2e0a 2020 2020 2020 2020 2222 220a  ge..        """.
-00007060: 2020 2020 6465 6620 636f 6d6d 6974 7465      def committe
-00007070: 645f 656e 7472 6965 7328 7365 6c66 2920  d_entries(self) 
-00007080: 2d3e 204c 6973 745b 2245 6e74 7279 5265  -> List["EntryRe
-00007090: 6622 5d3a 0a20 2020 2020 2020 2022 2222  f"]:.        """
-000070a0: 0a20 2020 2020 2020 2043 6f6d 6d69 7474  .        Committ
-000070b0: 6564 456e 7472 6965 7320 7370 6563 6966  edEntries specif
-000070c0: 6965 7320 656e 7472 6965 7320 746f 2062  ies entries to b
-000070d0: 6520 636f 6d6d 6974 7465 6420 746f 2061  e committed to a
-000070e0: 0a20 2020 2020 2020 2073 746f 7265 2f73  .        store/s
-000070f0: 7461 7465 2d6d 6163 6869 6e65 2e20 5468  tate-machine. Th
-00007100: 6573 6520 6861 7665 2070 7265 7669 6f75  ese have previou
-00007110: 736c 7920 6265 656e 2063 6f6d 6d69 7474  sly been committ
-00007120: 6564 2074 6f20 7374 6162 6c65 0a20 2020  ed to stable.   
-00007130: 2020 2020 2073 746f 7265 2e0a 2020 2020       store..    
-00007140: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00007150: 7461 6b65 5f63 6f6d 6d69 7474 6564 5f65  take_committed_e
-00007160: 6e74 7269 6573 2873 656c 6629 202d 3e20  ntries(self) -> 
-00007170: 4c69 7374 5b22 456e 7472 7922 5d3a 0a20  List["Entry"]:. 
-00007180: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007190: 2020 2054 616b 6520 7468 6520 436f 6d6d     Take the Comm
-000071a0: 6974 456e 7472 6965 732e 0a20 2020 2020  itEntries..     
-000071b0: 2020 2022 2222 0a20 2020 2064 6566 206d     """.    def m
-000071c0: 6573 7361 6765 7328 7365 6c66 2920 2d3e  essages(self) ->
-000071d0: 204c 6973 745b 224d 6573 7361 6765 5265   List["MessageRe
-000071e0: 6622 5d3a 0a20 2020 2020 2020 2022 2222  f"]:.        """
-000071f0: 0a20 2020 2020 2020 204d 6573 7361 6765  .        Message
-00007200: 7320 7370 6563 6966 6965 7320 6f75 7462  s specifies outb
-00007210: 6f75 6e64 206d 6573 7361 6765 7320 746f  ound messages to
-00007220: 2062 6520 7365 6e74 2e0a 2020 2020 2020   be sent..      
-00007230: 2020 2222 220a 2020 2020 6465 6620 7461    """.    def ta
-00007240: 6b65 5f6d 6573 7361 6765 7328 7365 6c66  ke_messages(self
-00007250: 2920 2d3e 204c 6973 745b 224d 6573 7361  ) -> List["Messa
-00007260: 6765 225d 3a0a 2020 2020 2020 2020 2222  ge"]:.        ""
-00007270: 220a 2020 2020 2020 2020 5461 6b65 2074  ".        Take t
-00007280: 6865 204d 6573 7361 6765 732e 0a20 2020  he Messages..   
-00007290: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
-000072a0: 4c69 6768 7452 6561 6479 285f 5f41 5049  LightReady(__API
-000072b0: 5f4c 6967 6874 5265 6164 7929 3a0a 2020  _LightReady):.  
-000072c0: 2020 2222 220a 2020 2020 4c69 6768 7452    """.    LightR
-000072d0: 6561 6479 2065 6e63 6170 7375 6c61 7465  eady encapsulate
-000072e0: 7320 7468 6520 636f 6d6d 6974 2069 6e64  s the commit ind
-000072f0: 6578 2c20 636f 6d6d 6974 7465 6420 656e  ex, committed en
-00007300: 7472 6965 7320 616e 640a 2020 2020 6d65  tries and.    me
-00007310: 7373 6167 6573 2074 6861 7420 6172 6520  ssages that are 
-00007320: 7265 6164 7920 746f 2062 6520 6170 706c  ready to be appl
-00007330: 6965 6420 6f72 2062 6520 7365 6e74 2074  ied or be sent t
-00007340: 6f20 6f74 6865 7220 7065 6572 732e 0a20  o other peers.. 
-00007350: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
-00007360: 5f5f 696e 6974 5f5f 2873 656c 6629 202d  __init__(self) -
-00007370: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00007380: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
-00007390: 6629 202d 3e20 224c 6967 6874 5265 6164  f) -> "LightRead
-000073a0: 7952 6566 223a 202e 2e2e 0a20 2020 2040  yRef": ....    @
-000073b0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-000073c0: 2064 6566 2064 6566 6175 6c74 2829 202d   def default() -
-000073d0: 3e20 224c 6967 6874 5265 6164 7922 3a20  > "LightReady": 
-000073e0: 2e2e 2e0a 0a63 6c61 7373 204c 6967 6874  .....class Light
-000073f0: 5265 6164 7952 6566 285f 5f41 5049 5f4c  ReadyRef(__API_L
-00007400: 6967 6874 5265 6164 7929 3a0a 2020 2020  ightReady):.    
-00007410: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
-00007420: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
-00007430: 3a60 4c69 6768 7452 6561 6479 602e 0a20  :`LightReady`.. 
-00007440: 2020 2022 2222 0a0a 636c 6173 7320 5f5f     """..class __
-00007450: 4150 495f 536e 6170 7368 6f74 4d65 7461  API_SnapshotMeta
-00007460: 6461 7461 285f 5f43 6c6f 6e65 6162 6c65  data(__Cloneable
-00007470: 2c20 5f5f 456e 636f 6465 722c 205f 5f44  , __Encoder, __D
-00007480: 6563 6f64 6572 293a 0a20 2020 2064 6566  ecoder):.    def
-00007490: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
-000074a0: 2253 6e61 7073 686f 744d 6574 6164 6174  "SnapshotMetadat
-000074b0: 6122 3a20 2e2e 2e0a 2020 2020 6465 6620  a": ....    def 
-000074c0: 6765 745f 696e 6465 7828 7365 6c66 2920  get_index(self) 
-000074d0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-000074e0: 2222 220a 2020 2020 2020 2020 6069 6e64  """.        `ind
-000074f0: 6578 603a 2054 6865 2061 7070 6c69 6564  ex`: The applied
-00007500: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
-00007510: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00007520: 696e 6465 7828 7365 6c66 2c20 696e 6465  index(self, inde
-00007530: 783a 2069 6e74 2920 2d3e 204e 6f6e 653a  x: int) -> None:
-00007540: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007550: 2020 2020 2060 696e 6465 7860 3a20 5468       `index`: Th
-00007560: 6520 6170 706c 6965 6420 696e 6465 782e  e applied index.
-00007570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007580: 2064 6566 2063 6c65 6172 5f69 6e64 6578   def clear_index
-00007590: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000075a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000075b0: 2020 2020 6069 6e64 6578 603a 2054 6865      `index`: The
-000075c0: 2061 7070 6c69 6564 2069 6e64 6578 2e0a   applied index..
-000075d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000075e0: 6465 6620 6765 745f 7465 726d 2873 656c  def get_term(sel
-000075f0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00007600: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00007610: 7465 726d 603a 2054 6865 2074 6572 6d20  term`: The term 
-00007620: 6f66 2074 6865 2061 7070 6c69 6564 2069  of the applied i
-00007630: 6e64 6578 2e0a 2020 2020 2020 2020 2222  ndex..        ""
-00007640: 220a 2020 2020 6465 6620 7365 745f 7465  ".    def set_te
-00007650: 726d 2873 656c 662c 2074 6572 6d3a 2069  rm(self, term: i
-00007660: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00007670: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007680: 2060 7465 726d 603a 2054 6865 2074 6572   `term`: The ter
-00007690: 6d20 6f66 2074 6865 2061 7070 6c69 6564  m of the applied
-000076a0: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
-000076b0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-000076c0: 725f 7465 726d 2873 656c 6629 202d 3e20  r_term(self) -> 
-000076d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000076e0: 220a 2020 2020 2020 2020 6074 6572 6d60  ".        `term`
-000076f0: 3a20 5468 6520 7465 726d 206f 6620 7468  : The term of th
-00007700: 6520 6170 706c 6965 6420 696e 6465 782e  e applied index.
-00007710: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007720: 2064 6566 2067 6574 5f63 6f6e 665f 7374   def get_conf_st
-00007730: 6174 6528 7365 6c66 2920 2d3e 2022 436f  ate(self) -> "Co
-00007740: 6e66 5374 6174 6552 6566 223a 0a20 2020  nfStateRef":.   
-00007750: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007760: 2060 636f 6e66 5f73 7461 7465 603a 2054   `conf_state`: T
-00007770: 6865 2063 7572 7265 6e74 2060 436f 6e66  he current `Conf
-00007780: 5374 6174 6560 2e0a 2020 2020 2020 2020  State`..        
-00007790: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-000077a0: 636f 6e66 5f73 7461 7465 2873 656c 662c  conf_state(self,
-000077b0: 2063 6f6e 665f 7374 6174 653a 2022 436f   conf_state: "Co
-000077c0: 6e66 5374 6174 6522 207c 2022 436f 6e66  nfState" | "Conf
-000077d0: 5374 6174 6552 6566 2229 202d 3e20 4e6f  StateRef") -> No
-000077e0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-000077f0: 2020 2020 2020 2020 6063 6f6e 665f 7374          `conf_st
-00007800: 6174 6560 3a20 5468 6520 6375 7272 656e  ate`: The curren
-00007810: 7420 6043 6f6e 6653 7461 7465 602e 0a20  t `ConfState`.. 
-00007820: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00007830: 6566 2063 6c65 6172 5f63 6f6e 665f 7374  ef clear_conf_st
-00007840: 6174 6528 7365 6c66 2920 2d3e 204e 6f6e  ate(self) -> Non
-00007850: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00007860: 2020 2020 2020 2060 636f 6e66 5f73 7461         `conf_sta
-00007870: 7465 603a 2054 6865 2063 7572 7265 6e74  te`: The current
-00007880: 2060 436f 6e66 5374 6174 6560 2e0a 2020   `ConfState`..  
-00007890: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000078a0: 6620 6861 735f 636f 6e66 5f73 7461 7465  f has_conf_state
-000078b0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
-000078c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000078d0: 2020 2020 6063 6f6e 665f 7374 6174 6560      `conf_state`
-000078e0: 3a20 5468 6520 6375 7272 656e 7420 6043  : The current `C
-000078f0: 6f6e 6653 7461 7465 602e 0a20 2020 2020  onfState`..     
-00007900: 2020 2022 2222 0a0a 636c 6173 7320 536e     """..class Sn
-00007910: 6170 7368 6f74 4d65 7461 6461 7461 285f  apshotMetadata(_
-00007920: 5f41 5049 5f53 6e61 7073 686f 744d 6574  _API_SnapshotMet
-00007930: 6164 6174 6129 3a0a 2020 2020 2222 2220  adata):.    """ 
-00007940: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-00007950: 6e69 745f 5f28 7365 6c66 2920 2d3e 204e  nit__(self) -> N
-00007960: 6f6e 653a 202e 2e2e 0a20 2020 2040 7374  one: ....    @st
-00007970: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00007980: 6566 2064 6566 6175 6c74 2829 202d 3e20  ef default() -> 
-00007990: 2253 6e61 7073 686f 744d 6574 6164 6174  "SnapshotMetadat
-000079a0: 6122 3a20 2e2e 2e0a 2020 2020 4073 7461  a": ....    @sta
-000079b0: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-000079c0: 6620 6465 636f 6465 2876 3a20 6279 7465  f decode(v: byte
-000079d0: 7329 202d 3e20 2253 6e61 7073 686f 744d  s) -> "SnapshotM
-000079e0: 6574 6164 6174 6122 3a20 2e2e 2e0a 2020  etadata": ....  
-000079f0: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
-00007a00: 656c 6629 202d 3e20 2253 6e61 7073 686f  elf) -> "Snapsho
-00007a10: 744d 6574 6164 6174 6152 6566 223a 202e  tMetadataRef": .
-00007a20: 2e2e 0a0a 636c 6173 7320 536e 6170 7368  ....class Snapsh
-00007a30: 6f74 4d65 7461 6461 7461 5265 6628 5f5f  otMetadataRef(__
-00007a40: 4150 495f 536e 6170 7368 6f74 4d65 7461  API_SnapshotMeta
-00007a50: 6461 7461 293a 0a20 2020 2022 2222 0a20  data):.    """. 
-00007a60: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
-00007a70: 6520 6f66 203a 636c 6173 733a 6053 6e61  e of :class:`Sna
-00007a80: 7073 686f 744d 6574 6164 6174 6160 2e0a  pshotMetadata`..
-00007a90: 2020 2020 2222 220a 0a63 6c61 7373 205f      """..class _
-00007aa0: 5f41 5049 5f53 6e61 7073 686f 7428 5f5f  _API_Snapshot(__
-00007ab0: 436c 6f6e 6561 626c 652c 205f 5f45 6e63  Cloneable, __Enc
-00007ac0: 6f64 6572 2c20 5f5f 4465 636f 6465 7229  oder, __Decoder)
-00007ad0: 3a0a 2020 2020 6465 6620 636c 6f6e 6528  :.    def clone(
-00007ae0: 7365 6c66 2920 2d3e 2022 536e 6170 7368  self) -> "Snapsh
-00007af0: 6f74 223a 202e 2e2e 0a20 2020 2064 6566  ot": ....    def
-00007b00: 2067 6574 5f64 6174 6128 7365 6c66 2920   get_data(self) 
-00007b10: 2d3e 2062 7974 6573 3a0a 2020 2020 2020  -> bytes:.      
-00007b20: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00007b30: 6620 7365 745f 6461 7461 2873 656c 662c  f set_data(self,
-00007b40: 2064 6174 613a 2062 7974 6573 2920 2d3e   data: bytes) ->
-00007b50: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00007b60: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-00007b70: 6c65 6172 5f64 6174 6128 7365 6c66 2920  lear_data(self) 
-00007b80: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00007b90: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00007ba0: 2067 6574 5f6d 6574 6164 6174 6128 7365   get_metadata(se
-00007bb0: 6c66 2920 2d3e 2022 536e 6170 7368 6f74  lf) -> "Snapshot
-00007bc0: 4d65 7461 6461 7461 5265 6622 3a0a 2020  MetadataRef":.  
-00007bd0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-00007be0: 2020 6465 6620 7365 745f 6d65 7461 6461    def set_metada
-00007bf0: 7461 280a 2020 2020 2020 2020 7365 6c66  ta(.        self
-00007c00: 2c20 6d65 7461 5f64 6174 613a 2022 536e  , meta_data: "Sn
-00007c10: 6170 7368 6f74 4d65 7461 6461 7461 2220  apshotMetadata" 
-00007c20: 7c20 2253 6e61 7073 686f 744d 6574 6164  | "SnapshotMetad
-00007c30: 6174 6152 6566 220a 2020 2020 2920 2d3e  ataRef".    ) ->
-00007c40: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00007c50: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-00007c60: 6c65 6172 5f6d 6574 6164 6174 6128 7365  lear_metadata(se
-00007c70: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00007c80: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00007c90: 2064 6566 2068 6173 5f6d 6574 6164 6174   def has_metadat
-00007ca0: 6128 7365 6c66 2920 2d3e 2062 6f6f 6c3a  a(self) -> bool:
-00007cb0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00007cc0: 0a0a 636c 6173 7320 536e 6170 7368 6f74  ..class Snapshot
-00007cd0: 285f 5f41 5049 5f53 6e61 7073 686f 7429  (__API_Snapshot)
-00007ce0: 3a0a 2020 2020 2222 2220 2222 220a 0a20  :.    """ """.. 
-00007cf0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00007d00: 7365 6c66 2920 2d3e 204e 6f6e 653a 202e  self) -> None: .
-00007d10: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-00007d20: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
-00007d30: 6175 6c74 2829 202d 3e20 2253 6e61 7073  ault() -> "Snaps
-00007d40: 686f 7422 3a20 2e2e 2e0a 2020 2020 4073  hot": ....    @s
-00007d50: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00007d60: 6465 6620 6465 636f 6465 2876 3a20 6279  def decode(v: by
-00007d70: 7465 7329 202d 3e20 2253 6e61 7073 686f  tes) -> "Snapsho
-00007d80: 7422 3a20 2e2e 2e0a 2020 2020 6465 6620  t": ....    def 
-00007d90: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-00007da0: 3e20 2253 6e61 7073 686f 7452 6566 223a  > "SnapshotRef":
-00007db0: 202e 2e2e 0a0a 636c 6173 7320 536e 6170   .....class Snap
-00007dc0: 7368 6f74 5265 6628 5f5f 4150 495f 536e  shotRef(__API_Sn
-00007dd0: 6170 7368 6f74 293a 0a20 2020 2022 2222  apshot):.    """
-00007de0: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
-00007df0: 7970 6520 6f66 203a 636c 6173 733a 6053  ype of :class:`S
-00007e00: 6e61 7073 686f 7460 2e0a 2020 2020 2222  napshot`..    ""
-00007e10: 220a 0a63 6c61 7373 205f 5f41 5049 5f4d  "..class __API_M
-00007e20: 6573 7361 6765 285f 5f43 6c6f 6e65 6162  essage(__Cloneab
-00007e30: 6c65 2c20 5f5f 456e 636f 6465 722c 205f  le, __Encoder, _
-00007e40: 5f44 6563 6f64 6572 293a 0a20 2020 2064  _Decoder):.    d
-00007e50: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-00007e60: 3e20 224d 6573 7361 6765 223a 202e 2e2e  > "Message": ...
-00007e70: 0a20 2020 2064 6566 2067 6574 5f63 6f6d  .    def get_com
-00007e80: 6d69 7428 7365 6c66 2920 2d3e 2069 6e74  mit(self) -> int
-00007e90: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00007ea0: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
-00007eb0: 6d6d 6974 2873 656c 662c 2063 6f6d 6d69  mmit(self, commi
-00007ec0: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-00007ed0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00007ee0: 0a20 2020 2064 6566 2063 6c65 6172 5f63  .    def clear_c
-00007ef0: 6f6d 6d69 7428 7365 6c66 2920 2d3e 204e  ommit(self) -> N
-00007f00: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00007f10: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00007f20: 5f63 6f6d 6d69 745f 7465 726d 2873 656c  _commit_term(sel
-00007f30: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00007f40: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00007f50: 6566 2073 6574 5f63 6f6d 6d69 745f 7465  ef set_commit_te
-00007f60: 726d 2873 656c 662c 2063 6f6d 6d69 745f  rm(self, commit_
-00007f70: 7465 726d 3a20 696e 7429 202d 3e20 4e6f  term: int) -> No
-00007f80: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-00007f90: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-00007fa0: 725f 636f 6d6d 6974 5f74 6572 6d28 7365  r_commit_term(se
-00007fb0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00007fc0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00007fd0: 2064 6566 2067 6574 5f66 726f 6d28 7365   def get_from(se
-00007fe0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00007ff0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-00008000: 6465 6620 7365 745f 6672 6f6d 2873 656c  def set_from(sel
-00008010: 662c 2066 726f 6d5f 3a20 696e 7429 202d  f, from_: int) -
-00008020: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00008030: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-00008040: 636c 6561 725f 6672 6f6d 2873 656c 6629  clear_from(self)
-00008050: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00008060: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00008070: 6620 6765 745f 696e 6465 7828 7365 6c66  f get_index(self
-00008080: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00008090: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-000080a0: 6620 7365 745f 696e 6465 7828 7365 6c66  f set_index(self
-000080b0: 2c20 696e 6465 783a 2069 6e74 2920 2d3e  , index: int) ->
-000080c0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000080d0: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-000080e0: 6c65 6172 5f69 6e64 6578 2873 656c 6629  lear_index(self)
-000080f0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00008100: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00008110: 6620 6765 745f 7465 726d 2873 656c 6629  f get_term(self)
-00008120: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00008130: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00008140: 2073 6574 5f74 6572 6d28 7365 6c66 2c20   set_term(self, 
-00008150: 7465 726d 3a20 696e 7429 202d 3e20 4e6f  term: int) -> No
-00008160: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-00008170: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-00008180: 725f 7465 726d 2873 656c 6629 202d 3e20  r_term(self) -> 
+00001810: 2220 2222 220a 0a63 6c61 7373 2054 6872  " """..class Thr
+00001820: 6561 6453 6166 654c 6f67 6765 7228 5f5f  eadSafeLogger(__
+00001830: 4150 495f 4c6f 6767 6572 293a 0a20 2020  API_Logger):.   
+00001840: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00001850: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00001860: 2020 2073 656c 662c 2063 6861 6e5f 7369     self, chan_si
+00001870: 7a65 3a20 696e 742c 206f 7665 7266 6c6f  ze: int, overflo
+00001880: 775f 7374 7261 7465 6779 3a20 224f 7665  w_strategy: "Ove
+00001890: 7266 6c6f 7753 7472 6174 6567 7922 0a20  rflowStrategy". 
+000018a0: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+000018b0: 2e0a 0a63 6c61 7373 205f 5f41 5049 5f52  ...class __API_R
+000018c0: 6166 7453 7461 7465 285f 5f43 6c6f 6e65  aftState(__Clone
+000018d0: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
+000018e0: 6c6f 6e65 2873 656c 6629 202d 3e20 2252  lone(self) -> "R
+000018f0: 6166 7453 7461 7465 223a 202e 2e2e 0a20  aftState": .... 
+00001900: 2020 2064 6566 2069 6e69 7469 616c 697a     def initializ
+00001910: 6564 2873 656c 6629 202d 3e20 626f 6f6c  ed(self) -> bool
+00001920: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00001930: 2020 2020 2020 496e 6469 6361 7465 7320        Indicates 
+00001940: 7468 6520 6052 6166 7453 7461 7465 6020  the `RaftState` 
+00001950: 6973 2069 6e69 7469 616c 697a 6564 206f  is initialized o
+00001960: 7220 6e6f 742e 0a20 2020 2020 2020 2022  r not..        "
+00001970: 2222 0a20 2020 2064 6566 2067 6574 5f63  "".    def get_c
+00001980: 6f6e 665f 7374 6174 6528 7365 6c66 2920  onf_state(self) 
+00001990: 2d3e 2022 436f 6e66 5374 6174 6552 6566  -> "ConfStateRef
+000019a0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+000019b0: 2020 2020 2020 2060 636f 6e66 5f73 7461         `conf_sta
+000019c0: 7465 603a 2052 6563 6f72 6473 2074 6865  te`: Records the
+000019d0: 2063 7572 7265 6e74 206e 6f64 6520 4944   current node ID
+000019e0: 7320 6c69 6b65 2060 5b31 2c20 322c 2033  s like `[1, 2, 3
+000019f0: 5d60 2069 6e20 7468 6520 636c 7573 7465  ]` in the cluste
+00001a00: 722e 2045 7665 7279 2052 6166 7420 6e6f  r. Every Raft no
+00001a10: 6465 206d 7573 7420 6861 7665 2061 0a20  de must have a. 
+00001a20: 2020 2020 2020 2075 6e69 7175 6520 4944         unique ID
+00001a30: 2069 6e20 7468 6520 636c 7573 7465 723b   in the cluster;
+00001a40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001a50: 2064 6566 2073 6574 5f63 6f6e 665f 7374   def set_conf_st
+00001a60: 6174 6528 7365 6c66 2c20 6373 3a20 2243  ate(self, cs: "C
+00001a70: 6f6e 6653 7461 7465 5265 6622 2920 2d3e  onfStateRef") ->
+00001a80: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00001a90: 2222 0a20 2020 2020 2020 2060 636f 6e66  "".        `conf
+00001aa0: 5f73 7461 7465 603a 2052 6563 6f72 6473  _state`: Records
+00001ab0: 2074 6865 2063 7572 7265 6e74 206e 6f64   the current nod
+00001ac0: 6520 4944 7320 6c69 6b65 2060 5b31 2c20  e IDs like `[1, 
+00001ad0: 322c 2033 5d60 2069 6e20 7468 6520 636c  2, 3]` in the cl
+00001ae0: 7573 7465 722e 2045 7665 7279 2052 6166  uster. Every Raf
+00001af0: 7420 6e6f 6465 206d 7573 7420 6861 7665  t node must have
+00001b00: 2061 0a20 2020 2020 2020 2075 6e69 7175   a.        uniqu
+00001b10: 6520 4944 2069 6e20 7468 6520 636c 7573  e ID in the clus
+00001b20: 7465 723b 0a20 2020 2020 2020 2022 2222  ter;.        """
+00001b30: 0a20 2020 2064 6566 2067 6574 5f68 6172  .    def get_har
+00001b40: 645f 7374 6174 6528 7365 6c66 2920 2d3e  d_state(self) ->
+00001b50: 2022 4861 7264 5374 6174 6552 6566 223a   "HardStateRef":
+00001b60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001b70: 2020 2020 2060 6861 7264 5f73 7461 7465       `hard_state
+00001b80: 603a 2043 6f6e 7461 696e 7320 7468 6520  `: Contains the 
+00001b90: 6c61 7374 206d 6574 6120 696e 666f 726d  last meta inform
+00001ba0: 6174 696f 6e20 696e 636c 7564 696e 6720  ation including 
+00001bb0: 636f 6d6d 6974 2069 6e64 6578 2c20 7468  commit index, th
+00001bc0: 6520 766f 7465 206c 6561 6465 722c 2061  e vote leader, a
+00001bd0: 6e64 2074 6865 2076 6f74 6520 7465 726d  nd the vote term
+00001be0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00001bf0: 2020 6465 6620 7365 745f 6861 7264 5f73    def set_hard_s
+00001c00: 7461 7465 2873 656c 662c 2068 733a 2022  tate(self, hs: "
+00001c10: 4861 7264 5374 6174 6552 6566 2229 202d  HardStateRef") -
+00001c20: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00001c30: 2222 220a 2020 2020 2020 2020 6068 6172  """.        `har
+00001c40: 645f 7374 6174 6560 3a20 436f 6e74 6169  d_state`: Contai
+00001c50: 6e73 2074 6865 206c 6173 7420 6d65 7461  ns the last meta
+00001c60: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e63   information inc
+00001c70: 6c75 6469 6e67 2063 6f6d 6d69 7420 696e  luding commit in
+00001c80: 6465 782c 2074 6865 2076 6f74 6520 6c65  dex, the vote le
+00001c90: 6164 6572 2c20 616e 6420 7468 6520 766f  ader, and the vo
+00001ca0: 7465 2074 6572 6d2e 0a20 2020 2020 2020  te term..       
+00001cb0: 2022 2222 0a0a 636c 6173 7320 5261 6674   """..class Raft
+00001cc0: 5374 6174 6528 5f5f 4150 495f 5261 6674  State(__API_Raft
+00001cd0: 5374 6174 6529 3a0a 2020 2020 2222 220a  State):.    """.
+00001ce0: 2020 2020 486f 6c64 7320 626f 7468 2074      Holds both t
+00001cf0: 6865 2068 6172 6420 7374 6174 6520 2863  he hard state (c
+00001d00: 6f6d 6d69 7420 696e 6465 782c 2076 6f74  ommit index, vot
+00001d10: 6520 6c65 6164 6572 2c20 7465 726d 2920  e leader, term) 
+00001d20: 616e 6420 7468 6520 636f 6e66 6967 7572  and the configur
+00001d30: 6174 696f 6e20 7374 6174 650a 2020 2020  ation state.    
+00001d40: 2843 7572 7265 6e74 206e 6f64 6520 4944  (Current node ID
+00001d50: 7329 0a20 2020 2022 2222 0a0a 2020 2020  s).    """..    
+00001d60: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00001d70: 6629 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  f) -> None: ....
+00001d80: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
+00001d90: 2873 656c 6629 202d 3e20 2252 6166 7453  (self) -> "RaftS
+00001da0: 7461 7465 5265 6622 3a20 2e2e 2e0a 2020  tateRef": ....  
+00001db0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+00001dc0: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
+00001dd0: 2920 2d3e 2022 5261 6674 5374 6174 6522  ) -> "RaftState"
+00001de0: 3a20 2e2e 2e0a 0a63 6c61 7373 2052 6166  : .....class Raf
+00001df0: 7453 7461 7465 5265 6628 5f5f 4150 495f  tStateRef(__API_
+00001e00: 5261 6674 5374 6174 6529 3a0a 2020 2020  RaftState):.    
+00001e10: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
+00001e20: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
+00001e30: 3a60 5261 6674 5374 6174 6560 2e0a 2020  :`RaftState`..  
+00001e40: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
+00001e50: 5049 5f53 746f 7261 6765 436f 7265 3a0a  PI_StorageCore:.
+00001e60: 2020 2020 6465 6620 6170 7065 6e64 2873      def append(s
+00001e70: 656c 662c 2065 6e74 733a 204c 6973 745b  elf, ents: List[
+00001e80: 2245 6e74 7279 225d 207c 204c 6973 745b  "Entry"] | List[
+00001e90: 2245 6e74 7279 5265 6622 5d29 202d 3e20  "EntryRef"]) -> 
+00001ea0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00001eb0: 220a 2020 2020 2020 2020 4170 7065 6e64  ".        Append
+00001ec0: 2074 6865 206e 6577 2065 6e74 7269 6573   the new entries
+00001ed0: 2074 6f20 7374 6f72 6167 652e 0a0a 2020   to storage...  
+00001ee0: 2020 2020 2020 2320 5061 6e69 6373 0a0a        # Panics..
+00001ef0: 2020 2020 2020 2020 5061 6e69 6373 2069          Panics i
+00001f00: 6620 6065 6e74 7360 2063 6f6e 7461 696e  f `ents` contain
+00001f10: 7320 636f 6d70 6163 7465 6420 656e 7472  s compacted entr
+00001f20: 6965 732c 206f 7220 7468 6572 6527 7320  ies, or there's 
+00001f30: 6120 6761 7020 6265 7477 6565 6e20 6065  a gap between `e
+00001f40: 6e74 7360 2061 6e64 2074 6865 206c 6173  nts` and the las
+00001f50: 740a 2020 2020 2020 2020 7265 6365 6976  t.        receiv
+00001f60: 6564 2065 6e74 7279 2069 6e20 7468 6520  ed entry in the 
+00001f70: 7374 6f72 6167 652e 0a20 2020 2020 2020  storage..       
+00001f80: 2022 2222 0a20 2020 2064 6566 2061 7070   """.    def app
+00001f90: 6c79 5f73 6e61 7073 686f 7428 7365 6c66  ly_snapshot(self
+00001fa0: 2c20 736e 6170 7368 6f74 3a20 2253 6e61  , snapshot: "Sna
+00001fb0: 7073 686f 7422 207c 2022 536e 6170 7368  pshot" | "Snapsh
+00001fc0: 6f74 5265 6622 2920 2d3e 204e 6f6e 653a  otRef") -> None:
+00001fd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001fe0: 2020 2020 204f 7665 7277 7269 7465 7320       Overwrites 
+00001ff0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
+00002000: 7468 6973 2053 746f 7261 6765 206f 626a  this Storage obj
+00002010: 6563 7420 7769 7468 2074 686f 7365 206f  ect with those o
+00002020: 6620 7468 6520 6769 7665 6e20 736e 6170  f the given snap
+00002030: 7368 6f74 2e0a 0a20 2020 2020 2020 2023  shot...        #
+00002040: 2050 616e 6963 730a 0a20 2020 2020 2020   Panics..       
+00002050: 2050 616e 6963 7320 6966 2074 6865 2073   Panics if the s
+00002060: 6e61 7073 686f 7420 696e 6465 7820 6973  napshot index is
+00002070: 206c 6573 7320 7468 616e 2074 6865 2073   less than the s
+00002080: 746f 7261 6765 2773 2066 6972 7374 2069  torage's first i
+00002090: 6e64 6578 2e0a 2020 2020 2020 2020 2222  ndex..        ""
+000020a0: 220a 2020 2020 6465 6620 636f 6d70 6163  ".    def compac
+000020b0: 7428 7365 6c66 2c20 636f 6d70 6163 745f  t(self, compact_
+000020c0: 696e 6465 783a 2069 6e74 2920 2d3e 204e  index: int) -> N
+000020d0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000020e0: 0a20 2020 2020 2020 2044 6973 6361 7264  .        Discard
+000020f0: 7320 616c 6c20 6c6f 6720 656e 7472 6965  s all log entrie
+00002100: 7320 7072 696f 7220 746f 2063 6f6d 7061  s prior to compa
+00002110: 6374 5f69 6e64 6578 2e0a 2020 2020 2020  ct_index..      
+00002120: 2020 4974 2069 7320 7468 6520 6170 706c    It is the appl
+00002130: 6963 6174 696f 6e27 7320 7265 7370 6f6e  ication's respon
+00002140: 7369 6269 6c69 7479 2074 6f20 6e6f 7420  sibility to not 
+00002150: 6174 7465 6d70 7420 746f 2063 6f6d 7061  attempt to compa
+00002160: 6374 2061 6e20 696e 6465 780a 2020 2020  ct an index.    
+00002170: 2020 2020 6772 6561 7465 7220 7468 616e      greater than
+00002180: 2052 6166 744c 6f67 2e61 7070 6c69 6564   RaftLog.applied
+00002190: 2e0a 0a20 2020 2020 2020 2023 2050 616e  ...        # Pan
+000021a0: 6963 730a 0a20 2020 2020 2020 2050 616e  ics..        Pan
+000021b0: 6963 7320 6966 2060 636f 6d70 6163 745f  ics if `compact_
+000021c0: 696e 6465 7860 2069 7320 6869 6768 6572  index` is higher
+000021d0: 2074 6861 6e20 6053 746f 7261 6765 3a3a   than `Storage::
+000021e0: 6c61 7374 5f69 6e64 6578 2826 7365 6c66  last_index(&self
+000021f0: 2920 2b20 3160 2e0a 2020 2020 2020 2020  ) + 1`..        
+00002200: 2222 220a 2020 2020 6465 6620 636f 6d6d  """.    def comm
+00002210: 6974 5f74 6f28 7365 6c66 2c20 696e 6465  it_to(self, inde
+00002220: 783a 2069 6e74 2920 2d3e 204e 6f6e 653a  x: int) -> None:
+00002230: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002240: 2020 2020 2043 6f6d 6d69 7420 746f 2061       Commit to a
+00002250: 6e20 696e 6465 782e 0a0a 2020 2020 2020  n index...      
+00002260: 2020 2320 5061 6e69 6373 0a0a 2020 2020    # Panics..    
+00002270: 2020 2020 5061 6e69 6373 2069 6620 7468      Panics if th
+00002280: 6572 6520 6973 206e 6f20 7375 6368 2065  ere is no such e
+00002290: 6e74 7279 2069 6e20 7261 6674 206c 6f67  ntry in raft log
+000022a0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+000022b0: 2020 2064 6566 2063 6f6d 6d69 745f 746f     def commit_to
+000022c0: 5f61 6e64 5f73 6574 5f63 6f6e 665f 7374  _and_set_conf_st
+000022d0: 6174 6573 280a 2020 2020 2020 2020 7365  ates(.        se
+000022e0: 6c66 2c20 6964 783a 2069 6e74 2c20 6373  lf, idx: int, cs
+000022f0: 3a20 4f70 7469 6f6e 616c 5b22 436f 6e66  : Optional["Conf
+00002300: 5374 6174 6522 5d20 7c20 4f70 7469 6f6e  State"] | Option
+00002310: 616c 5b22 436f 6e66 5374 6174 6552 6566  al["ConfStateRef
+00002320: 225d 0a20 2020 2029 202d 3e20 4e6f 6e65  "].    ) -> None
+00002330: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00002340: 2020 2020 2020 436f 6d6d 6974 2074 6f20        Commit to 
+00002350: 6069 6478 6020 616e 6420 7365 7420 636f  `idx` and set co
+00002360: 6e66 6967 7572 6174 696f 6e20 746f 2074  nfiguration to t
+00002370: 6865 2067 6976 656e 2073 7461 7465 732e  he given states.
+00002380: 204f 6e6c 7920 7573 6564 2066 6f72 2074   Only used for t
+00002390: 6573 7473 2e0a 2020 2020 2020 2020 2222  ests..        ""
+000023a0: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
+000023b0: 6e66 5f73 7461 7465 2873 656c 662c 2063  nf_state(self, c
+000023c0: 733a 2022 436f 6e66 5374 6174 6522 207c  s: "ConfState" |
+000023d0: 2022 436f 6e66 5374 6174 6552 6566 2229   "ConfStateRef")
+000023e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000023f0: 2020 2222 220a 2020 2020 2020 2020 5361    """.        Sa
+00002400: 7665 7320 7468 6520 6375 7272 656e 7420  ves the current 
+00002410: 636f 6e66 2073 7461 7465 2e0a 2020 2020  conf state..    
+00002420: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00002430: 6861 7264 5f73 7461 7465 2873 656c 6629  hard_state(self)
+00002440: 202d 3e20 2248 6172 6453 7461 7465 5265   -> "HardStateRe
+00002450: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
+00002460: 2020 2020 2020 2020 4765 7420 7468 6520          Get the 
+00002470: 6861 7264 2073 7461 7465 2e0a 2020 2020  hard state..    
+00002480: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00002490: 7365 745f 6861 7264 7374 6174 6528 7365  set_hardstate(se
+000024a0: 6c66 2c20 6873 3a20 2248 6172 6453 7461  lf, hs: "HardSta
+000024b0: 7465 2220 7c20 2248 6172 6453 7461 7465  te" | "HardState
+000024c0: 5265 6622 2920 2d3e 204e 6f6e 653a 0a20  Ref") -> None:. 
+000024d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000024e0: 2020 2053 6176 6573 2074 6865 2063 7572     Saves the cur
+000024f0: 7265 6e74 2048 6172 6453 7461 7465 2e0a  rent HardState..
+00002500: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002510: 6465 6620 7472 6967 6765 725f 736e 6170  def trigger_snap
+00002520: 5f75 6e61 7661 696c 6162 6c65 2873 656c  _unavailable(sel
+00002530: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00002540: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00002550: 5472 6967 6765 7220 6120 536e 6170 7368  Trigger a Snapsh
+00002560: 6f74 5465 6d70 6f72 6172 696c 7955 6e61  otTemporarilyUna
+00002570: 7661 696c 6162 6c65 2065 7272 6f72 2e0a  vailable error..
+00002580: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00002590: 6465 6620 7472 6967 6765 725f 6c6f 675f  def trigger_log_
+000025a0: 756e 6176 6169 6c61 626c 6528 7365 6c66  unavailable(self
+000025b0: 2c20 763a 2062 6f6f 6c29 202d 3e20 4e6f  , v: bool) -> No
+000025c0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+000025d0: 2020 2020 2020 2020 5365 7420 6120 4c6f          Set a Lo
+000025e0: 6754 656d 706f 7261 7269 6c79 556e 6176  gTemporarilyUnav
+000025f0: 6169 6c61 626c 6520 6572 726f 722e 0a20  ailable error.. 
+00002600: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00002610: 6566 2074 616b 655f 6765 745f 656e 7472  ef take_get_entr
+00002620: 6965 735f 636f 6e74 6578 7428 7365 6c66  ies_context(self
+00002630: 2920 2d3e 204f 7074 696f 6e61 6c5b 2247  ) -> Optional["G
+00002640: 6574 456e 7472 6965 7343 6f6e 7465 7874  etEntriesContext
+00002650: 225d 3a0a 2020 2020 2020 2020 2222 220a  "]:.        """.
+00002660: 2020 2020 2020 2020 5461 6b65 2067 6574          Take get
+00002670: 2065 6e74 7269 6573 2063 6f6e 7465 7874   entries context
+00002680: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
+00002690: 6c61 7373 204d 656d 5374 6f72 6167 6543  lass MemStorageC
+000026a0: 6f72 6528 5f5f 4150 495f 5374 6f72 6167  ore(__API_Storag
+000026b0: 6543 6f72 6529 3a0a 2020 2020 2222 220a  eCore):.    """.
+000026c0: 2020 2020 5468 6520 4d65 6d6f 7279 2053      The Memory S
+000026d0: 746f 7261 6765 2043 6f72 6520 696e 7374  torage Core inst
+000026e0: 616e 6365 2068 6f6c 6473 2074 6865 2061  ance holds the a
+000026f0: 6374 7561 6c20 7374 6174 6520 6f66 2074  ctual state of t
+00002700: 6865 2073 746f 7261 6765 2073 7472 7563  he storage struc
+00002710: 742e 2054 6f20 6163 6365 7373 2074 6869  t. To access thi
+00002720: 730a 2020 2020 7661 6c75 652c 2075 7365  s.    value, use
+00002730: 2074 6865 2060 726c 6020 616e 6420 6077   the `rl` and `w
+00002740: 6c60 2066 756e 6374 696f 6e73 206f 6e20  l` functions on 
+00002750: 7468 6520 6d61 696e 204d 656d 5374 6f72  the main MemStor
+00002760: 6167 6520 696d 706c 656d 656e 7461 7469  age implementati
+00002770: 6f6e 2e0a 2020 2020 2222 220a 0a20 2020  on..    """..   
+00002780: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
+00002790: 6c66 2920 2d3e 2022 4d65 6d53 746f 7261  lf) -> "MemStora
+000027a0: 6765 436f 7265 5265 6622 3a20 2e2e 2e0a  geCoreRef": ....
+000027b0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+000027c0: 640a 2020 2020 6465 6620 6465 6661 756c  d.    def defaul
+000027d0: 7428 2920 2d3e 2022 4d65 6d53 746f 7261  t() -> "MemStora
+000027e0: 6765 436f 7265 223a 202e 2e2e 0a0a 636c  geCore": .....cl
+000027f0: 6173 7320 4d65 6d53 746f 7261 6765 436f  ass MemStorageCo
+00002800: 7265 5265 6628 5f5f 4150 495f 5374 6f72  reRef(__API_Stor
+00002810: 6167 6543 6f72 6529 3a0a 2020 2020 2222  ageCore):.    ""
+00002820: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
+00002830: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
+00002840: 4d65 6d53 746f 7261 6765 602e 0a20 2020  MemStorage`..   
+00002850: 2022 2222 0a0a 636c 6173 7320 5374 6f72   """..class Stor
+00002860: 6167 6543 6f72 6528 5f5f 4150 495f 5374  ageCore(__API_St
+00002870: 6f72 6167 6543 6f72 6529 3a0a 2020 2020  orageCore):.    
+00002880: 2222 2220 2222 220a 0a20 2020 2064 6566  """ """..    def
+00002890: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
+000028a0: 2d3e 2022 5374 6f72 6167 6543 6f72 6552  -> "StorageCoreR
+000028b0: 6566 223a 202e 2e2e 0a20 2020 2040 7374  ef": ....    @st
+000028c0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+000028d0: 6566 2064 6566 6175 6c74 2829 202d 3e20  ef default() -> 
+000028e0: 2253 746f 7261 6765 436f 7265 223a 202e  "StorageCore": .
+000028f0: 2e2e 0a0a 636c 6173 7320 5374 6f72 6167  ....class Storag
+00002900: 6543 6f72 6552 6566 285f 5f41 5049 5f53  eCoreRef(__API_S
+00002910: 746f 7261 6765 436f 7265 293a 0a20 2020  torageCore):.   
+00002920: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
+00002930: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
+00002940: 733a 6053 746f 7261 6765 436f 7265 602e  s:`StorageCore`.
+00002950: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+00002960: 5f5f 4150 495f 5374 6f72 6167 6528 5f5f  __API_Storage(__
+00002970: 436c 6f6e 6561 626c 6529 3a0a 2020 2020  Cloneable):.    
+00002980: 6465 6620 636c 6f6e 6528 7365 6c66 2920  def clone(self) 
+00002990: 2d3e 2041 6e79 3a20 2e2e 2e0a 2020 2020  -> Any: ....    
+000029a0: 6465 6620 696e 6974 6961 6c69 7a65 5f77  def initialize_w
+000029b0: 6974 685f 636f 6e66 5f73 7461 7465 280a  ith_conf_state(.
+000029c0: 2020 2020 2020 2020 7365 6c66 2c20 636f          self, co
+000029d0: 6e66 5f73 7461 7465 3a20 2243 6f6e 6653  nf_state: "ConfS
+000029e0: 7461 7465 2220 7c20 2243 6f6e 6653 7461  tate" | "ConfSta
+000029f0: 7465 5265 6622 0a20 2020 2029 202d 3e20  teRef".    ) -> 
+00002a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00002a10: 220a 2020 2020 2020 2020 496e 6974 6961  ".        Initia
+00002a20: 6c69 7a65 2061 2060 4d65 6d53 746f 7261  lize a `MemStora
+00002a30: 6765 6020 7769 7468 2061 2067 6976 656e  ge` with a given
+00002a40: 2060 436f 6e66 6967 602e 0a0a 2020 2020   `Config`...    
+00002a50: 2020 2020 596f 7520 7368 6f75 6c64 2075      You should u
+00002a60: 7365 2074 6865 2073 616d 6520 696e 7075  se the same inpu
+00002a70: 7420 746f 2069 6e69 7469 616c 697a 6520  t to initialize 
+00002a80: 616c 6c20 6e6f 6465 732e 0a20 2020 2020  all nodes..     
+00002a90: 2020 2022 2222 0a20 2020 2064 6566 2069     """.    def i
+00002aa0: 6e69 7469 616c 5f73 7461 7465 2873 656c  nitial_state(sel
+00002ab0: 6629 202d 3e20 5261 6674 5374 6174 653a  f) -> RaftState:
+00002ac0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002ad0: 2020 2020 2049 6d70 6c65 6d65 6e74 7320       Implements 
+00002ae0: 7468 6520 5374 6f72 6167 6520 7472 6169  the Storage trai
+00002af0: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+00002b00: 2020 2064 6566 2065 6e74 7269 6573 280a     def entries(.
+00002b10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00002b20: 2020 2020 2020 6c6f 773a 2069 6e74 2c0a        low: int,.
+00002b30: 2020 2020 2020 2020 6869 6768 3a20 696e          high: in
+00002b40: 742c 0a20 2020 2020 2020 2063 6f6e 7465  t,.        conte
+00002b50: 7874 3a20 2247 6574 456e 7472 6965 7343  xt: "GetEntriesC
+00002b60: 6f6e 7465 7874 5265 6622 2c0a 2020 2020  ontextRef",.    
+00002b70: 2020 2020 6d61 785f 7369 7a65 3a20 4f70      max_size: Op
+00002b80: 7469 6f6e 616c 5b69 6e74 5d2c 0a20 2020  tional[int],.   
+00002b90: 2029 202d 3e20 4c69 7374 5b22 456e 7472   ) -> List["Entr
+00002ba0: 7922 5d3a 0a20 2020 2020 2020 2022 2222  y"]:.        """
+00002bb0: 0a20 2020 2020 2020 2049 6d70 6c65 6d65  .        Impleme
+00002bc0: 6e74 7320 7468 6520 5374 6f72 6167 6520  nts the Storage 
+00002bd0: 7472 6169 742e 0a20 2020 2020 2020 2022  trait..        "
+00002be0: 2222 0a20 2020 2064 6566 2074 6572 6d28  "".    def term(
+00002bf0: 7365 6c66 2c20 6964 783a 2069 6e74 2920  self, idx: int) 
+00002c00: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00002c10: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
+00002c20: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
+00002c30: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
+00002c40: 2020 2222 220a 2020 2020 6465 6620 6669    """.    def fi
+00002c50: 7273 745f 696e 6465 7828 7365 6c66 2920  rst_index(self) 
+00002c60: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00002c70: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
+00002c80: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
+00002c90: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
+00002ca0: 2020 2222 220a 2020 2020 6465 6620 6c61    """.    def la
+00002cb0: 7374 5f69 6e64 6578 2873 656c 6629 202d  st_index(self) -
+00002cc0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00002cd0: 2222 0a20 2020 2020 2020 2049 6d70 6c65  "".        Imple
+00002ce0: 6d65 6e74 7320 7468 6520 5374 6f72 6167  ments the Storag
+00002cf0: 6520 7472 6169 742e 0a20 2020 2020 2020  e trait..       
+00002d00: 2022 2222 0a20 2020 2064 6566 2073 6e61   """.    def sna
+00002d10: 7073 686f 7428 7365 6c66 2c20 7265 7175  pshot(self, requ
+00002d20: 6573 745f 696e 6465 783a 2069 6e74 2c20  est_index: int, 
+00002d30: 746f 3a20 696e 7429 202d 3e20 2253 6e61  to: int) -> "Sna
+00002d40: 7073 686f 7422 3a0a 2020 2020 2020 2020  pshot":.        
+00002d50: 2222 220a 2020 2020 2020 2020 496d 706c  """.        Impl
+00002d60: 656d 656e 7473 2074 6865 2053 746f 7261  ements the Stora
+00002d70: 6765 2074 7261 6974 2e0a 2020 2020 2020  ge trait..      
+00002d80: 2020 2222 220a 0a63 6c61 7373 204d 656d    """..class Mem
+00002d90: 5374 6f72 6167 6528 5f5f 4150 495f 5374  Storage(__API_St
+00002da0: 6f72 6167 6529 3a0a 2020 2020 2222 220a  orage):.    """.
+00002db0: 2020 2020 604d 656d 5374 6f72 6167 6560      `MemStorage`
+00002dc0: 2069 7320 6120 7468 7265 6164 2d73 6166   is a thread-saf
+00002dd0: 6520 6275 7420 696e 636f 6d70 6c65 7465  e but incomplete
+00002de0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00002df0: 6f66 2060 5374 6f72 6167 6560 2c20 6d61  of `Storage`, ma
+00002e00: 696e 6c79 2066 6f72 2074 6573 7473 2e0a  inly for tests..
+00002e10: 0a20 2020 2041 2072 6561 6c20 6053 746f  .    A real `Sto
+00002e20: 7261 6765 6020 7368 6f75 6c64 2073 6176  rage` should sav
+00002e30: 6520 626f 7468 2072 6166 7420 6c6f 6773  e both raft logs
+00002e40: 2061 6e64 2061 7070 6c69 6564 2064 6174   and applied dat
+00002e50: 612e 2048 6f77 6576 6572 2060 4d65 6d53  a. However `MemS
+00002e60: 746f 7261 6765 6020 6f6e 6c79 0a20 2020  torage` only.   
+00002e70: 2063 6f6e 7461 696e 7320 7261 6674 206c   contains raft l
+00002e80: 6f67 732e 2053 6f20 796f 7520 6361 6e20  ogs. So you can 
+00002e90: 6361 6c6c 2060 4d65 6d53 746f 7261 6765  call `MemStorage
+00002ea0: 3a3a 6170 7065 6e64 6020 746f 2070 6572  ::append` to per
+00002eb0: 7369 7374 206e 6577 2072 6563 6569 7665  sist new receive
+00002ec0: 6420 756e 7374 6162 6c65 2072 6166 740a  d unstable raft.
+00002ed0: 2020 2020 6c6f 6773 2061 6e64 2074 6865      logs and the
+00002ee0: 6e20 6163 6365 7373 2074 6865 6d20 7769  n access them wi
+00002ef0: 7468 2060 5374 6f72 6167 6560 2041 5049  th `Storage` API
+00002f00: 732e 2054 6865 206f 6e6c 7920 6578 6365  s. The only exce
+00002f10: 7074 696f 6e20 6973 2060 5374 6f72 6167  ption is `Storag
+00002f20: 653a 3a73 6e61 7073 686f 7460 2e20 5468  e::snapshot`. Th
+00002f30: 6572 650a 2020 2020 6973 206e 6f20 6461  ere.    is no da
+00002f40: 7461 2069 6e20 6053 6e61 7073 686f 7460  ta in `Snapshot`
+00002f50: 2072 6574 7572 6e65 6420 6279 2060 4d65   returned by `Me
+00002f60: 6d53 746f 7261 6765 3a3a 736e 6170 7368  mStorage::snapsh
+00002f70: 6f74 6020 6265 6361 7573 6520 6170 706c  ot` because appl
+00002f80: 6965 6420 6461 7461 2069 7320 6e6f 7420  ied data is not 
+00002f90: 7374 6f72 6564 0a20 2020 2069 6e20 604d  stored.    in `M
+00002fa0: 656d 5374 6f72 6167 6560 2e0a 2020 2020  emStorage`..    
+00002fb0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+00002fc0: 6e69 745f 5f28 7365 6c66 2920 2d3e 204e  nit__(self) -> N
+00002fd0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+00002fe0: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
+00002ff0: 2d3e 2022 4d65 6d53 746f 7261 6765 5265  -> "MemStorageRe
+00003000: 6622 3a20 2e2e 2e0a 2020 2020 6465 6620  f": ....    def 
+00003010: 636c 6f6e 6528 7365 6c66 2920 2d3e 2022  clone(self) -> "
+00003020: 4d65 6d53 746f 7261 6765 223a 202e 2e2e  MemStorage": ...
+00003030: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00003040: 6f64 0a20 2020 2064 6566 2064 6566 6175  od.    def defau
+00003050: 6c74 2829 202d 3e20 224d 656d 5374 6f72  lt() -> "MemStor
+00003060: 6167 6522 3a20 2e2e 2e0a 2020 2020 4073  age": ....    @s
+00003070: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00003080: 6465 6620 6e65 775f 7769 7468 5f63 6f6e  def new_with_con
+00003090: 665f 7374 6174 6528 0a20 2020 2020 2020  f_state(.       
+000030a0: 2063 6f6e 665f 7374 6174 653a 2022 436f   conf_state: "Co
+000030b0: 6e66 5374 6174 6522 207c 2022 436f 6e66  nfState" | "Conf
+000030c0: 5374 6174 6552 6566 222c 0a20 2020 2029  StateRef",.    )
+000030d0: 202d 3e20 224d 656d 5374 6f72 6167 6522   -> "MemStorage"
+000030e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000030f0: 2020 2020 2020 4372 6561 7465 2061 206e        Create a n
+00003100: 6577 2060 4d65 6d53 746f 7261 6765 6020  ew `MemStorage` 
+00003110: 7769 7468 2061 2067 6976 656e 2060 436f  with a given `Co
+00003120: 6e66 6967 602e 2054 6865 2067 6976 656e  nfig`. The given
+00003130: 2060 436f 6e66 6967 6020 7769 6c6c 2062   `Config` will b
+00003140: 6520 7573 6564 2074 6f0a 2020 2020 2020  e used to.      
+00003150: 2020 696e 6974 6961 6c69 7a65 2074 6865    initialize the
+00003160: 2073 746f 7261 6765 2e0a 0a20 2020 2020   storage...     
+00003170: 2020 2059 6f75 2073 686f 756c 6420 7573     You should us
+00003180: 6520 7468 6520 7361 6d65 2069 6e70 7574  e the same input
+00003190: 2074 6f20 696e 6974 6961 6c69 7a65 2061   to initialize a
+000031a0: 6c6c 206e 6f64 6573 2e0a 2020 2020 2020  ll nodes..      
+000031b0: 2020 2222 220a 2020 2020 6465 6620 776c    """.    def wl
+000031c0: 2873 656c 6629 202d 3e20 224d 656d 5374  (self) -> "MemSt
+000031d0: 6f72 6167 6543 6f72 6552 6566 223a 0a20  orageCoreRef":. 
+000031e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000031f0: 2020 204f 7065 6e73 2075 7020 6120 7772     Opens up a wr
+00003200: 6974 6520 6c6f 636b 206f 6e20 7468 6520  ite lock on the 
+00003210: 7374 6f72 6167 6520 616e 6420 7265 7475  storage and retu
+00003220: 726e 7320 6775 6172 6420 6861 6e64 6c65  rns guard handle
+00003230: 2e20 5573 6520 7468 6973 0a20 2020 2020  . Use this.     
+00003240: 2020 2077 6974 6820 6675 6e63 7469 6f6e     with function
+00003250: 7320 7468 6174 2074 616b 6520 6120 6d75  s that take a mu
+00003260: 7461 626c 6520 7265 6665 7265 6e63 6520  table reference 
+00003270: 746f 2073 656c 662e 0a20 2020 2020 2020  to self..       
+00003280: 2022 2222 0a20 2020 2064 6566 2072 6c28   """.    def rl(
+00003290: 7365 6c66 2920 2d3e 2022 4d65 6d53 746f  self) -> "MemSto
+000032a0: 7261 6765 436f 7265 5265 6622 3a0a 2020  rageCoreRef":.  
+000032b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000032c0: 2020 4f70 656e 7320 7570 2061 2072 6561    Opens up a rea
+000032d0: 6420 6c6f 636b 206f 6e20 7468 6520 7374  d lock on the st
+000032e0: 6f72 6167 6520 616e 6420 7265 7475 726e  orage and return
+000032f0: 7320 6120 6775 6172 6420 6861 6e64 6c65  s a guard handle
+00003300: 2e20 5573 6520 7468 6973 0a20 2020 2020  . Use this.     
+00003310: 2020 2077 6974 6820 6675 6e63 7469 6f6e     with function
+00003320: 7320 7468 6174 2064 6f6e 2774 2072 6571  s that don't req
+00003330: 7569 7265 206d 7574 6174 696f 6e2e 0a20  uire mutation.. 
+00003340: 2020 2020 2020 2022 2222 0a0a 636c 6173         """..clas
+00003350: 7320 4d65 6d53 746f 7261 6765 5265 6628  s MemStorageRef(
+00003360: 5f5f 4150 495f 5374 6f72 6167 6529 3a0a  __API_Storage):.
+00003370: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
+00003380: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
+00003390: 6c61 7373 3a60 4d65 6d53 746f 7261 6765  lass:`MemStorage
+000033a0: 602e 0a20 2020 2022 2222 0a0a 2020 2020  `..    """..    
+000033b0: 6465 6620 636c 6f6e 6528 7365 6c66 2920  def clone(self) 
+000033c0: 2d3e 2022 4d65 6d53 746f 7261 6765 223a  -> "MemStorage":
+000033d0: 202e 2e2e 0a20 2020 2064 6566 2077 6c28   ....    def wl(
+000033e0: 7365 6c66 2920 2d3e 2022 4d65 6d53 746f  self) -> "MemSto
+000033f0: 7261 6765 436f 7265 5265 6622 3a0a 2020  rageCoreRef":.  
+00003400: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00003410: 2020 4f70 656e 7320 7570 2061 2077 7269    Opens up a wri
+00003420: 7465 206c 6f63 6b20 6f6e 2074 6865 2073  te lock on the s
+00003430: 746f 7261 6765 2061 6e64 2072 6574 7572  torage and retur
+00003440: 6e73 2067 7561 7264 2068 616e 646c 652e  ns guard handle.
+00003450: 2055 7365 2074 6869 730a 2020 2020 2020   Use this.      
+00003460: 2020 7769 7468 2066 756e 6374 696f 6e73    with functions
+00003470: 2074 6861 7420 7461 6b65 2061 206d 7574   that take a mut
+00003480: 6162 6c65 2072 6566 6572 656e 6365 2074  able reference t
+00003490: 6f20 7365 6c66 2e0a 2020 2020 2020 2020  o self..        
+000034a0: 2222 220a 2020 2020 6465 6620 726c 2873  """.    def rl(s
+000034b0: 656c 6629 202d 3e20 224d 656d 5374 6f72  elf) -> "MemStor
+000034c0: 6167 6543 6f72 6552 6566 223a 0a20 2020  ageCoreRef":.   
+000034d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000034e0: 204f 7065 6e73 2075 7020 6120 7265 6164   Opens up a read
+000034f0: 206c 6f63 6b20 6f6e 2074 6865 2073 746f   lock on the sto
+00003500: 7261 6765 2061 6e64 2072 6574 7572 6e73  rage and returns
+00003510: 2061 2067 7561 7264 2068 616e 646c 652e   a guard handle.
+00003520: 2055 7365 2074 6869 730a 2020 2020 2020   Use this.      
+00003530: 2020 7769 7468 2066 756e 6374 696f 6e73    with functions
+00003540: 2074 6861 7420 646f 6e27 7420 7265 7175   that don't requ
+00003550: 6972 6520 6d75 7461 7469 6f6e 2e0a 2020  ire mutation..  
+00003560: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
+00003570: 2053 746f 7261 6765 285f 5f41 5049 5f53   Storage(__API_S
+00003580: 746f 7261 6765 293a 0a20 2020 2022 2222  torage):.    """
+00003590: 0a20 2020 2053 746f 7261 6765 2073 6176  .    Storage sav
+000035a0: 6573 2061 6c6c 2074 6865 2069 6e66 6f72  es all the infor
+000035b0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+000035c0: 2063 7572 7265 6e74 2052 6166 7420 696d   current Raft im
+000035d0: 706c 656d 656e 7461 7469 6f6e 2c20 696e  plementation, in
+000035e0: 636c 7564 696e 6720 5261 6674 204c 6f67  cluding Raft Log
+000035f0: 2c0a 2020 2020 636f 6d6d 6974 2069 6e64  ,.    commit ind
+00003600: 6578 2c20 7468 6520 6c65 6164 6572 2074  ex, the leader t
+00003610: 6f20 766f 7465 2066 6f72 2c20 6574 632e  o vote for, etc.
+00003620: 0a0a 2020 2020 4966 2061 6e79 2053 746f  ..    If any Sto
+00003630: 7261 6765 206d 6574 686f 6420 7265 7475  rage method retu
+00003640: 726e 7320 616e 2065 7272 6f72 2c20 7468  rns an error, th
+00003650: 6520 7261 6674 2069 6e73 7461 6e63 6520  e raft instance 
+00003660: 7769 6c6c 0a20 2020 2062 6563 6f6d 6520  will.    become 
+00003670: 696e 6f70 6572 6162 6c65 2061 6e64 2072  inoperable and r
+00003680: 6566 7573 6520 746f 2070 6172 7469 6369  efuse to partici
+00003690: 7061 7465 2069 6e20 656c 6563 7469 6f6e  pate in election
+000036a0: 733b 2074 6865 0a20 2020 2061 7070 6c69  s; the.    appli
+000036b0: 6361 7469 6f6e 2069 7320 7265 7370 6f6e  cation is respon
+000036c0: 7369 626c 6520 666f 7220 636c 6561 6e75  sible for cleanu
+000036d0: 7020 616e 6420 7265 636f 7665 7279 2069  p and recovery i
+000036e0: 6e20 7468 6973 2063 6173 652e 0a20 2020  n this case..   
+000036f0: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00003700: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+00003710: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+00003720: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+00003730: 202d 3e20 2253 746f 7261 6765 5265 6622   -> "StorageRef"
+00003740: 3a20 2e2e 2e0a 2020 2020 6465 6620 636c  : ....    def cl
+00003750: 6f6e 6528 7365 6c66 2920 2d3e 2022 5374  one(self) -> "St
+00003760: 6f72 6167 6522 3a20 2e2e 2e0a 2020 2020  orage": ....    
+00003770: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00003780: 2020 6465 6620 6465 6661 756c 7428 2920    def default() 
+00003790: 2d3e 2022 5374 6f72 6167 6522 3a20 2e2e  -> "Storage": ..
+000037a0: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+000037b0: 686f 640a 2020 2020 6465 6620 6e65 775f  hod.    def new_
+000037c0: 7769 7468 5f63 6f6e 665f 7374 6174 6528  with_conf_state(
+000037d0: 0a20 2020 2020 2020 2063 6f6e 665f 7374  .        conf_st
+000037e0: 6174 653a 2022 436f 6e66 5374 6174 6522  ate: "ConfState"
+000037f0: 207c 2022 436f 6e66 5374 6174 6552 6566   | "ConfStateRef
+00003800: 222c 0a20 2020 2029 202d 3e20 2253 746f  ",.    ) -> "Sto
+00003810: 7261 6765 223a 0a20 2020 2020 2020 2022  rage":.        "
+00003820: 2222 2022 2222 0a20 2020 2064 6566 2077  "" """.    def w
+00003830: 6c28 7365 6c66 2920 2d3e 2041 6e79 3a0a  l(self) -> Any:.
+00003840: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003850: 2020 2020 4f70 656e 7320 7570 2061 2077      Opens up a w
+00003860: 7269 7465 206c 6f63 6b20 6f6e 2074 6865  rite lock on the
+00003870: 2073 746f 7261 6765 2061 6e64 2072 6574   storage and ret
+00003880: 7572 6e73 2067 7561 7264 2068 616e 646c  urns guard handl
+00003890: 652e 2055 7365 2074 6869 730a 2020 2020  e. Use this.    
+000038a0: 2020 2020 7769 7468 2066 756e 6374 696f      with functio
+000038b0: 6e73 2074 6861 7420 7461 6b65 2061 206d  ns that take a m
+000038c0: 7574 6162 6c65 2072 6566 6572 656e 6365  utable reference
+000038d0: 2074 6f20 7365 6c66 2e0a 2020 2020 2020   to self..      
+000038e0: 2020 2222 220a 2020 2020 6465 6620 726c    """.    def rl
+000038f0: 2873 656c 6629 202d 3e20 416e 793a 0a20  (self) -> Any:. 
+00003900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003910: 2020 204f 7065 6e73 2075 7020 6120 7265     Opens up a re
+00003920: 6164 206c 6f63 6b20 6f6e 2074 6865 2073  ad lock on the s
+00003930: 746f 7261 6765 2061 6e64 2072 6574 7572  torage and retur
+00003940: 6e73 2061 2067 7561 7264 2068 616e 646c  ns a guard handl
+00003950: 652e 2055 7365 2074 6869 730a 2020 2020  e. Use this.    
+00003960: 2020 2020 7769 7468 2066 756e 6374 696f      with functio
+00003970: 6e73 2074 6861 7420 646f 6e27 7420 7265  ns that don't re
+00003980: 7175 6972 6520 6d75 7461 7469 6f6e 2e0a  quire mutation..
+00003990: 2020 2020 2020 2020 2222 220a 0a63 6c61          """..cla
+000039a0: 7373 2053 746f 7261 6765 5265 6628 5f5f  ss StorageRef(__
+000039b0: 4150 495f 5374 6f72 6167 6529 3a0a 2020  API_Storage):.  
+000039c0: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
+000039d0: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
+000039e0: 7373 3a60 5374 6f72 6167 6560 2e0a 2020  ss:`Storage`..  
+000039f0: 2020 2222 220a 0a20 2020 2064 6566 2063    """..    def c
+00003a00: 6c6f 6e65 2873 656c 6629 202d 3e20 2253  lone(self) -> "S
+00003a10: 746f 7261 6765 223a 202e 2e2e 0a20 2020  torage": ....   
+00003a20: 2064 6566 2077 6c28 7365 6c66 2920 2d3e   def wl(self) ->
+00003a30: 2041 6e79 3a0a 2020 2020 2020 2020 2222   Any:.        ""
+00003a40: 220a 2020 2020 2020 2020 4f70 656e 7320  ".        Opens 
+00003a50: 7570 2061 2077 7269 7465 206c 6f63 6b20  up a write lock 
+00003a60: 6f6e 2074 6865 2073 746f 7261 6765 2061  on the storage a
+00003a70: 6e64 2072 6574 7572 6e73 2067 7561 7264  nd returns guard
+00003a80: 2068 616e 646c 652e 2055 7365 2074 6869   handle. Use thi
+00003a90: 730a 2020 2020 2020 2020 7769 7468 2066  s.        with f
+00003aa0: 756e 6374 696f 6e73 2074 6861 7420 7461  unctions that ta
+00003ab0: 6b65 2061 206d 7574 6162 6c65 2072 6566  ke a mutable ref
+00003ac0: 6572 656e 6365 2074 6f20 7365 6c66 2e0a  erence to self..
+00003ad0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003ae0: 6465 6620 726c 2873 656c 6629 202d 3e20  def rl(self) -> 
+00003af0: 416e 793a 0a20 2020 2020 2020 2022 2222  Any:.        """
+00003b00: 0a20 2020 2020 2020 204f 7065 6e73 2075  .        Opens u
+00003b10: 7020 6120 7265 6164 206c 6f63 6b20 6f6e  p a read lock on
+00003b20: 2074 6865 2073 746f 7261 6765 2061 6e64   the storage and
+00003b30: 2072 6574 7572 6e73 2061 2067 7561 7264   returns a guard
+00003b40: 2068 616e 646c 652e 2055 7365 2074 6869   handle. Use thi
+00003b50: 730a 2020 2020 2020 2020 7769 7468 2066  s.        with f
+00003b60: 756e 6374 696f 6e73 2074 6861 7420 646f  unctions that do
+00003b70: 6e27 7420 7265 7175 6972 6520 6d75 7461  n't require muta
+00003b80: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
+00003b90: 220a 0a63 6c61 7373 205f 5f41 5049 5f52  "..class __API_R
+00003ba0: 6561 6479 3a0a 2020 2020 6465 6620 6873  eady:.    def hs
+00003bb0: 2873 656c 6629 202d 3e20 4f70 7469 6f6e  (self) -> Option
+00003bc0: 616c 5b22 4861 7264 5374 6174 6552 6566  al["HardStateRef
+00003bd0: 225d 3a0a 2020 2020 2020 2020 2222 220a  "]:.        """.
+00003be0: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
+00003bf0: 656e 7420 7374 6174 6520 6f66 2061 204e  ent state of a N
+00003c00: 6f64 6520 746f 2062 6520 7361 7665 6420  ode to be saved 
+00003c10: 746f 2073 7461 626c 6520 7374 6f72 6167  to stable storag
+00003c20: 652e 0a20 2020 2020 2020 2048 6172 6453  e..        HardS
+00003c30: 7461 7465 2077 696c 6c20 6265 204e 6f6e  tate will be Non
+00003c40: 6520 7374 6174 6520 6966 2074 6865 7265  e state if there
+00003c50: 2069 7320 6e6f 2075 7064 6174 652e 0a20   is no update.. 
+00003c60: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00003c70: 6566 2073 7328 7365 6c66 2920 2d3e 204f  ef ss(self) -> O
+00003c80: 7074 696f 6e61 6c5b 2253 6f66 7453 7461  ptional["SoftSta
+00003c90: 7465 5265 6622 5d3a 0a20 2020 2020 2020  teRef"]:.       
+00003ca0: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
+00003cb0: 2063 7572 7265 6e74 2076 6f6c 6174 696c   current volatil
+00003cc0: 6520 7374 6174 6520 6f66 2061 204e 6f64  e state of a Nod
+00003cd0: 652e 0a20 2020 2020 2020 2053 6f66 7453  e..        SoftS
+00003ce0: 7461 7465 2077 696c 6c20 6265 204e 6f6e  tate will be Non
+00003cf0: 6520 6966 2074 6865 7265 2069 7320 6e6f  e if there is no
+00003d00: 2075 7064 6174 652e 0a20 2020 2020 2020   update..       
+00003d10: 2049 7420 6973 206e 6f74 2072 6571 7569   It is not requi
+00003d20: 7265 6420 746f 2063 6f6e 7375 6d65 206f  red to consume o
+00003d30: 7220 7374 6f72 6520 536f 6674 5374 6174  r store SoftStat
+00003d40: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00003d50: 2020 2064 6566 206d 7573 745f 7379 6e63     def must_sync
+00003d60: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+00003d70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003d80: 2020 2020 4d75 7374 5379 6e63 2069 7320      MustSync is 
+00003d90: 6661 6c73 6520 6966 2061 6e64 206f 6e6c  false if and onl
+00003da0: 7920 6966 0a20 2020 2020 2020 2031 2e20  y if.        1. 
+00003db0: 6e6f 2048 6172 6453 7461 7465 206f 7220  no HardState or 
+00003dc0: 6f6e 6c79 2069 7473 2063 6f6d 6d69 7420  only its commit 
+00003dd0: 6973 2064 6966 6665 7265 6e74 2066 726f  is different fro
+00003de0: 6d20 6265 666f 7265 0a20 2020 2020 2020  m before.       
+00003df0: 2032 2e20 6e6f 2045 6e74 7269 6573 2061   2. no Entries a
+00003e00: 6e64 2053 6e61 7073 686f 740a 2020 2020  nd Snapshot.    
+00003e10: 2020 2020 4966 2069 7427 7320 6661 6c73      If it's fals
+00003e20: 652c 2061 6e20 6173 796e 6368 726f 6e6f  e, an asynchrono
+00003e30: 7573 2077 7269 7465 206f 6620 4861 7264  us write of Hard
+00003e40: 5374 6174 6520 6973 2070 6572 6d69 7373  State is permiss
+00003e50: 6962 6c65 2062 6566 6f72 6520 6361 6c6c  ible before call
+00003e60: 696e 670a 2020 2020 2020 2020 5b60 5261  ing.        [`Ra
+00003e70: 774e 6f64 653a 3a6f 6e5f 7065 7273 6973  wNode::on_persis
+00003e80: 745f 7265 6164 7960 5d20 6f72 205b 6052  t_ready`] or [`R
+00003e90: 6177 4e6f 6465 3a3a 6164 7661 6e63 6560  awNode::advance`
+00003ea0: 5d20 6f72 2069 7473 2066 616d 696c 6965  ] or its familie
+00003eb0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00003ec0: 2020 2064 6566 206e 756d 6265 7228 7365     def number(se
+00003ed0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00003ee0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00003ef0: 5468 6520 6e75 6d62 6572 206f 6620 6375  The number of cu
+00003f00: 7272 656e 7420 5265 6164 792e 0a20 2020  rrent Ready..   
+00003f10: 2020 2020 2049 7420 6973 2075 7365 6420       It is used 
+00003f20: 666f 7220 6964 656e 7469 6679 696e 6720  for identifying 
+00003f30: 7468 6520 6469 6666 6572 656e 7420 5265  the different Re
+00003f40: 6164 7920 616e 6420 5265 6164 7952 6563  ady and ReadyRec
+00003f50: 6f72 642e 0a20 2020 2020 2020 2022 2222  ord..        """
+00003f60: 0a20 2020 2064 6566 2073 6e61 7073 686f  .    def snapsho
+00003f70: 7428 7365 6c66 2920 2d3e 2022 536e 6170  t(self) -> "Snap
+00003f80: 7368 6f74 5265 6622 3a0a 2020 2020 2020  shotRef":.      
+00003f90: 2020 2222 220a 2020 2020 2020 2020 536e    """.        Sn
+00003fa0: 6170 7368 6f74 2073 7065 6369 6669 6573  apshot specifies
+00003fb0: 2074 6865 2073 6e61 7073 686f 7420 746f   the snapshot to
+00003fc0: 2062 6520 7361 7665 6420 746f 2073 7461   be saved to sta
+00003fd0: 626c 6520 7374 6f72 6167 652e 0a20 2020  ble storage..   
+00003fe0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00003ff0: 2063 6f6d 6d69 7474 6564 5f65 6e74 7269   committed_entri
+00004000: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
+00004010: 5b22 456e 7472 7952 6566 225d 3a0a 2020  ["EntryRef"]:.  
+00004020: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004030: 2020 436f 6d6d 6974 7465 6445 6e74 7269    CommittedEntri
+00004040: 6573 2073 7065 6369 6669 6573 2065 6e74  es specifies ent
+00004050: 7269 6573 2074 6f20 6265 2063 6f6d 6d69  ries to be commi
+00004060: 7474 6564 2074 6f20 610a 2020 2020 2020  tted to a.      
+00004070: 2020 7374 6f72 652f 7374 6174 652d 6d61    store/state-ma
+00004080: 6368 696e 652e 2054 6865 7365 2068 6176  chine. These hav
+00004090: 6520 7072 6576 696f 7573 6c79 2062 6565  e previously bee
+000040a0: 6e20 636f 6d6d 6974 7465 6420 746f 2073  n committed to s
+000040b0: 7461 626c 650a 2020 2020 2020 2020 7374  table.        st
+000040c0: 6f72 652e 0a20 2020 2020 2020 2022 2222  ore..        """
+000040d0: 0a20 2020 2064 6566 2074 616b 655f 636f  .    def take_co
+000040e0: 6d6d 6974 7465 645f 656e 7472 6965 7328  mmitted_entries(
+000040f0: 7365 6c66 2920 2d3e 204c 6973 745b 2245  self) -> List["E
+00004100: 6e74 7279 225d 3a0a 2020 2020 2020 2020  ntry"]:.        
+00004110: 2222 220a 2020 2020 2020 2020 5461 6b65  """.        Take
+00004120: 2074 6865 2043 6f6d 6d69 7445 6e74 7269   the CommitEntri
+00004130: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00004140: 2020 2020 6465 6620 656e 7472 6965 7328      def entries(
+00004150: 7365 6c66 2920 2d3e 204c 6973 745b 2245  self) -> List["E
+00004160: 6e74 7279 5265 6622 5d3a 0a20 2020 2020  ntryRef"]:.     
+00004170: 2020 2022 2222 0a20 2020 2020 2020 2045     """.        E
+00004180: 6e74 7269 6573 2073 7065 6369 6669 6573  ntries specifies
+00004190: 2065 6e74 7269 6573 2074 6f20 6265 2073   entries to be s
+000041a0: 6176 6564 2074 6f20 7374 6162 6c65 2073  aved to stable s
+000041b0: 746f 7261 6765 2e0a 2020 2020 2020 2020  torage..        
+000041c0: 2222 220a 2020 2020 6465 6620 7461 6b65  """.    def take
+000041d0: 5f65 6e74 7269 6573 2873 656c 6629 202d  _entries(self) -
+000041e0: 3e20 4c69 7374 5b22 456e 7472 7922 5d3a  > List["Entry"]:
+000041f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004200: 2020 2020 2054 616b 6520 7468 6520 456e       Take the En
+00004210: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
+00004220: 2222 0a20 2020 2064 6566 206d 6573 7361  "".    def messa
+00004230: 6765 7328 7365 6c66 2920 2d3e 204c 6973  ges(self) -> Lis
+00004240: 745b 224d 6573 7361 6765 5265 6622 5d3a  t["MessageRef"]:
+00004250: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004260: 2020 2020 204d 6573 7361 6765 7320 7370       Messages sp
+00004270: 6563 6966 6965 7320 6f75 7462 6f75 6e64  ecifies outbound
+00004280: 206d 6573 7361 6765 7320 746f 2062 6520   messages to be 
+00004290: 7365 6e74 2e0a 2020 2020 2020 2020 4966  sent..        If
+000042a0: 2069 7420 636f 6e74 6169 6e73 2061 204d   it contains a M
+000042b0: 7367 536e 6170 206d 6573 7361 6765 2c20  sgSnap message, 
+000042c0: 7468 6520 6170 706c 6963 6174 696f 6e20  the application 
+000042d0: 4d55 5354 2072 6570 6f72 7420 6261 636b  MUST report back
+000042e0: 2074 6f20 7261 6674 0a20 2020 2020 2020   to raft.       
+000042f0: 2077 6865 6e20 7468 6520 736e 6170 7368   when the snapsh
+00004300: 6f74 2068 6173 2062 6565 6e20 7265 6365  ot has been rece
+00004310: 6976 6564 206f 7220 6861 7320 6661 696c  ived or has fail
+00004320: 6564 2062 7920 6361 6c6c 696e 6720 5265  ed by calling Re
+00004330: 706f 7274 536e 6170 7368 6f74 2e0a 2020  portSnapshot..  
+00004340: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00004350: 6620 7461 6b65 5f6d 6573 7361 6765 7328  f take_messages(
+00004360: 7365 6c66 2920 2d3e 204c 6973 745b 224d  self) -> List["M
+00004370: 6573 7361 6765 225d 3a0a 2020 2020 2020  essage"]:.      
+00004380: 2020 2222 220a 2020 2020 2020 2020 5461    """.        Ta
+00004390: 6b65 2074 6865 204d 6573 7361 6765 732e  ke the Messages.
+000043a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000043b0: 2064 6566 2070 6572 7369 7374 6564 5f6d   def persisted_m
+000043c0: 6573 7361 6765 7328 7365 6c66 2920 2d3e  essages(self) ->
+000043d0: 204c 6973 745b 224d 6573 7361 6765 5265   List["MessageRe
+000043e0: 6622 5d3a 0a20 2020 2020 2020 2022 2222  f"]:.        """
+000043f0: 0a20 2020 2020 2020 2050 6572 7369 7374  .        Persist
+00004400: 6564 204d 6573 7361 6765 7320 7370 6563  ed Messages spec
+00004410: 6966 6965 7320 6f75 7462 6f75 6e64 206d  ifies outbound m
+00004420: 6573 7361 6765 7320 746f 2062 6520 7365  essages to be se
+00004430: 6e74 2041 4654 4552 2074 6865 2048 6172  nt AFTER the Har
+00004440: 6453 7461 7465 2c0a 2020 2020 2020 2020  dState,.        
+00004450: 456e 7472 6965 7320 616e 6420 536e 6170  Entries and Snap
+00004460: 7368 6f74 2061 7265 2070 6572 7369 7374  shot are persist
+00004470: 6564 2074 6f20 7374 6162 6c65 2073 746f  ed to stable sto
+00004480: 7261 6765 2e0a 2020 2020 2020 2020 2222  rage..        ""
+00004490: 220a 2020 2020 6465 6620 7461 6b65 5f70  ".    def take_p
+000044a0: 6572 7369 7374 6564 5f6d 6573 7361 6765  ersisted_message
+000044b0: 7328 7365 6c66 2920 2d3e 204c 6973 745b  s(self) -> List[
+000044c0: 224d 6573 7361 6765 225d 3a0a 2020 2020  "Message"]:.    
+000044d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000044e0: 5461 6b65 2074 6865 2050 6572 7369 7374  Take the Persist
+000044f0: 6564 204d 6573 7361 6765 732e 0a20 2020  ed Messages..   
+00004500: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00004510: 2072 6561 645f 7374 6174 6573 2873 656c   read_states(sel
+00004520: 6629 202d 3e20 4c69 7374 5b22 5265 6164  f) -> List["Read
+00004530: 5374 6174 6552 6566 225d 3a0a 2020 2020  StateRef"]:.    
+00004540: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004550: 5265 6164 5374 6174 6573 2073 7065 6369  ReadStates speci
+00004560: 6669 6573 2074 6865 2073 7461 7465 2066  fies the state f
+00004570: 6f72 2072 6561 6420 6f6e 6c79 2071 7565  or read only que
+00004580: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
+00004590: 2020 2020 6465 6620 7461 6b65 5f72 6561      def take_rea
+000045a0: 645f 7374 6174 6573 2873 656c 6629 202d  d_states(self) -
+000045b0: 3e20 4c69 7374 5b22 5265 6164 5374 6174  > List["ReadStat
+000045c0: 6522 5d3a 0a20 2020 2020 2020 2022 2222  e"]:.        """
+000045d0: 0a20 2020 2020 2020 2052 6561 6453 7461  .        ReadSta
+000045e0: 7465 7320 7370 6563 6966 6965 7320 7468  tes specifies th
+000045f0: 6520 7374 6174 6520 666f 7220 7265 6164  e state for read
+00004600: 206f 6e6c 7920 7175 6572 792e 0a20 2020   only query..   
+00004610: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
+00004620: 5265 6164 7928 5f5f 4150 495f 5265 6164  Ready(__API_Read
+00004630: 7929 3a0a 2020 2020 2222 220a 2020 2020  y):.    """.    
+00004640: 5265 6164 7920 656e 6361 7073 756c 6174  Ready encapsulat
+00004650: 6573 2074 6865 2065 6e74 7269 6573 2061  es the entries a
+00004660: 6e64 206d 6573 7361 6765 7320 7468 6174  nd messages that
+00004670: 2061 7265 2072 6561 6479 2074 6f20 7265   are ready to re
+00004680: 6164 2c0a 2020 2020 6265 2073 6176 6564  ad,.    be saved
+00004690: 2074 6f20 7374 6162 6c65 2073 746f 7261   to stable stora
+000046a0: 6765 2c20 636f 6d6d 6974 7465 6420 6f72  ge, committed or
+000046b0: 2073 656e 7420 746f 206f 7468 6572 2070   sent to other p
+000046c0: 6565 7273 2e0a 2020 2020 2222 220a 0a20  eers..    """.. 
+000046d0: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+000046e0: 7365 6c66 2920 2d3e 2022 5265 6164 7952  self) -> "ReadyR
+000046f0: 6566 223a 202e 2e2e 0a20 2020 2040 7374  ef": ....    @st
+00004700: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00004710: 6566 2064 6566 6175 6c74 2829 202d 3e20  ef default() -> 
+00004720: 2252 6561 6479 223a 202e 2e2e 0a0a 636c  "Ready": .....cl
+00004730: 6173 7320 5265 6164 7952 6566 285f 5f41  ass ReadyRef(__A
+00004740: 5049 5f52 6561 6479 293a 0a20 2020 2022  PI_Ready):.    "
+00004750: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
+00004760: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+00004770: 6052 6561 6479 602e 0a20 2020 2022 2222  `Ready`..    """
+00004780: 0a0a 636c 6173 7320 5f5f 4150 495f 5261  ..class __API_Ra
+00004790: 774e 6f64 653a 0a20 2020 2064 6566 2061  wNode:.    def a
+000047a0: 6476 616e 6365 5f61 7070 6c79 2873 656c  dvance_apply(sel
+000047b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+000047c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000047d0: 4164 7661 6e63 6520 6170 706c 7920 746f  Advance apply to
+000047e0: 2074 6865 2069 6e64 6578 206f 6620 7468   the index of th
+000047f0: 6520 6c61 7374 2063 6f6d 6d69 7474 6564  e last committed
+00004800: 2065 6e74 7269 6573 2067 6976 656e 2062   entries given b
+00004810: 6566 6f72 652e 0a20 2020 2020 2020 2022  efore..        "
+00004820: 2222 0a20 2020 2064 6566 2061 6476 616e  "".    def advan
+00004830: 6365 5f61 7070 6c79 5f74 6f28 7365 6c66  ce_apply_to(self
+00004840: 2c20 6170 706c 6965 643a 2069 6e74 2920  , applied: int) 
+00004850: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00004860: 2022 2222 0a20 2020 2020 2020 2041 6476   """.        Adv
+00004870: 616e 6365 2061 7070 6c79 2074 6f20 7468  ance apply to th
+00004880: 6520 7061 7373 6564 2069 6e64 6578 2e0a  e passed index..
+00004890: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000048a0: 6465 6620 6164 7661 6e63 6528 7365 6c66  def advance(self
+000048b0: 2c20 7264 3a20 2252 6561 6479 5265 6622  , rd: "ReadyRef"
+000048c0: 2920 2d3e 2022 4c69 6768 7452 6561 6479  ) -> "LightReady
+000048d0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+000048e0: 2020 2020 2020 2041 6476 616e 6365 7320         Advances 
+000048f0: 7468 6520 7265 6164 7920 6166 7465 7220  the ready after 
+00004900: 6675 6c6c 7920 7072 6f63 6573 7369 6e67  fully processing
+00004910: 2069 742e 0a0a 2020 2020 2020 2020 4675   it...        Fu
+00004920: 6c6c 7920 7072 6f63 6573 7369 6e67 2061  lly processing a
+00004930: 2072 6561 6479 2072 6571 7569 7265 7320   ready requires 
+00004940: 746f 2070 6572 7369 7374 2073 6e61 7073  to persist snaps
+00004950: 686f 742c 2065 6e74 7269 6573 2061 6e64  hot, entries and
+00004960: 2068 6172 6420 7374 6174 6573 2c20 6170   hard states, ap
+00004970: 706c 7920 616c 6c0a 2020 2020 2020 2020  ply all.        
+00004980: 636f 6d6d 6974 7465 6420 656e 7472 6965  committed entrie
+00004990: 732c 2073 656e 6420 616c 6c20 6d65 7373  s, send all mess
+000049a0: 6167 6573 2e0a 0a20 2020 2020 2020 2052  ages...        R
+000049b0: 6574 7572 6e73 2074 6865 204c 6967 6874  eturns the Light
+000049c0: 5265 6164 7920 7468 6174 2063 6f6e 7461  Ready that conta
+000049d0: 696e 7320 636f 6d6d 6974 2069 6e64 6578  ins commit index
+000049e0: 2c20 636f 6d6d 6974 7465 6420 656e 7472  , committed entr
+000049f0: 6965 7320 616e 6420 6d65 7373 6167 6573  ies and messages
+00004a00: 2e20 5b60 4c69 6768 7452 6561 6479 605d  . [`LightReady`]
+00004a10: 0a20 2020 2020 2020 2063 6f6e 7461 696e  .        contain
+00004a20: 7320 7570 6461 7465 7320 7468 6174 206f  s updates that o
+00004a30: 6e6c 7920 7661 6c69 6420 6166 7465 7220  nly valid after 
+00004a40: 7065 7273 6973 7469 6e67 206c 6173 7420  persisting last 
+00004a50: 7265 6164 792e 2049 7420 7368 6f75 6c64  ready. It should
+00004a60: 2061 6c73 6f20 6265 2066 756c 6c79 2070   also be fully p
+00004a70: 726f 6365 7373 6564 2e0a 2020 2020 2020  rocessed..      
+00004a80: 2020 5468 656e 205b 6053 656c 663a 3a61    Then [`Self::a
+00004a90: 6476 616e 6365 5f61 7070 6c79 605d 206f  dvance_apply`] o
+00004aa0: 7220 5b60 5365 6c66 3a3a 6164 7661 6e63  r [`Self::advanc
+00004ab0: 655f 6170 706c 795f 746f 605d 2073 686f  e_apply_to`] sho
+00004ac0: 756c 6420 6265 2075 7365 6420 6c61 7465  uld be used late
+00004ad0: 7220 746f 2075 7064 6174 6520 6170 706c  r to update appl
+00004ae0: 7969 6e67 0a20 2020 2020 2020 2070 726f  ying.        pro
+00004af0: 6772 6573 732e 0a20 2020 2020 2020 2022  gress..        "
+00004b00: 2222 0a20 2020 2064 6566 2061 6476 616e  "".    def advan
+00004b10: 6365 5f61 7070 656e 6428 7365 6c66 2c20  ce_append(self, 
+00004b20: 7264 3a20 2252 6561 6479 5265 6622 2920  rd: "ReadyRef") 
+00004b30: 2d3e 2022 4c69 6768 7452 6561 6479 223a  -> "LightReady":
+00004b40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00004b50: 2020 2020 2041 6476 616e 6365 7320 7468       Advances th
+00004b60: 6520 7265 6164 7920 7769 7468 6f75 7420  e ready without 
+00004b70: 6170 706c 7969 6e67 2063 6f6d 6d69 7474  applying committ
+00004b80: 6564 2065 6e74 7269 6573 2e20 5b60 5365  ed entries. [`Se
+00004b90: 6c66 3a3a 6164 7661 6e63 655f 6170 706c  lf::advance_appl
+00004ba0: 7960 5d20 6f72 0a20 2020 2020 2020 205b  y`] or.        [
+00004bb0: 6053 656c 663a 3a61 6476 616e 6365 5f61  `Self::advance_a
+00004bc0: 7070 6c79 5f74 6f60 5d20 7368 6f75 6c64  pply_to`] should
+00004bd0: 2062 6520 7573 6564 206c 6174 6572 2074   be used later t
+00004be0: 6f20 7570 6461 7465 2061 7070 6c79 696e  o update applyin
+00004bf0: 6720 7072 6f67 7265 7373 2e0a 0a20 2020  g progress...   
+00004c00: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
+00004c10: 204c 6967 6874 5265 6164 7920 7468 6174   LightReady that
+00004c20: 2063 6f6e 7461 696e 7320 636f 6d6d 6974   contains commit
+00004c30: 2069 6e64 6578 2c20 636f 6d6d 6974 7465   index, committe
+00004c40: 6420 656e 7472 6965 7320 616e 6420 6d65  d entries and me
+00004c50: 7373 6167 6573 2e0a 0a20 2020 2020 2020  ssages...       
+00004c60: 2053 696e 6365 2052 6561 6479 206d 7573   Since Ready mus
+00004c70: 7420 6265 2070 6572 7369 7374 6564 2069  t be persisted i
+00004c80: 6e20 6f72 6465 722c 2063 616c 6c69 6e67  n order, calling
+00004c90: 2074 6869 7320 6675 6e63 7469 6f6e 2069   this function i
+00004ca0: 6d70 6c69 6369 746c 7920 6d65 616e 730a  mplicitly means.
+00004cb0: 2020 2020 2020 2020 616c 6c20 7265 6164          all read
+00004cc0: 7920 636f 6c6c 6563 7465 6420 6265 666f  y collected befo
+00004cd0: 7265 2068 6176 6520 6265 656e 2070 6572  re have been per
+00004ce0: 7369 7374 6564 2e0a 2020 2020 2020 2020  sisted..        
+00004cf0: 2222 220a 2020 2020 6465 6620 6164 7661  """.    def adva
+00004d00: 6e63 655f 6170 7065 6e64 5f61 7379 6e63  nce_append_async
+00004d10: 2873 656c 662c 2072 643a 2022 5265 6164  (self, rd: "Read
+00004d20: 7952 6566 2229 202d 3e20 4e6f 6e65 3a0a  yRef") -> None:.
+00004d30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00004d40: 2020 2020 5361 6d65 2061 7320 5b60 5365      Same as [`Se
+00004d50: 6c66 3a3a 6164 7661 6e63 655f 6170 7065  lf::advance_appe
+00004d60: 6e64 605d 2065 7863 6570 7420 7468 6174  nd`] except that
+00004d70: 2069 7420 616c 6c6f 7773 2074 6f20 6f6e   it allows to on
+00004d80: 6c79 2073 746f 7265 2074 6865 2075 7064  ly store the upd
+00004d90: 6174 6573 2069 6e20 6361 6368 652e 0a20  ates in cache.. 
+00004da0: 2020 2020 2020 205b 6053 656c 663a 3a6f         [`Self::o
+00004db0: 6e5f 7065 7273 6973 745f 7265 6164 7960  n_persist_ready`
+00004dc0: 5d20 7368 6f75 6c64 2062 6520 7573 6564  ] should be used
+00004dd0: 206c 6174 6572 2074 6f20 7570 6461 7465   later to update
+00004de0: 2074 6865 2070 6572 7369 7374 696e 6720   the persisting 
+00004df0: 7072 6f67 7265 7373 2e0a 0a20 2020 2020  progress...     
+00004e00: 2020 2052 6166 7420 776f 726b 7320 6f6e     Raft works on
+00004e10: 2061 6e20 6173 7375 6d70 7469 6f6e 2070   an assumption p
+00004e20: 6572 7369 7374 6564 2075 7064 6174 6573  ersisted updates
+00004e30: 2073 686f 756c 6420 6e6f 7420 6265 206c   should not be l
+00004e40: 6f73 742c 2077 6869 6368 2075 7375 616c  ost, which usual
+00004e50: 6c79 2072 6571 7569 7265 7320 6578 7065  ly requires expe
+00004e60: 6e73 6976 650a 2020 2020 2020 2020 6f70  nsive.        op
+00004e70: 6572 6174 696f 6e73 206c 696b 6520 6066  erations like `f
+00004e80: 7379 6e63 602e 2060 6164 7661 6e63 655f  sync`. `advance_
+00004e90: 6170 7065 6e64 5f61 7379 6e63 6020 616c  append_async` al
+00004ea0: 6c6f 7773 2079 6f75 2074 6f20 636f 6e74  lows you to cont
+00004eb0: 726f 6c20 7468 6520 7261 7465 206f 6620  rol the rate of 
+00004ec0: 7375 6368 206f 7065 7261 7469 6f6e 7320  such operations 
+00004ed0: 616e 640a 2020 2020 2020 2020 6765 7420  and.        get 
+00004ee0: 6120 7265 6173 6f6e 6162 6c65 2062 6174  a reasonable bat
+00004ef0: 6368 2073 697a 652e 2048 6f77 6576 6572  ch size. However
+00004f00: 2c20 6974 2773 2073 7469 6c6c 2072 6571  , it's still req
+00004f10: 7569 7265 6420 7468 6174 2074 6865 2075  uired that the u
+00004f20: 7064 6174 6573 2063 616e 2062 6520 7265  pdates can be re
+00004f30: 6164 2062 7920 7261 6674 2066 726f 6d20  ad by raft from 
+00004f40: 7468 650a 2020 2020 2020 2020 6053 746f  the.        `Sto
+00004f50: 7261 6765 6020 7472 6169 7420 6265 666f  rage` trait befo
+00004f60: 7265 2063 616c 6c69 6e67 2060 6164 7661  re calling `adva
+00004f70: 6e63 655f 6170 7065 6e64 5f61 7379 6e63  nce_append_async
+00004f80: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
+00004f90: 2020 2064 6566 2068 6173 5f72 6561 6479     def has_ready
+00004fa0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+00004fb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00004fc0: 2020 2020 4861 7352 6561 6479 2063 616c      HasReady cal
+00004fd0: 6c65 6420 7768 656e 2052 6177 4e6f 6465  led when RawNode
+00004fe0: 2075 7365 7220 6e65 6564 2074 6f20 6368   user need to ch
+00004ff0: 6563 6b20 6966 2061 6e79 2052 6561 6479  eck if any Ready
+00005000: 2070 656e 6469 6e67 2e0a 2020 2020 2020   pending..      
+00005010: 2020 2222 220a 2020 2020 6465 6620 7469    """.    def ti
+00005020: 636b 2873 656c 6629 202d 3e20 626f 6f6c  ck(self) -> bool
+00005030: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00005040: 2020 2020 2020 5469 636b 2061 6476 616e        Tick advan
+00005050: 6365 7320 7468 6520 696e 7465 726e 616c  ces the internal
+00005060: 206c 6f67 6963 616c 2063 6c6f 636b 2062   logical clock b
+00005070: 7920 6120 7369 6e67 6c65 2074 6963 6b2e  y a single tick.
+00005080: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00005090: 7320 7472 7565 2074 6f20 696e 6469 6361  s true to indica
+000050a0: 7465 2074 6861 7420 7468 6572 6520 7769  te that there wi
+000050b0: 6c6c 2070 726f 6261 626c 7920 6265 2073  ll probably be s
+000050c0: 6f6d 6520 7265 6164 696e 6573 7320 7768  ome readiness wh
+000050d0: 6963 680a 2020 2020 2020 2020 6e65 6564  ich.        need
+000050e0: 7320 746f 2062 6520 6861 6e64 6c65 642e  s to be handled.
+000050f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005100: 2064 6566 2073 6574 5f62 6174 6368 5f61   def set_batch_a
+00005110: 7070 656e 6428 7365 6c66 2c20 6261 7463  ppend(self, batc
+00005120: 685f 6170 7065 6e64 3a20 626f 6f6c 2920  h_append: bool) 
+00005130: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00005140: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+00005150: 2077 6865 7468 6572 2074 6f20 6261 7463   whether to batc
+00005160: 6820 6170 7065 6e64 206d 7367 2061 7420  h append msg at 
+00005170: 7275 6e74 696d 652e 0a20 2020 2020 2020  runtime..       
+00005180: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00005190: 5f70 7269 6f72 6974 7928 7365 6c66 2c20  _priority(self, 
+000051a0: 7072 696f 7269 7479 3a20 696e 7429 202d  priority: int) -
+000051b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000051c0: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
+000051d0: 2070 7269 6f72 6974 7920 6f66 206e 6f64   priority of nod
+000051e0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+000051f0: 2020 2064 6566 2072 6570 6f72 745f 736e     def report_sn
+00005200: 6170 7368 6f74 2873 656c 662c 2069 643a  apshot(self, id:
+00005210: 2069 6e74 2c20 736e 6170 7368 6f74 3a20   int, snapshot: 
+00005220: 2253 6e61 7073 686f 7453 7461 7475 7322  "SnapshotStatus"
+00005230: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00005240: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00005250: 6570 6f72 7453 6e61 7073 686f 7420 7265  eportSnapshot re
+00005260: 706f 7274 7320 7468 6520 7374 6174 7573  ports the status
+00005270: 206f 6620 7468 6520 7365 6e74 2073 6e61   of the sent sna
+00005280: 7073 686f 742e 0a20 2020 2020 2020 2022  pshot..        "
+00005290: 2222 0a20 2020 2064 6566 2072 6570 6f72  "".    def repor
+000052a0: 745f 756e 7265 6163 6861 626c 6528 7365  t_unreachable(se
+000052b0: 6c66 2c20 6964 3a20 696e 7429 202d 3e20  lf, id: int) -> 
+000052c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000052d0: 220a 2020 2020 2020 2020 5265 706f 7274  ".        Report
+000052e0: 556e 7265 6163 6861 626c 6520 7265 706f  Unreachable repo
+000052f0: 7274 7320 7468 6520 6769 7665 6e20 6e6f  rts the given no
+00005300: 6465 2069 7320 6e6f 7420 7265 6163 6861  de is not reacha
+00005310: 626c 6520 666f 7220 7468 6520 6c61 7374  ble for the last
+00005320: 2073 656e 642e 0a20 2020 2020 2020 2022   send..        "
+00005330: 2222 0a20 2020 2064 6566 2074 7261 6e73  "".    def trans
+00005340: 6665 725f 6c65 6164 6572 2873 656c 662c  fer_leader(self,
+00005350: 2074 7261 6e73 6665 7265 653a 2069 6e74   transferee: int
+00005360: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00005370: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
+00005380: 7261 6e73 6665 724c 6561 6465 7220 7472  ransferLeader tr
+00005390: 6965 7320 746f 2074 7261 6e73 6665 7220  ies to transfer 
+000053a0: 6c65 6164 6572 7368 6970 2074 6f20 7468  leadership to th
+000053b0: 6520 6769 7665 6e20 7472 616e 7366 6572  e given transfer
+000053c0: 6565 2e0a 2020 2020 2020 2020 2222 220a  ee..        """.
+000053d0: 2020 2020 6465 6620 736e 6170 2873 656c      def snap(sel
+000053e0: 6629 202d 3e20 4f70 7469 6f6e 616c 5b22  f) -> Optional["
+000053f0: 536e 6170 7368 6f74 5265 6622 5d3a 0a20  SnapshotRef"]:. 
+00005400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005410: 2020 2047 7261 6273 2074 6865 2073 6e61     Grabs the sna
+00005420: 7073 686f 7420 6672 6f6d 2074 6865 2072  pshot from the r
+00005430: 6166 7420 6966 2061 7661 696c 6162 6c65  aft if available
+00005440: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00005450: 2020 6465 6620 7374 6570 2873 656c 662c    def step(self,
+00005460: 206d 7367 3a20 224d 6573 7361 6765 2220   msg: "Message" 
+00005470: 7c20 224d 6573 7361 6765 5265 6622 2920  | "MessageRef") 
+00005480: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00005490: 2022 2222 0a20 2020 2020 2020 2053 7465   """.        Ste
+000054a0: 7020 6164 7661 6e63 6573 2074 6865 2073  p advances the s
+000054b0: 7461 7465 206d 6163 6869 6e65 2075 7369  tate machine usi
+000054c0: 6e67 2074 6865 2067 6976 656e 206d 6573  ng the given mes
+000054d0: 7361 6765 2e0a 2020 2020 2020 2020 2222  sage..        ""
+000054e0: 220a 2020 2020 6465 6620 736b 6970 5f62  ".    def skip_b
+000054f0: 6361 7374 5f63 6f6d 6d69 7428 7365 6c66  cast_commit(self
+00005500: 2c20 736b 6970 3a20 626f 6f6c 2920 2d3e  , skip: bool) ->
+00005510: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00005520: 2222 0a20 2020 2020 2020 2053 6574 2077  "".        Set w
+00005530: 6865 7468 6572 2073 6b69 7020 6272 6f61  hether skip broa
+00005540: 6463 6173 7420 656d 7074 7920 636f 6d6d  dcast empty comm
+00005550: 6974 206d 6573 7361 6765 7320 6174 2072  it messages at r
+00005560: 756e 7469 6d65 2e0a 2020 2020 2020 2020  untime..        
+00005570: 2222 220a 2020 2020 6465 6620 6361 6d70  """.    def camp
+00005580: 6169 676e 2873 656c 6629 202d 3e20 4e6f  aign(self) -> No
+00005590: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+000055a0: 2020 2020 2020 2020 4361 6d70 6169 676e          Campaign
+000055b0: 2063 6175 7365 7320 7468 6973 2052 6177   causes this Raw
+000055c0: 4e6f 6465 2074 6f20 7472 616e 7369 7469  Node to transiti
+000055d0: 6f6e 2074 6f20 6361 6e64 6964 6174 6520  on to candidate 
+000055e0: 7374 6174 652e 0a20 2020 2020 2020 2022  state..        "
+000055f0: 2222 0a20 2020 2064 6566 2070 726f 706f  "".    def propo
+00005600: 7365 2873 656c 662c 2063 6f6e 7465 7874  se(self, context
+00005610: 3a20 6279 7465 732c 2064 6174 613a 2062  : bytes, data: b
+00005620: 7974 6573 2920 2d3e 204e 6f6e 653a 0a20  ytes) -> None:. 
+00005630: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005640: 2020 2050 726f 706f 7365 2070 726f 706f     Propose propo
+00005650: 7365 7320 6461 7461 2062 6520 6170 7065  ses data be appe
+00005660: 6e64 6564 2074 6f20 7468 6520 7261 6674  nded to the raft
+00005670: 206c 6f67 2e0a 2020 2020 2020 2020 2222   log..        ""
+00005680: 220a 2020 2020 6465 6620 7072 6f70 6f73  ".    def propos
+00005690: 655f 636f 6e66 5f63 6861 6e67 6528 0a20  e_conf_change(. 
+000056a0: 2020 2020 2020 2073 656c 662c 2063 6f6e         self, con
+000056b0: 7465 7874 3a20 6279 7465 732c 2063 633a  text: bytes, cc:
+000056c0: 2022 436f 6e66 4368 616e 6765 2220 7c20   "ConfChange" | 
+000056d0: 2243 6f6e 6643 6861 6e67 6552 6566 220a  "ConfChangeRef".
+000056e0: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+000056f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005700: 2020 2050 726f 706f 7365 436f 6e66 4368     ProposeConfCh
+00005710: 616e 6765 2070 726f 706f 7365 7320 6120  ange proposes a 
+00005720: 636f 6e66 6967 2063 6861 6e67 652e 0a0a  config change...
+00005730: 2020 2020 2020 2020 4966 2074 6865 206e          If the n
+00005740: 6f64 6520 656e 7465 7273 206a 6f69 6e74  ode enters joint
+00005750: 2073 7461 7465 2077 6974 6820 6061 7574   state with `aut
+00005760: 6f5f 6c65 6176 6560 2073 6574 2074 6f20  o_leave` set to 
+00005770: 7472 7565 2c20 6974 2773 0a20 2020 2020  true, it's.     
+00005780: 2020 2063 616c 6c65 7227 7320 7265 7370     caller's resp
+00005790: 6f6e 7369 6269 6c69 7479 2074 6f20 7072  onsibility to pr
+000057a0: 6f70 6f73 6520 616e 2065 6d70 7479 2063  opose an empty c
+000057b0: 6f6e 6620 6368 616e 6765 2061 6761 696e  onf change again
+000057c0: 2074 6f20 666f 7263 650a 2020 2020 2020   to force.      
+000057d0: 2020 6c65 6176 696e 6720 6a6f 696e 7420    leaving joint 
+000057e0: 7374 6174 652e 0a20 2020 2020 2020 2022  state..        "
+000057f0: 2222 0a20 2020 2064 6566 2070 726f 706f  "".    def propo
+00005800: 7365 5f63 6f6e 665f 6368 616e 6765 5f76  se_conf_change_v
+00005810: 3228 0a20 2020 2020 2020 2073 656c 662c  2(.        self,
+00005820: 2063 6f6e 7465 7874 3a20 6279 7465 732c   context: bytes,
+00005830: 2063 633a 2022 436f 6e66 4368 616e 6765   cc: "ConfChange
+00005840: 5632 2220 7c20 2243 6f6e 6643 6861 6e67  V2" | "ConfChang
+00005850: 6556 3252 6566 220a 2020 2020 2920 2d3e  eV2Ref".    ) ->
+00005860: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00005870: 2222 0a20 2020 2020 2020 2050 726f 706f  "".        Propo
+00005880: 7365 436f 6e66 4368 616e 6765 2070 726f  seConfChange pro
+00005890: 706f 7365 7320 6120 636f 6e66 6967 2063  poses a config c
+000058a0: 6861 6e67 652e 0a0a 2020 2020 2020 2020  hange...        
+000058b0: 4966 2074 6865 206e 6f64 6520 656e 7465  If the node ente
+000058c0: 7273 206a 6f69 6e74 2073 7461 7465 2077  rs joint state w
+000058d0: 6974 6820 6061 7574 6f5f 6c65 6176 6560  ith `auto_leave`
+000058e0: 2073 6574 2074 6f20 7472 7565 2c20 6974   set to true, it
+000058f0: 2773 0a20 2020 2020 2020 2063 616c 6c65  's.        calle
+00005900: 7227 7320 7265 7370 6f6e 7369 6269 6c69  r's responsibili
+00005910: 7479 2074 6f20 7072 6f70 6f73 6520 616e  ty to propose an
+00005920: 2065 6d70 7479 2063 6f6e 6620 6368 616e   empty conf chan
+00005930: 6765 2061 6761 696e 2074 6f20 666f 7263  ge again to forc
+00005940: 650a 2020 2020 2020 2020 6c65 6176 696e  e.        leavin
+00005950: 6720 6a6f 696e 7420 7374 6174 652e 0a20  g joint state.. 
+00005960: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00005970: 6566 2061 7070 6c79 5f63 6f6e 665f 6368  ef apply_conf_ch
+00005980: 616e 6765 2873 656c 662c 2063 633a 2022  ange(self, cc: "
+00005990: 436f 6e66 4368 616e 6765 2220 7c20 2243  ConfChange" | "C
+000059a0: 6f6e 6643 6861 6e67 6552 6566 2229 202d  onfChangeRef") -
+000059b0: 3e20 436f 6e66 5374 6174 653a 0a20 2020  > ConfState:.   
+000059c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000059d0: 2041 7070 6c69 6573 2061 2063 6f6e 6669   Applies a confi
+000059e0: 6720 6368 616e 6765 2074 6f20 7468 6520  g change to the 
+000059f0: 6c6f 6361 6c20 6e6f 6465 2e20 5468 6520  local node. The 
+00005a00: 6170 7020 6d75 7374 2063 616c 6c20 7468  app must call th
+00005a10: 6973 2077 6865 6e20 6974 0a20 2020 2020  is when it.     
+00005a20: 2020 2061 7070 6c69 6573 2061 2063 6f6e     applies a con
+00005a30: 6669 6775 7261 7469 6f6e 2063 6861 6e67  figuration chang
+00005a40: 652c 2065 7863 6570 7420 7768 656e 2069  e, except when i
+00005a50: 7420 6465 6369 6465 7320 746f 2072 656a  t decides to rej
+00005a60: 6563 7420 7468 650a 2020 2020 2020 2020  ect the.        
+00005a70: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
+00005a80: 616e 6765 2c20 696e 2077 6869 6368 2063  ange, in which c
+00005a90: 6173 6520 6e6f 2063 616c 6c20 6d75 7374  ase no call must
+00005aa0: 2074 616b 6520 706c 6163 652e 0a20 2020   take place..   
+00005ab0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00005ac0: 2061 7070 6c79 5f63 6f6e 665f 6368 616e   apply_conf_chan
+00005ad0: 6765 5f76 3228 0a20 2020 2020 2020 2073  ge_v2(.        s
+00005ae0: 656c 662c 2063 633a 2022 436f 6e66 4368  elf, cc: "ConfCh
+00005af0: 616e 6765 5632 2220 7c20 2243 6f6e 6643  angeV2" | "ConfC
+00005b00: 6861 6e67 6556 3252 6566 220a 2020 2020  hangeV2Ref".    
+00005b10: 2920 2d3e 2022 436f 6e66 5374 6174 6522  ) -> "ConfState"
+00005b20: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00005b30: 2020 2020 2020 4170 706c 6965 7320 6120        Applies a 
+00005b40: 636f 6e66 6967 2063 6861 6e67 6520 746f  config change to
+00005b50: 2074 6865 206c 6f63 616c 206e 6f64 652e   the local node.
+00005b60: 2054 6865 2061 7070 206d 7573 7420 6361   The app must ca
+00005b70: 6c6c 2074 6869 7320 7768 656e 2069 740a  ll this when it.
+00005b80: 2020 2020 2020 2020 6170 706c 6965 7320          applies 
+00005b90: 6120 636f 6e66 6967 7572 6174 696f 6e20  a configuration 
+00005ba0: 6368 616e 6765 2c20 6578 6365 7074 2077  change, except w
+00005bb0: 6865 6e20 6974 2064 6563 6964 6573 2074  hen it decides t
+00005bc0: 6f20 7265 6a65 6374 2074 6865 0a20 2020  o reject the.   
+00005bd0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+00005be0: 6f6e 2063 6861 6e67 652c 2069 6e20 7768  on change, in wh
+00005bf0: 6963 6820 6361 7365 206e 6f20 6361 6c6c  ich case no call
+00005c00: 206d 7573 7420 7461 6b65 2070 6c61 6365   must take place
+00005c10: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00005c20: 2020 6465 6620 7069 6e67 2873 656c 6629    def ping(self)
+00005c30: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00005c40: 2020 2222 220a 2020 2020 2020 2020 4272    """.        Br
+00005c50: 6f61 6463 6173 7420 6865 6172 7462 6561  oadcast heartbea
+00005c60: 7473 2074 6f20 616c 6c20 7468 6520 666f  ts to all the fo
+00005c70: 6c6c 6f77 6572 732e 0a0a 2020 2020 2020  llowers...      
+00005c80: 2020 4966 2069 7427 7320 6e6f 7420 6c65    If it's not le
+00005c90: 6164 6572 2c20 6e6f 7468 696e 6720 7769  ader, nothing wi
+00005ca0: 6c6c 2068 6170 7065 6e2e 0a20 2020 2020  ll happen..     
+00005cb0: 2020 2022 2222 0a20 2020 2064 6566 206f     """.    def o
+00005cc0: 6e5f 7065 7273 6973 745f 7265 6164 7928  n_persist_ready(
+00005cd0: 7365 6c66 2c20 6e75 6d62 6572 3a20 696e  self, number: in
+00005ce0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+00005cf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005d00: 4e6f 7469 6669 6573 2074 6861 7420 7468  Notifies that th
+00005d10: 6520 7265 6164 7920 6f66 2074 6869 7320  e ready of this 
+00005d20: 6e75 6d62 6572 2068 6173 2062 6565 6e20  number has been 
+00005d30: 7065 7273 6973 7465 642e 0a0a 2020 2020  persisted...    
+00005d40: 2020 2020 5369 6e63 6520 5265 6164 7920      Since Ready 
+00005d50: 6d75 7374 2062 6520 7065 7273 6973 7465  must be persiste
+00005d60: 6420 696e 206f 7264 6572 2c20 6361 6c6c  d in order, call
+00005d70: 696e 6720 7468 6973 2066 756e 6374 696f  ing this functio
+00005d80: 6e20 696d 706c 6963 6974 6c79 206d 6561  n implicitly mea
+00005d90: 6e73 0a20 2020 2020 2020 2061 6c6c 2072  ns.        all r
+00005da0: 6561 6469 6573 2077 6974 6820 6e75 6d62  eadies with numb
+00005db0: 6572 7320 736d 616c 6c65 7220 7468 616e  ers smaller than
+00005dc0: 2074 6869 7320 6f6e 6520 6861 7665 2062   this one have b
+00005dd0: 6565 6e20 7065 7273 6973 7465 642e 0a0a  een persisted...
+00005de0: 2020 2020 2020 2020 5b60 5365 6c66 3a3a          [`Self::
+00005df0: 6861 735f 7265 6164 7960 5d20 616e 6420  has_ready`] and 
+00005e00: 5b60 5365 6c66 3a3a 7265 6164 7960 5d20  [`Self::ready`] 
+00005e10: 7368 6f75 6c64 2062 6520 6361 6c6c 6564  should be called
+00005e20: 206c 6174 6572 2074 6f20 6861 6e64 6c65   later to handle
+00005e30: 2066 7572 7468 6572 0a20 2020 2020 2020   further.       
+00005e40: 2075 7064 6174 6573 2074 6861 7420 6265   updates that be
+00005e50: 636f 6d65 2076 616c 6964 2061 6674 6572  come valid after
+00005e60: 2072 6561 6479 2062 6569 6e67 2070 6572   ready being per
+00005e70: 7369 7374 6564 2e0a 2020 2020 2020 2020  sisted..        
+00005e80: 2222 220a 2020 2020 6465 6620 7265 6164  """.    def read
+00005e90: 5f69 6e64 6578 2873 656c 662c 2072 6374  _index(self, rct
+00005ea0: 783a 2062 7974 6573 2920 2d3e 204e 6f6e  x: bytes) -> Non
+00005eb0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00005ec0: 2020 2020 2020 2052 6561 6449 6e64 6578         ReadIndex
+00005ed0: 2072 6571 7565 7374 7320 6120 7265 6164   requests a read
+00005ee0: 2073 7461 7465 2e20 5468 6520 7265 6164   state. The read
+00005ef0: 2073 7461 7465 2077 696c 6c20 6265 2073   state will be s
+00005f00: 6574 2069 6e20 7265 6164 792e 0a20 2020  et in ready..   
+00005f10: 2020 2020 2052 6561 6420 5374 6174 6520       Read State 
+00005f20: 6861 7320 6120 7265 6164 2069 6e64 6578  has a read index
+00005f30: 2e20 4f6e 6365 2074 6865 2061 7070 6c69  . Once the appli
+00005f40: 6361 7469 6f6e 2061 6476 616e 6365 7320  cation advances 
+00005f50: 6675 7274 6865 7220 7468 616e 2074 6865  further than the
+00005f60: 2072 6561 640a 2020 2020 2020 2020 696e   read.        in
+00005f70: 6465 782c 2061 6e79 206c 696e 6561 7269  dex, any lineari
+00005f80: 7a61 626c 6520 7265 6164 2072 6571 7565  zable read reque
+00005f90: 7374 7320 6973 7375 6564 2062 6566 6f72  sts issued befor
+00005fa0: 6520 7468 6520 7265 6164 2072 6571 7565  e the read reque
+00005fb0: 7374 2063 616e 2062 650a 2020 2020 2020  st can be.      
+00005fc0: 2020 7072 6f63 6573 7365 6420 7361 6665    processed safe
+00005fd0: 6c79 2e20 5468 6520 7265 6164 2073 7461  ly. The read sta
+00005fe0: 7465 2077 696c 6c20 6861 7665 2074 6865  te will have the
+00005ff0: 2073 616d 6520 7263 7478 2061 7474 6163   same rctx attac
+00006000: 6865 642e 0a20 2020 2020 2020 2022 2222  hed..        """
+00006010: 0a20 2020 2064 6566 2072 6561 6479 2873  .    def ready(s
+00006020: 656c 6629 202d 3e20 5265 6164 793a 0a20  elf) -> Ready:. 
+00006030: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006040: 2020 2052 6574 7572 6e73 2074 6865 206f     Returns the o
+00006050: 7574 7374 616e 6469 6e67 2077 6f72 6b20  utstanding work 
+00006060: 7468 6174 2074 6865 2061 7070 6c69 6361  that the applica
+00006070: 7469 6f6e 206e 6565 6473 2074 6f20 6861  tion needs to ha
+00006080: 6e64 6c65 2e0a 0a20 2020 2020 2020 2054  ndle...        T
+00006090: 6869 7320 696e 636c 7564 6573 2061 7070  his includes app
+000060a0: 656e 6469 6e67 2061 6e64 2061 7070 6c79  ending and apply
+000060b0: 696e 6720 656e 7472 6965 7320 6f72 2061  ing entries or a
+000060c0: 2073 6e61 7073 686f 742c 2075 7064 6174   snapshot, updat
+000060d0: 696e 6720 7468 6520 4861 7264 5374 6174  ing the HardStat
+000060e0: 652c 0a20 2020 2020 2020 2061 6e64 2073  e,.        and s
+000060f0: 656e 6469 6e67 206d 6573 7361 6765 732e  ending messages.
+00006100: 2054 6865 2072 6574 7572 6e65 6420 6052   The returned `R
+00006110: 6561 6479 6020 2a4d 5553 542a 2062 6520  eady` *MUST* be 
+00006120: 6861 6e64 6c65 6420 616e 6420 7375 6273  handled and subs
+00006130: 6571 7565 6e74 6c79 0a20 2020 2020 2020  equently.       
+00006140: 2070 6173 7365 6420 6261 636b 2076 6961   passed back via
+00006150: 2060 6164 7661 6e63 6560 206f 7220 6974   `advance` or it
+00006160: 7320 6661 6d69 6c69 6573 2e20 4265 666f  s families. Befo
+00006170: 7265 2074 6861 742c 202a 444f 204e 4f54  re that, *DO NOT
+00006180: 2a20 6361 6c6c 2061 6e79 2066 756e 6374  * call any funct
+00006190: 696f 6e20 6c69 6b65 0a20 2020 2020 2020  ion like.       
+000061a0: 2060 7374 6570 602c 2060 7072 6f70 6f73   `step`, `propos
+000061b0: 6560 2c20 6063 616d 7061 6967 6e60 2074  e`, `campaign` t
+000061c0: 6f20 6368 616e 6765 2069 6e74 6572 6e61  o change interna
+000061d0: 6c20 7374 6174 652e 0a0a 2020 2020 2020  l state...      
+000061e0: 2020 5b60 5365 6c66 3a3a 6861 735f 7265    [`Self::has_re
+000061f0: 6164 7960 5d20 7368 6f75 6c64 2062 6520  ady`] should be 
+00006200: 6361 6c6c 6564 2066 6972 7374 2074 6f20  called first to 
+00006210: 6368 6563 6b20 6966 2069 7427 7320 6e65  check if it's ne
+00006220: 6365 7373 6172 7920 746f 2068 616e 646c  cessary to handl
+00006230: 6520 7468 6520 7265 6164 792e 0a20 2020  e the ready..   
+00006240: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00006250: 2072 6571 7565 7374 5f73 6e61 7073 686f   request_snapsho
+00006260: 7428 7365 6c66 2920 2d3e 2022 5265 6164  t(self) -> "Read
+00006270: 7922 3a0a 2020 2020 2020 2020 2222 220a  y":.        """.
+00006280: 2020 2020 2020 2020 5265 7175 6573 7420          Request 
+00006290: 6120 736e 6170 7368 6f74 2066 726f 6d20  a snapshot from 
+000062a0: 6120 6c65 6164 6572 2e0a 2020 2020 2020  a leader..      
+000062b0: 2020 5468 6520 736e 6170 7368 6f74 2773    The snapshot's
+000062c0: 2069 6e64 6578 206d 7573 7420 6265 2067   index must be g
+000062d0: 7265 6174 6572 206f 7220 6571 7561 6c20  reater or equal 
+000062e0: 746f 2074 6865 2072 6571 7565 7374 5f69  to the request_i
+000062f0: 6e64 6578 2028 6c61 7374 5f69 6e64 6578  ndex (last_index
+00006300: 2920 6f72 0a20 2020 2020 2020 2074 6865  ) or.        the
+00006310: 206c 6561 6465 7227 7320 7465 726d 206d   leader's term m
+00006320: 7573 7420 6265 2067 7265 6174 6572 2074  ust be greater t
+00006330: 6861 6e20 7468 6520 7265 7175 6573 7420  han the request 
+00006340: 7465 726d 2028 6c61 7374 5f69 6e64 6578  term (last_index
+00006350: 2773 2074 6572 6d29 2e0a 2020 2020 2020  's term)..      
+00006360: 2020 2222 220a 2020 2020 6465 6620 6f6e    """.    def on
+00006370: 5f65 6e74 7269 6573 5f66 6574 6368 6564  _entries_fetched
+00006380: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00006390: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000063a0: 2020 2020 4120 6361 6c6c 6261 636b 2077      A callback w
+000063b0: 6865 6e20 656e 7472 6965 7320 6172 6520  hen entries are 
+000063c0: 6665 7463 6865 6420 6173 796e 6368 726f  fetched asynchro
+000063d0: 6e6f 7573 6c79 2e0a 2020 2020 2020 2020  nously..        
+000063e0: 5468 6520 636f 6e74 6578 7420 7368 6f75  The context shou
+000063f0: 6c64 2070 726f 7669 6465 2074 6865 2063  ld provide the c
+00006400: 6f6e 7465 7874 2070 6173 7365 6420 6672  ontext passed fr
+00006410: 6f6d 2053 746f 7261 6765 2e65 6e74 6972  om Storage.entir
+00006420: 6573 2829 2e0a 2020 2020 2020 2020 5365  es()..        Se
+00006430: 6520 6d6f 7265 2069 6e20 7468 6520 636f  e more in the co
+00006440: 6d6d 656e 7420 6f66 2053 746f 7261 6765  mment of Storage
+00006450: 2e65 6e74 6972 6573 2829 2e0a 0a20 2020  .entires()...   
+00006460: 2020 2020 2023 2050 616e 6963 730a 0a20       # Panics.. 
+00006470: 2020 2020 2020 2050 616e 6963 7320 6966         Panics if
+00006480: 2070 6173 7365 6420 7769 7468 2074 6865   passed with the
+00006490: 2063 6f6e 7465 7874 206f 6620 636f 6e74   context of cont
+000064a0: 6578 742e 6361 6e5f 6173 796e 6328 2920  ext.can_async() 
+000064b0: 3d3d 2066 616c 7365 0a20 2020 2020 2020  == false.       
+000064c0: 2022 2222 0a0a 636c 6173 7320 496e 4d65   """..class InMe
+000064d0: 6d6f 7279 5261 774e 6f64 6528 5f5f 4150  moryRawNode(__AP
+000064e0: 495f 5261 774e 6f64 6529 3a0a 2020 2020  I_RawNode):.    
+000064f0: 2222 220a 2020 2020 5261 774e 6f64 6520  """.    RawNode 
+00006500: 6973 2061 2074 6872 6561 642d 756e 7361  is a thread-unsa
+00006510: 6665 204e 6f64 652e 0a20 2020 2054 6865  fe Node..    The
+00006520: 206d 6574 686f 6473 206f 6620 7468 6973   methods of this
+00006530: 2073 7472 7563 7420 636f 7272 6573 706f   struct correspo
+00006540: 6e64 2074 6f20 7468 6520 6d65 7468 6f64  nd to the method
+00006550: 7320 6f66 204e 6f64 6520 616e 6420 6172  s of Node and ar
+00006560: 6520 6465 7363 7269 6265 640a 2020 2020  e described.    
+00006570: 6d6f 7265 2066 756c 6c79 2074 6865 7265  more fully there
+00006580: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00006590: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000065a0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000065b0: 2020 2063 6667 3a20 2243 6f6e 6669 6722     cfg: "Config"
+000065c0: 207c 2022 436f 6e66 6967 5265 6622 2c0a   | "ConfigRef",.
+000065d0: 2020 2020 2020 2020 7374 6f72 653a 2022          store: "
+000065e0: 4d65 6d53 746f 7261 6765 2220 7c20 224d  MemStorage" | "M
+000065f0: 656d 5374 6f72 6167 6552 6566 222c 0a20  emStorageRef",. 
+00006600: 2020 2020 2020 206c 6f67 6765 723a 2022         logger: "
+00006610: 4c6f 6767 6572 2220 7c20 224c 6f67 6765  Logger" | "Logge
+00006620: 7252 6566 222c 0a20 2020 2029 202d 3e20  rRef",.    ) -> 
+00006630: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+00006640: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+00006650: 202d 3e20 2249 6e4d 656d 6f72 7952 6177   -> "InMemoryRaw
+00006660: 4e6f 6465 5265 6622 3a20 2e2e 2e0a 2020  NodeRef": ....  
+00006670: 2020 6465 6620 6765 745f 7261 6674 2873    def get_raft(s
+00006680: 656c 6629 202d 3e20 2249 6e4d 656d 6f72  elf) -> "InMemor
+00006690: 7952 6166 7452 6566 223a 0a20 2020 2020  yRaftRef":.     
+000066a0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+000066b0: 6566 2073 746f 7265 2873 656c 6629 202d  ef store(self) -
+000066c0: 3e20 224d 656d 5374 6f72 6167 6552 6566  > "MemStorageRef
+000066d0: 223a 0a20 2020 2020 2020 2022 2222 5265  ":.        """Re
+000066e0: 7475 726e 7320 7468 6520 7374 6f72 6520  turns the store 
+000066f0: 6173 2061 206d 7574 6162 6c65 2072 6566  as a mutable ref
+00006700: 6572 656e 6365 2e22 2222 0a0a 636c 6173  erence."""..clas
+00006710: 7320 496e 4d65 6d6f 7279 5261 774e 6f64  s InMemoryRawNod
+00006720: 6552 6566 285f 5f41 5049 5f52 6177 4e6f  eRef(__API_RawNo
+00006730: 6465 293a 0a20 2020 2022 2222 0a20 2020  de):.    """.   
+00006740: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+00006750: 6f66 203a 636c 6173 733a 6049 6e4d 656d  of :class:`InMem
+00006760: 6f72 7952 6177 4e6f 6465 602e 0a20 2020  oryRawNode`..   
+00006770: 2022 2222 0a0a 2020 2020 6465 6620 6765   """..    def ge
+00006780: 745f 7261 6674 2873 656c 6629 202d 3e20  t_raft(self) -> 
+00006790: 2249 6e4d 656d 6f72 7952 6166 7452 6566  "InMemoryRaftRef
+000067a0: 223a 0a20 2020 2020 2020 2022 2222 2022  ":.        """ "
+000067b0: 2222 0a20 2020 2064 6566 2073 746f 7265  "".    def store
+000067c0: 2873 656c 6629 202d 3e20 224d 656d 5374  (self) -> "MemSt
+000067d0: 6f72 6167 6552 6566 223a 0a20 2020 2020  orageRef":.     
+000067e0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+000067f0: 6520 7374 6f72 6520 6173 2061 206d 7574  e store as a mut
+00006800: 6162 6c65 2072 6566 6572 656e 6365 2e22  able reference."
+00006810: 2222 0a20 2020 2023 2064 6566 2073 7461  "".    # def sta
+00006820: 7475 7328 7365 6c66 2920 2d3e 2049 6e4d  tus(self) -> InM
+00006830: 656d 6f72 7953 7461 7475 733a 0a20 2020  emoryStatus:.   
+00006840: 2023 2020 2020 2022 2222 0a20 2020 2023   #     """.    #
+00006850: 2020 2020 2053 7461 7475 7320 7265 7475       Status retu
+00006860: 726e 7320 7468 6520 6375 7272 656e 7420  rns the current 
+00006870: 7374 6174 7573 206f 6620 7468 6520 6769  status of the gi
+00006880: 7665 6e20 6772 6f75 702e 0a20 2020 2023  ven group..    #
+00006890: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
+000068a0: 5261 774e 6f64 6528 5f5f 4150 495f 5261  RawNode(__API_Ra
+000068b0: 774e 6f64 6529 3a0a 2020 2020 2222 220a  wNode):.    """.
+000068c0: 2020 2020 5261 774e 6f64 6520 6973 2061      RawNode is a
+000068d0: 2074 6872 6561 642d 756e 7361 6665 204e   thread-unsafe N
+000068e0: 6f64 652e 0a20 2020 2054 6865 206d 6574  ode..    The met
+000068f0: 686f 6473 206f 6620 7468 6973 2073 7472  hods of this str
+00006900: 7563 7420 636f 7272 6573 706f 6e64 2074  uct correspond t
+00006910: 6f20 7468 6520 6d65 7468 6f64 7320 6f66  o the methods of
+00006920: 204e 6f64 6520 616e 6420 6172 6520 6465   Node and are de
+00006930: 7363 7269 6265 640a 2020 2020 6d6f 7265  scribed.    more
+00006940: 2066 756c 6c79 2074 6865 7265 2e0a 2020   fully there..  
+00006950: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+00006960: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00006970: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
+00006980: 6667 3a20 2243 6f6e 6669 6722 207c 2022  fg: "Config" | "
+00006990: 436f 6e66 6967 5265 6622 2c0a 2020 2020  ConfigRef",.    
+000069a0: 2020 2020 7374 6f72 653a 2022 5374 6f72      store: "Stor
+000069b0: 6167 6522 207c 2022 5374 6f72 6167 6552  age" | "StorageR
+000069c0: 6566 222c 0a20 2020 2020 2020 206c 6f67  ef",.        log
+000069d0: 6765 723a 2022 4c6f 6767 6572 2220 7c20  ger: "Logger" | 
+000069e0: 224c 6f67 6765 7252 6566 222c 0a20 2020  "LoggerRef",.   
+000069f0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+00006a00: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
+00006a10: 2873 656c 6629 202d 3e20 2252 6177 4e6f  (self) -> "RawNo
+00006a20: 6465 5265 6622 3a20 2e2e 2e0a 2020 2020  deRef": ....    
+00006a30: 6465 6620 6765 745f 7261 6674 2873 656c  def get_raft(sel
+00006a40: 6629 202d 3e20 2252 6166 7452 6566 223a  f) -> "RaftRef":
+00006a50: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00006a60: 0a20 2020 2064 6566 2073 746f 7265 2873  .    def store(s
+00006a70: 656c 6629 202d 3e20 2253 746f 7261 6765  elf) -> "Storage
+00006a80: 5265 6622 3a0a 2020 2020 2020 2020 2222  Ref":.        ""
+00006a90: 2252 6574 7572 6e73 2074 6865 2073 746f  "Returns the sto
+00006aa0: 7265 2061 7320 6120 6d75 7461 626c 6520  re as a mutable 
+00006ab0: 7265 6665 7265 6e63 652e 2222 220a 2020  reference.""".  
+00006ac0: 2020 2320 6465 6620 7374 6174 7573 2873    # def status(s
+00006ad0: 656c 6629 202d 3e20 5374 6174 7573 3a0a  elf) -> Status:.
+00006ae0: 2020 2020 2320 2020 2020 2222 220a 2020      #     """.  
+00006af0: 2020 2320 2020 2020 5374 6174 7573 2072    #     Status r
+00006b00: 6574 7572 6e73 2074 6865 2063 7572 7265  eturns the curre
+00006b10: 6e74 2073 7461 7475 7320 6f66 2074 6865  nt status of the
+00006b20: 2067 6976 656e 2067 726f 7570 2e0a 2020   given group..  
+00006b30: 2020 2320 2020 2020 2222 220a 0a63 6c61    #     """..cla
+00006b40: 7373 2052 6177 4e6f 6465 5265 6628 5f5f  ss RawNodeRef(__
+00006b50: 4150 495f 5261 774e 6f64 6529 3a0a 2020  API_RawNode):.  
+00006b60: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
+00006b70: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
+00006b80: 7373 3a60 5261 774e 6f64 6560 2e0a 2020  ss:`RawNode`..  
+00006b90: 2020 2222 220a 0a20 2020 2064 6566 2067    """..    def g
+00006ba0: 6574 5f72 6166 7428 7365 6c66 2920 2d3e  et_raft(self) ->
+00006bb0: 2022 5261 6674 5265 6622 3a0a 2020 2020   "RaftRef":.    
+00006bc0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+00006bd0: 6465 6620 7374 6f72 6528 7365 6c66 2920  def store(self) 
+00006be0: 2d3e 2022 5374 6f72 6167 6552 6566 223a  -> "StorageRef":
+00006bf0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00006c00: 726e 7320 7468 6520 7374 6f72 6520 6173  rns the store as
+00006c10: 2061 206d 7574 6162 6c65 2072 6566 6572   a mutable refer
+00006c20: 656e 6365 2e22 2222 0a20 2020 2023 2064  ence.""".    # d
+00006c30: 6566 2073 7461 7475 7328 7365 6c66 2920  ef status(self) 
+00006c40: 2d3e 2049 6e4d 656d 6f72 7953 7461 7475  -> InMemoryStatu
+00006c50: 733a 0a20 2020 2023 2020 2020 2022 2222  s:.    #     """
+00006c60: 0a20 2020 2023 2020 2020 2053 7461 7475  .    #     Statu
+00006c70: 7320 7265 7475 726e 7320 7468 6520 6375  s returns the cu
+00006c80: 7272 656e 7420 7374 6174 7573 206f 6620  rrent status of 
+00006c90: 7468 6520 6769 7665 6e20 6772 6f75 702e  the given group.
+00006ca0: 0a20 2020 2023 2020 2020 2022 2222 0a0a  .    #     """..
+00006cb0: 636c 6173 7320 5f5f 4150 495f 5065 6572  class __API_Peer
+00006cc0: 3a0a 2020 2020 6465 6620 6765 745f 6964  :.    def get_id
+00006cd0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00006ce0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006cf0: 2020 2060 6964 603a 2054 6865 2049 4420     `id`: The ID 
+00006d00: 6f66 2074 6865 2070 6565 722e 0a20 2020  of the peer..   
+00006d10: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00006d20: 2073 6574 5f69 6428 7365 6c66 2c20 6964   set_id(self, id
+00006d30: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00006d40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006d50: 2020 2020 6069 6460 3a20 5468 6520 4944      `id`: The ID
+00006d60: 206f 6620 7468 6520 7065 6572 2e0a 2020   of the peer..  
+00006d70: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00006d80: 6620 6765 745f 636f 6e74 6578 7428 7365  f get_context(se
+00006d90: 6c66 2920 2d3e 2062 7974 6573 3a0a 2020  lf) -> bytes:.  
+00006da0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006db0: 2020 6063 6f6e 7465 7874 603a 2049 6620    `context`: If 
+00006dc0: 7468 6572 6520 6973 2063 6f6e 7465 7874  there is context
+00006dd0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00006de0: 2074 6865 2070 6565 7220 286c 696b 6520   the peer (like 
+00006df0: 636f 6e6e 6563 7469 6f6e 2069 6e66 6f72  connection infor
+00006e00: 6d61 7469 6f6e 292c 2069 7420 6361 6e20  mation), it can 
+00006e10: 6265 0a20 2020 2020 2020 2073 6572 6961  be.        seria
+00006e20: 6c69 7a65 6420 616e 6420 7374 6f72 6564  lized and stored
+00006e30: 2068 6572 652e 0a20 2020 2020 2020 2022   here..        "
+00006e40: 2222 0a20 2020 2064 6566 2073 6574 5f63  "".    def set_c
+00006e50: 6f6e 7465 7874 2873 656c 662c 2063 6f6e  ontext(self, con
+00006e60: 7465 7874 3a20 6279 7465 7329 202d 3e20  text: bytes) -> 
+00006e70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00006e80: 220a 2020 2020 2020 2020 6063 6f6e 7465  ".        `conte
+00006e90: 7874 603a 2049 6620 7468 6572 6520 6973  xt`: If there is
+00006ea0: 2063 6f6e 7465 7874 2061 7373 6f63 6961   context associa
+00006eb0: 7465 6420 7769 7468 2074 6865 2070 6565  ted with the pee
+00006ec0: 7220 286c 696b 6520 636f 6e6e 6563 7469  r (like connecti
+00006ed0: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 292c  on information),
+00006ee0: 2069 7420 6361 6e20 6265 0a20 2020 2020   it can be.     
+00006ef0: 2020 2073 6572 6961 6c69 7a65 6420 616e     serialized an
+00006f00: 6420 7374 6f72 6564 2068 6572 652e 0a20  d stored here.. 
+00006f10: 2020 2020 2020 2022 2222 0a0a 636c 6173         """..clas
+00006f20: 7320 5065 6572 285f 5f41 5049 5f50 6565  s Peer(__API_Pee
+00006f30: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
+00006f40: 5265 7072 6573 656e 7473 2061 2050 6565  Represents a Pee
+00006f50: 7220 6e6f 6465 2069 6e20 7468 6520 636c  r node in the cl
+00006f60: 7573 7465 722e 0a20 2020 2022 2222 0a0a  uster..    """..
+00006f70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00006f80: 2873 656c 6629 202d 3e20 4e6f 6e65 3a20  (self) -> None: 
+00006f90: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
+00006fa0: 5f72 6566 2873 656c 6629 202d 3e20 2250  _ref(self) -> "P
+00006fb0: 6565 7252 6566 223a 202e 2e2e 0a0a 636c  eerRef": .....cl
+00006fc0: 6173 7320 5065 6572 5265 6628 5f5f 4150  ass PeerRef(__AP
+00006fd0: 495f 5065 6572 293a 0a20 2020 2022 2222  I_Peer):.    """
+00006fe0: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
+00006ff0: 7970 6520 6f66 203a 636c 6173 733a 6050  ype of :class:`P
+00007000: 6565 7260 2e0a 2020 2020 2222 220a 0a63  eer`..    """..c
+00007010: 6c61 7373 205f 5f41 5049 5f4c 6967 6874  lass __API_Light
+00007020: 5265 6164 793a 0a20 2020 2064 6566 2063  Ready:.    def c
+00007030: 6f6d 6d69 745f 696e 6465 7828 7365 6c66  ommit_index(self
+00007040: 2920 2d3e 204f 7074 696f 6e61 6c5b 696e  ) -> Optional[in
+00007050: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
+00007060: 2020 2020 2020 2020 5468 6520 6375 7272          The curr
+00007070: 656e 7420 636f 6d6d 6974 2069 6e64 6578  ent commit index
+00007080: 2e0a 2020 2020 2020 2020 4974 2077 696c  ..        It wil
+00007090: 6c20 6265 204e 6f6e 6520 7374 6174 6520  l be None state 
+000070a0: 6966 2074 6865 7265 2069 7320 6e6f 2075  if there is no u
+000070b0: 7064 6174 652e 0a20 2020 2020 2020 2049  pdate..        I
+000070c0: 7420 6973 206e 6f74 2072 6571 7569 7265  t is not require
+000070d0: 6420 746f 2073 6176 6520 6974 2074 6f20  d to save it to 
+000070e0: 7374 6162 6c65 2073 746f 7261 6765 2e0a  stable storage..
+000070f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007100: 6465 6620 636f 6d6d 6974 7465 645f 656e  def committed_en
+00007110: 7472 6965 7328 7365 6c66 2920 2d3e 204c  tries(self) -> L
+00007120: 6973 745b 2245 6e74 7279 5265 6622 5d3a  ist["EntryRef"]:
+00007130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007140: 2020 2020 2043 6f6d 6d69 7474 6564 456e       CommittedEn
+00007150: 7472 6965 7320 7370 6563 6966 6965 7320  tries specifies 
+00007160: 656e 7472 6965 7320 746f 2062 6520 636f  entries to be co
+00007170: 6d6d 6974 7465 6420 746f 2061 0a20 2020  mmitted to a.   
+00007180: 2020 2020 2073 746f 7265 2f73 7461 7465       store/state
+00007190: 2d6d 6163 6869 6e65 2e20 5468 6573 6520  -machine. These 
+000071a0: 6861 7665 2070 7265 7669 6f75 736c 7920  have previously 
+000071b0: 6265 656e 2063 6f6d 6d69 7474 6564 2074  been committed t
+000071c0: 6f20 7374 6162 6c65 0a20 2020 2020 2020  o stable.       
+000071d0: 2073 746f 7265 2e0a 2020 2020 2020 2020   store..        
+000071e0: 2222 220a 2020 2020 6465 6620 7461 6b65  """.    def take
+000071f0: 5f63 6f6d 6d69 7474 6564 5f65 6e74 7269  _committed_entri
+00007200: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
+00007210: 5b22 456e 7472 7922 5d3a 0a20 2020 2020  ["Entry"]:.     
+00007220: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
+00007230: 616b 6520 7468 6520 436f 6d6d 6974 456e  ake the CommitEn
+00007240: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
+00007250: 2222 0a20 2020 2064 6566 206d 6573 7361  "".    def messa
+00007260: 6765 7328 7365 6c66 2920 2d3e 204c 6973  ges(self) -> Lis
+00007270: 745b 224d 6573 7361 6765 5265 6622 5d3a  t["MessageRef"]:
+00007280: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007290: 2020 2020 204d 6573 7361 6765 7320 7370       Messages sp
+000072a0: 6563 6966 6965 7320 6f75 7462 6f75 6e64  ecifies outbound
+000072b0: 206d 6573 7361 6765 7320 746f 2062 6520   messages to be 
+000072c0: 7365 6e74 2e0a 2020 2020 2020 2020 2222  sent..        ""
+000072d0: 220a 2020 2020 6465 6620 7461 6b65 5f6d  ".    def take_m
+000072e0: 6573 7361 6765 7328 7365 6c66 2920 2d3e  essages(self) ->
+000072f0: 204c 6973 745b 224d 6573 7361 6765 225d   List["Message"]
+00007300: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00007310: 2020 2020 2020 5461 6b65 2074 6865 204d        Take the M
+00007320: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
+00007330: 2022 2222 0a0a 636c 6173 7320 4c69 6768   """..class Ligh
+00007340: 7452 6561 6479 285f 5f41 5049 5f4c 6967  tReady(__API_Lig
+00007350: 6874 5265 6164 7929 3a0a 2020 2020 2222  htReady):.    ""
+00007360: 220a 2020 2020 4c69 6768 7452 6561 6479  ".    LightReady
+00007370: 2065 6e63 6170 7375 6c61 7465 7320 7468   encapsulates th
+00007380: 6520 636f 6d6d 6974 2069 6e64 6578 2c20  e commit index, 
+00007390: 636f 6d6d 6974 7465 6420 656e 7472 6965  committed entrie
+000073a0: 7320 616e 640a 2020 2020 6d65 7373 6167  s and.    messag
+000073b0: 6573 2074 6861 7420 6172 6520 7265 6164  es that are read
+000073c0: 7920 746f 2062 6520 6170 706c 6965 6420  y to be applied 
+000073d0: 6f72 2062 6520 7365 6e74 2074 6f20 6f74  or be sent to ot
+000073e0: 6865 7220 7065 6572 732e 0a20 2020 2022  her peers..    "
+000073f0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00007400: 6974 5f5f 2873 656c 6629 202d 3e20 4e6f  it__(self) -> No
+00007410: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+00007420: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
+00007430: 3e20 224c 6967 6874 5265 6164 7952 6566  > "LightReadyRef
+00007440: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
+00007450: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00007460: 2064 6566 6175 6c74 2829 202d 3e20 224c   default() -> "L
+00007470: 6967 6874 5265 6164 7922 3a20 2e2e 2e0a  ightReady": ....
+00007480: 0a63 6c61 7373 204c 6967 6874 5265 6164  .class LightRead
+00007490: 7952 6566 285f 5f41 5049 5f4c 6967 6874  yRef(__API_Light
+000074a0: 5265 6164 7929 3a0a 2020 2020 2222 220a  Ready):.    """.
+000074b0: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
+000074c0: 7065 206f 6620 3a63 6c61 7373 3a60 4c69  pe of :class:`Li
+000074d0: 6768 7452 6561 6479 602e 0a20 2020 2022  ghtReady`..    "
+000074e0: 2222 0a0a 636c 6173 7320 5f5f 4150 495f  ""..class __API_
+000074f0: 536e 6170 7368 6f74 4d65 7461 6461 7461  SnapshotMetadata
+00007500: 285f 5f43 6c6f 6e65 6162 6c65 2c20 5f5f  (__Cloneable, __
+00007510: 456e 636f 6465 722c 205f 5f44 6563 6f64  Encoder, __Decod
+00007520: 6572 293a 0a20 2020 2064 6566 2063 6c6f  er):.    def clo
+00007530: 6e65 2873 656c 6629 202d 3e20 2253 6e61  ne(self) -> "Sna
+00007540: 7073 686f 744d 6574 6164 6174 6122 3a20  pshotMetadata": 
+00007550: 2e2e 2e0a 2020 2020 6465 6620 6765 745f  ....    def get_
+00007560: 696e 6465 7828 7365 6c66 2920 2d3e 2069  index(self) -> i
+00007570: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+00007580: 2020 2020 2020 2020 6069 6e64 6578 603a          `index`:
+00007590: 2054 6865 2061 7070 6c69 6564 2069 6e64   The applied ind
+000075a0: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
+000075b0: 2020 2020 6465 6620 7365 745f 696e 6465      def set_inde
+000075c0: 7828 7365 6c66 2c20 696e 6465 783a 2069  x(self, index: i
+000075d0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+000075e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000075f0: 2060 696e 6465 7860 3a20 5468 6520 6170   `index`: The ap
+00007600: 706c 6965 6420 696e 6465 782e 0a20 2020  plied index..   
+00007610: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00007620: 2063 6c65 6172 5f69 6e64 6578 2873 656c   clear_index(sel
+00007630: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00007640: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007650: 6069 6e64 6578 603a 2054 6865 2061 7070  `index`: The app
+00007660: 6c69 6564 2069 6e64 6578 2e0a 2020 2020  lied index..    
+00007670: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00007680: 6765 745f 7465 726d 2873 656c 6629 202d  get_term(self) -
+00007690: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+000076a0: 2222 0a20 2020 2020 2020 2060 7465 726d  "".        `term
+000076b0: 603a 2054 6865 2074 6572 6d20 6f66 2074  `: The term of t
+000076c0: 6865 2061 7070 6c69 6564 2069 6e64 6578  he applied index
+000076d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000076e0: 2020 6465 6620 7365 745f 7465 726d 2873    def set_term(s
+000076f0: 656c 662c 2074 6572 6d3a 2069 6e74 2920  elf, term: int) 
+00007700: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00007710: 2022 2222 0a20 2020 2020 2020 2060 7465   """.        `te
+00007720: 726d 603a 2054 6865 2074 6572 6d20 6f66  rm`: The term of
+00007730: 2074 6865 2061 7070 6c69 6564 2069 6e64   the applied ind
+00007740: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
+00007750: 2020 2020 6465 6620 636c 6561 725f 7465      def clear_te
+00007760: 726d 2873 656c 6629 202d 3e20 4e6f 6e65  rm(self) -> None
+00007770: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00007780: 2020 2020 2020 6074 6572 6d60 3a20 5468        `term`: Th
+00007790: 6520 7465 726d 206f 6620 7468 6520 6170  e term of the ap
+000077a0: 706c 6965 6420 696e 6465 782e 0a20 2020  plied index..   
+000077b0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+000077c0: 2067 6574 5f63 6f6e 665f 7374 6174 6528   get_conf_state(
+000077d0: 7365 6c66 2920 2d3e 2022 436f 6e66 5374  self) -> "ConfSt
+000077e0: 6174 6552 6566 223a 0a20 2020 2020 2020  ateRef":.       
+000077f0: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
+00007800: 6e66 5f73 7461 7465 603a 2054 6865 2063  nf_state`: The c
+00007810: 7572 7265 6e74 2060 436f 6e66 5374 6174  urrent `ConfStat
+00007820: 6560 2e0a 2020 2020 2020 2020 2222 220a  e`..        """.
+00007830: 2020 2020 6465 6620 7365 745f 636f 6e66      def set_conf
+00007840: 5f73 7461 7465 2873 656c 662c 2063 6f6e  _state(self, con
+00007850: 665f 7374 6174 653a 2022 436f 6e66 5374  f_state: "ConfSt
+00007860: 6174 6522 207c 2022 436f 6e66 5374 6174  ate" | "ConfStat
+00007870: 6552 6566 2229 202d 3e20 4e6f 6e65 3a0a  eRef") -> None:.
+00007880: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007890: 2020 2020 6063 6f6e 665f 7374 6174 6560      `conf_state`
+000078a0: 3a20 5468 6520 6375 7272 656e 7420 6043  : The current `C
+000078b0: 6f6e 6653 7461 7465 602e 0a20 2020 2020  onfState`..     
+000078c0: 2020 2022 2222 0a20 2020 2064 6566 2063     """.    def c
+000078d0: 6c65 6172 5f63 6f6e 665f 7374 6174 6528  lear_conf_state(
+000078e0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000078f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007900: 2020 2060 636f 6e66 5f73 7461 7465 603a     `conf_state`:
+00007910: 2054 6865 2063 7572 7265 6e74 2060 436f   The current `Co
+00007920: 6e66 5374 6174 6560 2e0a 2020 2020 2020  nfState`..      
+00007930: 2020 2222 220a 2020 2020 6465 6620 6861    """.    def ha
+00007940: 735f 636f 6e66 5f73 7461 7465 2873 656c  s_conf_state(sel
+00007950: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
+00007960: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007970: 6063 6f6e 665f 7374 6174 6560 3a20 5468  `conf_state`: Th
+00007980: 6520 6375 7272 656e 7420 6043 6f6e 6653  e current `ConfS
+00007990: 7461 7465 602e 0a20 2020 2020 2020 2022  tate`..        "
+000079a0: 2222 0a0a 636c 6173 7320 536e 6170 7368  ""..class Snapsh
+000079b0: 6f74 4d65 7461 6461 7461 285f 5f41 5049  otMetadata(__API
+000079c0: 5f53 6e61 7073 686f 744d 6574 6164 6174  _SnapshotMetadat
+000079d0: 6129 3a0a 2020 2020 2222 2220 2222 220a  a):.    """ """.
+000079e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000079f0: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
+00007a00: 202e 2e2e 0a20 2020 2040 7374 6174 6963   ....    @static
+00007a10: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+00007a20: 6566 6175 6c74 2829 202d 3e20 2253 6e61  efault() -> "Sna
+00007a30: 7073 686f 744d 6574 6164 6174 6122 3a20  pshotMetadata": 
+00007a40: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+00007a50: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
+00007a60: 636f 6465 2876 3a20 6279 7465 7329 202d  code(v: bytes) -
+00007a70: 3e20 2253 6e61 7073 686f 744d 6574 6164  > "SnapshotMetad
+00007a80: 6174 6122 3a20 2e2e 2e0a 2020 2020 6465  ata": ....    de
+00007a90: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+00007aa0: 202d 3e20 2253 6e61 7073 686f 744d 6574   -> "SnapshotMet
+00007ab0: 6164 6174 6152 6566 223a 202e 2e2e 0a0a  adataRef": .....
+00007ac0: 636c 6173 7320 536e 6170 7368 6f74 4d65  class SnapshotMe
+00007ad0: 7461 6461 7461 5265 6628 5f5f 4150 495f  tadataRef(__API_
+00007ae0: 536e 6170 7368 6f74 4d65 7461 6461 7461  SnapshotMetadata
+00007af0: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
+00007b00: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
+00007b10: 203a 636c 6173 733a 6053 6e61 7073 686f   :class:`Snapsho
+00007b20: 744d 6574 6164 6174 6160 2e0a 2020 2020  tMetadata`..    
+00007b30: 2222 220a 0a63 6c61 7373 205f 5f41 5049  """..class __API
+00007b40: 5f53 6e61 7073 686f 7428 5f5f 436c 6f6e  _Snapshot(__Clon
+00007b50: 6561 626c 652c 205f 5f45 6e63 6f64 6572  eable, __Encoder
+00007b60: 2c20 5f5f 4465 636f 6465 7229 3a0a 2020  , __Decoder):.  
+00007b70: 2020 6465 6620 636c 6f6e 6528 7365 6c66    def clone(self
+00007b80: 2920 2d3e 2022 536e 6170 7368 6f74 223a  ) -> "Snapshot":
+00007b90: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+00007ba0: 5f64 6174 6128 7365 6c66 2920 2d3e 2062  _data(self) -> b
+00007bb0: 7974 6573 3a0a 2020 2020 2020 2020 2222  ytes:.        ""
+00007bc0: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+00007bd0: 745f 6461 7461 2873 656c 662c 2064 6174  t_data(self, dat
+00007be0: 613a 2062 7974 6573 2920 2d3e 204e 6f6e  a: bytes) -> Non
+00007bf0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+00007c00: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+00007c10: 5f64 6174 6128 7365 6c66 2920 2d3e 204e  _data(self) -> N
+00007c20: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00007c30: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00007c40: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
+00007c50: 2d3e 2022 536e 6170 7368 6f74 4d65 7461  -> "SnapshotMeta
+00007c60: 6461 7461 5265 6622 3a0a 2020 2020 2020  dataRef":.      
+00007c70: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+00007c80: 6620 7365 745f 6d65 7461 6461 7461 280a  f set_metadata(.
+00007c90: 2020 2020 2020 2020 7365 6c66 2c20 6d65          self, me
+00007ca0: 7461 5f64 6174 613a 2022 536e 6170 7368  ta_data: "Snapsh
+00007cb0: 6f74 4d65 7461 6461 7461 2220 7c20 2253  otMetadata" | "S
+00007cc0: 6e61 7073 686f 744d 6574 6164 6174 6152  napshotMetadataR
+00007cd0: 6566 220a 2020 2020 2920 2d3e 204e 6f6e  ef".    ) -> Non
+00007ce0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+00007cf0: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+00007d00: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
+00007d10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00007d20: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00007d30: 2068 6173 5f6d 6574 6164 6174 6128 7365   has_metadata(se
+00007d40: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00007d50: 2020 2020 2022 2222 2022 2222 0a0a 636c       """ """..cl
+00007d60: 6173 7320 536e 6170 7368 6f74 285f 5f41  ass Snapshot(__A
+00007d70: 5049 5f53 6e61 7073 686f 7429 3a0a 2020  PI_Snapshot):.  
+00007d80: 2020 2222 2220 2222 220a 0a20 2020 2064    """ """..    d
+00007d90: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00007da0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+00007db0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00007dc0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
+00007dd0: 2829 202d 3e20 2253 6e61 7073 686f 7422  () -> "Snapshot"
+00007de0: 3a20 2e2e 2e0a 2020 2020 4073 7461 7469  : ....    @stati
+00007df0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00007e00: 6465 636f 6465 2876 3a20 6279 7465 7329  decode(v: bytes)
+00007e10: 202d 3e20 2253 6e61 7073 686f 7422 3a20   -> "Snapshot": 
+00007e20: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
+00007e30: 5f72 6566 2873 656c 6629 202d 3e20 2253  _ref(self) -> "S
+00007e40: 6e61 7073 686f 7452 6566 223a 202e 2e2e  napshotRef": ...
+00007e50: 0a0a 636c 6173 7320 536e 6170 7368 6f74  ..class Snapshot
+00007e60: 5265 6628 5f5f 4150 495f 536e 6170 7368  Ref(__API_Snapsh
+00007e70: 6f74 293a 0a20 2020 2022 2222 0a20 2020  ot):.    """.   
+00007e80: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+00007e90: 6f66 203a 636c 6173 733a 6053 6e61 7073  of :class:`Snaps
+00007ea0: 686f 7460 2e0a 2020 2020 2222 220a 0a63  hot`..    """..c
+00007eb0: 6c61 7373 205f 5f41 5049 5f4d 6573 7361  lass __API_Messa
+00007ec0: 6765 285f 5f43 6c6f 6e65 6162 6c65 2c20  ge(__Cloneable, 
+00007ed0: 5f5f 456e 636f 6465 722c 205f 5f44 6563  __Encoder, __Dec
+00007ee0: 6f64 6572 293a 0a20 2020 2064 6566 2063  oder):.    def c
+00007ef0: 6c6f 6e65 2873 656c 6629 202d 3e20 224d  lone(self) -> "M
+00007f00: 6573 7361 6765 223a 202e 2e2e 0a20 2020  essage": ....   
+00007f10: 2064 6566 2067 6574 5f63 6f6d 6d69 7428   def get_commit(
+00007f20: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+00007f30: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00007f40: 2020 6465 6620 7365 745f 636f 6d6d 6974    def set_commit
+00007f50: 2873 656c 662c 2063 6f6d 6d69 743a 2069  (self, commit: i
+00007f60: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00007f70: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00007f80: 2064 6566 2063 6c65 6172 5f63 6f6d 6d69   def clear_commi
+00007f90: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+00007fa0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00007fb0: 0a20 2020 2064 6566 2067 6574 5f63 6f6d  .    def get_com
+00007fc0: 6d69 745f 7465 726d 2873 656c 6629 202d  mit_term(self) -
+00007fd0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00007fe0: 2222 2022 2222 0a20 2020 2064 6566 2073  "" """.    def s
+00007ff0: 6574 5f63 6f6d 6d69 745f 7465 726d 2873  et_commit_term(s
+00008000: 656c 662c 2063 6f6d 6d69 745f 7465 726d  elf, commit_term
+00008010: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00008020: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00008030: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
+00008040: 6d6d 6974 5f74 6572 6d28 7365 6c66 2920  mmit_term(self) 
+00008050: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00008060: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00008070: 2067 6574 5f66 726f 6d28 7365 6c66 2920   get_from(self) 
+00008080: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00008090: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+000080a0: 7365 745f 6672 6f6d 2873 656c 662c 2066  set_from(self, f
+000080b0: 726f 6d5f 3a20 696e 7429 202d 3e20 4e6f  rom_: int) -> No
+000080c0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+000080d0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
+000080e0: 725f 6672 6f6d 2873 656c 6629 202d 3e20  r_from(self) -> 
+000080f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00008100: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
+00008110: 745f 696e 6465 7828 7365 6c66 2920 2d3e  t_index(self) ->
+00008120: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00008130: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+00008140: 745f 696e 6465 7828 7365 6c66 2c20 696e  t_index(self, in
+00008150: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
+00008160: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+00008170: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+00008180: 5f69 6e64 6578 2873 656c 6629 202d 3e20  _index(self) -> 
 00008190: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
 000081a0: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-000081b0: 745f 6c6f 675f 7465 726d 2873 656c 6629  t_log_term(self)
-000081c0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-000081d0: 2022 2222 0a20 2020 2020 2020 2060 6c6f   """.        `lo
-000081e0: 6754 6572 6d60 3a20 6c6f 6754 6572 6d20  gTerm`: logTerm 
-000081f0: 6973 2067 656e 6572 616c 6c79 2075 7365  is generally use
-00008200: 6420 666f 7220 6170 7065 6e64 696e 6720  d for appending 
-00008210: 5261 6674 206c 6f67 7320 746f 2066 6f6c  Raft logs to fol
-00008220: 6c6f 7765 7273 2e20 466f 7220 6578 616d  lowers. For exam
-00008230: 706c 652c 0a20 2020 2020 2020 2028 7479  ple,.        (ty
-00008240: 7065 3d4d 7367 4170 7065 6e64 2c69 6e64  pe=MsgAppend,ind
-00008250: 6578 3d31 3030 2c6c 6f67 5f74 6572 6d3d  ex=100,log_term=
-00008260: 3529 206d 6561 6e73 206c 6561 6465 7220  5) means leader 
-00008270: 6170 7065 6e64 7320 656e 7472 6965 7320  appends entries 
-00008280: 7374 6172 7469 6e67 2061 740a 2020 2020  starting at.    
-00008290: 2020 2020 696e 6465 783d 3130 312c 2061      index=101, a
-000082a0: 6e64 2074 6865 2074 6572 6d20 6f66 2065  nd the term of e
-000082b0: 6e74 7279 2061 7420 696e 6465 7820 3130  ntry at index 10
-000082c0: 3020 6973 2035 2e0a 2020 2020 2020 2020  0 is 5..        
-000082d0: 2874 7970 653d 4d73 6741 7070 656e 6452  (type=MsgAppendR
-000082e0: 6573 706f 6e73 652c 7265 6a65 6374 3d74  esponse,reject=t
-000082f0: 7275 652c 696e 6465 783d 3130 302c 6c6f  rue,index=100,lo
-00008300: 675f 7465 726d 3d35 2920 6d65 616e 7320  g_term=5) means 
-00008310: 666f 6c6c 6f77 6572 2072 656a 6563 7473  follower rejects
-00008320: 2073 6f6d 650a 2020 2020 2020 2020 656e   some.        en
-00008330: 7472 6965 7320 6672 6f6d 2069 7473 206c  tries from its l
-00008340: 6561 6465 7220 6173 2069 7420 616c 7265  eader as it alre
-00008350: 6164 7920 6861 7320 616e 2065 6e74 7279  ady has an entry
-00008360: 2077 6974 6820 7465 726d 2035 2061 7420   with term 5 at 
-00008370: 696e 6465 7820 3130 302e 0a20 2020 2020  index 100..     
-00008380: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
-00008390: 6574 5f6c 6f67 5f74 6572 6d28 7365 6c66  et_log_term(self
-000083a0: 2c20 6c6f 675f 696e 6465 783a 2069 6e74  , log_index: int
-000083b0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000083c0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-000083d0: 6c6f 6754 6572 6d60 3a20 6c6f 6754 6572  logTerm`: logTer
-000083e0: 6d20 6973 2067 656e 6572 616c 6c79 2075  m is generally u
-000083f0: 7365 6420 666f 7220 6170 7065 6e64 696e  sed for appendin
-00008400: 6720 5261 6674 206c 6f67 7320 746f 2066  g Raft logs to f
-00008410: 6f6c 6c6f 7765 7273 2e20 466f 7220 6578  ollowers. For ex
-00008420: 616d 706c 652c 0a20 2020 2020 2020 2028  ample,.        (
-00008430: 7479 7065 3d4d 7367 4170 7065 6e64 2c69  type=MsgAppend,i
-00008440: 6e64 6578 3d31 3030 2c6c 6f67 5f74 6572  ndex=100,log_ter
-00008450: 6d3d 3529 206d 6561 6e73 206c 6561 6465  m=5) means leade
-00008460: 7220 6170 7065 6e64 7320 656e 7472 6965  r appends entrie
-00008470: 7320 7374 6172 7469 6e67 2061 740a 2020  s starting at.  
-00008480: 2020 2020 2020 696e 6465 783d 3130 312c        index=101,
-00008490: 2061 6e64 2074 6865 2074 6572 6d20 6f66   and the term of
-000084a0: 2065 6e74 7279 2061 7420 696e 6465 7820   entry at index 
-000084b0: 3130 3020 6973 2035 2e0a 2020 2020 2020  100 is 5..      
-000084c0: 2020 2874 7970 653d 4d73 6741 7070 656e    (type=MsgAppen
-000084d0: 6452 6573 706f 6e73 652c 7265 6a65 6374  dResponse,reject
-000084e0: 3d74 7275 652c 696e 6465 783d 3130 302c  =true,index=100,
-000084f0: 6c6f 675f 7465 726d 3d35 2920 6d65 616e  log_term=5) mean
-00008500: 7320 666f 6c6c 6f77 6572 2072 656a 6563  s follower rejec
-00008510: 7473 2073 6f6d 650a 2020 2020 2020 2020  ts some.        
-00008520: 656e 7472 6965 7320 6672 6f6d 2069 7473  entries from its
-00008530: 206c 6561 6465 7220 6173 2069 7420 616c   leader as it al
-00008540: 7265 6164 7920 6861 7320 616e 2065 6e74  ready has an ent
-00008550: 7279 2077 6974 6820 7465 726d 2035 2061  ry with term 5 a
-00008560: 7420 696e 6465 7820 3130 302e 0a20 2020  t index 100..   
-00008570: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00008580: 2063 6c65 6172 5f6c 6f67 5f74 6572 6d28   clear_log_term(
-00008590: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-000085a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000085b0: 2020 2060 6c6f 6754 6572 6d60 3a20 6c6f     `logTerm`: lo
-000085c0: 6754 6572 6d20 6973 2067 656e 6572 616c  gTerm is general
-000085d0: 6c79 2075 7365 6420 666f 7220 6170 7065  ly used for appe
-000085e0: 6e64 696e 6720 5261 6674 206c 6f67 7320  nding Raft logs 
-000085f0: 746f 2066 6f6c 6c6f 7765 7273 2e20 466f  to followers. Fo
-00008600: 7220 6578 616d 706c 652c 0a20 2020 2020  r example,.     
-00008610: 2020 2028 7479 7065 3d4d 7367 4170 7065     (type=MsgAppe
-00008620: 6e64 2c69 6e64 6578 3d31 3030 2c6c 6f67  nd,index=100,log
-00008630: 5f74 6572 6d3d 3529 206d 6561 6e73 206c  _term=5) means l
-00008640: 6561 6465 7220 6170 7065 6e64 7320 656e  eader appends en
-00008650: 7472 6965 7320 7374 6172 7469 6e67 2061  tries starting a
-00008660: 740a 2020 2020 2020 2020 696e 6465 783d  t.        index=
-00008670: 3130 312c 2061 6e64 2074 6865 2074 6572  101, and the ter
-00008680: 6d20 6f66 2065 6e74 7279 2061 7420 696e  m of entry at in
-00008690: 6465 7820 3130 3020 6973 2035 2e0a 2020  dex 100 is 5..  
-000086a0: 2020 2020 2020 2874 7970 653d 4d73 6741        (type=MsgA
-000086b0: 7070 656e 6452 6573 706f 6e73 652c 7265  ppendResponse,re
-000086c0: 6a65 6374 3d74 7275 652c 696e 6465 783d  ject=true,index=
-000086d0: 3130 302c 6c6f 675f 7465 726d 3d35 2920  100,log_term=5) 
-000086e0: 6d65 616e 7320 666f 6c6c 6f77 6572 2072  means follower r
-000086f0: 656a 6563 7473 2073 6f6d 650a 2020 2020  ejects some.    
-00008700: 2020 2020 656e 7472 6965 7320 6672 6f6d      entries from
-00008710: 2069 7473 206c 6561 6465 7220 6173 2069   its leader as i
-00008720: 7420 616c 7265 6164 7920 6861 7320 616e  t already has an
-00008730: 2065 6e74 7279 2077 6974 6820 7465 726d   entry with term
-00008740: 2035 2061 7420 696e 6465 7820 3130 302e   5 at index 100.
-00008750: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008760: 2064 6566 2067 6574 5f70 7269 6f72 6974   def get_priorit
-00008770: 7928 7365 6c66 2920 2d3e 2069 6e74 3a0a  y(self) -> int:.
-00008780: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008790: 2020 2020 6070 7269 6f72 6974 7960 3a20      `priority`: 
-000087a0: 4966 2074 6869 7320 6e65 7720 6669 656c  If this new fiel
-000087b0: 6420 6973 206e 6f74 2073 6574 2c20 7468  d is not set, th
-000087c0: 656e 2075 7365 2074 6865 2061 626f 7665  en use the above
-000087d0: 206f 6c64 2066 6965 6c64 3b20 6f74 6865   old field; othe
-000087e0: 7277 6973 650a 2020 2020 2020 2020 7573  rwise.        us
-000087f0: 6520 7468 6520 6e65 7720 6669 656c 642e  e the new field.
-00008800: 2057 6865 6e20 6272 6f61 6463 6173 7469   When broadcasti
-00008810: 6e67 2072 6571 7565 7374 2076 6f74 652c  ng request vote,
-00008820: 2062 6f74 6820 6669 656c 6473 2061 7265   both fields are
-00008830: 0a20 2020 2020 2020 2073 6574 2069 6620  .        set if 
-00008840: 7468 6520 7072 696f 7269 7479 2069 7320  the priority is 
-00008850: 6c61 7267 6572 2074 6861 6e20 302e 2054  larger than 0. T
-00008860: 6869 7320 6368 616e 6765 2069 7320 6e6f  his change is no
-00008870: 7420 6120 6675 6c6c 790a 2020 2020 2020  t a fully.      
-00008880: 2020 636f 6d70 6174 6962 6c65 2063 6861    compatible cha
-00008890: 6e67 652c 2062 7574 2069 7420 6d61 6b65  nge, but it make
-000088a0: 7320 6d69 6e69 6d61 6c20 696d 7061 6374  s minimal impact
-000088b0: 2074 6861 7420 6f6e 6c79 206e 6577 2070   that only new p
-000088c0: 7269 6f72 6974 790a 2020 2020 2020 2020  riority.        
-000088d0: 6973 206e 6f74 2072 6563 6f67 6e69 7a65  is not recognize
-000088e0: 6420 6279 2074 6865 206f 6c64 206e 6f64  d by the old nod
-000088f0: 6573 2064 7572 696e 6720 726f 6c6c 696e  es during rollin
-00008900: 6720 7570 6461 7465 2e0a 2020 2020 2020  g update..      
-00008910: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00008920: 745f 7072 696f 7269 7479 2873 656c 662c  t_priority(self,
-00008930: 2070 7269 6f72 6974 793a 2069 6e74 2920   priority: int) 
-00008940: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00008950: 2022 2222 0a20 2020 2020 2020 2060 7072   """.        `pr
-00008960: 696f 7269 7479 603a 2049 6620 7468 6973  iority`: If this
-00008970: 206e 6577 2066 6965 6c64 2069 7320 6e6f   new field is no
-00008980: 7420 7365 742c 2074 6865 6e20 7573 6520  t set, then use 
-00008990: 7468 6520 6162 6f76 6520 6f6c 6420 6669  the above old fi
-000089a0: 656c 643b 206f 7468 6572 7769 7365 0a20  eld; otherwise. 
-000089b0: 2020 2020 2020 2075 7365 2074 6865 206e         use the n
-000089c0: 6577 2066 6965 6c64 2e20 5768 656e 2062  ew field. When b
-000089d0: 726f 6164 6361 7374 696e 6720 7265 7175  roadcasting requ
-000089e0: 6573 7420 766f 7465 2c20 626f 7468 2066  est vote, both f
-000089f0: 6965 6c64 7320 6172 650a 2020 2020 2020  ields are.      
-00008a00: 2020 7365 7420 6966 2074 6865 2070 7269    set if the pri
-00008a10: 6f72 6974 7920 6973 206c 6172 6765 7220  ority is larger 
-00008a20: 7468 616e 2030 2e20 5468 6973 2063 6861  than 0. This cha
-00008a30: 6e67 6520 6973 206e 6f74 2061 2066 756c  nge is not a ful
-00008a40: 6c79 0a20 2020 2020 2020 2063 6f6d 7061  ly.        compa
-00008a50: 7469 626c 6520 6368 616e 6765 2c20 6275  tible change, bu
-00008a60: 7420 6974 206d 616b 6573 206d 696e 696d  t it makes minim
-00008a70: 616c 2069 6d70 6163 7420 7468 6174 206f  al impact that o
-00008a80: 6e6c 7920 6e65 7720 7072 696f 7269 7479  nly new priority
-00008a90: 0a20 2020 2020 2020 2069 7320 6e6f 7420  .        is not 
-00008aa0: 7265 636f 676e 697a 6564 2062 7920 7468  recognized by th
-00008ab0: 6520 6f6c 6420 6e6f 6465 7320 6475 7269  e old nodes duri
-00008ac0: 6e67 2072 6f6c 6c69 6e67 2075 7064 6174  ng rolling updat
-00008ad0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00008ae0: 2020 2064 6566 2063 6c65 6172 5f70 7269     def clear_pri
-00008af0: 6f72 6974 7928 7365 6c66 2920 2d3e 204e  ority(self) -> N
-00008b00: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00008b10: 0a20 2020 2020 2020 2060 7072 696f 7269  .        `priori
-00008b20: 7479 603a 2049 6620 7468 6973 206e 6577  ty`: If this new
-00008b30: 2066 6965 6c64 2069 7320 6e6f 7420 7365   field is not se
-00008b40: 742c 2074 6865 6e20 7573 6520 7468 6520  t, then use the 
-00008b50: 6162 6f76 6520 6f6c 6420 6669 656c 643b  above old field;
-00008b60: 206f 7468 6572 7769 7365 0a20 2020 2020   otherwise.     
-00008b70: 2020 2075 7365 2074 6865 206e 6577 2066     use the new f
-00008b80: 6965 6c64 2e20 5768 656e 2062 726f 6164  ield. When broad
-00008b90: 6361 7374 696e 6720 7265 7175 6573 7420  casting request 
-00008ba0: 766f 7465 2c20 626f 7468 2066 6965 6c64  vote, both field
-00008bb0: 7320 6172 650a 2020 2020 2020 2020 7365  s are.        se
-00008bc0: 7420 6966 2074 6865 2070 7269 6f72 6974  t if the priorit
-00008bd0: 7920 6973 206c 6172 6765 7220 7468 616e  y is larger than
-00008be0: 2030 2e20 5468 6973 2063 6861 6e67 6520   0. This change 
-00008bf0: 6973 206e 6f74 2061 2066 756c 6c79 0a20  is not a fully. 
-00008c00: 2020 2020 2020 2063 6f6d 7061 7469 626c         compatibl
-00008c10: 6520 6368 616e 6765 2c20 6275 7420 6974  e change, but it
-00008c20: 206d 616b 6573 206d 696e 696d 616c 2069   makes minimal i
-00008c30: 6d70 6163 7420 7468 6174 206f 6e6c 7920  mpact that only 
-00008c40: 6e65 7720 7072 696f 7269 7479 0a20 2020  new priority.   
-00008c50: 2020 2020 2069 7320 6e6f 7420 7265 636f       is not reco
-00008c60: 676e 697a 6564 2062 7920 7468 6520 6f6c  gnized by the ol
-00008c70: 6420 6e6f 6465 7320 6475 7269 6e67 2072  d nodes during r
-00008c80: 6f6c 6c69 6e67 2075 7064 6174 652e 0a20  olling update.. 
-00008c90: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00008ca0: 6566 2067 6574 5f63 6f6e 7465 7874 2873  ef get_context(s
-00008cb0: 656c 6629 202d 3e20 6279 7465 733a 0a20  elf) -> bytes:. 
-00008cc0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00008cd0: 2020 2064 6566 2073 6574 5f63 6f6e 7465     def set_conte
-00008ce0: 7874 2873 656c 662c 2063 6f6e 7465 7874  xt(self, context
-00008cf0: 3a20 6279 7465 7329 202d 3e20 4e6f 6e65  : bytes) -> None
-00008d00: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00008d10: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
-00008d20: 636f 6e74 6578 7428 7365 6c66 2920 2d3e  context(self) ->
-00008d30: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00008d40: 2222 2022 2222 0a20 2020 2064 6566 2067  "" """.    def g
-00008d50: 6574 5f72 656a 6563 745f 6869 6e74 2873  et_reject_hint(s
-00008d60: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-00008d70: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00008d80: 2064 6566 2073 6574 5f72 656a 6563 745f   def set_reject_
-00008d90: 6869 6e74 2873 656c 662c 2072 656a 6563  hint(self, rejec
-00008da0: 745f 6869 6e74 3a20 626f 6f6c 2920 2d3e  t_hint: bool) ->
-00008db0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00008dc0: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-00008dd0: 6c65 6172 5f72 656a 6563 745f 6869 6e74  lear_reject_hint
-00008de0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00008df0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00008e00: 2020 2020 6465 6620 6765 745f 656e 7472      def get_entr
-00008e10: 6965 7328 7365 6c66 2920 2d3e 204c 6973  ies(self) -> Lis
-00008e20: 745b 2245 6e74 7279 5265 6622 5d3a 0a20  t["EntryRef"]:. 
-00008e30: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00008e40: 2020 2064 6566 2073 6574 5f65 6e74 7269     def set_entri
-00008e50: 6573 2873 656c 662c 2065 6e74 733a 204c  es(self, ents: L
-00008e60: 6973 745b 2245 6e74 7279 225d 207c 204c  ist["Entry"] | L
-00008e70: 6973 745b 2245 6e74 7279 5265 6622 5d29  ist["EntryRef"])
-00008e80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00008e90: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00008ea0: 6620 636c 6561 725f 656e 7472 6965 7328  f clear_entries(
-00008eb0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00008ec0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00008ed0: 2020 2064 6566 2067 6574 5f6d 7367 5f74     def get_msg_t
-00008ee0: 7970 6528 7365 6c66 2920 2d3e 2022 4d65  ype(self) -> "Me
-00008ef0: 7373 6167 6554 7970 6522 3a0a 2020 2020  ssageType":.    
-00008f00: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-00008f10: 6465 6620 7365 745f 6d73 675f 7479 7065  def set_msg_type
-00008f20: 2873 656c 662c 2074 7970 3a20 224d 6573  (self, typ: "Mes
-00008f30: 7361 6765 5479 7065 2229 202d 3e20 4e6f  sageType") -> No
-00008f40: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-00008f50: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-00008f60: 725f 6d73 675f 7479 7065 2873 656c 6629  r_msg_type(self)
-00008f70: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00008f80: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00008f90: 6620 6765 745f 7265 6a65 6374 2873 656c  f get_reject(sel
-00008fa0: 6629 202d 3e20 626f 6f6c 3a0a 2020 2020  f) -> bool:.    
-00008fb0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-00008fc0: 6465 6620 7365 745f 7265 6a65 6374 2873  def set_reject(s
-00008fd0: 656c 662c 2072 656a 6563 743a 2062 6f6f  elf, reject: boo
-00008fe0: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
-00008ff0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-00009000: 6465 6620 636c 6561 725f 7265 6a65 6374  def clear_reject
-00009010: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00009020: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-00009030: 2020 2020 6465 6620 6765 745f 736e 6170      def get_snap
-00009040: 7368 6f74 2873 656c 6629 202d 3e20 2253  shot(self) -> "S
-00009050: 6e61 7073 686f 7452 6566 223a 0a20 2020  napshotRef":.   
-00009060: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009070: 2064 6566 2073 6574 5f73 6e61 7073 686f   def set_snapsho
-00009080: 7428 7365 6c66 2c20 736e 6170 7368 6f74  t(self, snapshot
-00009090: 3a20 2253 6e61 7073 686f 7422 207c 2022  : "Snapshot" | "
-000090a0: 536e 6170 7368 6f74 5265 6622 2920 2d3e  SnapshotRef") ->
-000090b0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000090c0: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-000090d0: 6c65 6172 5f73 6e61 7073 686f 7428 7365  lear_snapshot(se
-000090e0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-000090f0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009100: 2064 6566 2067 6574 5f74 6f28 7365 6c66   def get_to(self
-00009110: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00009120: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00009130: 6620 7365 745f 746f 2873 656c 662c 2074  f set_to(self, t
-00009140: 6f3a 2069 6e74 2920 2d3e 204e 6f6e 653a  o: int) -> None:
-00009150: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00009160: 0a20 2020 2064 6566 2063 6c65 6172 5f74  .    def clear_t
-00009170: 6f28 7365 6c66 2920 2d3e 204e 6f6e 653a  o(self) -> None:
-00009180: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00009190: 0a20 2020 2064 6566 2067 6574 5f72 6571  .    def get_req
-000091a0: 7565 7374 5f73 6e61 7073 686f 7428 7365  uest_snapshot(se
-000091b0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-000091c0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-000091d0: 6465 6620 7365 745f 7265 7175 6573 745f  def set_request_
-000091e0: 736e 6170 7368 6f74 2873 656c 662c 2072  snapshot(self, r
-000091f0: 6571 7565 7374 5f73 6e61 7073 686f 743a  equest_snapshot:
-00009200: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-00009210: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00009220: 2020 2064 6566 2063 6c65 6172 5f72 6571     def clear_req
-00009230: 7565 7374 5f73 6e61 7073 686f 7428 7365  uest_snapshot(se
-00009240: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00009250: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009260: 2064 6566 2068 6173 5f73 6e61 7073 686f   def has_snapsho
-00009270: 7428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  t(self) -> bool:
-00009280: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00009290: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
-000092a0: 5f73 697a 6528 7365 6c66 2920 2d3e 2069  _size(self) -> i
-000092b0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-000092c0: 2020 2020 2020 2020 436f 6d70 7574 6520          Compute 
-000092d0: 616e 6420 6361 6368 6520 7369 7a65 206f  and cache size o
-000092e0: 6620 7468 6973 206d 6573 7361 6765 2061  f this message a
-000092f0: 6e64 2061 6c6c 206e 6573 7465 6420 6d65  nd all nested me
-00009300: 7373 6167 6573 0a20 2020 2020 2020 2022  ssages.        "
-00009310: 2222 0a0a 636c 6173 7320 4d65 7373 6167  ""..class Messag
-00009320: 6528 5f5f 4150 495f 4d65 7373 6167 6529  e(__API_Message)
-00009330: 3a0a 2020 2020 2222 2220 2222 220a 0a20  :.    """ """.. 
-00009340: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00009350: 7365 6c66 2920 2d3e 204e 6f6e 653a 202e  self) -> None: .
-00009360: 2e2e 0a20 2020 2064 6566 206d 616b 655f  ...    def make_
-00009370: 7265 6628 7365 6c66 2920 2d3e 2022 4d65  ref(self) -> "Me
-00009380: 7373 6167 6552 6566 223a 202e 2e2e 0a20  ssageRef": .... 
-00009390: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-000093a0: 0a20 2020 2064 6566 2064 6566 6175 6c74  .    def default
-000093b0: 2829 202d 3e20 224d 6573 7361 6765 223a  () -> "Message":
-000093c0: 202e 2e2e 0a20 2020 2040 7374 6174 6963   ....    @static
-000093d0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-000093e0: 6563 6f64 6528 763a 2062 7974 6573 2920  ecode(v: bytes) 
-000093f0: 2d3e 2022 4d65 7373 6167 6522 3a20 2e2e  -> "Message": ..
-00009400: 2e0a 0a63 6c61 7373 204d 6573 7361 6765  ...class Message
-00009410: 5265 6628 4d65 7373 6167 6529 3a0a 2020  Ref(Message):.  
-00009420: 2020 2222 220a 2020 2020 5265 6665 7265    """.    Refere
-00009430: 6e63 6520 7479 7065 206f 6620 3a63 6c61  nce type of :cla
-00009440: 7373 3a60 4d65 7373 6167 6560 2e0a 2020  ss:`Message`..  
-00009450: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-00009460: 5049 5f48 6172 6453 7461 7465 285f 5f43  PI_HardState(__C
-00009470: 6c6f 6e65 6162 6c65 2c20 5f5f 456e 636f  loneable, __Enco
-00009480: 6465 722c 205f 5f44 6563 6f64 6572 293a  der, __Decoder):
-00009490: 0a20 2020 2064 6566 2063 6c6f 6e65 2873  .    def clone(s
-000094a0: 656c 6629 202d 3e20 2248 6172 6453 7461  elf) -> "HardSta
-000094b0: 7465 223a 202e 2e2e 0a20 2020 2064 6566  te": ....    def
-000094c0: 2067 6574 5f74 6572 6d28 7365 6c66 2920   get_term(self) 
-000094d0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-000094e0: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-000094f0: 7365 745f 7465 726d 2873 656c 662c 2074  set_term(self, t
-00009500: 6572 6d3a 2069 6e74 2920 2d3e 204e 6f6e  erm: int) -> Non
-00009510: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00009520: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00009530: 5f74 6572 6d28 7365 6c66 2920 2d3e 204e  _term(self) -> N
-00009540: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00009550: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00009560: 5f76 6f74 6528 7365 6c66 2920 2d3e 2069  _vote(self) -> i
+000081b0: 745f 7465 726d 2873 656c 6629 202d 3e20  t_term(self) -> 
+000081c0: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+000081d0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+000081e0: 5f74 6572 6d28 7365 6c66 2c20 7465 726d  _term(self, term
+000081f0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00008200: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00008210: 2020 2020 6465 6620 636c 6561 725f 7465      def clear_te
+00008220: 726d 2873 656c 6629 202d 3e20 4e6f 6e65  rm(self) -> None
+00008230: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+00008240: 220a 2020 2020 6465 6620 6765 745f 6c6f  ".    def get_lo
+00008250: 675f 7465 726d 2873 656c 6629 202d 3e20  g_term(self) -> 
+00008260: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+00008270: 0a20 2020 2020 2020 2060 6c6f 6754 6572  .        `logTer
+00008280: 6d60 3a20 6c6f 6754 6572 6d20 6973 2067  m`: logTerm is g
+00008290: 656e 6572 616c 6c79 2075 7365 6420 666f  enerally used fo
+000082a0: 7220 6170 7065 6e64 696e 6720 5261 6674  r appending Raft
+000082b0: 206c 6f67 7320 746f 2066 6f6c 6c6f 7765   logs to followe
+000082c0: 7273 2e20 466f 7220 6578 616d 706c 652c  rs. For example,
+000082d0: 0a20 2020 2020 2020 2028 7479 7065 3d4d  .        (type=M
+000082e0: 7367 4170 7065 6e64 2c69 6e64 6578 3d31  sgAppend,index=1
+000082f0: 3030 2c6c 6f67 5f74 6572 6d3d 3529 206d  00,log_term=5) m
+00008300: 6561 6e73 206c 6561 6465 7220 6170 7065  eans leader appe
+00008310: 6e64 7320 656e 7472 6965 7320 7374 6172  nds entries star
+00008320: 7469 6e67 2061 740a 2020 2020 2020 2020  ting at.        
+00008330: 696e 6465 783d 3130 312c 2061 6e64 2074  index=101, and t
+00008340: 6865 2074 6572 6d20 6f66 2065 6e74 7279  he term of entry
+00008350: 2061 7420 696e 6465 7820 3130 3020 6973   at index 100 is
+00008360: 2035 2e0a 2020 2020 2020 2020 2874 7970   5..        (typ
+00008370: 653d 4d73 6741 7070 656e 6452 6573 706f  e=MsgAppendRespo
+00008380: 6e73 652c 7265 6a65 6374 3d74 7275 652c  nse,reject=true,
+00008390: 696e 6465 783d 3130 302c 6c6f 675f 7465  index=100,log_te
+000083a0: 726d 3d35 2920 6d65 616e 7320 666f 6c6c  rm=5) means foll
+000083b0: 6f77 6572 2072 656a 6563 7473 2073 6f6d  ower rejects som
+000083c0: 650a 2020 2020 2020 2020 656e 7472 6965  e.        entrie
+000083d0: 7320 6672 6f6d 2069 7473 206c 6561 6465  s from its leade
+000083e0: 7220 6173 2069 7420 616c 7265 6164 7920  r as it already 
+000083f0: 6861 7320 616e 2065 6e74 7279 2077 6974  has an entry wit
+00008400: 6820 7465 726d 2035 2061 7420 696e 6465  h term 5 at inde
+00008410: 7820 3130 302e 0a20 2020 2020 2020 2022  x 100..        "
+00008420: 2222 0a20 2020 2064 6566 2073 6574 5f6c  "".    def set_l
+00008430: 6f67 5f74 6572 6d28 7365 6c66 2c20 6c6f  og_term(self, lo
+00008440: 675f 696e 6465 783a 2069 6e74 2920 2d3e  g_index: int) ->
+00008450: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00008460: 2222 0a20 2020 2020 2020 2060 6c6f 6754  "".        `logT
+00008470: 6572 6d60 3a20 6c6f 6754 6572 6d20 6973  erm`: logTerm is
+00008480: 2067 656e 6572 616c 6c79 2075 7365 6420   generally used 
+00008490: 666f 7220 6170 7065 6e64 696e 6720 5261  for appending Ra
+000084a0: 6674 206c 6f67 7320 746f 2066 6f6c 6c6f  ft logs to follo
+000084b0: 7765 7273 2e20 466f 7220 6578 616d 706c  wers. For exampl
+000084c0: 652c 0a20 2020 2020 2020 2028 7479 7065  e,.        (type
+000084d0: 3d4d 7367 4170 7065 6e64 2c69 6e64 6578  =MsgAppend,index
+000084e0: 3d31 3030 2c6c 6f67 5f74 6572 6d3d 3529  =100,log_term=5)
+000084f0: 206d 6561 6e73 206c 6561 6465 7220 6170   means leader ap
+00008500: 7065 6e64 7320 656e 7472 6965 7320 7374  pends entries st
+00008510: 6172 7469 6e67 2061 740a 2020 2020 2020  arting at.      
+00008520: 2020 696e 6465 783d 3130 312c 2061 6e64    index=101, and
+00008530: 2074 6865 2074 6572 6d20 6f66 2065 6e74   the term of ent
+00008540: 7279 2061 7420 696e 6465 7820 3130 3020  ry at index 100 
+00008550: 6973 2035 2e0a 2020 2020 2020 2020 2874  is 5..        (t
+00008560: 7970 653d 4d73 6741 7070 656e 6452 6573  ype=MsgAppendRes
+00008570: 706f 6e73 652c 7265 6a65 6374 3d74 7275  ponse,reject=tru
+00008580: 652c 696e 6465 783d 3130 302c 6c6f 675f  e,index=100,log_
+00008590: 7465 726d 3d35 2920 6d65 616e 7320 666f  term=5) means fo
+000085a0: 6c6c 6f77 6572 2072 656a 6563 7473 2073  llower rejects s
+000085b0: 6f6d 650a 2020 2020 2020 2020 656e 7472  ome.        entr
+000085c0: 6965 7320 6672 6f6d 2069 7473 206c 6561  ies from its lea
+000085d0: 6465 7220 6173 2069 7420 616c 7265 6164  der as it alread
+000085e0: 7920 6861 7320 616e 2065 6e74 7279 2077  y has an entry w
+000085f0: 6974 6820 7465 726d 2035 2061 7420 696e  ith term 5 at in
+00008600: 6465 7820 3130 302e 0a20 2020 2020 2020  dex 100..       
+00008610: 2022 2222 0a20 2020 2064 6566 2063 6c65   """.    def cle
+00008620: 6172 5f6c 6f67 5f74 6572 6d28 7365 6c66  ar_log_term(self
+00008630: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00008640: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00008650: 6c6f 6754 6572 6d60 3a20 6c6f 6754 6572  logTerm`: logTer
+00008660: 6d20 6973 2067 656e 6572 616c 6c79 2075  m is generally u
+00008670: 7365 6420 666f 7220 6170 7065 6e64 696e  sed for appendin
+00008680: 6720 5261 6674 206c 6f67 7320 746f 2066  g Raft logs to f
+00008690: 6f6c 6c6f 7765 7273 2e20 466f 7220 6578  ollowers. For ex
+000086a0: 616d 706c 652c 0a20 2020 2020 2020 2028  ample,.        (
+000086b0: 7479 7065 3d4d 7367 4170 7065 6e64 2c69  type=MsgAppend,i
+000086c0: 6e64 6578 3d31 3030 2c6c 6f67 5f74 6572  ndex=100,log_ter
+000086d0: 6d3d 3529 206d 6561 6e73 206c 6561 6465  m=5) means leade
+000086e0: 7220 6170 7065 6e64 7320 656e 7472 6965  r appends entrie
+000086f0: 7320 7374 6172 7469 6e67 2061 740a 2020  s starting at.  
+00008700: 2020 2020 2020 696e 6465 783d 3130 312c        index=101,
+00008710: 2061 6e64 2074 6865 2074 6572 6d20 6f66   and the term of
+00008720: 2065 6e74 7279 2061 7420 696e 6465 7820   entry at index 
+00008730: 3130 3020 6973 2035 2e0a 2020 2020 2020  100 is 5..      
+00008740: 2020 2874 7970 653d 4d73 6741 7070 656e    (type=MsgAppen
+00008750: 6452 6573 706f 6e73 652c 7265 6a65 6374  dResponse,reject
+00008760: 3d74 7275 652c 696e 6465 783d 3130 302c  =true,index=100,
+00008770: 6c6f 675f 7465 726d 3d35 2920 6d65 616e  log_term=5) mean
+00008780: 7320 666f 6c6c 6f77 6572 2072 656a 6563  s follower rejec
+00008790: 7473 2073 6f6d 650a 2020 2020 2020 2020  ts some.        
+000087a0: 656e 7472 6965 7320 6672 6f6d 2069 7473  entries from its
+000087b0: 206c 6561 6465 7220 6173 2069 7420 616c   leader as it al
+000087c0: 7265 6164 7920 6861 7320 616e 2065 6e74  ready has an ent
+000087d0: 7279 2077 6974 6820 7465 726d 2035 2061  ry with term 5 a
+000087e0: 7420 696e 6465 7820 3130 302e 0a20 2020  t index 100..   
+000087f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00008800: 2067 6574 5f70 7269 6f72 6974 7928 7365   get_priority(se
+00008810: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00008820: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008830: 6070 7269 6f72 6974 7960 3a20 4966 2074  `priority`: If t
+00008840: 6869 7320 6e65 7720 6669 656c 6420 6973  his new field is
+00008850: 206e 6f74 2073 6574 2c20 7468 656e 2075   not set, then u
+00008860: 7365 2074 6865 2061 626f 7665 206f 6c64  se the above old
+00008870: 2066 6965 6c64 3b20 6f74 6865 7277 6973   field; otherwis
+00008880: 650a 2020 2020 2020 2020 7573 6520 7468  e.        use th
+00008890: 6520 6e65 7720 6669 656c 642e 2057 6865  e new field. Whe
+000088a0: 6e20 6272 6f61 6463 6173 7469 6e67 2072  n broadcasting r
+000088b0: 6571 7565 7374 2076 6f74 652c 2062 6f74  equest vote, bot
+000088c0: 6820 6669 656c 6473 2061 7265 0a20 2020  h fields are.   
+000088d0: 2020 2020 2073 6574 2069 6620 7468 6520       set if the 
+000088e0: 7072 696f 7269 7479 2069 7320 6c61 7267  priority is larg
+000088f0: 6572 2074 6861 6e20 302e 2054 6869 7320  er than 0. This 
+00008900: 6368 616e 6765 2069 7320 6e6f 7420 6120  change is not a 
+00008910: 6675 6c6c 790a 2020 2020 2020 2020 636f  fully.        co
+00008920: 6d70 6174 6962 6c65 2063 6861 6e67 652c  mpatible change,
+00008930: 2062 7574 2069 7420 6d61 6b65 7320 6d69   but it makes mi
+00008940: 6e69 6d61 6c20 696d 7061 6374 2074 6861  nimal impact tha
+00008950: 7420 6f6e 6c79 206e 6577 2070 7269 6f72  t only new prior
+00008960: 6974 790a 2020 2020 2020 2020 6973 206e  ity.        is n
+00008970: 6f74 2072 6563 6f67 6e69 7a65 6420 6279  ot recognized by
+00008980: 2074 6865 206f 6c64 206e 6f64 6573 2064   the old nodes d
+00008990: 7572 696e 6720 726f 6c6c 696e 6720 7570  uring rolling up
+000089a0: 6461 7465 2e0a 2020 2020 2020 2020 2222  date..        ""
+000089b0: 220a 2020 2020 6465 6620 7365 745f 7072  ".    def set_pr
+000089c0: 696f 7269 7479 2873 656c 662c 2070 7269  iority(self, pri
+000089d0: 6f72 6974 793a 2069 6e74 2920 2d3e 204e  ority: int) -> N
+000089e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000089f0: 0a20 2020 2020 2020 2060 7072 696f 7269  .        `priori
+00008a00: 7479 603a 2049 6620 7468 6973 206e 6577  ty`: If this new
+00008a10: 2066 6965 6c64 2069 7320 6e6f 7420 7365   field is not se
+00008a20: 742c 2074 6865 6e20 7573 6520 7468 6520  t, then use the 
+00008a30: 6162 6f76 6520 6f6c 6420 6669 656c 643b  above old field;
+00008a40: 206f 7468 6572 7769 7365 0a20 2020 2020   otherwise.     
+00008a50: 2020 2075 7365 2074 6865 206e 6577 2066     use the new f
+00008a60: 6965 6c64 2e20 5768 656e 2062 726f 6164  ield. When broad
+00008a70: 6361 7374 696e 6720 7265 7175 6573 7420  casting request 
+00008a80: 766f 7465 2c20 626f 7468 2066 6965 6c64  vote, both field
+00008a90: 7320 6172 650a 2020 2020 2020 2020 7365  s are.        se
+00008aa0: 7420 6966 2074 6865 2070 7269 6f72 6974  t if the priorit
+00008ab0: 7920 6973 206c 6172 6765 7220 7468 616e  y is larger than
+00008ac0: 2030 2e20 5468 6973 2063 6861 6e67 6520   0. This change 
+00008ad0: 6973 206e 6f74 2061 2066 756c 6c79 0a20  is not a fully. 
+00008ae0: 2020 2020 2020 2063 6f6d 7061 7469 626c         compatibl
+00008af0: 6520 6368 616e 6765 2c20 6275 7420 6974  e change, but it
+00008b00: 206d 616b 6573 206d 696e 696d 616c 2069   makes minimal i
+00008b10: 6d70 6163 7420 7468 6174 206f 6e6c 7920  mpact that only 
+00008b20: 6e65 7720 7072 696f 7269 7479 0a20 2020  new priority.   
+00008b30: 2020 2020 2069 7320 6e6f 7420 7265 636f       is not reco
+00008b40: 676e 697a 6564 2062 7920 7468 6520 6f6c  gnized by the ol
+00008b50: 6420 6e6f 6465 7320 6475 7269 6e67 2072  d nodes during r
+00008b60: 6f6c 6c69 6e67 2075 7064 6174 652e 0a20  olling update.. 
+00008b70: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00008b80: 6566 2063 6c65 6172 5f70 7269 6f72 6974  ef clear_priorit
+00008b90: 7928 7365 6c66 2920 2d3e 204e 6f6e 653a  y(self) -> None:
+00008ba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00008bb0: 2020 2020 2060 7072 696f 7269 7479 603a       `priority`:
+00008bc0: 2049 6620 7468 6973 206e 6577 2066 6965   If this new fie
+00008bd0: 6c64 2069 7320 6e6f 7420 7365 742c 2074  ld is not set, t
+00008be0: 6865 6e20 7573 6520 7468 6520 6162 6f76  hen use the abov
+00008bf0: 6520 6f6c 6420 6669 656c 643b 206f 7468  e old field; oth
+00008c00: 6572 7769 7365 0a20 2020 2020 2020 2075  erwise.        u
+00008c10: 7365 2074 6865 206e 6577 2066 6965 6c64  se the new field
+00008c20: 2e20 5768 656e 2062 726f 6164 6361 7374  . When broadcast
+00008c30: 696e 6720 7265 7175 6573 7420 766f 7465  ing request vote
+00008c40: 2c20 626f 7468 2066 6965 6c64 7320 6172  , both fields ar
+00008c50: 650a 2020 2020 2020 2020 7365 7420 6966  e.        set if
+00008c60: 2074 6865 2070 7269 6f72 6974 7920 6973   the priority is
+00008c70: 206c 6172 6765 7220 7468 616e 2030 2e20   larger than 0. 
+00008c80: 5468 6973 2063 6861 6e67 6520 6973 206e  This change is n
+00008c90: 6f74 2061 2066 756c 6c79 0a20 2020 2020  ot a fully.     
+00008ca0: 2020 2063 6f6d 7061 7469 626c 6520 6368     compatible ch
+00008cb0: 616e 6765 2c20 6275 7420 6974 206d 616b  ange, but it mak
+00008cc0: 6573 206d 696e 696d 616c 2069 6d70 6163  es minimal impac
+00008cd0: 7420 7468 6174 206f 6e6c 7920 6e65 7720  t that only new 
+00008ce0: 7072 696f 7269 7479 0a20 2020 2020 2020  priority.       
+00008cf0: 2069 7320 6e6f 7420 7265 636f 676e 697a   is not recogniz
+00008d00: 6564 2062 7920 7468 6520 6f6c 6420 6e6f  ed by the old no
+00008d10: 6465 7320 6475 7269 6e67 2072 6f6c 6c69  des during rolli
+00008d20: 6e67 2075 7064 6174 652e 0a20 2020 2020  ng update..     
+00008d30: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00008d40: 6574 5f63 6f6e 7465 7874 2873 656c 6629  et_context(self)
+00008d50: 202d 3e20 6279 7465 733a 0a20 2020 2020   -> bytes:.     
+00008d60: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00008d70: 6566 2073 6574 5f63 6f6e 7465 7874 2873  ef set_context(s
+00008d80: 656c 662c 2063 6f6e 7465 7874 3a20 6279  elf, context: by
+00008d90: 7465 7329 202d 3e20 4e6f 6e65 3a0a 2020  tes) -> None:.  
+00008da0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00008db0: 2020 6465 6620 636c 6561 725f 636f 6e74    def clear_cont
+00008dc0: 6578 7428 7365 6c66 2920 2d3e 204e 6f6e  ext(self) -> Non
+00008dd0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+00008de0: 2222 0a20 2020 2064 6566 2067 6574 5f72  "".    def get_r
+00008df0: 656a 6563 745f 6869 6e74 2873 656c 6629  eject_hint(self)
+00008e00: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00008e10: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00008e20: 2073 6574 5f72 656a 6563 745f 6869 6e74   set_reject_hint
+00008e30: 2873 656c 662c 2072 656a 6563 745f 6869  (self, reject_hi
+00008e40: 6e74 3a20 626f 6f6c 2920 2d3e 204e 6f6e  nt: bool) -> Non
+00008e50: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+00008e60: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+00008e70: 5f72 656a 6563 745f 6869 6e74 2873 656c  _reject_hint(sel
+00008e80: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00008e90: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+00008ea0: 6465 6620 6765 745f 656e 7472 6965 7328  def get_entries(
+00008eb0: 7365 6c66 2920 2d3e 204c 6973 745b 2245  self) -> List["E
+00008ec0: 6e74 7279 5265 6622 5d3a 0a20 2020 2020  ntryRef"]:.     
+00008ed0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00008ee0: 6566 2073 6574 5f65 6e74 7269 6573 2873  ef set_entries(s
+00008ef0: 656c 662c 2065 6e74 733a 204c 6973 745b  elf, ents: List[
+00008f00: 2245 6e74 7279 225d 207c 204c 6973 745b  "Entry"] | List[
+00008f10: 2245 6e74 7279 5265 6622 5d29 202d 3e20  "EntryRef"]) -> 
+00008f20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00008f30: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
+00008f40: 6561 725f 656e 7472 6965 7328 7365 6c66  ear_entries(self
+00008f50: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00008f60: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00008f70: 6566 2067 6574 5f6d 7367 5f74 7970 6528  ef get_msg_type(
+00008f80: 7365 6c66 2920 2d3e 2022 4d65 7373 6167  self) -> "Messag
+00008f90: 6554 7970 6522 3a0a 2020 2020 2020 2020  eType":.        
+00008fa0: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00008fb0: 7365 745f 6d73 675f 7479 7065 2873 656c  set_msg_type(sel
+00008fc0: 662c 2074 7970 3a20 224d 6573 7361 6765  f, typ: "Message
+00008fd0: 5479 7065 2229 202d 3e20 4e6f 6e65 3a0a  Type") -> None:.
+00008fe0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00008ff0: 2020 2020 6465 6620 636c 6561 725f 6d73      def clear_ms
+00009000: 675f 7479 7065 2873 656c 6629 202d 3e20  g_type(self) -> 
+00009010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00009020: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
+00009030: 745f 7265 6a65 6374 2873 656c 6629 202d  t_reject(self) -
+00009040: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00009050: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00009060: 7365 745f 7265 6a65 6374 2873 656c 662c  set_reject(self,
+00009070: 2072 656a 6563 743a 2062 6f6f 6c29 202d   reject: bool) -
+00009080: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00009090: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+000090a0: 636c 6561 725f 7265 6a65 6374 2873 656c  clear_reject(sel
+000090b0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+000090c0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+000090d0: 6465 6620 6765 745f 736e 6170 7368 6f74  def get_snapshot
+000090e0: 2873 656c 6629 202d 3e20 2253 6e61 7073  (self) -> "Snaps
+000090f0: 686f 7452 6566 223a 0a20 2020 2020 2020  hotRef":.       
+00009100: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00009110: 2073 6574 5f73 6e61 7073 686f 7428 7365   set_snapshot(se
+00009120: 6c66 2c20 736e 6170 7368 6f74 3a20 2253  lf, snapshot: "S
+00009130: 6e61 7073 686f 7422 207c 2022 536e 6170  napshot" | "Snap
+00009140: 7368 6f74 5265 6622 2920 2d3e 204e 6f6e  shotRef") -> Non
+00009150: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+00009160: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+00009170: 5f73 6e61 7073 686f 7428 7365 6c66 2920  _snapshot(self) 
+00009180: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00009190: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+000091a0: 2067 6574 5f74 6f28 7365 6c66 2920 2d3e   get_to(self) ->
+000091b0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+000091c0: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+000091d0: 745f 746f 2873 656c 662c 2074 6f3a 2069  t_to(self, to: i
+000091e0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+000091f0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009200: 2064 6566 2063 6c65 6172 5f74 6f28 7365   def clear_to(se
+00009210: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00009220: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009230: 2064 6566 2067 6574 5f72 6571 7565 7374   def get_request
+00009240: 5f73 6e61 7073 686f 7428 7365 6c66 2920  _snapshot(self) 
+00009250: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00009260: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+00009270: 7365 745f 7265 7175 6573 745f 736e 6170  set_request_snap
+00009280: 7368 6f74 2873 656c 662c 2072 6571 7565  shot(self, reque
+00009290: 7374 5f73 6e61 7073 686f 743a 2069 6e74  st_snapshot: int
+000092a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+000092b0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+000092c0: 6566 2063 6c65 6172 5f72 6571 7565 7374  ef clear_request
+000092d0: 5f73 6e61 7073 686f 7428 7365 6c66 2920  _snapshot(self) 
+000092e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000092f0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00009300: 2068 6173 5f73 6e61 7073 686f 7428 7365   has_snapshot(se
+00009310: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00009320: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009330: 2064 6566 2063 6f6d 7075 7465 5f73 697a   def compute_siz
+00009340: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0a  e(self) -> int:.
+00009350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009360: 2020 2020 436f 6d70 7574 6520 616e 6420      Compute and 
+00009370: 6361 6368 6520 7369 7a65 206f 6620 7468  cache size of th
+00009380: 6973 206d 6573 7361 6765 2061 6e64 2061  is message and a
+00009390: 6c6c 206e 6573 7465 6420 6d65 7373 6167  ll nested messag
+000093a0: 6573 0a20 2020 2020 2020 2022 2222 0a0a  es.        """..
+000093b0: 636c 6173 7320 4d65 7373 6167 6528 5f5f  class Message(__
+000093c0: 4150 495f 4d65 7373 6167 6529 3a0a 2020  API_Message):.  
+000093d0: 2020 2222 2220 2222 220a 0a20 2020 2064    """ """..    d
+000093e0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+000093f0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+00009400: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+00009410: 7365 6c66 2920 2d3e 2022 4d65 7373 6167  self) -> "Messag
+00009420: 6552 6566 223a 202e 2e2e 0a20 2020 2040  eRef": ....    @
+00009430: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+00009440: 2064 6566 2064 6566 6175 6c74 2829 202d   def default() -
+00009450: 3e20 224d 6573 7361 6765 223a 202e 2e2e  > "Message": ...
+00009460: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00009470: 6f64 0a20 2020 2064 6566 2064 6563 6f64  od.    def decod
+00009480: 6528 763a 2062 7974 6573 2920 2d3e 2022  e(v: bytes) -> "
+00009490: 4d65 7373 6167 6522 3a20 2e2e 2e0a 0a63  Message": .....c
+000094a0: 6c61 7373 204d 6573 7361 6765 5265 6628  lass MessageRef(
+000094b0: 4d65 7373 6167 6529 3a0a 2020 2020 2222  Message):.    ""
+000094c0: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
+000094d0: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
+000094e0: 4d65 7373 6167 6560 2e0a 2020 2020 2222  Message`..    ""
+000094f0: 220a 0a63 6c61 7373 205f 5f41 5049 5f48  "..class __API_H
+00009500: 6172 6453 7461 7465 285f 5f43 6c6f 6e65  ardState(__Clone
+00009510: 6162 6c65 2c20 5f5f 456e 636f 6465 722c  able, __Encoder,
+00009520: 205f 5f44 6563 6f64 6572 293a 0a20 2020   __Decoder):.   
+00009530: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
+00009540: 202d 3e20 2248 6172 6453 7461 7465 223a   -> "HardState":
+00009550: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+00009560: 5f74 6572 6d28 7365 6c66 2920 2d3e 2069  _term(self) -> i
 00009570: 6e74 3a0a 2020 2020 2020 2020 2222 2220  nt:.        """ 
 00009580: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00009590: 766f 7465 2873 656c 662c 2076 6f74 653a  vote(self, vote:
+00009590: 7465 726d 2873 656c 662c 2074 6572 6d3a  term(self, term:
 000095a0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
 000095b0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-000095c0: 2020 2064 6566 2063 6c65 6172 5f76 6f74     def clear_vot
-000095d0: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+000095c0: 2020 2064 6566 2063 6c65 6172 5f74 6572     def clear_ter
+000095d0: 6d28 7365 6c66 2920 2d3e 204e 6f6e 653a  m(self) -> None:
 000095e0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-000095f0: 0a20 2020 2064 6566 2067 6574 5f63 6f6d  .    def get_com
-00009600: 6d69 7428 7365 6c66 2920 2d3e 2069 6e74  mit(self) -> int
-00009610: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00009620: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
-00009630: 6d6d 6974 2873 656c 662c 2063 6f6d 6d69  mmit(self, commi
-00009640: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-00009650: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-00009660: 0a20 2020 2064 6566 2063 6c65 6172 5f63  .    def clear_c
-00009670: 6f6d 6d69 7428 7365 6c66 2920 2d3e 204e  ommit(self) -> N
-00009680: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00009690: 2022 2222 0a0a 636c 6173 7320 4861 7264   """..class Hard
-000096a0: 5374 6174 6528 5f5f 4150 495f 4861 7264  State(__API_Hard
-000096b0: 5374 6174 6529 3a0a 2020 2020 2222 2220  State):.    """ 
-000096c0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
-000096d0: 6e69 745f 5f28 7365 6c66 2920 2d3e 204e  nit__(self) -> N
-000096e0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-000096f0: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
-00009700: 2d3e 2022 4861 7264 5374 6174 6552 6566  -> "HardStateRef
-00009710: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
-00009720: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00009730: 2064 6566 6175 6c74 2829 202d 3e20 2248   default() -> "H
-00009740: 6172 6453 7461 7465 223a 202e 2e2e 0a20  ardState": .... 
-00009750: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00009760: 0a20 2020 2064 6566 2064 6563 6f64 6528  .    def decode(
-00009770: 763a 2062 7974 6573 2920 2d3e 2022 4861  v: bytes) -> "Ha
-00009780: 7264 5374 6174 6522 3a20 2e2e 2e0a 0a63  rdState": .....c
-00009790: 6c61 7373 2048 6172 6453 7461 7465 5265  lass HardStateRe
-000097a0: 6628 5f5f 4150 495f 4861 7264 5374 6174  f(__API_HardStat
-000097b0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-000097c0: 5265 6665 7265 6e63 6520 7479 7065 206f  Reference type o
-000097d0: 6620 3a63 6c61 7373 3a60 4861 7264 5374  f :class:`HardSt
-000097e0: 6174 6560 2e0a 2020 2020 2222 220a 0a63  ate`..    """..c
-000097f0: 6c61 7373 205f 5f41 5049 5f47 6574 456e  lass __API_GetEn
-00009800: 7472 6965 7343 6f6e 7465 7874 3a0a 2020  triesContext:.  
-00009810: 2020 6465 6620 6361 6e5f 6173 796e 6328    def can_async(
-00009820: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-00009830: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009840: 2020 2043 6865 636b 2069 6620 7468 6520     Check if the 
-00009850: 6361 6c6c 6572 2773 2063 6f6e 7465 7874  caller's context
-00009860: 2073 7570 706f 7274 2066 6574 6368 696e   support fetchin
-00009870: 6720 656e 7472 6965 7320 6173 796e 6368  g entries asynch
-00009880: 726f 6e6f 7573 6c79 2e0a 2020 2020 2020  ronously..      
-00009890: 2020 2222 220a 0a63 6c61 7373 2047 6574    """..class Get
-000098a0: 456e 7472 6965 7343 6f6e 7465 7874 285f  EntriesContext(_
-000098b0: 5f41 5049 5f47 6574 456e 7472 6965 7343  _API_GetEntriesC
-000098c0: 6f6e 7465 7874 293a 0a20 2020 2022 2222  ontext):.    """
-000098d0: 0a20 2020 2052 6563 6f72 6473 2074 6865  .    Records the
-000098e0: 2063 6f6e 7465 7874 206f 6620 7468 6520   context of the 
-000098f0: 6361 6c6c 6572 2077 686f 2063 616c 6c73  caller who calls
-00009900: 2065 6e74 7269 6573 2829 206f 6620 5374   entries() of St
-00009910: 6f72 6167 6520 7472 6169 742e 0a20 2020  orage trait..   
-00009920: 2022 2222 0a0a 2020 2020 4073 7461 7469   """..    @stati
-00009930: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-00009940: 656d 7074 7928 6361 6e5f 6173 796e 633a  empty(can_async:
-00009950: 2062 6f6f 6c29 202d 3e20 2247 6574 456e   bool) -> "GetEn
-00009960: 7472 6965 7343 6f6e 7465 7874 223a 0a20  triesContext":. 
-00009970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009980: 2020 2055 7365 6420 666f 7220 6361 6c6c     Used for call
-00009990: 6572 7320 6f75 7420 6f66 2072 6166 742e  ers out of raft.
-000099a0: 2043 616c 6c65 7220 6361 6e20 6375 7374   Caller can cust
-000099b0: 6f6d 697a 6520 6966 2069 7420 7375 7070  omize if it supp
-000099c0: 6f72 7473 2061 7379 6e63 2e0a 2020 2020  orts async..    
-000099d0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-000099e0: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-000099f0: 3e20 2247 6574 456e 7472 6965 7343 6f6e  > "GetEntriesCon
-00009a00: 7465 7874 5265 6622 3a20 2e2e 2e0a 0a63  textRef": .....c
-00009a10: 6c61 7373 2047 6574 456e 7472 6965 7343  lass GetEntriesC
-00009a20: 6f6e 7465 7874 5265 6628 5f5f 4150 495f  ontextRef(__API_
-00009a30: 4765 7445 6e74 7269 6573 436f 6e74 6578  GetEntriesContex
-00009a40: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
-00009a50: 5265 6665 7265 6e63 6520 7479 7065 206f  Reference type o
-00009a60: 6620 3a63 6c61 7373 3a60 4765 7445 6e74  f :class:`GetEnt
-00009a70: 7269 6573 436f 6e74 6578 7460 2e0a 2020  riesContext`..  
-00009a80: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-00009a90: 5049 5f45 6e74 7279 285f 5f43 6c6f 6e65  PI_Entry(__Clone
-00009aa0: 6162 6c65 2c20 5f5f 456e 636f 6465 722c  able, __Encoder,
-00009ab0: 205f 5f44 6563 6f64 6572 293a 0a20 2020   __Decoder):.   
-00009ac0: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
-00009ad0: 202d 3e20 2245 6e74 7279 223a 202e 2e2e   -> "Entry": ...
-00009ae0: 0a20 2020 2064 6566 2067 6574 5f63 6f6e  .    def get_con
-00009af0: 7465 7874 2873 656c 6629 202d 3e20 6279  text(self) -> by
-00009b00: 7465 733a 0a20 2020 2020 2020 2022 2222  tes:.        """
-00009b10: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00009b20: 5f63 6f6e 7465 7874 2873 656c 662c 2063  _context(self, c
-00009b30: 6f6e 7465 7874 3a20 6279 7465 7329 202d  ontext: bytes) -
-00009b40: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00009b50: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-00009b60: 636c 6561 725f 636f 6e74 6578 7428 7365  clear_context(se
-00009b70: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00009b80: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009b90: 2064 6566 2067 6574 5f64 6174 6128 7365   def get_data(se
-00009ba0: 6c66 2920 2d3e 2062 7974 6573 3a0a 2020  lf) -> bytes:.  
-00009bb0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-00009bc0: 2020 6465 6620 7365 745f 6461 7461 2873    def set_data(s
-00009bd0: 656c 662c 2064 6174 613a 2062 7974 6573  elf, data: bytes
-00009be0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00009bf0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00009c00: 6566 2063 6c65 6172 5f64 6174 6128 7365  ef clear_data(se
-00009c10: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00009c20: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-00009c30: 2064 6566 2067 6574 5f65 6e74 7279 5f74   def get_entry_t
-00009c40: 7970 6528 7365 6c66 2920 2d3e 2022 456e  ype(self) -> "En
-00009c50: 7472 7954 7970 6522 3a0a 2020 2020 2020  tryType":.      
-00009c60: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00009c70: 6620 7365 745f 656e 7472 795f 7479 7065  f set_entry_type
-00009c80: 2873 656c 662c 2074 7970 3a20 2245 6e74  (self, typ: "Ent
-00009c90: 7279 5479 7065 2229 202d 3e20 4e6f 6e65  ryType") -> None
-00009ca0: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00009cb0: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
-00009cc0: 656e 7472 795f 7479 7065 2873 656c 6629  entry_type(self)
-00009cd0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00009ce0: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-00009cf0: 6620 6765 745f 7465 726d 2873 656c 6629  f get_term(self)
-00009d00: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00009d10: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00009d20: 2073 6574 5f74 6572 6d28 7365 6c66 2c20   set_term(self, 
-00009d30: 7465 726d 3a20 696e 7429 202d 3e20 4e6f  term: int) -> No
-00009d40: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-00009d50: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-00009d60: 725f 7465 726d 2873 656c 6629 202d 3e20  r_term(self) -> 
+000095f0: 0a20 2020 2064 6566 2067 6574 5f76 6f74  .    def get_vot
+00009600: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0a  e(self) -> int:.
+00009610: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00009620: 2020 2020 6465 6620 7365 745f 766f 7465      def set_vote
+00009630: 2873 656c 662c 2076 6f74 653a 2069 6e74  (self, vote: int
+00009640: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00009650: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+00009660: 6566 2063 6c65 6172 5f76 6f74 6528 7365  ef clear_vote(se
+00009670: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+00009680: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009690: 2064 6566 2067 6574 5f63 6f6d 6d69 7428   def get_commit(
+000096a0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+000096b0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+000096c0: 2020 6465 6620 7365 745f 636f 6d6d 6974    def set_commit
+000096d0: 2873 656c 662c 2063 6f6d 6d69 743a 2069  (self, commit: i
+000096e0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+000096f0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+00009700: 2064 6566 2063 6c65 6172 5f63 6f6d 6d69   def clear_commi
+00009710: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+00009720: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00009730: 0a0a 636c 6173 7320 4861 7264 5374 6174  ..class HardStat
+00009740: 6528 5f5f 4150 495f 4861 7264 5374 6174  e(__API_HardStat
+00009750: 6529 3a0a 2020 2020 2222 2220 2222 220a  e):.    """ """.
+00009760: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00009770: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
+00009780: 202e 2e2e 0a20 2020 2064 6566 206d 616b   ....    def mak
+00009790: 655f 7265 6628 7365 6c66 2920 2d3e 2022  e_ref(self) -> "
+000097a0: 4861 7264 5374 6174 6552 6566 223a 202e  HardStateRef": .
+000097b0: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+000097c0: 7468 6f64 0a20 2020 2064 6566 2064 6566  thod.    def def
+000097d0: 6175 6c74 2829 202d 3e20 2248 6172 6453  ault() -> "HardS
+000097e0: 7461 7465 223a 202e 2e2e 0a20 2020 2040  tate": ....    @
+000097f0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+00009800: 2064 6566 2064 6563 6f64 6528 763a 2062   def decode(v: b
+00009810: 7974 6573 2920 2d3e 2022 4861 7264 5374  ytes) -> "HardSt
+00009820: 6174 6522 3a20 2e2e 2e0a 0a63 6c61 7373  ate": .....class
+00009830: 2048 6172 6453 7461 7465 5265 6628 5f5f   HardStateRef(__
+00009840: 4150 495f 4861 7264 5374 6174 6529 3a0a  API_HardState):.
+00009850: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
+00009860: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
+00009870: 6c61 7373 3a60 4861 7264 5374 6174 6560  lass:`HardState`
+00009880: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
+00009890: 205f 5f41 5049 5f47 6574 456e 7472 6965   __API_GetEntrie
+000098a0: 7343 6f6e 7465 7874 3a0a 2020 2020 6465  sContext:.    de
+000098b0: 6620 6361 6e5f 6173 796e 6328 7365 6c66  f can_async(self
+000098c0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+000098d0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+000098e0: 6865 636b 2069 6620 7468 6520 6361 6c6c  heck if the call
+000098f0: 6572 2773 2063 6f6e 7465 7874 2073 7570  er's context sup
+00009900: 706f 7274 2066 6574 6368 696e 6720 656e  port fetching en
+00009910: 7472 6965 7320 6173 796e 6368 726f 6e6f  tries asynchrono
+00009920: 7573 6c79 2e0a 2020 2020 2020 2020 2222  usly..        ""
+00009930: 220a 0a63 6c61 7373 2047 6574 456e 7472  "..class GetEntr
+00009940: 6965 7343 6f6e 7465 7874 285f 5f41 5049  iesContext(__API
+00009950: 5f47 6574 456e 7472 6965 7343 6f6e 7465  _GetEntriesConte
+00009960: 7874 293a 0a20 2020 2022 2222 0a20 2020  xt):.    """.   
+00009970: 2052 6563 6f72 6473 2074 6865 2063 6f6e   Records the con
+00009980: 7465 7874 206f 6620 7468 6520 6361 6c6c  text of the call
+00009990: 6572 2077 686f 2063 616c 6c73 2065 6e74  er who calls ent
+000099a0: 7269 6573 2829 206f 6620 5374 6f72 6167  ries() of Storag
+000099b0: 6520 7472 6169 742e 0a20 2020 2022 2222  e trait..    """
+000099c0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+000099d0: 686f 640a 2020 2020 6465 6620 656d 7074  hod.    def empt
+000099e0: 7928 6361 6e5f 6173 796e 633a 2062 6f6f  y(can_async: boo
+000099f0: 6c29 202d 3e20 2247 6574 456e 7472 6965  l) -> "GetEntrie
+00009a00: 7343 6f6e 7465 7874 223a 0a20 2020 2020  sContext":.     
+00009a10: 2020 2022 2222 0a20 2020 2020 2020 2055     """.        U
+00009a20: 7365 6420 666f 7220 6361 6c6c 6572 7320  sed for callers 
+00009a30: 6f75 7420 6f66 2072 6166 742e 2043 616c  out of raft. Cal
+00009a40: 6c65 7220 6361 6e20 6375 7374 6f6d 697a  ler can customiz
+00009a50: 6520 6966 2069 7420 7375 7070 6f72 7473  e if it supports
+00009a60: 2061 7379 6e63 2e0a 2020 2020 2020 2020   async..        
+00009a70: 2222 220a 2020 2020 6465 6620 6d61 6b65  """.    def make
+00009a80: 5f72 6566 2873 656c 6629 202d 3e20 2247  _ref(self) -> "G
+00009a90: 6574 456e 7472 6965 7343 6f6e 7465 7874  etEntriesContext
+00009aa0: 5265 6622 3a20 2e2e 2e0a 0a63 6c61 7373  Ref": .....class
+00009ab0: 2047 6574 456e 7472 6965 7343 6f6e 7465   GetEntriesConte
+00009ac0: 7874 5265 6628 5f5f 4150 495f 4765 7445  xtRef(__API_GetE
+00009ad0: 6e74 7269 6573 436f 6e74 6578 7429 3a0a  ntriesContext):.
+00009ae0: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
+00009af0: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
+00009b00: 6c61 7373 3a60 4765 7445 6e74 7269 6573  lass:`GetEntries
+00009b10: 436f 6e74 6578 7460 2e0a 2020 2020 2222  Context`..    ""
+00009b20: 220a 0a63 6c61 7373 205f 5f41 5049 5f45  "..class __API_E
+00009b30: 6e74 7279 285f 5f43 6c6f 6e65 6162 6c65  ntry(__Cloneable
+00009b40: 2c20 5f5f 456e 636f 6465 722c 205f 5f44  , __Encoder, __D
+00009b50: 6563 6f64 6572 293a 0a20 2020 2064 6566  ecoder):.    def
+00009b60: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
+00009b70: 2245 6e74 7279 223a 202e 2e2e 0a20 2020  "Entry": ....   
+00009b80: 2064 6566 2067 6574 5f63 6f6e 7465 7874   def get_context
+00009b90: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
+00009ba0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+00009bb0: 0a20 2020 2064 6566 2073 6574 5f63 6f6e  .    def set_con
+00009bc0: 7465 7874 2873 656c 662c 2063 6f6e 7465  text(self, conte
+00009bd0: 7874 3a20 6279 7465 7329 202d 3e20 4e6f  xt: bytes) -> No
+00009be0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+00009bf0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
+00009c00: 725f 636f 6e74 6578 7428 7365 6c66 2920  r_context(self) 
+00009c10: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00009c20: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00009c30: 2067 6574 5f64 6174 6128 7365 6c66 2920   get_data(self) 
+00009c40: 2d3e 2062 7974 6573 3a0a 2020 2020 2020  -> bytes:.      
+00009c50: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+00009c60: 6620 7365 745f 6461 7461 2873 656c 662c  f set_data(self,
+00009c70: 2064 6174 613a 2062 7974 6573 2920 2d3e   data: bytes) ->
+00009c80: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00009c90: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
+00009ca0: 6c65 6172 5f64 6174 6128 7365 6c66 2920  lear_data(self) 
+00009cb0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00009cc0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+00009cd0: 2067 6574 5f65 6e74 7279 5f74 7970 6528   get_entry_type(
+00009ce0: 7365 6c66 2920 2d3e 2022 456e 7472 7954  self) -> "EntryT
+00009cf0: 7970 6522 3a0a 2020 2020 2020 2020 2222  ype":.        ""
+00009d00: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+00009d10: 745f 656e 7472 795f 7479 7065 2873 656c  t_entry_type(sel
+00009d20: 662c 2074 7970 3a20 2245 6e74 7279 5479  f, typ: "EntryTy
+00009d30: 7065 2229 202d 3e20 4e6f 6e65 3a0a 2020  pe") -> None:.  
+00009d40: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+00009d50: 2020 6465 6620 636c 6561 725f 656e 7472    def clear_entr
+00009d60: 795f 7479 7065 2873 656c 6629 202d 3e20  y_type(self) -> 
 00009d70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
 00009d80: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-00009d90: 745f 696e 6465 7828 7365 6c66 2920 2d3e  t_index(self) ->
-00009da0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00009db0: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-00009dc0: 745f 696e 6465 7828 7365 6c66 2c20 696e  t_index(self, in
-00009dd0: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
-00009de0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-00009df0: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
-00009e00: 5f69 6e64 6578 2873 656c 6629 202d 3e20  _index(self) -> 
-00009e10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00009e20: 2220 2222 220a 2020 2020 6465 6620 6765  " """.    def ge
-00009e30: 745f 7379 6e63 5f6c 6f67 2873 656c 6629  t_sync_log(self)
-00009e40: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00009e50: 2020 2222 220a 2020 2020 2020 2020 4465    """.        De
-00009e60: 7072 6563 6174 6564 2120 4974 2069 7320  precated! It is 
-00009e70: 6b65 7074 2066 6f72 2062 6163 6b77 6172  kept for backwar
-00009e80: 6420 636f 6d70 6174 6962 696c 6974 792e  d compatibility.
-00009e90: 0a20 2020 2020 2020 2054 4f44 4f3a 2072  .        TODO: r
-00009ea0: 656d 6f76 6520 6974 2069 6e20 7468 6520  emove it in the 
-00009eb0: 6e65 7874 206d 616a 6f72 2072 656c 6561  next major relea
-00009ec0: 7365 2e0a 2020 2020 2020 2020 2222 220a  se..        """.
-00009ed0: 2020 2020 6465 6620 7365 745f 7379 6e63      def set_sync
-00009ee0: 5f6c 6f67 2873 656c 662c 2073 796e 635f  _log(self, sync_
-00009ef0: 6c6f 673a 2062 6f6f 6c29 202d 3e20 4e6f  log: bool) -> No
-00009f00: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00009f10: 2020 2020 2020 2020 4465 7072 6563 6174          Deprecat
-00009f20: 6564 2120 4974 2069 7320 6b65 7074 2066  ed! It is kept f
-00009f30: 6f72 2062 6163 6b77 6172 6420 636f 6d70  or backward comp
-00009f40: 6174 6962 696c 6974 792e 0a20 2020 2020  atibility..     
-00009f50: 2020 2054 4f44 4f3a 2072 656d 6f76 6520     TODO: remove 
-00009f60: 6974 2069 6e20 7468 6520 6e65 7874 206d  it in the next m
-00009f70: 616a 6f72 2072 656c 6561 7365 2e0a 2020  ajor release..  
-00009f80: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00009f90: 6620 636c 6561 725f 7379 6e63 5f6c 6f67  f clear_sync_log
-00009fa0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00009fb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009fc0: 2020 2020 4465 7072 6563 6174 6564 2120      Deprecated! 
-00009fd0: 4974 2069 7320 6b65 7074 2066 6f72 2062  It is kept for b
-00009fe0: 6163 6b77 6172 6420 636f 6d70 6174 6962  ackward compatib
-00009ff0: 696c 6974 792e 0a20 2020 2020 2020 2054  ility..        T
-0000a000: 4f44 4f3a 2072 656d 6f76 6520 6974 2069  ODO: remove it i
-0000a010: 6e20 7468 6520 6e65 7874 206d 616a 6f72  n the next major
-0000a020: 2072 656c 6561 7365 2e0a 2020 2020 2020   release..      
-0000a030: 2020 2222 220a 0a63 6c61 7373 2045 6e74    """..class Ent
-0000a040: 7279 285f 5f41 5049 5f45 6e74 7279 293a  ry(__API_Entry):
-0000a050: 0a20 2020 2022 2222 0a20 2020 2054 6865  .    """.    The
-0000a060: 2065 6e74 7279 2069 7320 6120 7479 7065   entry is a type
-0000a070: 206f 6620 6368 616e 6765 2074 6861 7420   of change that 
-0000a080: 6e65 6564 7320 746f 2062 6520 6170 706c  needs to be appl
-0000a090: 6965 642e 2049 7420 636f 6e74 6169 6e73  ied. It contains
-0000a0a0: 2074 776f 2064 6174 6120 6669 656c 6473   two data fields
-0000a0b0: 2e0a 2020 2020 5768 696c 6520 7468 6520  ..    While the 
-0000a0c0: 6669 656c 6473 2061 7265 2062 7569 6c74  fields are built
-0000a0d0: 2069 6e74 6f20 7468 6520 6d6f 6465 6c3b   into the model;
-0000a0e0: 2074 6865 6972 2075 7361 6765 2069 7320   their usage is 
-0000a0f0: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
-0000a100: 6520 656e 7472 795f 7479 7065 2e0a 0a20  e entry_type... 
-0000a110: 2020 2046 6f72 206e 6f72 6d61 6c20 656e     For normal en
-0000a120: 7472 6965 732c 2074 6865 2064 6174 6120  tries, the data 
-0000a130: 6669 656c 6420 7368 6f75 6c64 2063 6f6e  field should con
-0000a140: 7461 696e 2074 6865 2064 6174 6120 6368  tain the data ch
-0000a150: 616e 6765 2074 6861 7420 7368 6f75 6c64  ange that should
-0000a160: 2062 6520 6170 706c 6965 642e 0a20 2020   be applied..   
-0000a170: 2054 6865 2063 6f6e 7465 7874 2066 6965   The context fie
-0000a180: 6c64 2063 616e 2062 6520 7573 6564 2066  ld can be used f
-0000a190: 6f72 2061 6e79 2063 6f6e 7465 7874 7561  or any contextua
-0000a1a0: 6c20 6461 7461 2074 6861 7420 6d69 6768  l data that migh
-0000a1b0: 7420 6265 2072 656c 6576 616e 7420 746f  t be relevant to
-0000a1c0: 2074 6865 0a20 2020 2061 7070 6c69 6361   the.    applica
-0000a1d0: 7469 6f6e 206f 6620 7468 6520 6461 7461  tion of the data
-0000a1e0: 2e0a 0a20 2020 2046 6f72 2063 6f6e 6669  ...    For confi
-0000a1f0: 6775 7261 7469 6f6e 2063 6861 6e67 6573  guration changes
-0000a200: 2c20 7468 6520 6461 7461 2077 696c 6c20  , the data will 
-0000a210: 636f 6e74 6169 6e20 7468 6520 436f 6e66  contain the Conf
-0000a220: 4368 616e 6765 206d 6573 7361 6765 2061  Change message a
-0000a230: 6e64 2074 6865 0a20 2020 2063 6f6e 7465  nd the.    conte
-0000a240: 7874 2077 696c 6c20 7072 6f76 6964 6520  xt will provide 
-0000a250: 616e 7974 6869 6e67 206e 6565 6465 6420  anything needed 
-0000a260: 746f 2061 7373 6973 7420 7468 6520 636f  to assist the co
-0000a270: 6e66 6967 7572 6174 696f 6e20 6368 616e  nfiguration chan
-0000a280: 6765 2e20 5468 6520 636f 6e74 6578 740a  ge. The context.
-0000a290: 2020 2020 6966 2066 6f72 2074 6865 2075      if for the u
-0000a2a0: 7365 7220 746f 2073 6574 2061 6e64 2075  ser to set and u
-0000a2b0: 7365 2069 6e20 7468 6973 2063 6173 652e  se in this case.
-0000a2c0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-0000a2d0: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
-0000a2e0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-0000a2f0: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
-0000a300: 656c 6629 202d 3e20 2245 6e74 7279 5265  elf) -> "EntryRe
-0000a310: 6622 3a20 2e2e 2e0a 2020 2020 4073 7461  f": ....    @sta
-0000a320: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0000a330: 6620 6465 6661 756c 7428 2920 2d3e 2022  f default() -> "
-0000a340: 456e 7472 7922 3a20 2e2e 2e0a 2020 2020  Entry": ....    
-0000a350: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-0000a360: 2020 6465 6620 6465 636f 6465 2876 3a20    def decode(v: 
-0000a370: 6279 7465 7329 202d 3e20 2245 6e74 7279  bytes) -> "Entry
-0000a380: 223a 202e 2e2e 0a0a 636c 6173 7320 456e  ": .....class En
-0000a390: 7472 7952 6566 285f 5f41 5049 5f45 6e74  tryRef(__API_Ent
-0000a3a0: 7279 293a 0a20 2020 2022 2222 0a20 2020  ry):.    """.   
-0000a3b0: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-0000a3c0: 6f66 203a 636c 6173 733a 6045 6e74 7279  of :class:`Entry
-0000a3d0: 602e 0a20 2020 2022 2222 0a0a 636c 6173  `..    """..clas
-0000a3e0: 7320 5f5f 4150 495f 436f 6e66 5374 6174  s __API_ConfStat
-0000a3f0: 6528 5f5f 436c 6f6e 6561 626c 652c 205f  e(__Cloneable, _
-0000a400: 5f45 6e63 6f64 6572 2c20 5f5f 4465 636f  _Encoder, __Deco
-0000a410: 6465 7229 3a0a 2020 2020 6465 6620 636c  der):.    def cl
-0000a420: 6f6e 6528 7365 6c66 2920 2d3e 2022 436f  one(self) -> "Co
-0000a430: 6e66 5374 6174 6522 3a20 2e2e 2e0a 2020  nfState": ....  
-0000a440: 2020 6465 6620 6765 745f 6175 746f 5f6c    def get_auto_l
-0000a450: 6561 7665 2873 656c 6629 202d 3e20 626f  eave(self) -> bo
-0000a460: 6f6c 3a0a 2020 2020 2020 2020 2222 2220  ol:.        """ 
-0000a470: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-0000a480: 6175 746f 5f6c 6561 7665 2873 656c 662c  auto_leave(self,
-0000a490: 2061 7574 6f5f 6c65 6176 653a 2062 6f6f   auto_leave: boo
-0000a4a0: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
-0000a4b0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-0000a4c0: 6465 6620 636c 6561 725f 6175 746f 5f6c  def clear_auto_l
-0000a4d0: 6561 7665 2873 656c 6629 202d 3e20 4e6f  eave(self) -> No
-0000a4e0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000a4f0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
-0000a500: 6c65 6172 6e65 7273 2873 656c 6629 202d  learners(self) -
-0000a510: 3e20 4c69 7374 5b69 6e74 5d3a 0a20 2020  > List[int]:.   
-0000a520: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000a530: 2064 6566 2073 6574 5f6c 6561 726e 6572   def set_learner
-0000a540: 7328 7365 6c66 2c20 6c65 6172 6e65 7273  s(self, learners
-0000a550: 3a20 4c69 7374 5b69 6e74 5d29 202d 3e20  : List[int]) -> 
-0000a560: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000a570: 2220 2222 220a 2020 2020 6465 6620 636c  " """.    def cl
-0000a580: 6561 725f 6c65 6172 6e65 7273 2873 656c  ear_learners(sel
-0000a590: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000a5a0: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
-0000a5b0: 6465 6620 6765 745f 6c65 6172 6e65 7273  def get_learners
-0000a5c0: 5f6e 6578 7428 7365 6c66 2920 2d3e 204c  _next(self) -> L
-0000a5d0: 6973 745b 696e 745d 3a0a 2020 2020 2020  ist[int]:.      
-0000a5e0: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
-0000a5f0: 6620 7365 745f 6c65 6172 6e65 7273 5f6e  f set_learners_n
-0000a600: 6578 7428 7365 6c66 2c20 6c65 6172 6e65  ext(self, learne
-0000a610: 7273 5f6e 6578 743a 204c 6973 745b 696e  rs_next: List[in
-0000a620: 745d 2920 2d3e 204e 6f6e 653a 0a20 2020  t]) -> None:.   
-0000a630: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000a640: 2064 6566 2063 6c65 6172 5f6c 6561 726e   def clear_learn
-0000a650: 6572 735f 6e65 7874 2873 656c 6629 202d  ers_next(self) -
-0000a660: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000a670: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-0000a680: 6765 745f 766f 7465 7273 2873 656c 6629  get_voters(self)
-0000a690: 202d 3e20 4c69 7374 5b69 6e74 5d3a 0a20   -> List[int]:. 
-0000a6a0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-0000a6b0: 2020 2064 6566 2073 6574 5f76 6f74 6572     def set_voter
-0000a6c0: 7328 7365 6c66 2c20 766f 7465 7273 3a20  s(self, voters: 
-0000a6d0: 4c69 7374 5b69 6e74 5d29 202d 3e20 4e6f  List[int]) -> No
-0000a6e0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000a6f0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-0000a700: 725f 766f 7465 7273 2873 656c 6629 202d  r_voters(self) -
-0000a710: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000a720: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-0000a730: 6765 745f 766f 7465 7273 5f6f 7574 676f  get_voters_outgo
-0000a740: 696e 6728 7365 6c66 2920 2d3e 204c 6973  ing(self) -> Lis
-0000a750: 745b 696e 745d 3a0a 2020 2020 2020 2020  t[int]:.        
-0000a760: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
-0000a770: 7365 745f 766f 7465 7273 5f6f 7574 676f  set_voters_outgo
-0000a780: 696e 6728 7365 6c66 2c20 766f 7465 7273  ing(self, voters
-0000a790: 5f6f 7574 676f 696e 673a 204c 6973 745b  _outgoing: List[
-0000a7a0: 696e 745d 2920 2d3e 204e 6f6e 653a 0a20  int]) -> None:. 
-0000a7b0: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-0000a7c0: 2020 2064 6566 2063 6c65 6172 5f76 6f74     def clear_vot
-0000a7d0: 6572 735f 6f75 7467 6f69 6e67 2873 656c  ers_outgoing(sel
-0000a7e0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-0000a7f0: 2020 2020 2222 2220 2222 220a 0a63 6c61      """ """..cla
-0000a800: 7373 2043 6f6e 6653 7461 7465 285f 5f41  ss ConfState(__A
-0000a810: 5049 5f43 6f6e 6653 7461 7465 293a 0a20  PI_ConfState):. 
-0000a820: 2020 2022 2222 2022 2222 0a0a 2020 2020     """ """..    
-0000a830: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0000a840: 2020 2020 2020 7365 6c66 2c20 766f 7465        self, vote
-0000a850: 7273 3a20 4f70 7469 6f6e 616c 5b4c 6973  rs: Optional[Lis
-0000a860: 745b 696e 745d 5d2c 206c 6561 726e 6572  t[int]], learner
-0000a870: 733a 204f 7074 696f 6e61 6c5b 4c69 7374  s: Optional[List
-0000a880: 5b69 6e74 5d5d 0a20 2020 2029 202d 3e20  [int]].    ) -> 
-0000a890: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
-0000a8a0: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
-0000a8b0: 202d 3e20 2243 6f6e 6653 7461 7465 5265   -> "ConfStateRe
-0000a8c0: 6622 3a20 2e2e 2e0a 2020 2020 4073 7461  f": ....    @sta
-0000a8d0: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0000a8e0: 6620 6465 6661 756c 7428 2920 2d3e 2022  f default() -> "
-0000a8f0: 436f 6e66 5374 6174 6522 3a20 2e2e 2e0a  ConfState": ....
-0000a900: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-0000a910: 640a 2020 2020 6465 6620 6465 636f 6465  d.    def decode
-0000a920: 2876 3a20 6279 7465 7329 202d 3e20 2243  (v: bytes) -> "C
-0000a930: 6f6e 6653 7461 7465 223a 202e 2e2e 0a0a  onfState": .....
-0000a940: 636c 6173 7320 436f 6e66 5374 6174 6552  class ConfStateR
-0000a950: 6566 285f 5f41 5049 5f43 6f6e 6653 7461  ef(__API_ConfSta
-0000a960: 7465 293a 0a20 2020 2022 2222 0a20 2020  te):.    """.   
-0000a970: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-0000a980: 6f66 203a 636c 6173 733a 6043 6f6e 6653  of :class:`ConfS
-0000a990: 7461 7465 602e 0a20 2020 2022 2222 0a0a  tate`..    """..
-0000a9a0: 636c 6173 7320 5f5f 4150 495f 436f 6e66  class __API_Conf
-0000a9b0: 4368 616e 6765 5632 285f 5f43 6c6f 6e65  ChangeV2(__Clone
-0000a9c0: 6162 6c65 2c20 5f5f 456e 636f 6465 722c  able, __Encoder,
-0000a9d0: 205f 5f44 6563 6f64 6572 293a 0a20 2020   __Decoder):.   
-0000a9e0: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
-0000a9f0: 202d 3e20 2243 6f6e 6643 6861 6e67 6556   -> "ConfChangeV
-0000aa00: 3222 3a20 2e2e 2e0a 2020 2020 6465 6620  2": ....    def 
-0000aa10: 6765 745f 6368 616e 6765 7328 7365 6c66  get_changes(self
-0000aa20: 2920 2d3e 204c 6973 745b 2243 6f6e 6643  ) -> List["ConfC
-0000aa30: 6861 6e67 6553 696e 676c 6552 6566 225d  hangeSingleRef"]
-0000aa40: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-0000aa50: 220a 2020 2020 6465 6620 7365 745f 6368  ".    def set_ch
-0000aa60: 616e 6765 7328 0a20 2020 2020 2020 2073  anges(.        s
-0000aa70: 656c 662c 2063 6861 6e67 6573 3a20 4c69  elf, changes: Li
-0000aa80: 7374 5b22 436f 6e66 4368 616e 6765 5369  st["ConfChangeSi
-0000aa90: 6e67 6c65 225d 207c 204c 6973 745b 2243  ngle"] | List["C
-0000aaa0: 6f6e 6643 6861 6e67 6553 696e 676c 6552  onfChangeSingleR
-0000aab0: 6566 225d 0a20 2020 2029 202d 3e20 4e6f  ef"].    ) -> No
-0000aac0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000aad0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-0000aae0: 725f 6368 616e 6765 7328 7365 6c66 2920  r_changes(self) 
-0000aaf0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000ab00: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000ab10: 2067 6574 5f63 6f6e 7465 7874 2873 656c   get_context(sel
-0000ab20: 6629 202d 3e20 6279 7465 733a 0a20 2020  f) -> bytes:.   
-0000ab30: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000ab40: 2064 6566 2073 6574 5f63 6f6e 7465 7874   def set_context
-0000ab50: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
-0000ab60: 6279 7465 7329 202d 3e20 4e6f 6e65 3a0a  bytes) -> None:.
-0000ab70: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000ab80: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
-0000ab90: 6e74 6578 7428 7365 6c66 2920 2d3e 204e  ntext(self) -> N
-0000aba0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000abb0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-0000abc0: 5f74 7261 6e73 6974 696f 6e28 7365 6c66  _transition(self
-0000abd0: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000abe0: 5472 616e 7369 7469 6f6e 223a 0a20 2020  Transition":.   
-0000abf0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000ac00: 2064 6566 2073 6574 5f74 7261 6e73 6974   def set_transit
-0000ac10: 696f 6e28 7365 6c66 2c20 7472 616e 7369  ion(self, transi
-0000ac20: 7469 6f6e 3a20 2243 6f6e 6643 6861 6e67  tion: "ConfChang
-0000ac30: 6554 7261 6e73 6974 696f 6e22 2920 2d3e  eTransition") ->
-0000ac40: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000ac50: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
-0000ac60: 6c65 6172 5f74 7261 6e73 6974 696f 6e28  lear_transition(
-0000ac70: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-0000ac80: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-0000ac90: 2020 2064 6566 2065 6e74 6572 5f6a 6f69     def enter_joi
-0000aca0: 6e74 2873 656c 6629 202d 3e20 4f70 7469  nt(self) -> Opti
-0000acb0: 6f6e 616c 5b62 6f6f 6c5d 3a0a 2020 2020  onal[bool]:.    
-0000acc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000acd0: 4368 6563 6b73 2069 6620 7573 6573 204a  Checks if uses J
-0000ace0: 6f69 6e74 2043 6f6e 7365 6e73 7573 2e0a  oint Consensus..
-0000acf0: 0a20 2020 2020 2020 2049 7420 7769 6c6c  .        It will
-0000ad00: 2072 6574 7572 6e20 536f 6d65 2069 6620   return Some if 
-0000ad10: 616e 6420 6f6e 6c79 2069 6620 7468 6973  and only if this
-0000ad20: 2063 6f6e 6669 6720 6368 616e 6765 2077   config change w
-0000ad30: 696c 6c20 7573 6520 4a6f 696e 7420 436f  ill use Joint Co
-0000ad40: 6e73 656e 7375 732c 0a20 2020 2020 2020  nsensus,.       
-0000ad50: 2077 6869 6368 2069 7320 7468 6520 6361   which is the ca
-0000ad60: 7365 2069 6620 6974 2063 6f6e 7461 696e  se if it contain
-0000ad70: 7320 6d6f 7265 2074 6861 6e20 6f6e 6520  s more than one 
-0000ad80: 6368 616e 6765 206f 7220 6966 2074 6865  change or if the
-0000ad90: 2075 7365 206f 6620 4a6f 696e 740a 2020   use of Joint.  
-0000ada0: 2020 2020 2020 436f 6e73 656e 7375 7320        Consensus 
-0000adb0: 7761 7320 7265 7175 6573 7465 6420 6578  was requested ex
-0000adc0: 706c 6963 6974 6c79 2e20 5468 6520 626f  plicitly. The bo
-0000add0: 6f6c 2069 6e64 6963 6174 6573 2077 6865  ol indicates whe
-0000ade0: 7468 6572 2074 6865 204a 6f69 6e74 2053  ther the Joint S
-0000adf0: 7461 7465 0a20 2020 2020 2020 2077 696c  tate.        wil
-0000ae00: 6c20 6265 206c 6566 7420 6175 746f 6d61  l be left automa
-0000ae10: 7469 6361 6c6c 792e 0a20 2020 2020 2020  tically..       
-0000ae20: 2022 2222 0a20 2020 2064 6566 206d 6572   """.    def mer
-0000ae30: 6765 5f66 726f 6d5f 6279 7465 7328 7365  ge_from_bytes(se
-0000ae40: 6c66 2c20 623a 2062 7974 6573 2920 2d3e  lf, b: bytes) ->
-0000ae50: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000ae60: 2222 0a20 2020 2020 2020 2055 7064 6174  "".        Updat
-0000ae70: 6520 7468 6973 206d 6573 7361 6765 206f  e this message o
-0000ae80: 626a 6563 7420 7769 7468 2066 6965 6c64  bject with field
-0000ae90: 7320 7265 6164 2066 726f 6d20 6769 7665  s read from give
-0000aea0: 6e20 7374 7265 616d 2e0a 2020 2020 2020  n stream..      
-0000aeb0: 2020 2222 220a 2020 2020 6465 6620 6c65    """.    def le
-0000aec0: 6176 655f 6a6f 696e 7428 7365 6c66 2920  ave_joint(self) 
-0000aed0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-0000aee0: 2022 2222 0a20 2020 2020 2020 2043 6865   """.        Che
-0000aef0: 636b 7320 6966 2074 6865 2063 6f6e 6669  cks if the confi
-0000af00: 6775 7261 7469 6f6e 2063 6861 6e67 6520  guration change 
-0000af10: 6c65 6176 6573 2061 206a 6f69 6e74 2063  leaves a joint c
-0000af20: 6f6e 6669 6775 7261 7469 6f6e 2e0a 0a20  onfiguration... 
-0000af30: 2020 2020 2020 2054 6869 7320 6973 2074         This is t
-0000af40: 6865 2063 6173 6520 6966 2074 6865 2043  he case if the C
-0000af50: 6f6e 6643 6861 6e67 6556 3220 6973 207a  onfChangeV2 is z
-0000af60: 6572 6f2c 2077 6974 6820 7468 6520 706f  ero, with the po
-0000af70: 7373 6962 6c65 2065 7863 6570 7469 6f6e  ssible exception
-0000af80: 206f 660a 2020 2020 2020 2020 7468 6520   of.        the 
-0000af90: 436f 6e74 6578 7420 6669 656c 642e 0a20  Context field.. 
-0000afa0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000afb0: 6566 2061 735f 7631 2873 656c 6629 202d  ef as_v1(self) -
-0000afc0: 3e20 4f70 7469 6f6e 616c 5b22 436f 6e66  > Optional["Conf
-0000afd0: 4368 616e 6765 5265 6622 5d3a 0a20 2020  ChangeRef"]:.   
-0000afe0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000aff0: 2043 6f6e 7665 7274 7320 636f 6e66 2063   Converts conf c
-0000b000: 6861 6e67 6520 746f 2060 436f 6e66 4368  hange to `ConfCh
-0000b010: 616e 6765 602e 0a0a 2020 2020 2020 2020  ange`...        
-0000b020: 6043 6f6e 6643 6861 6e67 6556 3260 2063  `ConfChangeV2` c
-0000b030: 616e 2774 2062 6520 6368 616e 6765 6420  an't be changed 
-0000b040: 6261 636b 2074 6f20 6043 6f6e 6643 6861  back to `ConfCha
-0000b050: 6e67 6560 2e0a 2020 2020 2020 2020 2222  nge`..        ""
-0000b060: 220a 2020 2020 6465 6620 6173 5f76 3228  ".    def as_v2(
-0000b070: 7365 6c66 2920 2d3e 2022 436f 6e66 4368  self) -> "ConfCh
-0000b080: 616e 6765 5632 223a 0a20 2020 2020 2020  angeV2":.       
-0000b090: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
-0000b0a0: 7320 636f 6e66 2063 6861 6e67 6520 6173  s conf change as
-0000b0b0: 2060 436f 6e66 4368 616e 6765 5632 602e   `ConfChangeV2`.
-0000b0c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000b0d0: 2064 6566 2069 6e74 6f5f 7632 2873 656c   def into_v2(sel
-0000b0e0: 6629 202d 3e20 2243 6f6e 6643 6861 6e67  f) -> "ConfChang
-0000b0f0: 6556 3222 3a0a 2020 2020 2020 2020 2222  eV2":.        ""
-0000b100: 220a 2020 2020 2020 2020 436f 6e76 6572  ".        Conver
-0000b110: 7473 2063 6f6e 6620 6368 616e 6765 2074  ts conf change t
-0000b120: 6f20 6043 6f6e 6643 6861 6e67 6556 3260  o `ConfChangeV2`
-0000b130: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
-0000b140: 6c61 7373 2043 6f6e 6643 6861 6e67 6556  lass ConfChangeV
-0000b150: 3228 5f5f 4150 495f 436f 6e66 4368 616e  2(__API_ConfChan
-0000b160: 6765 5632 293a 0a20 2020 2022 2222 0a20  geV2):.    """. 
-0000b170: 2020 2043 6f6e 6643 6861 6e67 6556 3220     ConfChangeV2 
-0000b180: 6d65 7373 6167 6573 2069 6e69 7469 6174  messages initiat
-0000b190: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-0000b1a0: 6368 616e 6765 732e 2054 6865 7920 7375  changes. They su
-0000b1b0: 7070 6f72 7420 626f 7468 2074 6865 0a20  pport both the. 
-0000b1c0: 2020 2073 696d 706c 6520 226f 6e65 2061     simple "one a
-0000b1d0: 7420 6120 7469 6d65 2220 6d65 6d62 6572  t a time" member
-0000b1e0: 7368 6970 2063 6861 6e67 6520 7072 6f74  ship change prot
-0000b1f0: 6f63 6f6c 2061 6e64 2066 756c 6c20 4a6f  ocol and full Jo
-0000b200: 696e 7420 436f 6e73 656e 7375 730a 2020  int Consensus.  
-0000b210: 2020 616c 6c6f 7769 6e67 2066 6f72 2061    allowing for a
-0000b220: 7262 6974 7261 7279 2063 6861 6e67 6573  rbitrary changes
-0000b230: 2069 6e20 6d65 6d62 6572 7368 6970 2e0a   in membership..
-0000b240: 0a20 2020 2054 6865 2073 7570 706c 6965  .    The supplie
-0000b250: 6420 636f 6e74 6578 7420 6973 2074 7265  d context is tre
-0000b260: 6174 6564 2061 7320 616e 206f 7061 7175  ated as an opaqu
-0000b270: 6520 7061 796c 6f61 6420 616e 6420 6361  e payload and ca
-0000b280: 6e20 6265 2075 7365 6420 746f 0a20 2020  n be used to.   
-0000b290: 2061 7474 6163 6820 616e 2061 6374 696f   attach an actio
-0000b2a0: 6e20 6f6e 2074 6865 2073 7461 7465 206d  n on the state m
-0000b2b0: 6163 6869 6e65 2074 6f20 7468 6520 6170  achine to the ap
-0000b2c0: 706c 6963 6174 696f 6e20 6f66 2074 6865  plication of the
-0000b2d0: 2063 6f6e 6669 6720 6368 616e 6765 0a20   config change. 
-0000b2e0: 2020 2070 726f 706f 7361 6c2e 204e 6f74     proposal. Not
-0000b2f0: 6520 7468 6174 2063 6f6e 7472 6172 7920  e that contrary 
-0000b300: 746f 204a 6f69 6e74 2043 6f6e 7365 6e73  to Joint Consens
-0000b310: 7573 2061 7320 6f75 746c 696e 6564 2069  us as outlined i
-0000b320: 6e20 7468 6520 5261 6674 0a20 2020 2070  n the Raft.    p
-0000b330: 6170 6572 5b31 5d2c 2063 6f6e 6669 6775  aper[1], configu
-0000b340: 7261 7469 6f6e 2063 6861 6e67 6573 2062  ration changes b
-0000b350: 6563 6f6d 6520 6163 7469 7665 2077 6865  ecome active whe
-0000b360: 6e20 7468 6579 2061 7265 202a 6170 706c  n they are *appl
-0000b370: 6965 642a 2074 6f20 7468 650a 2020 2020  ied* to the.    
-0000b380: 7374 6174 6520 6d61 6368 696e 6520 286e  state machine (n
-0000b390: 6f74 2077 6865 6e20 7468 6579 2061 7265  ot when they are
-0000b3a0: 2061 7070 656e 6465 6420 746f 2074 6865   appended to the
-0000b3b0: 206c 6f67 292e 0a0a 2020 2020 5468 6520   log)...    The 
-0000b3c0: 7369 6d70 6c65 2070 726f 746f 636f 6c20  simple protocol 
-0000b3d0: 6361 6e20 6265 2075 7365 6420 7768 656e  can be used when
-0000b3e0: 6576 6572 206f 6e6c 7920 6120 7369 6e67  ever only a sing
-0000b3f0: 6c65 2063 6861 6e67 6520 6973 206d 6164  le change is mad
-0000b400: 652e 0a0a 2020 2020 4e6f 6e2d 7369 6d70  e...    Non-simp
-0000b410: 6c65 2063 6861 6e67 6573 2072 6571 7569  le changes requi
-0000b420: 7265 2074 6865 2075 7365 206f 6620 4a6f  re the use of Jo
-0000b430: 696e 7420 436f 6e73 656e 7375 732c 2066  int Consensus, f
-0000b440: 6f72 2077 6869 6368 2074 776f 0a20 2020  or which two.   
-0000b450: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
-0000b460: 6861 6e67 6573 2061 7265 2072 756e 2e20  hanges are run. 
-0000b470: 5468 6520 6669 7273 7420 636f 6e66 6967  The first config
-0000b480: 7572 6174 696f 6e20 6368 616e 6765 2073  uration change s
-0000b490: 7065 6369 6669 6573 2074 6865 0a20 2020  pecifies the.   
-0000b4a0: 2064 6573 6972 6564 2063 6861 6e67 6573   desired changes
-0000b4b0: 2061 6e64 2074 7261 6e73 6974 696f 6e73   and transitions
-0000b4c0: 2074 6865 2052 6166 7420 6772 6f75 7020   the Raft group 
-0000b4d0: 696e 746f 2074 6865 206a 6f69 6e74 2063  into the joint c
-0000b4e0: 6f6e 6669 6775 7261 7469 6f6e 2c0a 2020  onfiguration,.  
-0000b4f0: 2020 696e 2077 6869 6368 2071 756f 7275    in which quoru
-0000b500: 6d20 7265 7175 6972 6573 2061 206d 616a  m requires a maj
-0000b510: 6f72 6974 7920 6f66 2062 6f74 6820 7468  ority of both th
-0000b520: 6520 7072 652d 6368 616e 6765 7320 616e  e pre-changes an
-0000b530: 6420 706f 7374 2d63 6861 6e67 6573 0a20  d post-changes. 
-0000b540: 2020 2063 6f6e 6669 6775 7261 7469 6f6e     configuration
-0000b550: 2e20 4a6f 696e 7420 436f 6e73 656e 7375  . Joint Consensu
-0000b560: 7320 6176 6f69 6473 2065 6e74 6572 696e  s avoids enterin
-0000b570: 6720 6672 6167 696c 6520 696e 7465 726d  g fragile interm
-0000b580: 6564 6961 7465 0a20 2020 2063 6f6e 6669  ediate.    confi
-0000b590: 6775 7261 7469 6f6e 7320 7468 6174 2063  gurations that c
-0000b5a0: 6f75 6c64 2063 6f6d 7072 6f6d 6973 6520  ould compromise 
-0000b5b0: 7375 7276 6976 6162 696c 6974 792e 2046  survivability. F
-0000b5c0: 6f72 2065 7861 6d70 6c65 2c20 7769 7468  or example, with
-0000b5d0: 6f75 7420 7468 650a 2020 2020 7573 6520  out the.    use 
-0000b5e0: 6f66 204a 6f69 6e74 2043 6f6e 7365 6e73  of Joint Consens
-0000b5f0: 7573 2061 6e64 2072 756e 6e69 6e67 2061  us and running a
-0000b600: 6372 6f73 7320 7468 7265 6520 6176 6169  cross three avai
-0000b610: 6c61 6269 6c69 7479 207a 6f6e 6573 2077  lability zones w
-0000b620: 6974 6820 610a 2020 2020 7265 706c 6963  ith a.    replic
-0000b630: 6174 696f 6e20 6661 6374 6f72 206f 6620  ation factor of 
-0000b640: 7468 7265 652c 2069 7420 6973 206e 6f74  three, it is not
-0000b650: 2070 6f73 7369 626c 6520 746f 2072 6570   possible to rep
-0000b660: 6c61 6365 2061 2076 6f74 6572 2077 6974  lace a voter wit
-0000b670: 686f 7574 0a20 2020 2065 6e74 6572 696e  hout.    enterin
-0000b680: 6720 616e 2069 6e74 6572 6d65 6469 6174  g an intermediat
-0000b690: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-0000b6a0: 7468 6174 2064 6f65 7320 6e6f 7420 7375  that does not su
-0000b6b0: 7276 6976 6520 7468 6520 6f75 7461 6765  rvive the outage
-0000b6c0: 206f 660a 2020 2020 6f6e 6520 6176 6169   of.    one avai
-0000b6d0: 6c61 6269 6c69 7479 207a 6f6e 652e 0a0a  lability zone...
-0000b6e0: 2020 2020 5468 6520 7072 6f76 6964 6564      The provided
-0000b6f0: 2043 6f6e 6643 6861 6e67 6554 7261 6e73   ConfChangeTrans
-0000b700: 6974 696f 6e20 7370 6563 6966 6965 7320  ition specifies 
-0000b710: 686f 7720 2861 6e64 2077 6865 7468 6572  how (and whether
-0000b720: 2920 4a6f 696e 7420 436f 6e73 656e 7375  ) Joint Consensu
-0000b730: 730a 2020 2020 6973 2075 7365 642c 2061  s.    is used, a
-0000b740: 6e64 2061 7373 6967 6e73 2074 6865 2074  nd assigns the t
-0000b750: 6173 6b20 6f66 206c 6561 7669 6e67 2074  ask of leaving t
-0000b760: 6865 206a 6f69 6e74 2063 6f6e 6669 6775  he joint configu
-0000b770: 7261 7469 6f6e 2065 6974 6865 7220 746f  ration either to
-0000b780: 0a20 2020 2052 6166 7420 6f72 2074 6865  .    Raft or the
-0000b790: 2061 7070 6c69 6361 7469 6f6e 2e20 4c65   application. Le
-0000b7a0: 6176 696e 6720 7468 6520 6a6f 696e 7420  aving the joint 
-0000b7b0: 636f 6e66 6967 7572 6174 696f 6e20 6973  configuration is
-0000b7c0: 2061 6363 6f6d 706c 6973 6865 6420 6279   accomplished by
-0000b7d0: 0a20 2020 2070 726f 706f 7369 6e67 2061  .    proposing a
-0000b7e0: 2043 6f6e 6643 6861 6e67 6556 3220 7769   ConfChangeV2 wi
-0000b7f0: 7468 206f 6e6c 7920 616e 6420 6f70 7469  th only and opti
-0000b800: 6f6e 616c 6c79 2074 6865 2043 6f6e 7465  onally the Conte
-0000b810: 7874 2066 6965 6c64 0a20 2020 2070 6f70  xt field.    pop
-0000b820: 756c 6174 6564 2e0a 0a20 2020 2046 6f72  ulated...    For
-0000b830: 2064 6574 6169 6c73 206f 6e20 5261 6674   details on Raft
-0000b840: 206d 656d 6265 7273 6869 7020 6368 616e   membership chan
-0000b850: 6765 732c 2073 6565 3a0a 0a20 2020 205b  ges, see:..    [
-0000b860: 315d 3a20 6874 7470 733a 2f2f 6769 7468  1]: https://gith
-0000b870: 7562 2e63 6f6d 2f6f 6e67 6172 6469 652f  ub.com/ongardie/
-0000b880: 6469 7373 6572 7461 7469 6f6e 2f62 6c6f  dissertation/blo
-0000b890: 622f 6d61 7374 6572 2f6f 6e6c 696e 652d  b/master/online-
-0000b8a0: 7472 696d 2e70 6466 0a20 2020 2022 2222  trim.pdf.    """
-0000b8b0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0000b8c0: 5f5f 2873 656c 6629 202d 3e20 4e6f 6e65  __(self) -> None
-0000b8d0: 3a20 2e2e 2e0a 2020 2020 4073 7461 7469  : ....    @stati
-0000b8e0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-0000b8f0: 6465 6661 756c 7428 2920 2d3e 2022 436f  default() -> "Co
-0000b900: 6e66 4368 616e 6765 5632 223a 202e 2e2e  nfChangeV2": ...
-0000b910: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
-0000b920: 6628 7365 6c66 2920 2d3e 2022 436f 6e66  f(self) -> "Conf
-0000b930: 4368 616e 6765 5632 5265 6622 3a20 2e2e  ChangeV2Ref": ..
-0000b940: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000b950: 686f 640a 2020 2020 6465 6620 6465 636f  hod.    def deco
-0000b960: 6465 2876 3a20 6279 7465 7329 202d 3e20  de(v: bytes) -> 
-0000b970: 2243 6f6e 6643 6861 6e67 6556 3222 3a20  "ConfChangeV2": 
-0000b980: 2e2e 2e0a 0a63 6c61 7373 2043 6f6e 6643  .....class ConfC
-0000b990: 6861 6e67 6556 3252 6566 285f 5f41 5049  hangeV2Ref(__API
-0000b9a0: 5f43 6f6e 6643 6861 6e67 6556 3229 3a0a  _ConfChangeV2):.
-0000b9b0: 2020 2020 2222 220a 2020 2020 5265 6665      """.    Refe
-0000b9c0: 7265 6e63 6520 7479 7065 206f 6620 3a63  rence type of :c
-0000b9d0: 6c61 7373 3a60 436f 6e66 4368 616e 6765  lass:`ConfChange
-0000b9e0: 5632 602e 0a20 2020 2022 2222 0a0a 636c  V2`..    """..cl
-0000b9f0: 6173 7320 5f5f 4150 495f 436f 6e66 4368  ass __API_ConfCh
-0000ba00: 616e 6765 5369 6e67 6c65 285f 5f43 6c6f  angeSingle(__Clo
-0000ba10: 6e65 6162 6c65 2c20 5f5f 456e 636f 6465  neable, __Encode
-0000ba20: 722c 205f 5f44 6563 6f64 6572 293a 0a20  r, __Decoder):. 
-0000ba30: 2020 2064 6566 2063 6c6f 6e65 2873 656c     def clone(sel
-0000ba40: 6629 202d 3e20 2243 6f6e 6643 6861 6e67  f) -> "ConfChang
-0000ba50: 6553 696e 676c 6522 3a20 2e2e 2e0a 2020  eSingle": ....  
-0000ba60: 2020 6465 6620 6765 745f 6e6f 6465 5f69    def get_node_i
-0000ba70: 6428 7365 6c66 2920 2d3e 2069 6e74 3a0a  d(self) -> int:.
-0000ba80: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
-0000ba90: 2020 2020 6465 6620 7365 745f 6e6f 6465      def set_node
-0000baa0: 5f69 6428 7365 6c66 2c20 6e6f 6465 5f69  _id(self, node_i
-0000bab0: 643a 2069 6e74 293a 0a20 2020 2020 2020  d: int):.       
-0000bac0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000bad0: 2063 6c65 6172 5f6e 6f64 655f 6964 2873   clear_node_id(s
-0000bae0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-0000baf0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-0000bb00: 2020 6465 6620 6765 745f 6368 616e 6765    def get_change
-0000bb10: 5f74 7970 6528 7365 6c66 2920 2d3e 2022  _type(self) -> "
-0000bb20: 436f 6e66 4368 616e 6765 5479 7065 223a  ConfChangeType":
-0000bb30: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-0000bb40: 0a20 2020 2064 6566 2073 6574 5f63 6861  .    def set_cha
-0000bb50: 6e67 655f 7479 7065 2873 656c 662c 2074  nge_type(self, t
-0000bb60: 7970 3a20 2243 6f6e 6643 6861 6e67 6554  yp: "ConfChangeT
-0000bb70: 7970 6522 2920 2d3e 204e 6f6e 653a 0a20  ype") -> None:. 
-0000bb80: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-0000bb90: 2020 2064 6566 2063 6c65 6172 5f63 6861     def clear_cha
-0000bba0: 6e67 655f 7479 7065 2873 656c 6629 202d  nge_type(self) -
-0000bbb0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-0000bbc0: 2222 2220 2222 220a 0a63 6c61 7373 2043  """ """..class C
-0000bbd0: 6f6e 6643 6861 6e67 6553 696e 676c 6528  onfChangeSingle(
-0000bbe0: 5f5f 4150 495f 436f 6e66 4368 616e 6765  __API_ConfChange
-0000bbf0: 5369 6e67 6c65 293a 0a20 2020 2022 2222  Single):.    """
-0000bc00: 0a20 2020 2043 6f6e 6643 6861 6e67 6553  .    ConfChangeS
-0000bc10: 696e 676c 6520 6973 2061 6e20 696e 6469  ingle is an indi
-0000bc20: 7669 6475 616c 2063 6f6e 6669 6775 7261  vidual configura
-0000bc30: 7469 6f6e 2063 6861 6e67 6520 6f70 6572  tion change oper
-0000bc40: 6174 696f 6e2e 204d 756c 7469 706c 650a  ation. Multiple.
-0000bc50: 2020 2020 7375 6368 206f 7065 7261 7469      such operati
-0000bc60: 6f6e 7320 6361 6e20 6265 2063 6172 7269  ons can be carri
-0000bc70: 6564 206f 7574 2061 746f 6d69 6361 6c6c  ed out atomicall
-0000bc80: 7920 7669 6120 6120 436f 6e66 4368 616e  y via a ConfChan
-0000bc90: 6765 5632 2e0a 2020 2020 2222 220a 0a20  geV2..    """.. 
-0000bca0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000bcb0: 7365 6c66 2920 2d3e 204e 6f6e 653a 202e  self) -> None: .
-0000bcc0: 2e2e 0a20 2020 2064 6566 206d 616b 655f  ...    def make_
-0000bcd0: 7265 6628 7365 6c66 2920 2d3e 2022 436f  ref(self) -> "Co
-0000bce0: 6e66 4368 616e 6765 5369 6e67 6c65 5265  nfChangeSingleRe
-0000bcf0: 6622 3a20 2e2e 2e0a 2020 2020 4073 7461  f": ....    @sta
-0000bd00: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0000bd10: 6620 6465 6661 756c 7428 2920 2d3e 2022  f default() -> "
-0000bd20: 436f 6e66 4368 616e 6765 5369 6e67 6c65  ConfChangeSingle
-0000bd30: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
-0000bd40: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-0000bd50: 2064 6563 6f64 6528 763a 2062 7974 6573   decode(v: bytes
-0000bd60: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000bd70: 5369 6e67 6c65 223a 202e 2e2e 0a0a 636c  Single": .....cl
-0000bd80: 6173 7320 436f 6e66 4368 616e 6765 5369  ass ConfChangeSi
-0000bd90: 6e67 6c65 5265 6628 5f5f 4150 495f 436f  ngleRef(__API_Co
-0000bda0: 6e66 4368 616e 6765 5369 6e67 6c65 293a  nfChangeSingle):
-0000bdb0: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
-0000bdc0: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
-0000bdd0: 636c 6173 733a 6043 6f6e 6643 6861 6e67  class:`ConfChang
-0000bde0: 6553 696e 676c 6560 2e0a 2020 2020 2222  eSingle`..    ""
-0000bdf0: 220a 0a63 6c61 7373 205f 5f41 5049 5f43  "..class __API_C
-0000be00: 6f6e 6643 6861 6e67 6528 5f5f 436c 6f6e  onfChange(__Clon
-0000be10: 6561 626c 652c 205f 5f45 6e63 6f64 6572  eable, __Encoder
-0000be20: 2c20 5f5f 4465 636f 6465 7229 3a0a 2020  , __Decoder):.  
-0000be30: 2020 6465 6620 636c 6f6e 6528 7365 6c66    def clone(self
-0000be40: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000be50: 223a 202e 2e2e 0a20 2020 2064 6566 2067  ": ....    def g
-0000be60: 6574 5f69 6428 7365 6c66 2920 2d3e 2069  et_id(self) -> i
-0000be70: 6e74 3a0a 2020 2020 2020 2020 2222 2220  nt:.        """ 
-0000be80: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-0000be90: 6964 2873 656c 662c 2069 643a 2069 6e74  id(self, id: int
-0000bea0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000beb0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-0000bec0: 6566 2063 6c65 6172 5f69 6428 7365 6c66  ef clear_id(self
-0000bed0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000bee0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-0000bef0: 6566 2067 6574 5f6e 6f64 655f 6964 2873  ef get_node_id(s
-0000bf00: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-0000bf10: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000bf20: 2064 6566 2073 6574 5f6e 6f64 655f 6964   def set_node_id
-0000bf30: 2873 656c 662c 206e 6f64 655f 6964 3a20  (self, node_id: 
-0000bf40: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-0000bf50: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
-0000bf60: 2020 6465 6620 636c 6561 725f 6e6f 6465    def clear_node
-0000bf70: 5f69 6428 7365 6c66 2920 2d3e 204e 6f6e  _id(self) -> Non
-0000bf80: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
-0000bf90: 2222 0a20 2020 2064 6566 2067 6574 5f63  "".    def get_c
-0000bfa0: 6861 6e67 655f 7479 7065 2873 656c 6629  hange_type(self)
-0000bfb0: 202d 3e20 2243 6f6e 6643 6861 6e67 6554   -> "ConfChangeT
-0000bfc0: 7970 6522 3a0a 2020 2020 2020 2020 2222  ype":.        ""
-0000bfd0: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
-0000bfe0: 745f 6368 616e 6765 5f74 7970 6528 7365  t_change_type(se
-0000bff0: 6c66 2c20 7479 703a 2022 436f 6e66 4368  lf, typ: "ConfCh
-0000c000: 616e 6765 5479 7065 2229 202d 3e20 4e6f  angeType") -> No
-0000c010: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000c020: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-0000c030: 725f 6368 616e 6765 5f74 7970 6528 7365  r_change_type(se
-0000c040: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-0000c050: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
-0000c060: 2064 6566 2067 6574 5f63 6f6e 7465 7874   def get_context
-0000c070: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
-0000c080: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
-0000c090: 0a20 2020 2064 6566 2073 6574 5f63 6f6e  .    def set_con
-0000c0a0: 7465 7874 2873 656c 662c 2063 6f6e 7465  text(self, conte
-0000c0b0: 7874 3a20 6279 7465 7329 202d 3e20 4e6f  xt: bytes) -> No
-0000c0c0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
-0000c0d0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-0000c0e0: 725f 636f 6e74 6578 7428 7365 6c66 2920  r_context(self) 
-0000c0f0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000c100: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-0000c110: 206d 6572 6765 5f66 726f 6d5f 6279 7465   merge_from_byte
-0000c120: 7328 7365 6c66 2c20 623a 2062 7974 6573  s(self, b: bytes
-0000c130: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000c140: 2020 2022 2222 0a20 2020 2020 2020 2055     """.        U
-0000c150: 7064 6174 6520 7468 6973 206d 6573 7361  pdate this messa
-0000c160: 6765 206f 626a 6563 7420 7769 7468 2066  ge object with f
-0000c170: 6965 6c64 7320 7265 6164 2066 726f 6d20  ields read from 
-0000c180: 6769 7665 6e20 7374 7265 616d 2e0a 2020  given stream..  
-0000c190: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000c1a0: 6620 6173 5f76 3128 7365 6c66 2920 2d3e  f as_v1(self) ->
-0000c1b0: 204f 7074 696f 6e61 6c5b 2243 6f6e 6643   Optional["ConfC
-0000c1c0: 6861 6e67 6552 6566 225d 3a0a 2020 2020  hangeRef"]:.    
-0000c1d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000c1e0: 436f 6e76 6572 7473 2063 6f6e 6620 6368  Converts conf ch
-0000c1f0: 616e 6765 2074 6f20 6043 6f6e 6643 6861  ange to `ConfCha
-0000c200: 6e67 6560 2e0a 0a20 2020 2020 2020 2060  nge`...        `
-0000c210: 436f 6e66 4368 616e 6765 5632 6020 6361  ConfChangeV2` ca
-0000c220: 6e27 7420 6265 2063 6861 6e67 6564 2062  n't be changed b
-0000c230: 6163 6b20 746f 2060 436f 6e66 4368 616e  ack to `ConfChan
-0000c240: 6765 602e 0a20 2020 2020 2020 2022 2222  ge`..        """
-0000c250: 0a20 2020 2064 6566 2061 735f 7632 2873  .    def as_v2(s
-0000c260: 656c 6629 202d 3e20 2243 6f6e 6643 6861  elf) -> "ConfCha
-0000c270: 6e67 6556 3222 3a0a 2020 2020 2020 2020  ngeV2":.        
-0000c280: 2222 220a 2020 2020 2020 2020 4765 7473  """.        Gets
-0000c290: 2063 6f6e 6620 6368 616e 6765 2061 7320   conf change as 
-0000c2a0: 6043 6f6e 6643 6861 6e67 6556 3260 2e0a  `ConfChangeV2`..
-0000c2b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c2c0: 6465 6620 696e 746f 5f76 3228 7365 6c66  def into_v2(self
-0000c2d0: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
-0000c2e0: 5632 223a 0a20 2020 2020 2020 2022 2222  V2":.        """
-0000c2f0: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-0000c300: 7320 636f 6e66 2063 6861 6e67 6520 746f  s conf change to
-0000c310: 2060 436f 6e66 4368 616e 6765 5632 602e   `ConfChangeV2`.
-0000c320: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
-0000c330: 6173 7320 436f 6e66 4368 616e 6765 285f  ass ConfChange(_
-0000c340: 5f41 5049 5f43 6f6e 6643 6861 6e67 6529  _API_ConfChange)
-0000c350: 3a0a 2020 2020 2222 2220 2222 220a 0a20  :.    """ """.. 
-0000c360: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000c370: 7365 6c66 2920 2d3e 204e 6f6e 653a 202e  self) -> None: .
-0000c380: 2e2e 0a20 2020 2064 6566 206d 616b 655f  ...    def make_
-0000c390: 7265 6628 7365 6c66 2920 2d3e 2022 436f  ref(self) -> "Co
-0000c3a0: 6e66 4368 616e 6765 5265 6622 3a20 2e2e  nfChangeRef": ..
-0000c3b0: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000c3c0: 686f 640a 2020 2020 6465 6620 6465 6661  hod.    def defa
-0000c3d0: 756c 7428 2920 2d3e 2022 436f 6e66 4368  ult() -> "ConfCh
-0000c3e0: 616e 6765 223a 202e 2e2e 0a20 2020 2040  ange": ....    @
-0000c3f0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-0000c400: 2064 6566 2064 6563 6f64 6528 763a 2062   def decode(v: b
-0000c410: 7974 6573 2920 2d3e 2022 436f 6e66 4368  ytes) -> "ConfCh
-0000c420: 616e 6765 223a 202e 2e2e 0a0a 636c 6173  ange": .....clas
-0000c430: 7320 436f 6e66 4368 616e 6765 5265 6628  s ConfChangeRef(
-0000c440: 5f5f 4150 495f 436f 6e66 4368 616e 6765  __API_ConfChange
-0000c450: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
-0000c460: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
-0000c470: 203a 636c 6173 733a 6043 6f6e 6643 6861   :class:`ConfCha
-0000c480: 6e67 6560 2e0a 2020 2020 2222 220a 0a63  nge`..    """..c
-0000c490: 6c61 7373 205f 5f41 5049 5f55 6e73 7461  lass __API_Unsta
-0000c4a0: 626c 653a 0a20 2020 2064 6566 206d 6179  ble:.    def may
-0000c4b0: 6265 5f66 6972 7374 5f69 6e64 6578 2873  be_first_index(s
-0000c4c0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
-0000c4d0: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
-0000c4e0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-0000c4f0: 6e73 2074 6865 2069 6e64 6578 206f 6620  ns the index of 
-0000c500: 7468 6520 6669 7273 7420 706f 7373 6962  the first possib
-0000c510: 6c65 2065 6e74 7279 2069 6e20 656e 7472  le entry in entr
-0000c520: 6965 730a 2020 2020 2020 2020 6966 2069  ies.        if i
-0000c530: 7420 6861 7320 6120 736e 6170 7368 6f74  t has a snapshot
-0000c540: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000c550: 2020 6465 6620 6d61 7962 655f 6c61 7374    def maybe_last
-0000c560: 5f69 6e64 6578 2873 656c 6629 202d 3e20  _index(self) -> 
-0000c570: 4f70 7469 6f6e 616c 5b69 6e74 5d3a 0a20  Optional[int]:. 
-0000c580: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c590: 2020 2052 6574 7572 6e73 2074 6865 206c     Returns the l
-0000c5a0: 6173 7420 696e 6465 7820 6966 2069 7420  ast index if it 
-0000c5b0: 6861 7320 6174 206c 6561 7374 206f 6e65  has at least one
-0000c5c0: 2075 6e73 7461 626c 6520 656e 7472 7920   unstable entry 
-0000c5d0: 6f72 2073 6e61 7073 686f 742e 0a20 2020  or snapshot..   
-0000c5e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000c5f0: 206d 6179 6265 5f74 6572 6d28 7365 6c66   maybe_term(self
-0000c600: 2920 2d3e 204f 7074 696f 6e61 6c5b 696e  ) -> Optional[in
-0000c610: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-0000c620: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-0000c630: 7468 6520 7465 726d 206f 6620 7468 6520  the term of the 
-0000c640: 656e 7472 7920 6174 2069 6e64 6578 2069  entry at index i
-0000c650: 6478 2c20 6966 2074 6865 7265 2069 7320  dx, if there is 
-0000c660: 616e 792e 0a20 2020 2020 2020 2022 2222  any..        """
-0000c670: 0a20 2020 2064 6566 206d 7573 745f 6368  .    def must_ch
-0000c680: 6563 6b5f 6f75 746f 6662 6f75 6e64 7328  eck_outofbounds(
-0000c690: 7365 6c66 2c20 6c6f 3a20 696e 742c 2068  self, lo: int, h
-0000c6a0: 693a 2069 6e74 2920 2d3e 204e 6f6e 653a  i: int) -> None:
-0000c6b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c6c0: 2020 2020 2041 7373 6572 7473 2074 6865       Asserts the
-0000c6d0: 2060 6869 6020 616e 6420 606c 6f60 2076   `hi` and `lo` v
-0000c6e0: 616c 7565 7320 6167 6169 6e73 7420 6561  alues against ea
-0000c6f0: 6368 206f 7468 6572 2061 6e64 2061 6761  ch other and aga
-0000c700: 696e 7374 2074 6865 0a20 2020 2020 2020  inst the.       
-0000c710: 2065 6e74 7269 6573 2074 6865 6d73 656c   entries themsel
-0000c720: 7665 732e 0a20 2020 2020 2020 2022 2222  ves..        """
-0000c730: 0a20 2020 2064 6566 2073 6c69 6365 2873  .    def slice(s
-0000c740: 656c 662c 206c 6f3a 2069 6e74 2c20 6869  elf, lo: int, hi
-0000c750: 3a20 696e 7429 202d 3e20 4c69 7374 5b22  : int) -> List["
-0000c760: 456e 7472 7952 6566 225d 3a0a 2020 2020  EntryRef"]:.    
-0000c770: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000c780: 5265 7475 726e 7320 6120 736c 6963 6520  Returns a slice 
-0000c790: 6f66 2065 6e74 7269 6573 2062 6574 7765  of entries betwe
-0000c7a0: 656e 2074 6865 2068 6967 6820 616e 6420  en the high and 
-0000c7b0: 6c6f 772e 0a0a 2020 2020 2020 2020 2320  low...        # 
-0000c7c0: 5061 6e69 6373 0a0a 2020 2020 2020 2020  Panics..        
-0000c7d0: 5061 6e69 6373 2069 6620 7468 6520 606c  Panics if the `l
-0000c7e0: 6f60 206f 7220 6068 6960 2061 7265 206f  o` or `hi` are o
-0000c7f0: 7574 206f 6620 626f 756e 6473 2e0a 2020  ut of bounds..  
-0000c800: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
-0000c810: 606c 6f20 3e20 6869 602e 0a20 2020 2020  `lo > hi`..     
-0000c820: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
-0000c830: 7461 626c 655f 736e 6170 2873 656c 662c  table_snap(self,
-0000c840: 2069 6e64 6578 3a20 696e 7429 202d 3e20   index: int) -> 
-0000c850: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000c860: 220a 2020 2020 2020 2020 436c 6561 7273  ".        Clears
-0000c870: 2074 6865 2075 6e73 7461 626c 6520 736e   the unstable sn
-0000c880: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
-0000c890: 2222 220a 2020 2020 6465 6620 7374 6162  """.    def stab
-0000c8a0: 6c65 5f65 6e74 7269 6573 2873 656c 662c  le_entries(self,
-0000c8b0: 2069 6e64 6578 3a20 696e 742c 2074 6572   index: int, ter
-0000c8c0: 6d3a 2069 6e74 2920 2d3e 204e 6f6e 653a  m: int) -> None:
-0000c8d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c8e0: 2020 2020 2043 6c65 6172 7320 7468 6520       Clears the 
-0000c8f0: 756e 7374 6162 6c65 2065 6e74 7269 6573  unstable entries
-0000c900: 2061 6e64 206d 6f76 6573 2074 6865 2073   and moves the s
-0000c910: 7461 626c 6520 6f66 6673 6574 2075 7020  table offset up 
-0000c920: 746f 2074 6865 0a20 2020 2020 2020 206c  to the.        l
-0000c930: 6173 7420 696e 6465 782c 2069 6620 7468  ast index, if th
-0000c940: 6572 6520 6973 2061 6e79 2e0a 2020 2020  ere is any..    
-0000c950: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000c960: 7265 7374 6f72 6528 7365 6c66 2c20 736e  restore(self, sn
-0000c970: 6170 3a20 2253 6e61 7073 686f 7452 6566  ap: "SnapshotRef
-0000c980: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
-0000c990: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000c9a0: 4672 6f6d 2061 2067 6976 656e 2073 6e61  From a given sna
-0000c9b0: 7073 686f 742c 2072 6573 746f 7265 7320  pshot, restores 
-0000c9c0: 7468 6520 736e 6170 7368 6f74 2074 6f20  the snapshot to 
-0000c9d0: 7365 6c66 2c20 6275 7420 646f 6573 6e27  self, but doesn'
-0000c9e0: 7420 756e 7061 636b 2e0a 2020 2020 2020  t unpack..      
-0000c9f0: 2020 2222 220a 2020 2020 6465 6620 7472    """.    def tr
-0000ca00: 756e 6361 7465 5f61 6e64 5f61 7070 656e  uncate_and_appen
-0000ca10: 6428 7365 6c66 2c20 656e 7473 3a20 4c69  d(self, ents: Li
-0000ca20: 7374 5b22 456e 7472 7922 5d20 7c20 4c69  st["Entry"] | Li
-0000ca30: 7374 5b22 456e 7472 7952 6566 225d 2920  st["EntryRef"]) 
-0000ca40: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000ca50: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
-0000ca60: 656e 6420 656e 7472 6965 7320 746f 2075  end entries to u
-0000ca70: 6e73 7461 626c 652c 2074 7275 6e63 6174  nstable, truncat
-0000ca80: 6520 6c6f 6361 6c20 626c 6f63 6b20 6669  e local block fi
-0000ca90: 7273 7420 6966 206f 7665 726c 6170 7065  rst if overlappe
-0000caa0: 642e 0a0a 2020 2020 2020 2020 2320 5061  d...        # Pa
-0000cab0: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
-0000cac0: 6e69 6373 2069 6620 7472 756e 6361 7465  nics if truncate
-0000cad0: 206c 6f67 7320 746f 2074 6865 2065 6e74   logs to the ent
-0000cae0: 7279 2062 6566 6f72 6520 736e 6170 7368  ry before snapsh
-0000caf0: 6f74 0a20 2020 2020 2020 2022 2222 0a20  ot.        """. 
-0000cb00: 2020 2064 6566 2067 6574 5f65 6e74 7269     def get_entri
-0000cb10: 6573 5f73 697a 6528 7365 6c66 2920 2d3e  es_size(self) ->
-0000cb20: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000cb30: 220a 2020 2020 2020 2020 6065 6e74 7269  ".        `entri
-0000cb40: 6573 5f73 697a 6560 3a20 5468 6520 7369  es_size`: The si
-0000cb50: 7a65 206f 6620 656e 7472 6965 730a 2020  ze of entries.  
-0000cb60: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000cb70: 6620 7365 745f 656e 7472 6965 735f 7369  f set_entries_si
-0000cb80: 7a65 2873 656c 662c 2065 6e74 7269 6573  ze(self, entries
-0000cb90: 5f73 697a 653a 2069 6e74 2920 2d3e 204e  _size: int) -> N
-0000cba0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000cbb0: 0a20 2020 2020 2020 2060 656e 7472 6965  .        `entrie
-0000cbc0: 735f 7369 7a65 603a 2054 6865 2073 697a  s_size`: The siz
-0000cbd0: 6520 6f66 2065 6e74 7269 6573 0a20 2020  e of entries.   
-0000cbe0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000cbf0: 2067 6574 5f6f 6666 7365 7428 7365 6c66   get_offset(self
-0000cc00: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-0000cc10: 2020 2222 220a 2020 2020 2020 2020 606f    """.        `o
-0000cc20: 6666 7365 7460 3a20 5468 6520 6f66 6673  ffset`: The offs
-0000cc30: 6574 2066 726f 6d20 7468 6520 7665 6374  et from the vect
-0000cc40: 6f72 2069 6e64 6578 2e0a 2020 2020 2020  or index..      
-0000cc50: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-0000cc60: 745f 6f66 6673 6574 2873 656c 662c 206f  t_offset(self, o
-0000cc70: 6666 7365 743a 2069 6e74 2920 2d3e 204e  ffset: int) -> N
-0000cc80: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000cc90: 0a20 2020 2020 2020 2060 6f66 6673 6574  .        `offset
-0000cca0: 603a 2054 6865 206f 6666 7365 7420 6672  `: The offset fr
-0000ccb0: 6f6d 2074 6865 2076 6563 746f 7220 696e  om the vector in
-0000ccc0: 6465 782e 0a20 2020 2020 2020 2022 2222  dex..        """
-0000ccd0: 0a20 2020 2064 6566 2067 6574 5f65 6e74  .    def get_ent
-0000cce0: 7269 6573 2873 656c 6629 202d 3e20 4c69  ries(self) -> Li
-0000ccf0: 7374 5b22 456e 7472 7952 6566 225d 3a0a  st["EntryRef"]:.
-0000cd00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000cd10: 2020 2020 6065 6e74 7269 6573 603a 2041      `entries`: A
-0000cd20: 6c6c 2065 6e74 7269 6573 2074 6861 7420  ll entries that 
-0000cd30: 6861 7665 206e 6f74 2079 6574 2062 6565  have not yet bee
-0000cd40: 6e20 7772 6974 7465 6e20 746f 2073 746f  n written to sto
-0000cd50: 7261 6765 2e0a 2020 2020 2020 2020 2222  rage..        ""
-0000cd60: 220a 2020 2020 6465 6620 7365 745f 656e  ".    def set_en
-0000cd70: 7472 6965 7328 7365 6c66 2c20 656e 7473  tries(self, ents
-0000cd80: 3a20 4c69 7374 5b22 456e 7472 7922 5d20  : List["Entry"] 
-0000cd90: 7c20 4c69 7374 5b22 456e 7472 7952 6566  | List["EntryRef
-0000cda0: 225d 2920 2d3e 204e 6f6e 653a 0a20 2020  "]) -> None:.   
-0000cdb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000cdc0: 2060 656e 7472 6965 7360 3a20 416c 6c20   `entries`: All 
-0000cdd0: 656e 7472 6965 7320 7468 6174 2068 6176  entries that hav
-0000cde0: 6520 6e6f 7420 7965 7420 6265 656e 2077  e not yet been w
-0000cdf0: 7269 7474 656e 2074 6f20 7374 6f72 6167  ritten to storag
-0000ce00: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-0000ce10: 2020 2064 6566 2067 6574 5f6c 6f67 6765     def get_logge
-0000ce20: 7228 7365 6c66 2920 2d3e 2022 4c6f 6767  r(self) -> "Logg
-0000ce30: 6572 5265 6622 3a0a 2020 2020 2020 2020  erRef":.        
-0000ce40: 2222 220a 2020 2020 2020 2020 606c 6f67  """.        `log
-0000ce50: 6765 7260 3a20 5468 6520 7461 6720 746f  ger`: The tag to
-0000ce60: 2075 7365 2077 6865 6e20 6c6f 6767 696e   use when loggin
-0000ce70: 672e 0a20 2020 2020 2020 2022 2222 0a20  g..        """. 
-0000ce80: 2020 2064 6566 2073 6574 5f6c 6f67 6765     def set_logge
-0000ce90: 7228 7365 6c66 2c20 6c6f 6767 6572 3a20  r(self, logger: 
-0000cea0: 224c 6f67 6765 7222 207c 2022 4c6f 6767  "Logger" | "Logg
-0000ceb0: 6572 5265 6622 2920 2d3e 204e 6f6e 653a  erRef") -> None:
-0000cec0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ced0: 2020 2020 2060 6c6f 6767 6572 603a 2054       `logger`: T
-0000cee0: 6865 2074 6167 2074 6f20 7573 6520 7768  he tag to use wh
-0000cef0: 656e 206c 6f67 6769 6e67 2e0a 2020 2020  en logging..    
-0000cf00: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000cf10: 6765 745f 736e 6170 7368 6f74 2873 656c  get_snapshot(sel
-0000cf20: 6629 202d 3e20 4f70 7469 6f6e 616c 5b22  f) -> Optional["
-0000cf30: 536e 6170 7368 6f74 5265 6622 5d3a 0a20  SnapshotRef"]:. 
-0000cf40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cf50: 2020 2060 736e 6170 7368 6f74 603a 2054     `snapshot`: T
-0000cf60: 6865 2069 6e63 6f6d 696e 6720 756e 7374  he incoming unst
-0000cf70: 6162 6c65 2073 6e61 7073 686f 742c 2069  able snapshot, i
-0000cf80: 6620 616e 792e 0a20 2020 2020 2020 2022  f any..        "
-0000cf90: 2222 0a20 2020 2064 6566 2073 6574 5f73  "".    def set_s
-0000cfa0: 6e61 7073 686f 7428 7365 6c66 2c20 736e  napshot(self, sn
-0000cfb0: 6170 7368 6f74 3a20 2253 6e61 7073 686f  apshot: "Snapsho
-0000cfc0: 7422 207c 2022 536e 6170 7368 6f74 5265  t" | "SnapshotRe
-0000cfd0: 6622 2920 2d3e 204e 6f6e 653a 0a20 2020  f") -> None:.   
-0000cfe0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000cff0: 2060 736e 6170 7368 6f74 603a 2054 6865   `snapshot`: The
-0000d000: 2069 6e63 6f6d 696e 6720 756e 7374 6162   incoming unstab
-0000d010: 6c65 2073 6e61 7073 686f 742c 2069 6620  le snapshot, if 
-0000d020: 616e 792e 0a20 2020 2020 2020 2022 2222  any..        """
-0000d030: 0a0a 636c 6173 7320 556e 7374 6162 6c65  ..class Unstable
-0000d040: 285f 5f41 5049 5f55 6e73 7461 626c 6529  (__API_Unstable)
-0000d050: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-0000d060: 6520 6075 6e73 7461 626c 652e 656e 7472  e `unstable.entr
-0000d070: 6965 735b 695d 6020 6861 7320 7261 6674  ies[i]` has raft
-0000d080: 206c 6f67 2070 6f73 6974 696f 6e20 6069   log position `i
-0000d090: 2b75 6e73 7461 626c 652e 6f66 6673 6574  +unstable.offset
-0000d0a0: 602e 0a20 2020 204e 6f74 6520 7468 6174  `..    Note that
-0000d0b0: 2060 756e 7374 6162 6c65 2e6f 6666 7365   `unstable.offse
-0000d0c0: 7460 206d 6179 2062 6520 6c65 7373 2074  t` may be less t
-0000d0d0: 6861 6e20 7468 6520 6869 6768 6573 7420  han the highest 
-0000d0e0: 6c6f 670a 2020 2020 706f 7369 7469 6f6e  log.    position
-0000d0f0: 2069 6e20 7374 6f72 6167 653b 2074 6869   in storage; thi
-0000d100: 7320 6d65 616e 7320 7468 6174 2074 6865  s means that the
-0000d110: 206e 6578 7420 7772 6974 6520 746f 2073   next write to s
-0000d120: 746f 7261 6765 0a20 2020 206d 6967 6874  torage.    might
-0000d130: 206e 6565 6420 746f 2074 7275 6e63 6174   need to truncat
-0000d140: 6520 7468 6520 6c6f 6720 6265 666f 7265  e the log before
-0000d150: 2070 6572 7369 7374 696e 6720 756e 7374   persisting unst
-0000d160: 6162 6c65 2e65 6e74 7269 6573 2e0a 2020  able.entries..  
-0000d170: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-0000d180: 5f69 6e69 745f 5f28 7365 6c66 2c20 6f66  _init__(self, of
-0000d190: 6673 6574 3a20 696e 742c 206c 6f67 6765  fset: int, logge
-0000d1a0: 723a 2022 4c6f 6767 6572 2220 7c20 224c  r: "Logger" | "L
-0000d1b0: 6f67 6765 7252 6566 2229 202d 3e20 4e6f  oggerRef") -> No
-0000d1c0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-0000d1d0: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-0000d1e0: 3e20 2255 6e73 7461 626c 6552 6566 223a  > "UnstableRef":
-0000d1f0: 202e 2e2e 0a0a 636c 6173 7320 556e 7374   .....class Unst
-0000d200: 6162 6c65 5265 6628 5f5f 4150 495f 556e  ableRef(__API_Un
-0000d210: 7374 6162 6c65 293a 0a20 2020 2022 2222  stable):.    """
-0000d220: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
-0000d230: 7970 6520 6f66 203a 636c 6173 733a 6055  ype of :class:`U
-0000d240: 6e73 7461 626c 6560 2e0a 2020 2020 2222  nstable`..    ""
-0000d250: 220a 0a63 6c61 7373 205f 5f41 5049 5f53  "..class __API_S
-0000d260: 6f66 7453 7461 7465 3a0a 2020 2020 6465  oftState:.    de
-0000d270: 6620 6765 745f 6c65 6164 6572 5f69 6428  f get_leader_id(
-0000d280: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-0000d290: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d2a0: 2020 606c 6561 6465 725f 6964 603a 2054    `leader_id`: T
-0000d2b0: 6865 2070 6f74 656e 7469 616c 206c 6561  he potential lea
-0000d2c0: 6465 7220 6f66 2074 6865 2063 6c75 7374  der of the clust
-0000d2d0: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
-0000d2e0: 2020 2020 6465 6620 7365 745f 6c65 6164      def set_lead
-0000d2f0: 6572 5f69 6428 7365 6c66 2c20 6c65 6164  er_id(self, lead
-0000d300: 6572 5f69 643a 2069 6e74 2920 2d3e 204e  er_id: int) -> N
-0000d310: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000d320: 0a20 2020 2020 2020 2060 6c65 6164 6572  .        `leader
-0000d330: 5f69 6460 3a20 5468 6520 706f 7465 6e74  _id`: The potent
-0000d340: 6961 6c20 6c65 6164 6572 206f 6620 7468  ial leader of th
-0000d350: 6520 636c 7573 7465 722e 0a20 2020 2020  e cluster..     
-0000d360: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-0000d370: 6574 5f72 6166 745f 7374 6174 6528 7365  et_raft_state(se
-0000d380: 6c66 2920 2d3e 2022 5374 6174 6552 6f6c  lf) -> "StateRol
-0000d390: 6522 3a0a 2020 2020 2020 2020 2222 220a  e":.        """.
-0000d3a0: 2020 2020 2020 2020 6072 6166 745f 7374          `raft_st
-0000d3b0: 6174 6560 3a20 5468 6520 736f 6674 2072  ate`: The soft r
-0000d3c0: 6f6c 6520 7468 6973 206e 6f64 6520 6d61  ole this node ma
-0000d3d0: 7920 7461 6b65 2e0a 2020 2020 2020 2020  y take..        
-0000d3e0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-0000d3f0: 7261 6674 5f73 7461 7465 2873 656c 662c  raft_state(self,
-0000d400: 2072 6f6c 653a 2022 5374 6174 6552 6f6c   role: "StateRol
-0000d410: 6522 2920 2d3e 204e 6f6e 653a 0a20 2020  e") -> None:.   
-0000d420: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000d430: 2060 7261 6674 5f73 7461 7465 603a 2054   `raft_state`: T
-0000d440: 6865 2073 6f66 7420 726f 6c65 2074 6869  he soft role thi
-0000d450: 7320 6e6f 6465 206d 6179 2074 616b 652e  s node may take.
-0000d460: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
-0000d470: 6173 7320 536f 6674 5374 6174 6528 5f5f  ass SoftState(__
-0000d480: 4150 495f 536f 6674 5374 6174 6529 3a0a  API_SoftState):.
-0000d490: 2020 2020 2222 220a 2020 2020 536f 6674      """.    Soft
-0000d4a0: 5374 6174 6520 7072 6f76 6964 6573 2073  State provides s
-0000d4b0: 7461 7465 2074 6861 7420 6973 2075 7365  tate that is use
-0000d4c0: 6675 6c20 666f 7220 6c6f 6767 696e 6720  ful for logging 
-0000d4d0: 616e 6420 6465 6275 6767 696e 672e 0a20  and debugging.. 
-0000d4e0: 2020 2054 6865 2073 7461 7465 2069 7320     The state is 
-0000d4f0: 766f 6c61 7469 6c65 2061 6e64 2064 6f65  volatile and doe
-0000d500: 7320 6e6f 7420 6e65 6564 2074 6f20 6265  s not need to be
-0000d510: 2070 6572 7369 7374 6564 2074 6f20 7468   persisted to th
-0000d520: 6520 5741 4c2e 0a20 2020 2022 2222 0a0a  e WAL..    """..
-0000d530: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
-0000d540: 2873 656c 6629 202d 3e20 2253 6f66 7453  (self) -> "SoftS
-0000d550: 7461 7465 5265 6622 3a20 2e2e 2e0a 2020  tateRef": ....  
-0000d560: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-0000d570: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
-0000d580: 2920 2d3e 2022 536f 6674 5374 6174 6522  ) -> "SoftState"
-0000d590: 3a20 2e2e 2e0a 0a63 6c61 7373 2053 6f66  : .....class Sof
-0000d5a0: 7453 7461 7465 5265 6628 5f5f 4150 495f  tStateRef(__API_
-0000d5b0: 536f 6674 5374 6174 6529 3a0a 2020 2020  SoftState):.    
-0000d5c0: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
-0000d5d0: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
-0000d5e0: 3a60 536f 6674 5374 6174 6560 2e0a 2020  :`SoftState`..  
-0000d5f0: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-0000d600: 5049 5f52 6561 6453 7461 7465 285f 5f43  PI_ReadState(__C
-0000d610: 6c6f 6e65 6162 6c65 293a 0a20 2020 2064  loneable):.    d
-0000d620: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-0000d630: 3e20 2252 6561 6453 7461 7465 223a 202e  > "ReadState": .
-0000d640: 2e2e 0a20 2020 2064 6566 2067 6574 5f69  ...    def get_i
-0000d650: 6e64 6578 2873 656c 6629 202d 3e20 696e  ndex(self) -> in
-0000d660: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-0000d670: 2020 2020 2020 2060 696e 6465 7860 3a20         `index`: 
-0000d680: 5468 6520 696e 6465 7820 6f66 2074 6865  The index of the
-0000d690: 2072 6561 6420 7374 6174 652e 0a20 2020   read state..   
-0000d6a0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000d6b0: 2073 6574 5f69 6e64 6578 2873 656c 662c   set_index(self,
-0000d6c0: 2069 6478 3a20 696e 7429 202d 3e20 4e6f   idx: int) -> No
-0000d6d0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-0000d6e0: 2020 2020 2020 2020 6069 6e64 6578 603a          `index`:
-0000d6f0: 2054 6865 2069 6e64 6578 206f 6620 7468   The index of th
-0000d700: 6520 7265 6164 2073 7461 7465 2e0a 2020  e read state..  
-0000d710: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000d720: 6620 6765 745f 7265 7175 6573 745f 6374  f get_request_ct
-0000d730: 7828 7365 6c66 2920 2d3e 2062 7974 6573  x(self) -> bytes
-0000d740: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000d750: 2020 2020 2020 6072 6571 7565 7374 5f63        `request_c
-0000d760: 7478 603a 2041 2064 6174 6167 7261 6d20  tx`: A datagram 
-0000d770: 636f 6e73 6973 7469 6e67 206f 6620 636f  consisting of co
-0000d780: 6e74 6578 7420 6162 6f75 7420 7468 6520  ntext about the 
-0000d790: 7265 7175 6573 742e 0a20 2020 2020 2020  request..       
-0000d7a0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-0000d7b0: 5f72 6571 7565 7374 5f63 7478 2873 656c  _request_ctx(sel
-0000d7c0: 662c 2072 6571 7565 7374 5f63 7478 3a20  f, request_ctx: 
-0000d7d0: 6279 7465 7329 202d 3e20 4e6f 6e65 3a0a  bytes) -> None:.
-0000d7e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d7f0: 2020 2020 6072 6571 7565 7374 5f63 7478      `request_ctx
-0000d800: 603a 2041 2064 6174 6167 7261 6d20 636f  `: A datagram co
-0000d810: 6e73 6973 7469 6e67 206f 6620 636f 6e74  nsisting of cont
-0000d820: 6578 7420 6162 6f75 7420 7468 6520 7265  ext about the re
-0000d830: 7175 6573 742e 0a20 2020 2020 2020 2022  quest..        "
-0000d840: 2222 0a0a 636c 6173 7320 5265 6164 5374  ""..class ReadSt
-0000d850: 6174 6528 5f5f 4150 495f 5265 6164 5374  ate(__API_ReadSt
-0000d860: 6174 6529 3a0a 2020 2020 2222 220a 2020  ate):.    """.  
-0000d870: 2020 5265 6164 5374 6174 6520 7072 6f76    ReadState prov
-0000d880: 6964 6573 2073 7461 7465 2066 6f72 2072  ides state for r
-0000d890: 6561 6420 6f6e 6c79 2071 7565 7279 2e0a  ead only query..
-0000d8a0: 2020 2020 4974 2773 2063 616c 6c65 7227      It's caller'
-0000d8b0: 7320 7265 7370 6f6e 7369 6269 6c69 7479  s responsibility
-0000d8c0: 2074 6f20 7365 6e64 204d 7367 5265 6164   to send MsgRead
-0000d8d0: 496e 6465 7820 6669 7273 7420 6265 666f  Index first befo
-0000d8e0: 7265 2067 6574 7469 6e67 0a20 2020 2074  re getting.    t
-0000d8f0: 6869 7320 7374 6174 6520 6672 6f6d 2072  his state from r
-0000d900: 6561 6479 2e20 4974 2773 2061 6c73 6f20  eady. It's also 
-0000d910: 6361 6c6c 6572 2773 2064 7574 7920 746f  caller's duty to
-0000d920: 2064 6966 6665 7265 6e74 6961 7465 2069   differentiate i
-0000d930: 6620 7468 6973 0a20 2020 2073 7461 7465  f this.    state
-0000d940: 2069 7320 7768 6174 2069 7420 7265 7175   is what it requ
-0000d950: 6573 7473 2074 6872 6f75 6768 2072 6571  ests through req
-0000d960: 7565 7374 5f63 7478 2c20 652e 672e 2067  uest_ctx, e.g. g
-0000d970: 6976 656e 2061 2075 6e69 7175 6520 6964  iven a unique id
-0000d980: 2061 730a 2020 2020 7265 7175 6573 745f   as.    request_
-0000d990: 6374 782e 0a20 2020 2022 2222 0a0a 2020  ctx..    """..  
-0000d9a0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000d9b0: 656c 6629 202d 3e20 4e6f 6e65 3a20 2e2e  elf) -> None: ..
-0000d9c0: 2e0a 2020 2020 6465 6620 6d61 6b65 5f72  ..    def make_r
-0000d9d0: 6566 2873 656c 6629 202d 3e20 2252 6561  ef(self) -> "Rea
-0000d9e0: 6453 7461 7465 5265 6622 3a20 2e2e 2e0a  dStateRef": ....
-0000d9f0: 0a63 6c61 7373 2052 6561 6453 7461 7465  .class ReadState
-0000da00: 5265 6628 5f5f 4150 495f 5265 6164 5374  Ref(__API_ReadSt
-0000da10: 6174 6529 3a0a 2020 2020 2222 220a 2020  ate):.    """.  
-0000da20: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
-0000da30: 206f 6620 3a63 6c61 7373 3a60 5265 6164   of :class:`Read
-0000da40: 5374 6174 6560 2e0a 2020 2020 2222 220a  State`..    """.
-0000da50: 0a63 6c61 7373 205f 5f41 5049 5f52 6166  .class __API_Raf
-0000da60: 744c 6f67 3a0a 2020 2020 6465 6620 656e  tLog:.    def en
-0000da70: 7472 6965 7328 0a20 2020 2020 2020 2073  tries(.        s
-0000da80: 656c 662c 2069 6478 3a20 696e 742c 2063  elf, idx: int, c
-0000da90: 6f6e 7465 7874 3a20 2247 6574 456e 7472  ontext: "GetEntr
-0000daa0: 6965 7343 6f6e 7465 7874 5265 6622 2c20  iesContextRef", 
-0000dab0: 6d61 785f 7369 7a65 3a20 4f70 7469 6f6e  max_size: Option
-0000dac0: 616c 5b69 6e74 5d0a 2020 2020 2920 2d3e  al[int].    ) ->
-0000dad0: 204c 6973 745b 2245 6e74 7279 225d 3a0a   List["Entry"]:.
-0000dae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000daf0: 2020 2020 5265 7475 726e 7320 656e 7472      Returns entr
-0000db00: 6965 7320 7374 6172 7469 6e67 2066 726f  ies starting fro
-0000db10: 6d20 6120 7061 7274 6963 756c 6172 2069  m a particular i
-0000db20: 6e64 6578 2061 6e64 206e 6f74 2065 7863  ndex and not exc
-0000db30: 6565 6469 6e67 2061 2062 7974 6573 697a  eeding a bytesiz
-0000db40: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-0000db50: 2020 2064 6566 2061 6c6c 5f65 6e74 7269     def all_entri
-0000db60: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
-0000db70: 5b22 456e 7472 7922 5d3a 0a20 2020 2020  ["Entry"]:.     
-0000db80: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000db90: 6574 7572 6e73 2061 6c6c 2074 6865 2065  eturns all the e
-0000dba0: 6e74 7269 6573 2e20 4f6e 6c79 2075 7365  ntries. Only use
-0000dbb0: 6420 6279 2074 6573 7473 2e0a 2020 2020  d by tests..    
-0000dbc0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000dbd0: 6170 7065 6e64 2873 656c 662c 2065 6e74  append(self, ent
-0000dbe0: 733a 204c 6973 745b 2245 6e74 7279 225d  s: List["Entry"]
-0000dbf0: 207c 204c 6973 745b 2245 6e74 7279 5265   | List["EntryRe
-0000dc00: 6622 5d29 202d 3e20 696e 743a 0a20 2020  f"]) -> int:.   
-0000dc10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000dc20: 2041 7070 656e 6473 2061 2073 6574 206f   Appends a set o
-0000dc30: 6620 656e 7472 6965 7320 746f 2074 6865  f entries to the
-0000dc40: 2075 6e73 7461 626c 6520 6c69 7374 2e0a   unstable list..
-0000dc50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000dc60: 6465 6620 6170 706c 6965 6428 7365 6c66  def applied(self
-0000dc70: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-0000dc80: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-0000dc90: 7475 726e 7320 7468 6520 6c61 7374 2061  turns the last a
-0000dca0: 7070 6c69 6564 2069 6e64 6578 2e0a 2020  pplied index..  
-0000dcb0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000dcc0: 6620 6669 6e64 5f63 6f6e 666c 6963 7428  f find_conflict(
-0000dcd0: 7365 6c66 2c20 656e 7473 3a20 4c69 7374  self, ents: List
-0000dce0: 5b22 456e 7472 7922 5d20 7c20 4c69 7374  ["Entry"] | List
-0000dcf0: 5b22 456e 7472 7952 6566 225d 2920 2d3e  ["EntryRef"]) ->
-0000dd00: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000dd10: 220a 2020 2020 2020 2020 4669 6e64 7320  ".        Finds 
-0000dd20: 7468 6520 696e 6465 7820 6f66 2074 6865  the index of the
-0000dd30: 2063 6f6e 666c 6963 742e 0a0a 2020 2020   conflict...    
-0000dd40: 2020 2020 4974 2072 6574 7572 6e73 2074      It returns t
-0000dd50: 6865 2066 6972 7374 2069 6e64 6578 206f  he first index o
-0000dd60: 6620 636f 6e66 6c69 6374 696e 6720 656e  f conflicting en
-0000dd70: 7472 6965 7320 6265 7477 6565 6e20 7468  tries between th
-0000dd80: 6520 6578 6973 7469 6e67 0a20 2020 2020  e existing.     
-0000dd90: 2020 2065 6e74 7269 6573 2061 6e64 2074     entries and t
-0000dda0: 6865 2067 6976 656e 2065 6e74 7269 6573  he given entries
-0000ddb0: 2c20 6966 2074 6865 7265 2061 7265 2061  , if there are a
-0000ddc0: 6e79 2e0a 0a20 2020 2020 2020 2049 6620  ny...        If 
-0000ddd0: 7468 6572 6520 6172 6520 6e6f 2063 6f6e  there are no con
-0000dde0: 666c 6963 7469 6e67 2065 6e74 7269 6573  flicting entries
-0000ddf0: 2c20 616e 6420 7468 6520 6578 6973 7469  , and the existi
-0000de00: 6e67 2065 6e74 7269 6573 2063 6f6e 7461  ng entries conta
-0000de10: 696e 0a20 2020 2020 2020 2061 6c6c 2074  in.        all t
-0000de20: 6865 2067 6976 656e 2065 6e74 7269 6573  he given entries
-0000de30: 2c20 7a65 726f 2077 696c 6c20 6265 2072  , zero will be r
-0000de40: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
-0000de50: 2020 4966 2074 6865 7265 2061 7265 206e    If there are n
-0000de60: 6f20 636f 6e66 6c69 6374 696e 6720 656e  o conflicting en
-0000de70: 7472 6965 732c 2062 7574 2074 6865 2067  tries, but the g
-0000de80: 6976 656e 2065 6e74 7269 6573 2063 6f6e  iven entries con
-0000de90: 7461 696e 7320 6e65 770a 2020 2020 2020  tains new.      
-0000dea0: 2020 656e 7472 6965 732c 2074 6865 2069    entries, the i
-0000deb0: 6e64 6578 206f 6620 7468 6520 6669 7273  ndex of the firs
-0000dec0: 7420 6e65 7720 656e 7472 7920 7769 6c6c  t new entry will
-0000ded0: 2062 6520 7265 7475 726e 6564 2e0a 0a20   be returned... 
-0000dee0: 2020 2020 2020 2041 6e20 656e 7472 7920         An entry 
-0000def0: 6973 2063 6f6e 7369 6465 7265 6420 746f  is considered to
-0000df00: 2062 6520 636f 6e66 6c69 6374 696e 6720   be conflicting 
-0000df10: 6966 2069 7420 6861 7320 7468 6520 7361  if it has the sa
-0000df20: 6d65 2069 6e64 6578 2062 7574 0a20 2020  me index but.   
-0000df30: 2020 2020 2061 2064 6966 6665 7265 6e74       a different
-0000df40: 2074 6572 6d2e 0a0a 2020 2020 2020 2020   term...        
-0000df50: 5468 6520 6669 7273 7420 656e 7472 7920  The first entry 
-0000df60: 4d55 5354 2068 6176 6520 616e 2069 6e64  MUST have an ind
-0000df70: 6578 2065 7175 616c 2074 6f20 7468 6520  ex equal to the 
-0000df80: 6172 6775 6d65 6e74 2027 6672 6f6d 272e  argument 'from'.
-0000df90: 0a20 2020 2020 2020 2054 6865 2069 6e64  .        The ind
-0000dfa0: 6578 206f 6620 7468 6520 6769 7665 6e20  ex of the given 
-0000dfb0: 656e 7472 6965 7320 4d55 5354 2062 6520  entries MUST be 
-0000dfc0: 636f 6e74 696e 756f 7573 6c79 2069 6e63  continuously inc
-0000dfd0: 7265 6173 696e 672e 0a20 2020 2020 2020  reasing..       
-0000dfe0: 2022 2222 0a20 2020 2064 6566 2066 696e   """.    def fin
-0000dff0: 645f 636f 6e66 6c69 6374 5f62 795f 7465  d_conflict_by_te
-0000e000: 726d 2873 656c 662c 2069 6e64 6578 3a20  rm(self, index: 
-0000e010: 696e 742c 2074 6572 6d3a 2069 6e74 2920  int, term: int) 
-0000e020: 2d3e 2054 7570 6c65 5b69 6e74 2c20 4f70  -> Tuple[int, Op
-0000e030: 7469 6f6e 616c 5b69 6e74 5d5d 3a0a 2020  tional[int]]:.  
-0000e040: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e050: 2020 6669 6e64 5f63 6f6e 666c 6963 745f    find_conflict_
-0000e060: 6279 5f74 6572 6d20 7461 6b65 7320 616e  by_term takes an
-0000e070: 2028 6069 6e64 6578 602c 2060 7465 726d   (`index`, `term
-0000e080: 6029 2070 6169 7220 2869 6e64 6963 6174  `) pair (indicat
-0000e090: 696e 6720 6120 636f 6e66 6c69 6374 696e  ing a conflictin
-0000e0a0: 6720 6c6f 670a 2020 2020 2020 2020 656e  g log.        en
-0000e0b0: 7472 7920 6f6e 2061 206c 6561 6465 722f  try on a leader/
-0000e0c0: 666f 6c6c 6f77 6572 2064 7572 696e 6720  follower during 
-0000e0d0: 616e 2061 7070 656e 6429 2061 6e64 2066  an append) and f
-0000e0e0: 696e 6473 2074 6865 206c 6172 6765 7374  inds the largest
-0000e0f0: 2069 6e64 6578 2069 6e0a 2020 2020 2020   index in.      
-0000e100: 2020 6c6f 6720 7769 7468 206c 6f67 2e74    log with log.t
-0000e110: 6572 6d20 3c3d 2060 7465 726d 6020 616e  erm <= `term` an
-0000e120: 6420 6c6f 672e 696e 6465 7820 3c3d 2060  d log.index <= `
-0000e130: 696e 6465 7860 2e20 4966 206e 6f20 7375  index`. If no su
-0000e140: 6368 2069 6e64 6578 2065 7869 7374 730a  ch index exists.
-0000e150: 2020 2020 2020 2020 696e 2074 6865 206c          in the l
-0000e160: 6f67 2c20 7468 6520 6c6f 6727 7320 6669  og, the log's fi
-0000e170: 7273 7420 696e 6465 7820 6973 2072 6574  rst index is ret
-0000e180: 7572 6e65 642e 0a0a 2020 2020 2020 2020  urned...        
-0000e190: 5468 6520 696e 6465 7820 7072 6f76 6964  The index provid
-0000e1a0: 6564 204d 5553 5420 6265 2065 7175 616c  ed MUST be equal
-0000e1b0: 2074 6f20 6f72 206c 6573 7320 7468 616e   to or less than
-0000e1c0: 2073 656c 662e 6c61 7374 5f69 6e64 6578   self.last_index
-0000e1d0: 2829 2e20 496e 7661 6c69 640a 2020 2020  (). Invalid.    
-0000e1e0: 2020 2020 696e 7075 7473 206c 6f67 2061      inputs log a
-0000e1f0: 2077 6172 6e69 6e67 2061 6e64 2074 6865   warning and the
-0000e200: 2069 6e70 7574 2069 6e64 6578 2069 7320   input index is 
-0000e210: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
-0000e220: 2020 2052 6574 7572 6e20 2869 6e64 6578     Return (index
-0000e230: 2c20 7465 726d 290a 2020 2020 2020 2020  , term).        
-0000e240: 2222 220a 2020 2020 6465 6620 636f 6d6d  """.    def comm
-0000e250: 6974 5f74 6f28 7365 6c66 2c20 746f 5f63  it_to(self, to_c
-0000e260: 6f6d 6d69 743a 2069 6e74 2920 2d3e 204e  ommit: int) -> N
-0000e270: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000e280: 0a20 2020 2020 2020 2053 6574 7320 7468  .        Sets th
-0000e290: 6520 6c61 7374 2063 6f6d 6d69 7474 6564  e last committed
-0000e2a0: 2076 616c 7565 2074 6f20 7468 6520 7061   value to the pa
-0000e2b0: 7373 6564 2069 6e20 7661 6c75 652e 0a0a  ssed in value...
-0000e2c0: 2020 2020 2020 2020 2320 5061 6e69 6373          # Panics
-0000e2d0: 0a0a 2020 2020 2020 2020 5061 6e69 6373  ..        Panics
-0000e2e0: 2069 6620 7468 6520 696e 6465 7820 676f   if the index go
-0000e2f0: 6573 2070 6173 7420 7468 6520 6c61 7374  es past the last
-0000e300: 2069 6e64 6578 2e0a 2020 2020 2020 2020   index..        
-0000e310: 2222 220a 2020 2020 6465 6620 636f 6d6d  """.    def comm
-0000e320: 6974 5f69 6e66 6f28 7365 6c66 2920 2d3e  it_info(self) ->
-0000e330: 2054 7570 6c65 5b69 6e74 2c20 696e 745d   Tuple[int, int]
-0000e340: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000e350: 2020 2020 2020 5265 7475 726e 7320 7468        Returns th
-0000e360: 6520 636f 6d6d 6974 7465 6420 696e 6465  e committed inde
-0000e370: 7820 616e 6420 6974 7320 7465 726d 2e0a  x and its term..
-0000e380: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e390: 6465 6620 7374 6f72 6528 7365 6c66 2920  def store(self) 
-0000e3a0: 2d3e 2022 4d65 6d53 746f 7261 6765 5265  -> "MemStorageRe
-0000e3b0: 6622 3a0a 2020 2020 2020 2020 2222 2220  f":.        """ 
-0000e3c0: 2222 220a 2020 2020 6465 6620 6e65 7874  """.    def next
-0000e3d0: 5f65 6e74 7269 6573 2873 656c 662c 206d  _entries(self, m
-0000e3e0: 6178 5f73 697a 653a 204f 7074 696f 6e61  ax_size: Optiona
-0000e3f0: 6c5b 696e 745d 2920 2d3e 204f 7074 696f  l[int]) -> Optio
-0000e400: 6e61 6c5b 4c69 7374 5b22 456e 7472 7922  nal[List["Entry"
-0000e410: 5d5d 3a0a 2020 2020 2020 2020 2222 220a  ]]:.        """.
-0000e420: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-0000e430: 616c 6c20 7468 6520 6176 6169 6c61 626c  all the availabl
-0000e440: 6520 656e 7472 6965 7320 666f 7220 6578  e entries for ex
-0000e450: 6563 7574 696f 6e2e 0a20 2020 2020 2020  ecution..       
-0000e460: 2049 6620 6170 706c 6965 6420 6973 2073   If applied is s
-0000e470: 6d61 6c6c 6572 2074 6861 6e20 7468 6520  maller than the 
-0000e480: 696e 6465 7820 6f66 2073 6e61 7073 686f  index of snapsho
-0000e490: 742c 2069 7420 7265 7475 726e 7320 616c  t, it returns al
-0000e4a0: 6c20 636f 6d6d 6974 7465 640a 2020 2020  l committed.    
-0000e4b0: 2020 2020 656e 7472 6965 7320 6166 7465      entries afte
-0000e4c0: 7220 7468 6520 696e 6465 7820 6f66 2073  r the index of s
-0000e4d0: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
-0000e4e0: 2022 2222 0a20 2020 2064 6566 206e 6578   """.    def nex
-0000e4f0: 745f 656e 7472 6965 735f 7369 6e63 6528  t_entries_since(
-0000e500: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
-0000e510: 696e 6365 5f69 6478 3a20 696e 742c 206d  ince_idx: int, m
-0000e520: 6178 5f73 697a 653a 204f 7074 696f 6e61  ax_size: Optiona
-0000e530: 6c5b 696e 745d 0a20 2020 2029 202d 3e20  l[int].    ) -> 
-0000e540: 4f70 7469 6f6e 616c 5b4c 6973 745b 2245  Optional[List["E
-0000e550: 6e74 7279 225d 5d3a 0a20 2020 2020 2020  ntry"]]:.       
-0000e560: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-0000e570: 7572 6e73 2063 6f6d 6d69 7474 6564 2061  urns committed a
-0000e580: 6e64 2070 6572 7369 7374 6564 2065 6e74  nd persisted ent
-0000e590: 7269 6573 2073 696e 6365 206d 6178 2860  ries since max(`
-0000e5a0: 7369 6e63 655f 6964 7860 202b 2031 2c20  since_idx` + 1, 
-0000e5b0: 6669 7273 745f 696e 6465 7829 2e0a 2020  first_index)..  
-0000e5c0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0000e5d0: 6620 6861 735f 6e65 7874 5f65 6e74 7269  f has_next_entri
-0000e5e0: 6573 2873 656c 6629 202d 3e20 626f 6f6c  es(self) -> bool
-0000e5f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000e600: 2020 2020 2020 5265 7475 726e 7320 7768        Returns wh
-0000e610: 6574 6865 7220 7468 6572 6520 6172 6520  ether there are 
-0000e620: 6e65 7720 656e 7472 6965 732e 0a20 2020  new entries..   
-0000e630: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000e640: 2068 6173 5f6e 6578 745f 656e 7472 6965   has_next_entrie
-0000e650: 735f 7369 6e63 6528 7365 6c66 2c20 7369  s_since(self, si
-0000e660: 6e63 655f 6964 783a 2069 6e74 2920 2d3e  nce_idx: int) ->
-0000e670: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-0000e680: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-0000e690: 6e73 2077 6865 7468 6572 2074 6865 7265  ns whether there
-0000e6a0: 2061 7265 2063 6f6d 6d69 7474 6564 2061   are committed a
-0000e6b0: 6e64 2070 6572 7369 7374 6564 2065 6e74  nd persisted ent
-0000e6c0: 7269 6573 2073 696e 6365 0a20 2020 2020  ries since.     
-0000e6d0: 2020 206d 6178 2860 7369 6e63 655f 6964     max(`since_id
-0000e6e0: 7860 202b 2031 2c20 6669 7273 745f 696e  x` + 1, first_in
-0000e6f0: 6465 7829 2e0a 2020 2020 2020 2020 2222  dex)..        ""
-0000e700: 220a 2020 2020 6465 6620 6973 5f75 705f  ".    def is_up_
-0000e710: 746f 5f64 6174 6528 7365 6c66 2c20 6c61  to_date(self, la
-0000e720: 7374 5f69 6e64 6578 3a20 696e 742c 2074  st_index: int, t
-0000e730: 6572 6d3a 2069 6e74 2920 2d3e 2062 6f6f  erm: int) -> boo
-0000e740: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-0000e750: 2020 2020 2020 2044 6574 6572 6d69 6e65         Determine
-0000e760: 7320 6966 2074 6865 2067 6976 656e 2028  s if the given (
-0000e770: 6c61 7374 496e 6465 782c 7465 726d 2920  lastIndex,term) 
-0000e780: 6c6f 6720 6973 206d 6f72 6520 7570 2d74  log is more up-t
-0000e790: 6f2d 6461 7465 0a20 2020 2020 2020 2062  o-date.        b
-0000e7a0: 7920 636f 6d70 6172 696e 6720 7468 6520  y comparing the 
-0000e7b0: 696e 6465 7820 616e 6420 7465 726d 206f  index and term o
-0000e7c0: 6620 7468 6520 6c61 7374 2065 6e74 7279  f the last entry
-0000e7d0: 2069 6e20 7468 6520 6578 6973 7469 6e67   in the existing
-0000e7e0: 206c 6f67 732e 0a20 2020 2020 2020 2049   logs..        I
-0000e7f0: 6620 7468 6520 6c6f 6773 2068 6176 6520  f the logs have 
-0000e800: 6c61 7374 2065 6e74 7279 2077 6974 6820  last entry with 
-0000e810: 6469 6666 6572 656e 7420 7465 726d 732c  different terms,
-0000e820: 2074 6865 6e20 7468 6520 6c6f 6720 7769   then the log wi
-0000e830: 7468 2074 6865 0a20 2020 2020 2020 206c  th the.        l
-0000e840: 6174 6572 2074 6572 6d20 6973 206d 6f72  ater term is mor
-0000e850: 6520 7570 2d74 6f2d 6461 7465 2e20 4966  e up-to-date. If
-0000e860: 2074 6865 206c 6f67 7320 656e 6420 7769   the logs end wi
-0000e870: 7468 2074 6865 2073 616d 6520 7465 726d  th the same term
-0000e880: 2c20 7468 656e 0a20 2020 2020 2020 2077  , then.        w
-0000e890: 6869 6368 6576 6572 206c 6f67 2068 6173  hichever log has
-0000e8a0: 2074 6865 206c 6172 6765 7220 6c61 7374   the larger last
-0000e8b0: 5f69 6e64 6578 2069 7320 6d6f 7265 2075  _index is more u
-0000e8c0: 702d 746f 2d64 6174 652e 2049 6620 7468  p-to-date. If th
-0000e8d0: 6520 6c6f 6773 2061 7265 0a20 2020 2020  e logs are.     
-0000e8e0: 2020 2074 6865 2073 616d 652c 2074 6865     the same, the
-0000e8f0: 2067 6976 656e 206c 6f67 2069 7320 7570   given log is up
-0000e900: 2d74 6f2d 6461 7465 2e0a 2020 2020 2020  -to-date..      
-0000e910: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
-0000e920: 7962 655f 636f 6d6d 6974 2873 656c 662c  ybe_commit(self,
-0000e930: 206d 6178 5f69 6e64 6578 3a20 696e 742c   max_index: int,
-0000e940: 2074 6572 6d3a 2069 6e74 2920 2d3e 2062   term: int) -> b
-0000e950: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-0000e960: 0a20 2020 2020 2020 2041 7474 656d 7074  .        Attempt
-0000e970: 7320 746f 2063 6f6d 6d69 7420 7468 6520  s to commit the 
-0000e980: 696e 6465 7820 616e 6420 7465 726d 2061  index and term a
-0000e990: 6e64 2072 6574 7572 6e73 2077 6865 7468  nd returns wheth
-0000e9a0: 6572 2069 7420 6469 642e 0a20 2020 2020  er it did..     
-0000e9b0: 2020 2022 2222 0a20 2020 2064 6566 206d     """.    def m
-0000e9c0: 6179 6265 5f70 6572 7369 7374 2873 656c  aybe_persist(sel
-0000e9d0: 662c 2069 6e64 6578 3a20 696e 742c 2074  f, index: int, t
-0000e9e0: 6572 6d3a 2069 6e74 2920 2d3e 2062 6f6f  erm: int) -> boo
-0000e9f0: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-0000ea00: 2020 2020 2020 2041 7474 656d 7074 7320         Attempts 
-0000ea10: 746f 2070 6572 7369 7374 2074 6865 2069  to persist the i
-0000ea20: 6e64 6578 2061 6e64 2074 6572 6d20 616e  ndex and term an
-0000ea30: 6420 7265 7475 726e 7320 7768 6574 6865  d returns whethe
-0000ea40: 7220 6974 2064 6964 2e0a 2020 2020 2020  r it did..      
-0000ea50: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
-0000ea60: 7962 655f 7065 7273 6973 745f 736e 6170  ybe_persist_snap
-0000ea70: 2873 656c 662c 2069 6e64 6578 3a20 696e  (self, index: in
-0000ea80: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
-0000ea90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000eaa0: 4174 7465 6d70 7473 2074 6f20 7065 7273  Attempts to pers
-0000eab0: 6973 7420 7468 6520 736e 6170 7368 6f74  ist the snapshot
-0000eac0: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
-0000ead0: 7468 6572 2069 7420 6469 642e 0a20 2020  ther it did..   
-0000eae0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000eaf0: 206d 6179 6265 5f61 7070 656e 6428 0a20   maybe_append(. 
-0000eb00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000eb10: 2020 2020 2069 6478 3a20 696e 742c 0a20       idx: int,. 
-0000eb20: 2020 2020 2020 2074 6572 6d3a 2069 6e74         term: int
-0000eb30: 2c0a 2020 2020 2020 2020 636f 6d6d 6974  ,.        commit
-0000eb40: 7465 643a 2069 6e74 2c0a 2020 2020 2020  ted: int,.      
-0000eb50: 2020 656e 7473 3a20 4c69 7374 5b22 456e    ents: List["En
-0000eb60: 7472 7922 5d20 7c20 4c69 7374 5b22 456e  try"] | List["En
-0000eb70: 7472 7952 6566 225d 2c0a 2020 2020 2920  tryRef"],.    ) 
-0000eb80: 2d3e 204f 7074 696f 6e61 6c5b 5475 706c  -> Optional[Tupl
-0000eb90: 655b 696e 742c 2069 6e74 5d5d 3a0a 2020  e[int, int]]:.  
-0000eba0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ebb0: 2020 5265 7475 726e 7320 4e6f 6e65 2069    Returns None i
-0000ebc0: 6620 7468 6520 656e 7472 6965 7320 6361  f the entries ca
-0000ebd0: 6e6e 6f74 2062 6520 6170 7065 6e64 6564  nnot be appended
-0000ebe0: 2e20 4f74 6865 7277 6973 652c 0a20 2020  . Otherwise,.   
-0000ebf0: 2020 2020 2069 7420 7265 7475 726e 7320       it returns 
-0000ec00: 536f 6d65 2828 636f 6e66 6c69 6374 5f69  Some((conflict_i
-0000ec10: 6e64 6578 2c20 6c61 7374 5f69 6e64 6578  ndex, last_index
-0000ec20: 2929 2e0a 0a20 2020 2020 2020 2023 2050  ))...        # P
-0000ec30: 616e 6963 730a 0a20 2020 2020 2020 2050  anics..        P
-0000ec40: 616e 6963 7320 6966 2069 7420 6669 6e64  anics if it find
-0000ec50: 7320 6120 636f 6e66 6c69 6374 696e 6720  s a conflicting 
-0000ec60: 696e 6465 7820 6c65 7373 2074 6861 6e20  index less than 
-0000ec70: 636f 6d6d 6974 7465 6420 696e 6465 782e  committed index.
-0000ec80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ec90: 2064 6566 2073 6e61 7073 686f 7428 7365   def snapshot(se
-0000eca0: 6c66 2c20 7265 7175 6573 745f 696e 6465  lf, request_inde
-0000ecb0: 783a 2069 6e74 2c20 746f 3a20 696e 7429  x: int, to: int)
-0000ecc0: 202d 3e20 2253 6e61 7073 686f 7452 6566   -> "SnapshotRef
-0000ecd0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-0000ece0: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
-0000ecf0: 6865 2063 7572 7265 6e74 2073 6e61 7073  he current snaps
-0000ed00: 686f 740a 2020 2020 2020 2020 2222 220a  hot.        """.
-0000ed10: 2020 2020 6465 6620 7374 6162 6c65 5f65      def stable_e
-0000ed20: 6e74 7269 6573 2873 656c 662c 2069 6e64  ntries(self, ind
-0000ed30: 6578 3a20 696e 742c 2074 6572 6d3a 2069  ex: int, term: i
-0000ed40: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-0000ed50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ed60: 2043 6c65 6172 7320 7468 6520 756e 7374   Clears the unst
-0000ed70: 6162 6c65 2065 6e74 7269 6573 2061 6e64  able entries and
-0000ed80: 206d 6f76 6573 2074 6865 2073 7461 626c   moves the stabl
-0000ed90: 6520 6f66 6673 6574 2075 7020 746f 2074  e offset up to t
-0000eda0: 6865 0a20 2020 2020 2020 206c 6173 7420  he.        last 
-0000edb0: 696e 6465 782c 2069 6620 7468 6572 6520  index, if there 
-0000edc0: 6973 2061 6e79 2e0a 2020 2020 2020 2020  is any..        
-0000edd0: 2222 220a 2020 2020 6465 6620 7374 6162  """.    def stab
-0000ede0: 6c65 5f73 6e61 7028 7365 6c66 2c20 696e  le_snap(self, in
-0000edf0: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
-0000ee00: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-0000ee10: 2020 2020 2020 2043 6c65 6172 7320 7468         Clears th
-0000ee20: 6520 756e 7374 6162 6c65 2073 6e61 7073  e unstable snaps
-0000ee30: 686f 742e 0a20 2020 2020 2020 2022 2222  hot..        """
-0000ee40: 0a20 2020 2064 6566 2074 6572 6d28 7365  .    def term(se
-0000ee50: 6c66 2c20 6964 783a 2069 6e74 2920 2d3e  lf, idx: int) ->
-0000ee60: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-0000ee70: 220a 2020 2020 2020 2020 466f 7220 6120  ".        For a 
-0000ee80: 6769 7665 6e20 696e 6465 782c 2066 696e  given index, fin
-0000ee90: 6473 2074 6865 2074 6572 6d20 6173 736f  ds the term asso
-0000eea0: 6369 6174 6564 2077 6974 6820 6974 2e0a  ciated with it..
-0000eeb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000eec0: 6465 6620 6c61 7374 5f74 6572 6d28 7365  def last_term(se
-0000eed0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-0000eee0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000eef0: 4772 6162 7320 7468 6520 7465 726d 2066  Grabs the term f
-0000ef00: 726f 6d20 7468 6520 6c61 7374 2065 6e74  rom the last ent
-0000ef10: 7279 2e0a 0a20 2020 2020 2020 2023 2050  ry...        # P
-0000ef20: 616e 6963 730a 0a20 2020 2020 2020 2050  anics..        P
-0000ef30: 616e 6963 7320 6966 2074 6865 7265 2061  anics if there a
-0000ef40: 7265 2065 6e74 7269 6573 2062 7574 2074  re entries but t
-0000ef50: 6865 206c 6173 7420 7465 726d 2068 6173  he last term has
-0000ef60: 2062 6565 6e20 6469 7363 6172 6465 642e   been discarded.
-0000ef70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ef80: 2064 6566 206d 6174 6368 5f74 6572 6d28   def match_term(
-0000ef90: 7365 6c66 2c20 6964 783a 2069 6e74 2c20  self, idx: int, 
-0000efa0: 7465 726d 3a20 696e 7429 202d 3e20 626f  term: int) -> bo
-0000efb0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-0000efc0: 2020 2020 2020 2020 416e 7377 6572 7320          Answers 
-0000efd0: 7468 6520 7175 6573 7469 6f6e 3a20 446f  the question: Do
-0000efe0: 6573 2074 6869 7320 696e 6465 7820 6265  es this index be
-0000eff0: 6c6f 6e67 2074 6f20 7468 6973 2074 6572  long to this ter
-0000f000: 6d3f 0a20 2020 2020 2020 2022 2222 0a20  m?.        """. 
-0000f010: 2020 2064 6566 2066 6972 7374 5f69 6e64     def first_ind
-0000f020: 6578 2873 656c 6629 202d 3e20 696e 743a  ex(self) -> int:
-0000f030: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000f040: 2020 2020 2052 6574 7572 6e73 2074 6820       Returns th 
-0000f050: 6669 7273 7420 696e 6465 7820 696e 2074  first index in t
-0000f060: 6865 2073 746f 7265 2074 6861 7420 6973  he store that is
-0000f070: 2061 7661 696c 6162 6c65 2076 6961 2065   available via e
-0000f080: 6e74 7269 6573 0a0a 2020 2020 2020 2020  ntries..        
-0000f090: 2320 5061 6e69 6373 0a0a 2020 2020 2020  # Panics..      
-0000f0a0: 2020 5061 6e69 6373 2069 6620 7468 6520    Panics if the 
-0000f0b0: 7374 6f72 6520 646f 6573 6e27 7420 6861  store doesn't ha
-0000f0c0: 7665 2061 2066 6972 7374 2069 6e64 6578  ve a first index
-0000f0d0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000f0e0: 2020 6465 6620 6c61 7374 5f69 6e64 6578    def last_index
-0000f0f0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-0000f100: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f110: 2020 2052 6574 7572 6e73 2074 6865 206c     Returns the l
-0000f120: 6173 7420 696e 6465 7820 696e 2074 6865  ast index in the
-0000f130: 2073 746f 7265 2074 6861 7420 6973 2061   store that is a
-0000f140: 7661 696c 6162 6c65 2076 6961 2065 6e74  vailable via ent
-0000f150: 7269 6573 2e0a 0a20 2020 2020 2020 2023  ries...        #
-0000f160: 2050 616e 6963 730a 0a20 2020 2020 2020   Panics..       
-0000f170: 2050 616e 6963 7320 6966 2074 6865 2073   Panics if the s
-0000f180: 746f 7265 2064 6f65 736e 2774 2068 6176  tore doesn't hav
-0000f190: 6520 6120 6c61 7374 2069 6e64 6578 2e0a  e a last index..
-0000f1a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f1b0: 6465 6620 756e 7374 6162 6c65 2873 656c  def unstable(sel
-0000f1c0: 6629 202d 3e20 2255 6e73 7461 626c 6552  f) -> "UnstableR
-0000f1d0: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-0000f1e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000f1f0: 2061 2072 6566 6572 656e 6365 2074 6f20   a reference to 
-0000f200: 7468 6520 756e 7374 6162 6c65 206c 6f67  the unstable log
-0000f210: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000f220: 2020 6465 6620 756e 7374 6162 6c65 5f65    def unstable_e
-0000f230: 6e74 7269 6573 2873 656c 6629 202d 3e20  ntries(self) -> 
-0000f240: 4c69 7374 5b22 456e 7472 7952 6566 225d  List["EntryRef"]
-0000f250: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000f260: 2020 2020 2020 5265 7475 726e 7320 736c        Returns sl
-0000f270: 6963 6520 6f66 2065 6e74 7269 6573 2074  ice of entries t
-0000f280: 6861 7420 6172 6520 6e6f 7420 7065 7273  hat are not pers
-0000f290: 6973 7465 642e 0a20 2020 2020 2020 2022  isted..        "
-0000f2a0: 2222 0a20 2020 2064 6566 2075 6e73 7461  "".    def unsta
-0000f2b0: 626c 655f 736e 6170 7368 6f74 2873 656c  ble_snapshot(sel
-0000f2c0: 6629 202d 3e20 4f70 7469 6f6e 616c 5b22  f) -> Optional["
-0000f2d0: 536e 6170 7368 6f74 5265 6622 5d3a 0a20  SnapshotRef"]:. 
-0000f2e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f2f0: 2020 2052 6574 7572 6e73 2074 6865 2073     Returns the s
-0000f300: 6e61 7073 686f 7420 7468 6174 2061 7265  napshot that are
-0000f310: 206e 6f74 2070 6572 7369 7374 6564 2e0a   not persisted..
-0000f320: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f330: 6465 6620 6765 745f 6170 706c 6965 6428  def get_applied(
-0000f340: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-0000f350: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000f360: 2020 6061 7070 6c69 6564 603a 2054 6865    `applied`: The
-0000f370: 2068 6967 6865 7374 206c 6f67 2070 6f73   highest log pos
-0000f380: 6974 696f 6e20 7468 6174 2074 6865 2061  ition that the a
-0000f390: 7070 6c69 6361 7469 6f6e 2068 6173 2062  pplication has b
-0000f3a0: 6565 6e20 696e 7374 7275 6374 6564 0a20  een instructed. 
-0000f3b0: 2020 2020 2020 2074 6f20 6170 706c 7920         to apply 
-0000f3c0: 746f 2069 7473 2073 7461 7465 206d 6163  to its state mac
-0000f3d0: 6869 6e65 2e0a 0a20 2020 2020 2020 2049  hine...        I
-0000f3e0: 6e76 6172 6961 6e74 3a20 6170 706c 6965  nvariant: applie
-0000f3f0: 6420 3c3d 206d 696e 2863 6f6d 6d69 7474  d <= min(committ
-0000f400: 6564 2c20 7065 7273 6973 7465 6429 0a20  ed, persisted). 
-0000f410: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-0000f420: 6566 2073 6574 5f61 7070 6c69 6564 2873  ef set_applied(s
-0000f430: 656c 662c 2061 7070 6c69 6564 3a20 696e  elf, applied: in
-0000f440: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-0000f450: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f460: 6061 7070 6c69 6564 603a 2054 6865 2068  `applied`: The h
-0000f470: 6967 6865 7374 206c 6f67 2070 6f73 6974  ighest log posit
-0000f480: 696f 6e20 7468 6174 2074 6865 2061 7070  ion that the app
-0000f490: 6c69 6361 7469 6f6e 2068 6173 2062 6565  lication has bee
-0000f4a0: 6e20 696e 7374 7275 6374 6564 0a20 2020  n instructed.   
-0000f4b0: 2020 2020 2074 6f20 6170 706c 7920 746f       to apply to
-0000f4c0: 2069 7473 2073 7461 7465 206d 6163 6869   its state machi
-0000f4d0: 6e65 2e0a 0a20 2020 2020 2020 2049 6e76  ne...        Inv
-0000f4e0: 6172 6961 6e74 3a20 6170 706c 6965 6420  ariant: applied 
-0000f4f0: 3c3d 206d 696e 2863 6f6d 6d69 7474 6564  <= min(committed
-0000f500: 2c20 7065 7273 6973 7465 6429 0a20 2020  , persisted).   
-0000f510: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-0000f520: 2067 6574 5f63 6f6d 6d69 7474 6564 2873   get_committed(s
-0000f530: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-0000f540: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f550: 2060 636f 6d6d 6974 7465 6460 3a20 5468   `committed`: Th
-0000f560: 6520 6869 6768 6573 7420 6c6f 6720 706f  e highest log po
-0000f570: 7369 7469 6f6e 2074 6861 7420 6973 206b  sition that is k
-0000f580: 6e6f 776e 2074 6f20 6265 2069 6e20 7374  nown to be in st
-0000f590: 6162 6c65 2073 746f 7261 6765 0a20 2020  able storage.   
-0000f5a0: 2020 2020 206f 6e20 6120 7175 6f72 756d       on a quorum
-0000f5b0: 206f 6620 6e6f 6465 732e 0a0a 2020 2020   of nodes...    
-0000f5c0: 2020 2020 496e 7661 7269 616e 743a 2061      Invariant: a
-0000f5d0: 7070 6c69 6564 203c 3d20 636f 6d6d 6974  pplied <= commit
-0000f5e0: 7465 640a 2020 2020 2020 2020 2222 220a  ted.        """.
-0000f5f0: 2020 2020 6465 6620 7365 745f 636f 6d6d      def set_comm
-0000f600: 6974 7465 6428 7365 6c66 2c20 636f 6d6d  itted(self, comm
-0000f610: 6974 7465 643a 2069 6e74 2920 2d3e 204e  itted: int) -> N
-0000f620: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-0000f630: 0a20 2020 2020 2020 2060 636f 6d6d 6974  .        `commit
-0000f640: 7465 6460 3a20 5468 6520 6869 6768 6573  ted`: The highes
-0000f650: 7420 6c6f 6720 706f 7369 7469 6f6e 2074  t log position t
-0000f660: 6861 7420 6973 206b 6e6f 776e 2074 6f20  hat is known to 
-0000f670: 6265 2069 6e20 7374 6162 6c65 2073 746f  be in stable sto
-0000f680: 7261 6765 0a20 2020 2020 2020 206f 6e20  rage.        on 
-0000f690: 6120 7175 6f72 756d 206f 6620 6e6f 6465  a quorum of node
-0000f6a0: 732e 0a0a 2020 2020 2020 2020 496e 7661  s...        Inva
-0000f6b0: 7269 616e 743a 2061 7070 6c69 6564 203c  riant: applied <
-0000f6c0: 3d20 636f 6d6d 6974 7465 640a 2020 2020  = committed.    
-0000f6d0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000f6e0: 6765 745f 7065 7273 6973 7465 6428 7365  get_persisted(se
-0000f6f0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-0000f700: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f710: 6070 6572 7369 7374 6564 603a 2054 6865  `persisted`: The
-0000f720: 2068 6967 6865 7374 206c 6f67 2070 6f73   highest log pos
-0000f730: 6974 696f 6e20 7468 6174 2069 7320 6b6e  ition that is kn
-0000f740: 6f77 6e20 746f 2062 6520 7065 7273 6973  own to be persis
-0000f750: 7465 6420 696e 2073 7461 626c 650a 2020  ted in stable.  
-0000f760: 2020 2020 2020 7374 6f72 6167 652e 2049        storage. I
-0000f770: 7427 7320 7573 6564 2066 6f72 206c 696d  t's used for lim
-0000f780: 6974 696e 6720 7468 6520 7570 7065 7220  iting the upper 
-0000f790: 626f 756e 6420 6f66 2063 6f6d 6d69 7474  bound of committ
-0000f7a0: 6564 2061 6e64 0a20 2020 2020 2020 2070  ed and.        p
-0000f7b0: 6572 7369 7374 6564 2065 6e74 7269 6573  ersisted entries
-0000f7c0: 2e0a 0a20 2020 2020 2020 2049 6e76 6172  ...        Invar
-0000f7d0: 6961 6e74 3a20 7065 7273 6973 7465 6420  iant: persisted 
-0000f7e0: 3c20 756e 7374 6162 6c65 2e6f 6666 7365  < unstable.offse
-0000f7f0: 7420 2626 2061 7070 6c69 6564 203c 3d20  t && applied <= 
-0000f800: 7065 7273 6973 7465 640a 2020 2020 2020  persisted.      
-0000f810: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-0000f820: 745f 7065 7273 6973 7465 6428 7365 6c66  t_persisted(self
-0000f830: 2c20 7065 7273 6973 7465 643a 2069 6e74  , persisted: int
-0000f840: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-0000f850: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-0000f860: 7065 7273 6973 7465 6460 3a20 5468 6520  persisted`: The 
-0000f870: 6869 6768 6573 7420 6c6f 6720 706f 7369  highest log posi
-0000f880: 7469 6f6e 2074 6861 7420 6973 206b 6e6f  tion that is kno
-0000f890: 776e 2074 6f20 6265 2070 6572 7369 7374  wn to be persist
-0000f8a0: 6564 2069 6e20 7374 6162 6c65 0a20 2020  ed in stable.   
-0000f8b0: 2020 2020 2073 746f 7261 6765 2e20 4974       storage. It
-0000f8c0: 2773 2075 7365 6420 666f 7220 6c69 6d69  's used for limi
-0000f8d0: 7469 6e67 2074 6865 2075 7070 6572 2062  ting the upper b
-0000f8e0: 6f75 6e64 206f 6620 636f 6d6d 6974 7465  ound of committe
-0000f8f0: 6420 616e 640a 2020 2020 2020 2020 7065  d and.        pe
-0000f900: 7273 6973 7465 6420 656e 7472 6965 732e  rsisted entries.
-0000f910: 0a0a 2020 2020 2020 2020 496e 7661 7269  ..        Invari
-0000f920: 616e 743a 2070 6572 7369 7374 6564 203c  ant: persisted <
-0000f930: 2075 6e73 7461 626c 652e 6f66 6673 6574   unstable.offset
-0000f940: 2026 2620 6170 706c 6965 6420 3c3d 2070   && applied <= p
-0000f950: 6572 7369 7374 6564 0a20 2020 2020 2020  ersisted.       
-0000f960: 2022 2222 0a20 2020 2064 6566 2073 6c69   """.    def sli
-0000f970: 6365 280a 2020 2020 2020 2020 7365 6c66  ce(.        self
-0000f980: 2c0a 2020 2020 2020 2020 6c6f 773a 2069  ,.        low: i
-0000f990: 6e74 2c0a 2020 2020 2020 2020 6869 6768  nt,.        high
-0000f9a0: 3a20 696e 742c 0a20 2020 2020 2020 206d  : int,.        m
-0000f9b0: 6178 5f73 697a 653a 204f 7074 696f 6e61  ax_size: Optiona
-0000f9c0: 6c5b 696e 745d 2c0a 2020 2020 2020 2020  l[int],.        
-0000f9d0: 636f 6e74 6578 743a 2022 4765 7445 6e74  context: "GetEnt
-0000f9e0: 7269 6573 436f 6e74 6578 7452 6566 222c  riesContextRef",
-0000f9f0: 0a20 2020 2029 202d 3e20 4c69 7374 5b22  .    ) -> List["
-0000fa00: 456e 7472 7952 6566 225d 3a0a 2020 2020  EntryRef"]:.    
-0000fa10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000fa20: 4772 6162 7320 6120 736c 6963 6520 6f66  Grabs a slice of
-0000fa30: 2065 6e74 7269 6573 2066 726f 6d20 7468   entries from th
-0000fa40: 6520 7261 6674 2e20 556e 6c69 6b65 2061  e raft. Unlike a
-0000fa50: 2072 7573 7420 736c 6963 6520 706f 696e   rust slice poin
-0000fa60: 7465 722c 2074 6865 7365 2061 7265 0a20  ter, these are. 
-0000fa70: 2020 2020 2020 2072 6574 7572 6e65 6420         returned 
-0000fa80: 6279 2076 616c 7565 2e20 5468 6520 7265  by value. The re
-0000fa90: 7375 6c74 2069 7320 7472 756e 6361 7465  sult is truncate
-0000faa0: 6420 746f 2074 6865 206d 6178 5f73 697a  d to the max_siz
-0000fab0: 6520 696e 2062 7974 6573 2e0a 2020 2020  e in bytes..    
-0000fac0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-0000fad0: 7265 7374 6f72 6528 7365 6c66 2c20 736e  restore(self, sn
-0000fae0: 6170 7368 6f74 3a20 2253 6e61 7073 686f  apshot: "Snapsho
-0000faf0: 7422 207c 2022 536e 6170 7368 6f74 5265  t" | "SnapshotRe
-0000fb00: 6622 2920 2d3e 204e 6f6e 653a 0a20 2020  f") -> None:.   
-0000fb10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000fb20: 2052 6573 746f 7265 7320 7468 6520 6375   Restores the cu
-0000fb30: 7272 656e 7420 6c6f 6720 6672 6f6d 2061  rrent log from a
-0000fb40: 2073 6e61 7073 686f 742e 0a20 2020 2020   snapshot..     
-0000fb50: 2020 2022 2222 0a0a 636c 6173 7320 496e     """..class In
-0000fb60: 4d65 6d6f 7279 5261 6674 4c6f 6728 5f5f  MemoryRaftLog(__
-0000fb70: 4150 495f 5261 6674 4c6f 6729 3a0a 2020  API_RaftLog):.  
-0000fb80: 2020 2222 220a 2020 2020 5261 6674 206c    """.    Raft l
-0000fb90: 6f67 2069 6d70 6c65 6d65 6e74 6174 696f  og implementatio
-0000fba0: 6e0a 2020 2020 2222 220a 0a20 2020 2064  n.    """..    d
-0000fbb0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000fbc0: 2020 2020 2073 656c 662c 2073 746f 7265       self, store
-0000fbd0: 3a20 224d 656d 5374 6f72 6167 6552 6566  : "MemStorageRef
-0000fbe0: 222c 206c 6f67 6765 723a 2022 4c6f 6767  ", logger: "Logg
-0000fbf0: 6572 2220 7c20 224c 6f67 6765 7252 6566  er" | "LoggerRef
-0000fc00: 220a 2020 2020 2920 2d3e 204e 6f6e 653a  ".    ) -> None:
-0000fc10: 202e 2e2e 0a20 2020 2064 6566 206d 616b   ....    def mak
-0000fc20: 655f 7265 6628 7365 6c66 2920 2d3e 2022  e_ref(self) -> "
-0000fc30: 496e 4d65 6d6f 7279 5261 6674 4c6f 6752  InMemoryRaftLogR
-0000fc40: 6566 223a 202e 2e2e 0a20 2020 2064 6566  ef": ....    def
-0000fc50: 2067 6574 5f73 746f 7265 2873 656c 6629   get_store(self)
-0000fc60: 202d 3e20 224d 656d 5374 6f72 6167 6552   -> "MemStorageR
-0000fc70: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-0000fc80: 0a20 2020 2020 2020 2047 7261 6220 6120  .        Grab a 
-0000fc90: 7265 6164 2d6f 6e6c 7920 7265 6665 7265  read-only refere
-0000fca0: 6e63 6520 746f 2074 6865 2075 6e64 6572  nce to the under
-0000fcb0: 6c79 696e 6720 7374 6f72 6167 652e 0a20  lying storage.. 
-0000fcc0: 2020 2020 2020 2022 2222 0a0a 636c 6173         """..clas
-0000fcd0: 7320 496e 4d65 6d6f 7279 5261 6674 4c6f  s InMemoryRaftLo
-0000fce0: 6752 6566 285f 5f41 5049 5f52 6166 744c  gRef(__API_RaftL
-0000fcf0: 6f67 293a 0a20 2020 2022 2222 0a20 2020  og):.    """.   
-0000fd00: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
-0000fd10: 6f66 203a 636c 6173 733a 6049 6e4d 656d  of :class:`InMem
-0000fd20: 6f72 7952 6166 744c 6f67 602e 0a20 2020  oryRaftLog`..   
-0000fd30: 2022 2222 0a0a 2020 2020 6465 6620 6765   """..    def ge
-0000fd40: 745f 7374 6f72 6528 7365 6c66 2920 2d3e  t_store(self) ->
-0000fd50: 2022 4d65 6d53 746f 7261 6765 5265 6622   "MemStorageRef"
-0000fd60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000fd70: 2020 2020 2020 4772 6162 2061 2072 6561        Grab a rea
-0000fd80: 642d 6f6e 6c79 2072 6566 6572 656e 6365  d-only reference
-0000fd90: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
-0000fda0: 6e67 2073 746f 7261 6765 2e0a 2020 2020  ng storage..    
-0000fdb0: 2020 2020 2222 220a 0a63 6c61 7373 2052      """..class R
-0000fdc0: 6166 744c 6f67 285f 5f41 5049 5f52 6166  aftLog(__API_Raf
-0000fdd0: 744c 6f67 293a 0a20 2020 2022 2222 2022  tLog):.    """ "
-0000fde0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-0000fdf0: 6974 5f5f 2873 656c 662c 2073 746f 7265  it__(self, store
-0000fe00: 3a20 2253 746f 7261 6765 5265 6622 2c20  : "StorageRef", 
-0000fe10: 6c6f 6767 6572 3a20 224c 6f67 6765 7222  logger: "Logger"
-0000fe20: 207c 2022 4c6f 6767 6572 5265 6622 2920   | "LoggerRef") 
-0000fe30: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-0000fe40: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
-0000fe50: 6c66 2920 2d3e 2022 5261 6674 4c6f 6752  lf) -> "RaftLogR
-0000fe60: 6566 223a 202e 2e2e 0a20 2020 2064 6566  ef": ....    def
-0000fe70: 2067 6574 5f73 746f 7265 2873 656c 6629   get_store(self)
-0000fe80: 202d 3e20 2253 746f 7261 6765 5265 6622   -> "StorageRef"
-0000fe90: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000fea0: 2020 2020 2020 4772 6162 2061 2072 6561        Grab a rea
-0000feb0: 642d 6f6e 6c79 2072 6566 6572 656e 6365  d-only reference
-0000fec0: 2074 6f20 7468 6520 756e 6465 726c 7969   to the underlyi
-0000fed0: 6e67 2073 746f 7261 6765 2e0a 2020 2020  ng storage..    
-0000fee0: 2020 2020 2222 220a 0a63 6c61 7373 2052      """..class R
-0000fef0: 6166 744c 6f67 5265 6628 5f5f 4150 495f  aftLogRef(__API_
-0000ff00: 5261 6674 4c6f 6729 3a0a 2020 2020 2222  RaftLog):.    ""
-0000ff10: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
-0000ff20: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
-0000ff30: 5261 6674 4c6f 6760 2e0a 2020 2020 2222  RaftLog`..    ""
-0000ff40: 220a 0a20 2020 2064 6566 2067 6574 5f73  "..    def get_s
-0000ff50: 746f 7265 2873 656c 6629 202d 3e20 2253  tore(self) -> "S
-0000ff60: 746f 7261 6765 5265 6622 3a0a 2020 2020  torageRef":.    
-0000ff70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ff80: 4772 6162 2061 2072 6561 642d 6f6e 6c79  Grab a read-only
-0000ff90: 2072 6566 6572 656e 6365 2074 6f20 7468   reference to th
-0000ffa0: 6520 756e 6465 726c 7969 6e67 2073 746f  e underlying sto
-0000ffb0: 7261 6765 2e0a 2020 2020 2020 2020 2222  rage..        ""
-0000ffc0: 220a 0a63 6c61 7373 205f 5f41 5049 5f52  "..class __API_R
-0000ffd0: 6166 743a 0a20 2020 2064 6566 2061 7070  aft:.    def app
-0000ffe0: 656e 645f 656e 7472 7928 7365 6c66 2c20  end_entry(self, 
-0000fff0: 656e 7473 3a20 4c69 7374 5b22 456e 7472  ents: List["Entr
-00010000: 7922 5d20 7c20 4c69 7374 5b22 456e 7472  y"] | List["Entr
-00010010: 7952 6566 225d 2920 2d3e 2062 6f6f 6c3a  yRef"]) -> bool:
-00010020: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010030: 2020 2020 2041 7070 656e 6473 2061 2073       Appends a s
-00010040: 6c69 6365 206f 6620 656e 7472 6965 7320  lice of entries 
-00010050: 746f 2074 6865 206c 6f67 2e0a 2020 2020  to the log..    
-00010060: 2020 2020 5468 6520 656e 7472 6965 7320      The entries 
-00010070: 6172 6520 7570 6461 7465 6420 746f 206d  are updated to m
-00010080: 6174 6368 2074 6865 2063 7572 7265 6e74  atch the current
-00010090: 2069 6e64 6578 2061 6e64 2074 6572 6d2e   index and term.
-000100a0: 0a20 2020 2020 2020 204f 6e6c 7920 6361  .        Only ca
-000100b0: 6c6c 6564 2062 7920 6c65 6164 6572 2063  lled by leader c
-000100c0: 7572 7265 6e74 6c79 0a20 2020 2020 2020  urrently.       
-000100d0: 2022 2222 0a20 2020 2064 6566 2073 656e   """.    def sen
-000100e0: 645f 6170 7065 6e64 2873 656c 662c 2074  d_append(self, t
-000100f0: 6f3a 2069 6e74 2920 2d3e 204e 6f6e 653a  o: int) -> None:
-00010100: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010110: 2020 2020 2053 656e 6473 2061 6e20 6170       Sends an ap
-00010120: 7065 6e64 2052 5043 2077 6974 6820 6e65  pend RPC with ne
-00010130: 7720 656e 7472 6965 7320 2869 6620 616e  w entries (if an
-00010140: 7929 2061 6e64 2074 6865 2063 7572 7265  y) and the curre
-00010150: 6e74 2063 6f6d 6d69 7420 696e 6465 7820  nt commit index 
-00010160: 746f 2074 6865 2067 6976 656e 0a20 2020  to the given.   
-00010170: 2020 2020 2070 6565 722e 0a20 2020 2020       peer..     
-00010180: 2020 2022 2222 0a20 2020 2064 6566 206f     """.    def o
-00010190: 6e5f 7065 7273 6973 745f 656e 7472 6965  n_persist_entrie
-000101a0: 7328 7365 6c66 2c20 696e 6465 783a 2069  s(self, index: i
-000101b0: 6e74 2c20 7465 726d 3a20 696e 7429 202d  nt, term: int) -
-000101c0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000101d0: 2222 220a 2020 2020 2020 2020 4e6f 7469  """.        Noti
-000101e0: 6669 6573 2074 6861 7420 7468 6573 6520  fies that these 
-000101f0: 7261 6674 206c 6f67 7320 6861 7665 2062  raft logs have b
-00010200: 6565 6e20 7065 7273 6973 7465 642e 0a20  een persisted.. 
-00010210: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00010220: 6566 2061 7070 6c79 5f74 6f5f 6375 7272  ef apply_to_curr
-00010230: 656e 745f 7465 726d 2873 656c 6629 202d  ent_term(self) -
-00010240: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00010250: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
-00010260: 6b73 2069 6620 6c6f 6773 2061 7265 2061  ks if logs are a
-00010270: 7070 6c69 6564 2074 6f20 6375 7272 656e  pplied to curren
-00010280: 7420 7465 726d 2e0a 2020 2020 2020 2020  t term..        
-00010290: 2222 220a 2020 2020 6465 6620 636f 6d6d  """.    def comm
-000102a0: 6974 5f74 6f5f 6375 7272 656e 745f 7465  it_to_current_te
-000102b0: 726d 2873 656c 6629 202d 3e20 626f 6f6c  rm(self) -> bool
-000102c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000102d0: 2020 2020 2020 4368 6563 6b73 2069 6620        Checks if 
-000102e0: 6c6f 6773 2061 7265 2063 6f6d 6d69 7474  logs are committ
-000102f0: 6564 2074 6f20 6974 7320 7465 726d 2e0a  ed to its term..
-00010300: 0a20 2020 2020 2020 2054 6865 2063 6865  .        The che
-00010310: 636b 2069 7320 7573 6566 756c 2075 7375  ck is useful usu
-00010320: 616c 6c79 2077 6865 6e20 7261 6674 2069  ally when raft i
-00010330: 7320 6c65 6164 6572 2e0a 2020 2020 2020  s leader..      
-00010340: 2020 2222 220a 2020 2020 6465 6620 6772    """.    def gr
-00010350: 6f75 705f 636f 6d6d 6974 2873 656c 6629  oup_commit(self)
-00010360: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00010370: 2020 2222 220a 2020 2020 2020 2020 5768    """.        Wh
-00010380: 6574 6865 7220 656e 6162 6c65 2067 726f  ether enable gro
-00010390: 7570 2063 6f6d 6d69 742e 0a20 2020 2020  up commit..     
-000103a0: 2020 2022 2222 0a20 2020 2064 6566 2065     """.    def e
-000103b0: 6e61 626c 655f 6772 6f75 705f 636f 6d6d  nable_group_comm
-000103c0: 6974 2873 656c 662c 2065 6e61 626c 653a  it(self, enable:
-000103d0: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
-000103e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000103f0: 2020 2020 436f 6e66 6967 7572 6573 2067      Configures g
-00010400: 726f 7570 2063 6f6d 6d69 742e 0a0a 2020  roup commit...  
-00010410: 2020 2020 2020 4966 2067 726f 7570 2063        If group c
-00010420: 6f6d 6d69 7420 6973 2065 6e61 626c 6564  ommit is enabled
-00010430: 2c20 6f6e 6c79 206c 6f67 7320 7265 706c  , only logs repl
-00010440: 6963 6174 6564 2074 6f20 6174 206c 6561  icated to at lea
-00010450: 7374 2074 776f 0a20 2020 2020 2020 2064  st two.        d
-00010460: 6966 6665 7265 6e74 2067 726f 7570 7320  ifferent groups 
-00010470: 6172 6520 636f 6d6d 6974 7465 642e 0a0a  are committed...
-00010480: 2020 2020 2020 2020 596f 7520 7368 6f75          You shou
-00010490: 6c64 2075 7365 2060 6173 7369 676e 5f63  ld use `assign_c
-000104a0: 6f6d 6d69 745f 6772 6f75 7073 6020 746f  ommit_groups` to
-000104b0: 2063 6f6e 6669 6775 7265 2070 6565 7220   configure peer 
-000104c0: 6772 6f75 7073 2e0a 2020 2020 2020 2020  groups..        
-000104d0: 2222 220a 2020 2020 6465 6620 636c 6561  """.    def clea
-000104e0: 725f 636f 6d6d 6974 5f67 726f 7570 2873  r_commit_group(s
-000104f0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00010500: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010510: 2020 5265 6d6f 7665 7320 616c 6c20 636f    Removes all co
-00010520: 6d6d 6974 2067 726f 7570 2063 6f6e 6669  mmit group confi
-00010530: 6775 7261 7469 6f6e 732e 0a20 2020 2020  gurations..     
-00010540: 2020 2022 2222 0a20 2020 2064 6566 2063     """.    def c
-00010550: 6865 636b 5f67 726f 7570 5f63 6f6d 6d69  heck_group_commi
-00010560: 745f 636f 6e73 6973 7465 6e74 2873 656c  t_consistent(sel
-00010570: 6629 202d 3e20 4f70 7469 6f6e 616c 5b62  f) -> Optional[b
-00010580: 6f6f 6c5d 3a0a 2020 2020 2020 2020 2222  ool]:.        ""
-00010590: 220a 2020 2020 2020 2020 4368 6563 6b73  ".        Checks
-000105a0: 2077 6865 7468 6572 2074 6865 2072 6166   whether the raf
-000105b0: 7420 6772 6f75 7020 6973 2075 7369 6e67  t group is using
-000105c0: 2067 726f 7570 2063 6f6d 6d69 7420 616e   group commit an
-000105d0: 6420 636f 6e73 6973 7465 6e74 0a20 2020  d consistent.   
-000105e0: 2020 2020 206f 7665 7220 6772 6f75 702e       over group.
-000105f0: 0a0a 2020 2020 2020 2020 4966 2069 7420  ..        If it 
-00010600: 6361 6e27 7420 6765 7420 6120 636f 7272  can't get a corr
-00010610: 6563 7420 616e 7377 6572 2c20 604e 6f6e  ect answer, `Non
-00010620: 6560 2069 7320 7265 7475 726e 6564 2e0a  e` is returned..
-00010630: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010640: 6465 6620 6173 7369 676e 5f63 6f6d 6d69  def assign_commi
-00010650: 745f 6772 6f75 7073 2873 656c 662c 2069  t_groups(self, i
-00010660: 6473 3a20 4c69 7374 5b54 7570 6c65 5b69  ds: List[Tuple[i
-00010670: 6e74 2c20 696e 745d 5d29 202d 3e20 4e6f  nt, int]]) -> No
-00010680: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00010690: 2020 2020 2020 2020 4173 7369 676e 7320          Assigns 
-000106a0: 6772 6f75 7073 2074 6f20 7065 6572 732e  groups to peers.
-000106b0: 0a0a 2020 2020 2020 2020 5468 6520 7475  ..        The tu
-000106c0: 706c 6520 6973 2028 6070 6565 725f 6964  ple is (`peer_id
-000106d0: 602c 2060 6772 6f75 705f 6964 6029 2e20  `, `group_id`). 
-000106e0: 6067 726f 7570 5f69 6460 2073 686f 756c  `group_id` shoul
-000106f0: 6420 6265 206c 6172 6765 7220 7468 616e  d be larger than
-00010700: 2030 2e0a 0a20 2020 2020 2020 2054 6865   0...        The
-00010710: 2067 726f 7570 2069 6e66 6f72 6d61 7469   group informati
-00010720: 6f6e 2069 7320 6f6e 6c79 2073 746f 7265  on is only store
-00010730: 6420 696e 206d 656d 6f72 792e 2053 6f20  d in memory. So 
-00010740: 796f 7520 6e65 6564 2074 6f20 636f 6e66  you need to conf
-00010750: 6967 7572 650a 2020 2020 2020 2020 6974  igure.        it
-00010760: 2065 7665 7279 2074 696d 6520 6120 7261   every time a ra
-00010770: 6674 2073 7461 7465 206d 6163 6869 6e65  ft state machine
-00010780: 2069 7320 696e 6974 6961 6c69 7a65 6420   is initialized 
-00010790: 6f72 2061 2073 6e61 7073 686f 7420 6973  or a snapshot is
-000107a0: 2061 7070 6c69 6564 2e0a 2020 2020 2020   applied..      
-000107b0: 2020 2222 220a 2020 2020 6465 6620 636f    """.    def co
-000107c0: 6d6d 6974 5f61 7070 6c79 2873 656c 662c  mmit_apply(self,
-000107d0: 2061 7070 6c69 6564 3a20 696e 7429 202d   applied: int) -
-000107e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000107f0: 2222 220a 2020 2020 2020 2020 436f 6d6d  """.        Comm
-00010800: 6974 2074 6861 7420 7468 6520 5261 6674  it that the Raft
-00010810: 2070 6565 7220 6861 7320 6170 706c 6965   peer has applie
-00010820: 6420 7570 2074 6f20 7468 6520 6769 7665  d up to the give
-00010830: 6e20 696e 6465 782e 0a0a 2020 2020 2020  n index...      
-00010840: 2020 5265 6769 7374 6572 7320 7468 6520    Registers the 
-00010850: 6e65 7720 6170 706c 6965 6420 696e 6465  new applied inde
-00010860: 7820 746f 2074 6865 2052 6166 7420 6c6f  x to the Raft lo
-00010870: 672e 0a0a 2020 2020 2020 2020 2320 486f  g...        # Ho
-00010880: 6f6b 730a 0a20 2020 2020 2020 202a 2050  oks..        * P
-00010890: 6f73 743a 2043 6865 636b 7320 746f 2073  ost: Checks to s
-000108a0: 6565 2069 6620 6974 2773 2074 696d 6520  ee if it's time 
-000108b0: 746f 2066 696e 616c 697a 6520 6120 4a6f  to finalize a Jo
-000108c0: 696e 7420 436f 6e73 656e 7375 7320 7374  int Consensus st
-000108d0: 6174 652e 0a20 2020 2020 2020 2022 2222  ate..        """
-000108e0: 0a20 2020 2064 6566 206d 6179 6265 5f63  .    def maybe_c
-000108f0: 6f6d 6d69 7428 7365 6c66 2920 2d3e 2062  ommit(self) -> b
-00010900: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00010910: 0a20 2020 2020 2020 2041 7474 656d 7074  .        Attempt
-00010920: 7320 746f 2061 6476 616e 6365 2074 6865  s to advance the
-00010930: 2063 6f6d 6d69 7420 696e 6465 782e 2052   commit index. R
-00010940: 6574 7572 6e73 2074 7275 6520 6966 2074  eturns true if t
-00010950: 6865 2063 6f6d 6d69 7420 696e 6465 780a  he commit index.
-00010960: 2020 2020 2020 2020 6368 616e 6765 6420          changed 
-00010970: 2869 6e20 7768 6963 6820 6361 7365 2074  (in which case t
-00010980: 6865 2063 616c 6c65 7220 7368 6f75 6c64  he caller should
-00010990: 2063 616c 6c20 6072 2e62 6361 7374 5f61   call `r.bcast_a
-000109a0: 7070 656e 6460 292e 0a20 2020 2020 2020  ppend`)..       
-000109b0: 2022 2222 0a20 2020 2064 6566 2075 6e63   """.    def unc
-000109c0: 6f6d 6d69 7474 6564 5f73 697a 6528 7365  ommitted_size(se
-000109d0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-000109e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000109f0: 5265 7475 726e 2063 7572 7265 6e74 2075  Return current u
-00010a00: 6e63 6f6d 6d69 7474 6564 2073 697a 6520  ncommitted size 
-00010a10: 7265 636f 7264 6564 2062 7920 756e 636f  recorded by unco
-00010a20: 6d6d 6974 7465 645f 7374 6174 650a 2020  mmitted_state.  
-00010a30: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00010a40: 6620 6d61 7962 655f 696e 6372 6561 7365  f maybe_increase
-00010a50: 5f75 6e63 6f6d 6d69 7474 6564 5f73 697a  _uncommitted_siz
-00010a60: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
-00010a70: 2065 6e74 733a 204c 6973 745b 2245 6e74   ents: List["Ent
-00010a80: 7279 225d 207c 204c 6973 745b 2245 6e74  ry"] | List["Ent
-00010a90: 7279 5265 6622 5d0a 2020 2020 2920 2d3e  ryRef"].    ) ->
-00010aa0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00010ab0: 2222 0a20 2020 2020 2020 2049 6e63 7265  "".        Incre
-00010ac0: 6173 6520 7369 7a65 206f 6620 2765 6e74  ase size of 'ent
-00010ad0: 7327 2074 6f20 756e 636f 6d6d 6974 7465  s' to uncommitte
-00010ae0: 6420 7369 7a65 2e20 5265 7475 726e 2074  d size. Return t
-00010af0: 7275 6520 7768 656e 2073 697a 6520 6c69  rue when size li
-00010b00: 6d69 740a 2020 2020 2020 2020 6973 2073  mit.        is s
-00010b10: 6174 6973 6669 6564 2e20 4f74 6865 7277  atisfied. Otherw
-00010b20: 6973 6520 7265 7475 726e 2066 616c 7365  ise return false
-00010b30: 2061 6e64 2075 6e63 6f6d 6d69 7474 6564   and uncommitted
-00010b40: 2073 697a 6520 7265 6d61 696e 7320 756e   size remains un
-00010b50: 6368 616e 6765 642e 0a20 2020 2020 2020  changed..       
-00010b60: 2046 6f72 2072 6166 7420 7769 7468 206e   For raft with n
-00010b70: 6f20 6c69 6d69 7428 6f72 206e 6f6e 2d6c  o limit(or non-l
-00010b80: 6561 6465 7220 7261 6674 292c 2069 7420  eader raft), it 
-00010b90: 616c 7761 7973 2072 6574 7572 6e20 7472  always return tr
-00010ba0: 7565 2e0a 2020 2020 2020 2020 2222 220a  ue..        """.
-00010bb0: 2020 2020 6465 6620 7265 6475 6365 5f75      def reduce_u
-00010bc0: 6e63 6f6d 6d69 7474 6564 5f73 697a 6528  ncommitted_size(
-00010bd0: 7365 6c66 2c20 656e 7473 3a20 4c69 7374  self, ents: List
-00010be0: 5b22 456e 7472 7922 5d20 7c20 4c69 7374  ["Entry"] | List
-00010bf0: 5b22 456e 7472 7952 6566 225d 2920 2d3e  ["EntryRef"]) ->
-00010c00: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00010c10: 2222 0a20 2020 2020 2020 2052 6564 7563  "".        Reduc
-00010c20: 6520 7369 7a65 206f 6620 2765 6e74 7327  e size of 'ents'
-00010c30: 2066 726f 6d20 756e 636f 6d6d 6974 7465   from uncommitte
-00010c40: 6420 7369 7a65 2e0a 2020 2020 2020 2020  d size..        
-00010c50: 2222 220a 2020 2020 6465 6620 6263 6173  """.    def bcas
-00010c60: 745f 6170 7065 6e64 2873 656c 6629 202d  t_append(self) -
-00010c70: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00010c80: 2222 220a 2020 2020 2020 2020 5365 6e64  """.        Send
-00010c90: 7320 5250 432c 2077 6974 6820 656e 7472  s RPC, with entr
-00010ca0: 6965 7320 746f 2061 6c6c 2070 6565 7273  ies to all peers
-00010cb0: 2074 6861 7420 6172 6520 6e6f 7420 7570   that are not up
-00010cc0: 2d74 6f2d 6461 7465 0a20 2020 2020 2020  -to-date.       
-00010cd0: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
-00010ce0: 6520 7072 6f67 7265 7373 2072 6563 6f72  e progress recor
-00010cf0: 6465 6420 696e 2072 2e70 7273 2829 2e0a  ded in r.prs()..
-00010d00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010d10: 6465 6620 6263 6173 745f 6865 6172 7462  def bcast_heartb
-00010d20: 6561 7428 7365 6c66 2920 2d3e 204e 6f6e  eat(self) -> Non
-00010d30: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00010d40: 2020 2020 2020 2053 656e 6473 2052 5043         Sends RPC
-00010d50: 2c20 7769 7468 6f75 7420 656e 7472 6965  , without entrie
-00010d60: 7320 746f 2061 6c6c 2074 6865 2070 6565  s to all the pee
-00010d70: 7273 2e0a 2020 2020 2020 2020 2222 220a  rs..        """.
-00010d80: 2020 2020 6465 6620 7368 6f75 6c64 5f62      def should_b
-00010d90: 6361 7374 5f63 6f6d 6d69 7428 7365 6c66  cast_commit(self
-00010da0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00010db0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00010dc0: 7065 6369 6669 6573 2069 6620 7468 6520  pecifies if the 
-00010dd0: 636f 6d6d 6974 2073 686f 756c 6420 6265  commit should be
-00010de0: 2062 726f 6164 6361 7374 2e0a 2020 2020   broadcast..    
-00010df0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00010e00: 736b 6970 5f62 6361 7374 5f63 6f6d 6d69  skip_bcast_commi
-00010e10: 7428 7365 6c66 2c20 736b 6970 3a20 626f  t(self, skip: bo
-00010e20: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
-00010e30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010e40: 2053 6574 2077 6865 7468 6572 2073 6b69   Set whether ski
-00010e50: 7020 6272 6f61 6463 6173 7420 656d 7074  p broadcast empt
-00010e60: 7920 636f 6d6d 6974 206d 6573 7361 6765  y commit message
-00010e70: 7320 6174 2072 756e 7469 6d65 2e0a 2020  s at runtime..  
-00010e80: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00010e90: 6620 6265 636f 6d65 5f6c 6561 6465 7228  f become_leader(
-00010ea0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
-00010eb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010ec0: 2020 204d 616b 6573 2074 6869 7320 7261     Makes this ra
-00010ed0: 6674 2074 6865 206c 6561 6465 722e 0a0a  ft the leader...
-00010ee0: 2020 2020 2020 2020 2320 5061 6e69 6373          # Panics
-00010ef0: 0a0a 2020 2020 2020 2020 5061 6e69 6373  ..        Panics
-00010f00: 2069 6620 7468 6973 2069 7320 6120 666f   if this is a fo
-00010f10: 6c6c 6f77 6572 206e 6f64 652e 0a20 2020  llower node..   
-00010f20: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00010f30: 2062 6563 6f6d 655f 666f 6c6c 6f77 6572   become_follower
-00010f40: 2873 656c 662c 2074 6572 6d3a 2069 6e74  (self, term: int
-00010f50: 2c20 6c65 6164 6572 5f69 643a 2069 6e74  , leader_id: int
-00010f60: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00010f70: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00010f80: 6f6e 7665 7274 7320 7468 6973 206e 6f64  onverts this nod
-00010f90: 6520 746f 2061 2066 6f6c 6c6f 7765 722e  e to a follower.
-00010fa0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010fb0: 2064 6566 2062 6563 6f6d 655f 7072 655f   def become_pre_
-00010fc0: 6361 6e64 6964 6174 6528 7365 6c66 2920  candidate(self) 
-00010fd0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00010fe0: 2022 2222 0a20 2020 2020 2020 2043 6f6e   """.        Con
-00010ff0: 7665 7274 7320 7468 6973 206e 6f64 6520  verts this node 
-00011000: 746f 2061 2070 7265 2d63 616e 6469 6461  to a pre-candida
-00011010: 7465 0a0a 2020 2020 2020 2020 2320 5061  te..        # Pa
-00011020: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
-00011030: 6e69 6373 2069 6620 6120 6c65 6164 6572  nics if a leader
-00011040: 2061 6c72 6561 6479 2065 7869 7374 732e   already exists.
-00011050: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011060: 2064 6566 2062 6563 6f6d 655f 6361 6e64   def become_cand
-00011070: 6964 6174 6528 7365 6c66 2920 2d3e 204e  idate(self) -> N
-00011080: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00011090: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
-000110a0: 7320 7468 6973 206e 6f64 6520 746f 2061  s this node to a
-000110b0: 2063 616e 6469 6461 7465 0a0a 2020 2020   candidate..    
-000110c0: 2020 2020 2320 5061 6e69 6373 0a0a 2020      # Panics..  
-000110d0: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
-000110e0: 6120 6c65 6164 6572 2061 6c72 6561 6479  a leader already
-000110f0: 2065 7869 7374 732e 0a20 2020 2020 2020   exists..       
-00011100: 2022 2222 0a20 2020 2064 6566 2068 6561   """.    def hea
-00011110: 7274 6265 6174 5f74 696d 656f 7574 2873  rtbeat_timeout(s
-00011120: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-00011130: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011140: 2046 6574 6368 2074 6865 206c 656e 6774   Fetch the lengt
-00011150: 6820 6f66 2074 6865 2068 6561 7274 6265  h of the heartbe
-00011160: 6174 2074 696d 656f 7574 0a20 2020 2020  at timeout.     
-00011170: 2020 2022 2222 0a20 2020 2064 6566 2068     """.    def h
-00011180: 6561 7274 6265 6174 5f65 6c61 7073 6564  eartbeat_elapsed
-00011190: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-000111a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000111b0: 2020 2046 6574 6368 2074 6865 206e 756d     Fetch the num
-000111c0: 6265 7220 6f66 2074 6963 6b73 2065 6c61  ber of ticks ela
-000111d0: 7073 6564 2073 696e 6365 206c 6173 7420  psed since last 
-000111e0: 6865 6172 7462 6561 742e 0a20 2020 2020  heartbeat..     
-000111f0: 2020 2022 2222 0a20 2020 2064 6566 2065     """.    def e
-00011200: 6c65 6374 696f 6e5f 7469 6d65 6f75 7428  lection_timeout(
-00011210: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-00011220: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011230: 2020 4665 7463 6820 7468 6520 6c65 6e67    Fetch the leng
-00011240: 7468 206f 6620 7468 6520 656c 6563 7469  th of the electi
-00011250: 6f6e 2074 696d 656f 7574 2e0a 2020 2020  on timeout..    
-00011260: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00011270: 7261 6e64 6f6d 697a 6564 5f65 6c65 6374  randomized_elect
-00011280: 696f 6e5f 7469 6d65 6f75 7428 7365 6c66  ion_timeout(self
-00011290: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-000112a0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-000112b0: 7475 726e 2074 6865 206c 656e 6774 6820  turn the length 
-000112c0: 6f66 2074 6865 2063 7572 7265 6e74 2072  of the current r
-000112d0: 616e 646f 6d69 7a65 6420 656c 6563 7469  andomized electi
-000112e0: 6f6e 2074 696d 656f 7574 2e0a 2020 2020  on timeout..    
-000112f0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00011300: 7365 745f 7261 6e64 6f6d 697a 6564 5f65  set_randomized_e
-00011310: 6c65 6374 696f 6e5f 7469 6d65 6f75 7428  lection_timeout(
-00011320: 7365 6c66 2c20 7261 6e64 6f6d 697a 6564  self, randomized
-00011330: 5f65 6c65 6374 696f 6e5f 7469 6d65 6f75  _election_timeou
-00011340: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-00011350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011360: 2020 2020 2046 6f72 2074 6573 7469 6e67       For testing
-00011370: 206c 6561 6465 7220 6c65 6173 650a 2020   leader lease.  
-00011380: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00011390: 6620 7265 7365 745f 7261 6e64 6f6d 697a  f reset_randomiz
-000113a0: 6564 5f65 6c65 6374 696f 6e5f 7469 6d65  ed_election_time
-000113b0: 6f75 7428 7365 6c66 2920 2d3e 204e 6f6e  out(self) -> Non
-000113c0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000113d0: 2020 2020 2020 2052 6567 656e 6572 6174         Regenerat
-000113e0: 6573 2061 6e64 2073 746f 7265 7320 7468  es and stores th
-000113f0: 6520 656c 6563 7469 6f6e 2074 696d 656f  e election timeo
-00011400: 7574 2e0a 2020 2020 2020 2020 2222 220a  ut..        """.
-00011410: 2020 2020 6465 6620 7061 7373 5f65 6c65      def pass_ele
-00011420: 6374 696f 6e5f 7469 6d65 6f75 7428 7365  ction_timeout(se
-00011430: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00011440: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011450: 2060 7061 7373 5f65 6c65 6374 696f 6e5f   `pass_election_
-00011460: 7469 6d65 6f75 7460 2072 6574 7572 6e73  timeout` returns
-00011470: 2074 7275 6520 6966 2060 656c 6563 7469   true if `electi
-00011480: 6f6e 5f65 6c61 7073 6564 6020 6973 2067  on_elapsed` is g
-00011490: 7265 6174 6572 0a20 2020 2020 2020 2074  reater.        t
-000114a0: 6861 6e20 6f72 2065 7175 616c 2074 6f20  han or equal to 
-000114b0: 7468 6520 7261 6e64 6f6d 697a 6564 2065  the randomized e
-000114c0: 6c65 6374 696f 6e20 7469 6d65 6f75 7420  lection timeout 
-000114d0: 696e 0a20 2020 2020 2020 205b 6065 6c65  in.        [`ele
-000114e0: 6374 696f 6e5f 7469 6d65 6f75 7460 2c20  ction_timeout`, 
-000114f0: 3220 2a20 6065 6c65 6374 696f 6e5f 7469  2 * `election_ti
-00011500: 6d65 6f75 7460 202d 2031 5d2e 0a20 2020  meout` - 1]..   
-00011510: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00011520: 2073 656e 645f 7469 6d65 6f75 745f 6e6f   send_timeout_no
-00011530: 7728 7365 6c66 2c20 746f 3a20 696e 7429  w(self, to: int)
-00011540: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00011550: 2020 2222 220a 2020 2020 2020 2020 4973    """.        Is
-00011560: 7375 6573 2061 206d 6573 7361 6765 2074  sues a message t
-00011570: 6f20 7469 6d65 6f75 7420 696d 6d65 6469  o timeout immedi
-00011580: 6174 656c 792e 0a20 2020 2020 2020 2022  ately..        "
-00011590: 2222 0a20 2020 2064 6566 2072 6561 6479  "".    def ready
-000115a0: 5f72 6561 645f 636f 756e 7428 7365 6c66  _read_count(self
-000115b0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-000115c0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-000115d0: 7475 726e 7320 686f 7720 6d61 6e79 2072  turns how many r
-000115e0: 6561 6420 7374 6174 6573 2065 7869 7374  ead states exist
-000115f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00011600: 2020 6465 6620 7065 6e64 696e 675f 7265    def pending_re
-00011610: 6164 5f63 6f75 6e74 2873 656c 6629 202d  ad_count(self) -
-00011620: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-00011630: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00011640: 6e73 2074 6865 206e 756d 6265 7220 6f66  ns the number of
-00011650: 2070 656e 6469 6e67 2072 6561 642d 6f6e   pending read-on
-00011660: 6c79 206d 6573 7361 6765 732e 0a20 2020  ly messages..   
-00011670: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00011680: 206c 6f61 645f 7374 6174 6528 7365 6c66   load_state(self
-00011690: 2c20 6873 3a20 2248 6172 6453 7461 7465  , hs: "HardState
-000116a0: 2220 7c20 2248 6172 6453 7461 7465 5265  " | "HardStateRe
-000116b0: 6622 2920 2d3e 204e 6f6e 653a 0a20 2020  f") -> None:.   
-000116c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000116d0: 2046 6f72 2061 2067 6976 656e 2068 6172   For a given har
-000116e0: 6473 7461 7465 2c20 6c6f 6164 2074 6865  dstate, load the
-000116f0: 2073 7461 7465 2069 6e74 6f20 7365 6c66   state into self
-00011700: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00011710: 2020 6465 6620 736f 6674 5f73 7461 7465    def soft_state
-00011720: 2873 656c 6629 202d 3e20 2253 6f66 7453  (self) -> "SoftS
-00011730: 7461 7465 223a 0a20 2020 2020 2020 2022  tate":.        "
-00011740: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00011750: 6e73 2061 2076 616c 7565 2072 6570 7265  ns a value repre
-00011760: 7365 6e74 696e 6720 7468 6520 736f 6674  senting the soft
-00011770: 7374 6174 6520 6174 2074 6865 2074 696d  state at the tim
-00011780: 6520 6f66 2063 616c 6c69 6e67 2e0a 2020  e of calling..  
-00011790: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000117a0: 6620 6861 7264 5f73 7461 7465 2873 656c  f hard_state(sel
-000117b0: 6629 202d 3e20 2248 6172 6453 7461 7465  f) -> "HardState
-000117c0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-000117d0: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
-000117e0: 2076 616c 7565 2072 6570 7265 7365 6e74   value represent
-000117f0: 696e 6720 7468 6520 6861 7264 7374 6174  ing the hardstat
-00011800: 6520 6174 2074 6865 2074 696d 6520 6f66  e at the time of
-00011810: 2063 616c 6c69 6e67 2e0a 2020 2020 2020   calling..      
-00011820: 2020 2222 220a 2020 2020 6465 6620 7069    """.    def pi
-00011830: 6e67 2873 656c 6629 202d 3e20 4e6f 6e65  ng(self) -> None
-00011840: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00011850: 2020 2020 2020 4272 6f61 6463 6173 7473        Broadcasts
-00011860: 2068 6561 7274 6265 6174 7320 746f 2061   heartbeats to a
-00011870: 6c6c 2074 6865 2066 6f6c 6c6f 7765 7273  ll the followers
-00011880: 2069 6620 6974 2773 206c 6561 6465 722e   if it's leader.
-00011890: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000118a0: 2064 6566 2074 6963 6b28 7365 6c66 2920   def tick(self) 
-000118b0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
-000118c0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-000118d0: 7572 6e73 2074 7275 6520 746f 2069 6e64  urns true to ind
-000118e0: 6963 6174 6520 7468 6174 2074 6865 7265  icate that there
-000118f0: 2077 696c 6c20 7072 6f62 6162 6c79 2062   will probably b
-00011900: 6520 736f 6d65 2072 6561 6469 6e65 7373  e some readiness
-00011910: 206e 6565 6420 746f 2062 6520 6861 6e64   need to be hand
-00011920: 6c65 642e 0a20 2020 2020 2020 2022 2222  led..        """
-00011930: 0a20 2020 2064 6566 2074 6963 6b5f 656c  .    def tick_el
-00011940: 6563 7469 6f6e 2873 656c 6629 202d 3e20  ection(self) -> 
-00011950: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00011960: 220a 2020 2020 2020 2020 5275 6e20 6279  ".        Run by
-00011970: 2066 6f6c 6c6f 7765 7273 2061 6e64 2063   followers and c
-00011980: 616e 6469 6461 7465 7320 6166 7465 7220  andidates after 
-00011990: 7365 6c66 2e65 6c65 6374 696f 6e5f 7469  self.election_ti
-000119a0: 6d65 6f75 742e 0a0a 2020 2020 2020 2020  meout...        
-000119b0: 5265 7475 726e 7320 7472 7565 2074 6f20  Returns true to 
-000119c0: 696e 6469 6361 7465 2074 6861 7420 7468  indicate that th
-000119d0: 6572 6520 7769 6c6c 2070 726f 6261 626c  ere will probabl
-000119e0: 7920 6265 2073 6f6d 6520 7265 6164 696e  y be some readin
-000119f0: 6573 7320 6e65 6564 2074 6f20 6265 2068  ess need to be h
-00011a00: 616e 646c 6564 2e0a 2020 2020 2020 2020  andled..        
-00011a10: 2222 220a 2020 2020 6465 6620 7374 6570  """.    def step
-00011a20: 2873 656c 662c 206d 7367 3a20 224d 6573  (self, msg: "Mes
-00011a30: 7361 6765 2220 7c20 224d 6573 7361 6765  sage" | "Message
-00011a40: 5265 6622 2920 2d3e 204e 6f6e 653a 0a20  Ref") -> None:. 
-00011a50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011a60: 2020 2053 7465 7073 2074 6865 2072 6166     Steps the raf
-00011a70: 7420 616c 6f6e 6720 7669 6120 6120 6d65  t along via a me
-00011a80: 7373 6167 652e 2054 6869 7320 7368 6f75  ssage. This shou
-00011a90: 6c64 2062 6520 6361 6c6c 6564 2065 7665  ld be called eve
-00011aa0: 7279 7469 6d65 2079 6f75 7220 7261 6674  rytime your raft
-00011ab0: 2072 6563 6569 7665 7320 610a 2020 2020   receives a.    
-00011ac0: 2020 2020 6d65 7373 6167 6520 6672 6f6d      message from
-00011ad0: 2061 2070 6565 722e 0a20 2020 2020 2020   a peer..       
-00011ae0: 2022 2222 0a20 2020 2064 6566 2068 6173   """.    def has
-00011af0: 5f70 656e 6469 6e67 5f63 6f6e 6628 7365  _pending_conf(se
-00011b00: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00011b10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011b20: 2043 6865 636b 2069 6620 7468 6572 6520   Check if there 
-00011b30: 6973 2061 6e79 2070 656e 6469 6e67 2063  is any pending c
-00011b40: 6f6e 6663 6861 6e67 652e 0a0a 2020 2020  onfchange...    
-00011b50: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
-00011b60: 6361 6e20 6265 2066 616c 7365 2070 6f73  can be false pos
-00011b70: 6974 6976 652e 0a20 2020 2020 2020 2022  itive..        "
-00011b80: 2222 0a20 2020 2064 6566 2070 726f 6d6f  "".    def promo
-00011b90: 7461 626c 6528 7365 6c66 2920 2d3e 2062  table(self) -> b
-00011ba0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00011bb0: 0a20 2020 2020 2020 2049 6e64 6963 6174  .        Indicat
-00011bc0: 6573 2077 6865 7468 6572 2073 7461 7465  es whether state
-00011bd0: 206d 6163 6869 6e65 2063 616e 2062 6520   machine can be 
-00011be0: 7072 6f6d 6f74 6564 2074 6f20 6c65 6164  promoted to lead
-00011bf0: 6572 2c0a 2020 2020 2020 2020 7768 6963  er,.        whic
-00011c00: 6820 6973 2074 7275 6520 7768 656e 2069  h is true when i
-00011c10: 7427 7320 6120 766f 7465 7220 616e 6420  t's a voter and 
-00011c20: 6974 7320 6f77 6e20 6964 2069 7320 696e  its own id is in
-00011c30: 2070 726f 6772 6573 7320 6c69 7374 2e0a   progress list..
-00011c40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011c50: 6465 6620 706f 7374 5f63 6f6e 665f 6368  def post_conf_ch
-00011c60: 616e 6765 2873 656c 6629 202d 3e20 2243  ange(self) -> "C
-00011c70: 6f6e 6653 7461 7465 5265 6622 3a0a 2020  onfStateRef":.  
-00011c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011c90: 2020 5570 6461 7465 7320 7468 6520 696e    Updates the in
-00011ca0: 2d6d 656d 6f72 7920 7374 6174 6520 616e  -memory state an
-00011cb0: 642c 2077 6865 6e20 6e65 6365 7373 6172  d, when necessar
-00011cc0: 792c 2063 6172 7269 6573 206f 7574 2061  y, carries out a
-00011cd0: 6464 6974 696f 6e61 6c20 6163 7469 6f6e  dditional action
-00011ce0: 730a 2020 2020 2020 2020 7375 6368 2061  s.        such a
-00011cf0: 7320 7265 6163 7469 6e67 2074 6f20 7468  s reacting to th
-00011d00: 6520 7265 6d6f 7661 6c20 6f66 206e 6f64  e removal of nod
-00011d10: 6573 206f 7220 6368 616e 6765 6420 7175  es or changed qu
-00011d20: 6f72 756d 2072 6571 7569 7265 6d65 6e74  orum requirement
-00011d30: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00011d40: 2020 2064 6566 2069 6e5f 6c65 6173 6528     def in_lease(
-00011d50: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
-00011d60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011d70: 2020 2052 6574 7572 6e73 2077 6865 7468     Returns wheth
-00011d80: 6572 2074 6865 2063 7572 7265 6e74 2072  er the current r
-00011d90: 6166 7420 6973 2069 6e20 6c65 6173 652e  aft is in lease.
-00011da0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011db0: 2064 6566 2068 616e 646c 655f 6865 6172   def handle_hear
-00011dc0: 7462 6561 7428 7365 6c66 2c20 6d73 673a  tbeat(self, msg:
-00011dd0: 2022 4d65 7373 6167 6522 207c 2022 4d65   "Message" | "Me
-00011de0: 7373 6167 6552 6566 2229 202d 3e20 4e6f  ssageRef") -> No
-00011df0: 6e65 3a0a 2020 2020 2020 2020 2222 2246  ne:.        """F
-00011e00: 6f72 2061 206d 6573 7361 6765 2c20 636f  or a message, co
-00011e10: 6d6d 6974 2061 6e64 2073 656e 6420 6f75  mmit and send ou
-00011e20: 7420 6865 6172 7462 6561 742e 2222 220a  t heartbeat.""".
-00011e30: 2020 2020 6465 6620 6861 6e64 6c65 5f61      def handle_a
-00011e40: 7070 656e 645f 656e 7472 6965 7328 7365  ppend_entries(se
-00011e50: 6c66 2c20 6d73 673a 2022 4d65 7373 6167  lf, msg: "Messag
-00011e60: 6522 207c 2022 4d65 7373 6167 6552 6566  e" | "MessageRef
-00011e70: 2229 202d 3e20 4e6f 6e65 3a0a 2020 2020  ") -> None:.    
-00011e80: 2020 2020 2222 2246 6f72 2061 2067 6976      """For a giv
-00011e90: 656e 206d 6573 7361 6765 2c20 6170 7065  en message, appe
-00011ea0: 6e64 2074 6865 2065 6e74 7269 6573 2074  nd the entries t
-00011eb0: 6f20 7468 6520 6c6f 672e 2222 220a 2020  o the log.""".  
-00011ec0: 2020 6465 6620 7265 7175 6573 745f 736e    def request_sn
-00011ed0: 6170 7368 6f74 2873 656c 6629 202d 3e20  apshot(self) -> 
-00011ee0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00011ef0: 220a 2020 2020 2020 2020 5265 7175 6573  ".        Reques
-00011f00: 7420 6120 736e 6170 7368 6f74 2066 726f  t a snapshot fro
-00011f10: 6d20 6120 6c65 6164 6572 2e0a 2020 2020  m a leader..    
-00011f20: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00011f30: 7072 7328 7365 6c66 2920 2d3e 2022 5072  prs(self) -> "Pr
-00011f40: 6f67 7265 7373 5472 6163 6b65 7252 6566  ogressTrackerRef
-00011f50: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
-00011f60: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
-00011f70: 2072 6561 642d 6f6e 6c79 2072 6566 6572   read-only refer
-00011f80: 656e 6365 2074 6f20 7468 6520 7072 6f67  ence to the prog
-00011f90: 7265 7373 2073 6574 2e0a 2020 2020 2020  ress set..      
-00011fa0: 2020 2222 220a 2020 2020 6465 6620 7265    """.    def re
-00011fb0: 7365 7428 7365 6c66 2c20 7465 726d 3a20  set(self, term: 
-00011fc0: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-00011fd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011fe0: 2020 5265 7365 7473 2074 6865 2063 7572    Resets the cur
-00011ff0: 7265 6e74 206e 6f64 6520 746f 2061 2067  rent node to a g
-00012000: 6976 656e 2074 6572 6d2e 0a20 2020 2020  iven term..     
-00012010: 2020 2022 2222 0a20 2020 2064 6566 2072     """.    def r
-00012020: 6573 746f 7265 2873 656c 662c 2073 6e61  estore(self, sna
-00012030: 7073 686f 743a 2022 536e 6170 7368 6f74  pshot: "Snapshot
-00012040: 2220 7c20 2253 6e61 7073 686f 7452 6566  " | "SnapshotRef
-00012050: 2229 202d 3e20 626f 6f6c 3a0a 2020 2020  ") -> bool:.    
-00012060: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012070: 5265 636f 7665 7273 2074 6865 2073 7461  Recovers the sta
-00012080: 7465 206d 6163 6869 6e65 2066 726f 6d20  te machine from 
-00012090: 6120 736e 6170 7368 6f74 2e20 4974 2072  a snapshot. It r
-000120a0: 6573 746f 7265 7320 7468 6520 6c6f 6720  estores the log 
-000120b0: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
-000120c0: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
-000120d0: 2073 7461 7465 206d 6163 6869 6e65 2e0a   state machine..
-000120e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000120f0: 6465 6620 736e 6170 2873 656c 6629 202d  def snap(self) -
-00012100: 3e20 4f70 7469 6f6e 616c 5b22 536e 6170  > Optional["Snap
-00012110: 7368 6f74 5265 6622 5d3a 0a20 2020 2020  shotRef"]:.     
-00012120: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00012130: 7261 6273 2061 2072 6566 6572 656e 6365  rabs a reference
-00012140: 2074 6f20 7468 6520 736e 6170 7368 6f74   to the snapshot
-00012150: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012160: 2064 6566 2073 746f 7265 2873 656c 6629   def store(self)
-00012170: 202d 3e20 224d 656d 5374 6f72 6167 6552   -> "MemStorageR
-00012180: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-00012190: 0a20 2020 2020 2020 2047 7261 6273 2061  .        Grabs a
-000121a0: 6e20 696d 6d75 7461 626c 6520 7265 6665  n immutable refe
-000121b0: 7265 6e63 6520 746f 2074 6865 2073 746f  rence to the sto
-000121c0: 7265 2e0a 2020 2020 2020 2020 2222 220a  re..        """.
-000121d0: 2020 2020 6465 6620 6f6e 5f70 6572 7369      def on_persi
-000121e0: 7374 5f73 6e61 7028 7365 6c66 2c20 696e  st_snap(self, in
-000121f0: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
-00012200: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00012210: 2020 2020 2020 204e 6f74 6966 6965 7320         Notifies 
-00012220: 7468 6174 2074 6865 2073 6e61 7073 686f  that the snapsho
-00012230: 7420 6861 7665 2062 6565 6e20 7065 7273  t have been pers
-00012240: 6973 7465 642e 0a20 2020 2020 2020 2022  isted..        "
-00012250: 2222 0a20 2020 2064 6566 2061 626f 7274  "".    def abort
-00012260: 5f6c 6561 6465 725f 7472 616e 7366 6572  _leader_transfer
-00012270: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00012280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012290: 2020 2020 5374 6f70 7320 7468 6520 7472      Stops the tr
-000122a0: 616e 7366 6572 206f 6620 6120 6c65 6164  ansfer of a lead
-000122b0: 6572 2e0a 2020 2020 2020 2020 2222 220a  er..        """.
-000122c0: 2020 2020 6465 6620 6361 6d70 6169 676e      def campaign
-000122d0: 2873 656c 662c 2074 7970 3a20 7374 7229  (self, typ: str)
-000122e0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-000122f0: 2020 2222 220a 2020 2020 2020 2020 4361    """.        Ca
-00012300: 6d70 6169 676e 2074 6f20 6174 7465 6d70  mpaign to attemp
-00012310: 7420 746f 2062 6563 6f6d 6520 6120 6c65  t to become a le
-00012320: 6164 6572 2e0a 0a20 2020 2020 2020 2049  ader...        I
-00012330: 6620 7072 6576 6f74 6520 6973 2065 6e61  f prevote is ena
-00012340: 626c 6564 2c20 7468 6973 2069 7320 6861  bled, this is ha
-00012350: 6e64 6c65 6420 6173 2077 656c 6c2e 0a20  ndled as well.. 
-00012360: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00012370: 6566 2067 6574 5f6c 6561 645f 7472 616e  ef get_lead_tran
-00012380: 7366 6572 6565 2873 656c 6629 202d 3e20  sferee(self) -> 
-00012390: 4f70 7469 6f6e 616c 5b69 6e74 5d3a 0a20  Optional[int]:. 
-000123a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000123b0: 2020 2060 6c65 6164 5f74 7261 6e73 6665     `lead_transfe
-000123c0: 7265 6560 3a20 4944 206f 6620 7468 6520  ree`: ID of the 
-000123d0: 6c65 6164 6572 2074 7261 6e73 6665 7220  leader transfer 
-000123e0: 7461 7267 6574 2077 6865 6e20 6974 7320  target when its 
-000123f0: 7661 6c75 6520 6973 206e 6f74 204e 6f6e  value is not Non
-00012400: 652e 0a0a 2020 2020 2020 2020 4966 2074  e...        If t
-00012410: 6869 7320 6973 2053 6f6d 6528 6964 292c  his is Some(id),
-00012420: 2077 6520 666f 6c6c 6f77 2074 6865 2070   we follow the p
-00012430: 726f 6365 6475 7265 2064 6566 696e 6564  rocedure defined
-00012440: 2069 6e20 7261 6674 2074 6865 7369 7320   in raft thesis 
-00012450: 332e 3130 2e0a 2020 2020 2020 2020 2222  3.10..        ""
-00012460: 220a 2020 2020 6465 6620 7365 745f 6c65  ".    def set_le
-00012470: 6164 5f74 7261 6e73 6665 7265 6528 7365  ad_transferee(se
-00012480: 6c66 2c20 6c65 6164 5f74 7261 6e73 6665  lf, lead_transfe
-00012490: 7265 653a 2069 6e74 2920 2d3e 204e 6f6e  ree: int) -> Non
-000124a0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000124b0: 2020 2020 2020 2060 6c65 6164 5f74 7261         `lead_tra
-000124c0: 6e73 6665 7265 6560 3a20 4944 206f 6620  nsferee`: ID of 
-000124d0: 7468 6520 6c65 6164 6572 2074 7261 6e73  the leader trans
-000124e0: 6665 7220 7461 7267 6574 2077 6865 6e20  fer target when 
-000124f0: 6974 7320 7661 6c75 6520 6973 206e 6f74  its value is not
-00012500: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-00012510: 4966 2074 6869 7320 6973 2053 6f6d 6528  If this is Some(
-00012520: 6964 292c 2077 6520 666f 6c6c 6f77 2074  id), we follow t
-00012530: 6865 2070 726f 6365 6475 7265 2064 6566  he procedure def
-00012540: 696e 6564 2069 6e20 7261 6674 2074 6865  ined in raft the
-00012550: 7369 7320 332e 3130 2e0a 2020 2020 2020  sis 3.10..      
-00012560: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-00012570: 745f 7465 726d 2873 656c 6629 202d 3e20  t_term(self) -> 
-00012580: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00012590: 0a20 2020 2020 2020 2060 7465 726d 603a  .        `term`:
-000125a0: 2054 6865 2063 7572 7265 6e74 2065 6c65   The current ele
-000125b0: 6374 696f 6e20 7465 726d 2e0a 2020 2020  ction term..    
-000125c0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-000125d0: 7365 745f 7465 726d 2873 656c 662c 2074  set_term(self, t
-000125e0: 6572 6d3a 2069 6e74 2920 2d3e 204e 6f6e  erm: int) -> Non
-000125f0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00012600: 2020 2020 2020 2060 7465 726d 603a 2054         `term`: T
-00012610: 6865 2063 7572 7265 6e74 2065 6c65 6374  he current elect
-00012620: 696f 6e20 7465 726d 2e0a 2020 2020 2020  ion term..      
-00012630: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-00012640: 745f 766f 7465 2873 656c 6629 202d 3e20  t_vote(self) -> 
-00012650: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00012660: 0a20 2020 2020 2020 2060 766f 7465 603a  .        `vote`:
-00012670: 2057 6869 6368 2070 6565 7220 7468 6973   Which peer this
-00012680: 2072 6166 7420 6973 2076 6f74 696e 6720   raft is voting 
-00012690: 666f 722e 0a20 2020 2020 2020 2022 2222  for..        """
-000126a0: 0a20 2020 2064 6566 2073 6574 5f76 6f74  .    def set_vot
-000126b0: 6528 7365 6c66 2c20 766f 7465 3a20 696e  e(self, vote: in
-000126c0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-000126d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000126e0: 6076 6f74 6560 3a20 5768 6963 6820 7065  `vote`: Which pe
-000126f0: 6572 2074 6869 7320 7261 6674 2069 7320  er this raft is 
-00012700: 766f 7469 6e67 2066 6f72 2e0a 2020 2020  voting for..    
-00012710: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00012720: 6765 745f 7072 696f 7269 7479 2873 656c  get_priority(sel
-00012730: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00012740: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00012750: 7072 696f 7269 7479 603a 2054 6865 2065  priority`: The e
-00012760: 6c65 6374 696f 6e20 7072 696f 7269 7479  lection priority
-00012770: 206f 6620 7468 6973 206e 6f64 652e 0a20   of this node.. 
-00012780: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00012790: 6566 2073 6574 5f70 7269 6f72 6974 7928  ef set_priority(
-000127a0: 7365 6c66 2c20 7072 696f 7269 7479 3a20  self, priority: 
-000127b0: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
-000127c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000127d0: 2020 6070 7269 6f72 6974 7960 3a20 5468    `priority`: Th
-000127e0: 6520 656c 6563 7469 6f6e 2070 7269 6f72  e election prior
-000127f0: 6974 7920 6f66 2074 6869 7320 6e6f 6465  ity of this node
-00012800: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00012810: 2020 6465 6620 6765 745f 6c65 6164 6572    def get_leader
-00012820: 5f69 6428 7365 6c66 2920 2d3e 2069 6e74  _id(self) -> int
-00012830: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012840: 2020 2020 2020 606c 6561 6465 725f 6964        `leader_id
-00012850: 603a 2054 6865 206c 6561 6465 7220 6964  `: The leader id
-00012860: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012870: 2064 6566 2073 6574 5f6c 6561 6465 725f   def set_leader_
-00012880: 6964 2873 656c 662c 206c 6561 6465 725f  id(self, leader_
-00012890: 6964 3a20 696e 7429 202d 3e20 4e6f 6e65  id: int) -> None
-000128a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000128b0: 2020 2020 2020 606c 6561 6465 725f 6964        `leader_id
-000128c0: 603a 2054 6865 206c 6561 6465 7220 6964  `: The leader id
-000128d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000128e0: 2064 6566 2067 6574 5f6d 6178 5f6d 7367   def get_max_msg
-000128f0: 5f73 697a 6528 7365 6c66 2920 2d3e 2069  _size(self) -> i
-00012900: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-00012910: 2020 2020 2020 2020 606d 6178 5f6d 7367          `max_msg
-00012920: 5f73 697a 6560 3a20 5468 6520 6d61 7869  _size`: The maxi
-00012930: 6d75 6d20 6c65 6e67 7468 2028 696e 2062  mum length (in b
-00012940: 7974 6573 2920 6f66 2061 6c6c 2074 6865  ytes) of all the
-00012950: 2065 6e74 7269 6573 2e0a 2020 2020 2020   entries..      
-00012960: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00012970: 745f 6d61 785f 6d73 675f 7369 7a65 2873  t_max_msg_size(s
-00012980: 656c 662c 206d 6178 5f6d 7367 5f73 697a  elf, max_msg_siz
-00012990: 653a 2069 6e74 2920 2d3e 204e 6f6e 653a  e: int) -> None:
-000129a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000129b0: 2020 2020 2060 6d61 785f 6d73 675f 7369       `max_msg_si
-000129c0: 7a65 603a 2054 6865 206d 6178 696d 756d  ze`: The maximum
-000129d0: 206c 656e 6774 6820 2869 6e20 6279 7465   length (in byte
-000129e0: 7329 206f 6620 616c 6c20 7468 6520 656e  s) of all the en
-000129f0: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
-00012a00: 2222 0a20 2020 2064 6566 2067 6574 5f70  "".    def get_p
-00012a10: 656e 6469 6e67 5f63 6f6e 665f 696e 6465  ending_conf_inde
-00012a20: 7828 7365 6c66 2920 2d3e 2069 6e74 3a0a  x(self) -> int:.
-00012a30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012a40: 2020 2020 6070 656e 6469 6e67 5f63 6f6e      `pending_con
-00012a50: 665f 696e 6465 7860 3a20 4f6e 6c79 206f  f_index`: Only o
-00012a60: 6e65 2063 6f6e 6620 6368 616e 6765 206d  ne conf change m
-00012a70: 6179 2062 6520 7065 6e64 696e 6720 2869  ay be pending (i
-00012a80: 6e20 7468 6520 6c6f 672c 2062 7574 206e  n the log, but n
-00012a90: 6f74 2079 6574 0a20 2020 2020 2020 2061  ot yet.        a
-00012aa0: 7070 6c69 6564 2920 6174 2061 2074 696d  pplied) at a tim
-00012ab0: 652e 2054 6869 7320 6973 2065 6e66 6f72  e. This is enfor
-00012ac0: 6365 6420 7669 6120 6070 656e 6469 6e67  ced via `pending
-00012ad0: 5f63 6f6e 665f 696e 6465 7860 2c20 7768  _conf_index`, wh
-00012ae0: 6963 680a 2020 2020 2020 2020 6973 2073  ich.        is s
-00012af0: 6574 2074 6f20 6120 7661 6c75 6520 3e3d  et to a value >=
-00012b00: 2074 6865 206c 6f67 2069 6e64 6578 206f   the log index o
-00012b10: 6620 7468 6520 6c61 7465 7374 2070 656e  f the latest pen
-00012b20: 6469 6e67 0a20 2020 2020 2020 2063 6f6e  ding.        con
-00012b30: 6669 6775 7261 7469 6f6e 2063 6861 6e67  figuration chang
-00012b40: 6520 2869 6620 616e 7929 2e20 436f 6e66  e (if any). Conf
-00012b50: 6967 2063 6861 6e67 6573 2061 7265 206f  ig changes are o
-00012b60: 6e6c 7920 616c 6c6f 7765 6420 746f 0a20  nly allowed to. 
-00012b70: 2020 2020 2020 2062 6520 7072 6f70 6f73         be propos
-00012b80: 6564 2069 6620 7468 6520 6c65 6164 6572  ed if the leader
-00012b90: 2773 2061 7070 6c69 6564 2069 6e64 6578  's applied index
-00012ba0: 2069 7320 6772 6561 7465 7220 7468 616e   is greater than
-00012bb0: 2074 6869 730a 2020 2020 2020 2020 7661   this.        va
-00012bc0: 6c75 652e 0a0a 2020 2020 2020 2020 5468  lue...        Th
-00012bd0: 6973 2076 616c 7565 2069 7320 636f 6e73  is value is cons
-00012be0: 6572 7661 7469 7665 6c79 2073 6574 2069  ervatively set i
-00012bf0: 6e20 6361 7365 7320 7768 6572 6520 7468  n cases where th
-00012c00: 6572 6520 6d61 7920 6265 2061 2063 6f6e  ere may be a con
-00012c10: 6669 6775 7261 7469 6f6e 2063 6861 6e67  figuration chang
-00012c20: 6520 7065 6e64 696e 672c 0a20 2020 2020  e pending,.     
-00012c30: 2020 2062 7574 2073 6361 6e6e 696e 6720     but scanning 
-00012c40: 7468 6520 6c6f 6720 6973 2070 6f73 7369  the log is possi
-00012c50: 626c 7920 6578 7065 6e73 6976 652e 2054  bly expensive. T
-00012c60: 6869 7320 696d 706c 6965 7320 7468 6174  his implies that
-00012c70: 2074 6865 2069 6e64 6578 2073 7461 7465   the index state
-00012c80: 6420 6865 7265 206d 6179 206e 6f74 0a20  d here may not. 
-00012c90: 2020 2020 2020 206e 6563 6573 7361 7269         necessari
-00012ca0: 6c79 2062 6520 6120 636f 6e66 6967 2063  ly be a config c
-00012cb0: 6861 6e67 6520 656e 7472 792c 2061 6e64  hange entry, and
-00012cc0: 2069 7420 6d61 7920 6e6f 7420 6265 2061   it may not be a
-00012cd0: 2060 4265 6769 6e4d 656d 6265 7273 6869   `BeginMembershi
-00012ce0: 7043 6861 6e67 6560 2065 6e74 7279 2c20  pChange` entry, 
-00012cf0: 6576 656e 2069 660a 2020 2020 2020 2020  even if.        
-00012d00: 7765 2073 6574 2074 6869 7320 746f 206f  we set this to o
-00012d10: 6e65 2e0a 2020 2020 2020 2020 2222 220a  ne..        """.
-00012d20: 2020 2020 6465 6620 7365 745f 7065 6e64      def set_pend
-00012d30: 696e 675f 636f 6e66 5f69 6e64 6578 2873  ing_conf_index(s
-00012d40: 656c 662c 2070 656e 6469 6e67 5f63 6f6e  elf, pending_con
-00012d50: 665f 696e 6465 783a 2069 6e74 2920 2d3e  f_index: int) ->
-00012d60: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00012d70: 2222 0a20 2020 2020 2020 2060 7065 6e64  "".        `pend
-00012d80: 696e 675f 636f 6e66 5f69 6e64 6578 603a  ing_conf_index`:
-00012d90: 204f 6e6c 7920 6f6e 6520 636f 6e66 2063   Only one conf c
-00012da0: 6861 6e67 6520 6d61 7920 6265 2070 656e  hange may be pen
-00012db0: 6469 6e67 2028 696e 2074 6865 206c 6f67  ding (in the log
-00012dc0: 2c20 6275 7420 6e6f 7420 7965 740a 2020  , but not yet.  
-00012dd0: 2020 2020 2020 6170 706c 6965 6429 2061        applied) a
-00012de0: 7420 6120 7469 6d65 2e20 5468 6973 2069  t a time. This i
-00012df0: 7320 656e 666f 7263 6564 2076 6961 2060  s enforced via `
-00012e00: 7065 6e64 696e 675f 636f 6e66 5f69 6e64  pending_conf_ind
-00012e10: 6578 602c 2077 6869 6368 0a20 2020 2020  ex`, which.     
-00012e20: 2020 2069 7320 7365 7420 746f 2061 2076     is set to a v
-00012e30: 616c 7565 203e 3d20 7468 6520 6c6f 6720  alue >= the log 
-00012e40: 696e 6465 7820 6f66 2074 6865 206c 6174  index of the lat
-00012e50: 6573 7420 7065 6e64 696e 670a 2020 2020  est pending.    
-00012e60: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
-00012e70: 6e20 6368 616e 6765 2028 6966 2061 6e79  n change (if any
-00012e80: 292e 2043 6f6e 6669 6720 6368 616e 6765  ). Config change
-00012e90: 7320 6172 6520 6f6e 6c79 2061 6c6c 6f77  s are only allow
-00012ea0: 6564 2074 6f0a 2020 2020 2020 2020 6265  ed to.        be
-00012eb0: 2070 726f 706f 7365 6420 6966 2074 6865   proposed if the
-00012ec0: 206c 6561 6465 7227 7320 6170 706c 6965   leader's applie
-00012ed0: 6420 696e 6465 7820 6973 2067 7265 6174  d index is great
-00012ee0: 6572 2074 6861 6e20 7468 6973 0a20 2020  er than this.   
-00012ef0: 2020 2020 2076 616c 7565 2e0a 0a20 2020       value...   
-00012f00: 2020 2020 2054 6869 7320 7661 6c75 6520       This value 
-00012f10: 6973 2063 6f6e 7365 7276 6174 6976 656c  is conservativel
-00012f20: 7920 7365 7420 696e 2063 6173 6573 2077  y set in cases w
-00012f30: 6865 7265 2074 6865 7265 206d 6179 2062  here there may b
-00012f40: 6520 6120 636f 6e66 6967 7572 6174 696f  e a configuratio
-00012f50: 6e20 6368 616e 6765 2070 656e 6469 6e67  n change pending
-00012f60: 2c0a 2020 2020 2020 2020 6275 7420 7363  ,.        but sc
-00012f70: 616e 6e69 6e67 2074 6865 206c 6f67 2069  anning the log i
-00012f80: 7320 706f 7373 6962 6c79 2065 7870 656e  s possibly expen
-00012f90: 7369 7665 2e20 5468 6973 2069 6d70 6c69  sive. This impli
-00012fa0: 6573 2074 6861 7420 7468 6520 696e 6465  es that the inde
-00012fb0: 7820 7374 6174 6564 2068 6572 6520 6d61  x stated here ma
-00012fc0: 7920 6e6f 740a 2020 2020 2020 2020 6e65  y not.        ne
-00012fd0: 6365 7373 6172 696c 7920 6265 2061 2063  cessarily be a c
-00012fe0: 6f6e 6669 6720 6368 616e 6765 2065 6e74  onfig change ent
-00012ff0: 7279 2c20 616e 6420 6974 206d 6179 206e  ry, and it may n
-00013000: 6f74 2062 6520 6120 6042 6567 696e 4d65  ot be a `BeginMe
-00013010: 6d62 6572 7368 6970 4368 616e 6765 6020  mbershipChange` 
-00013020: 656e 7472 792c 2065 7665 6e20 6966 0a20  entry, even if. 
-00013030: 2020 2020 2020 2077 6520 7365 7420 7468         we set th
-00013040: 6973 2074 6f20 6f6e 652e 0a20 2020 2020  is to one..     
-00013050: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-00013060: 6574 5f70 656e 6469 6e67 5f72 6571 7565  et_pending_reque
-00013070: 7374 5f73 6e61 7073 686f 7428 7365 6c66  st_snapshot(self
-00013080: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00013090: 2020 2222 220a 2020 2020 2020 2020 6070    """.        `p
-000130a0: 656e 6469 6e67 5f72 6571 7565 7374 5f73  ending_request_s
-000130b0: 6e61 7073 686f 7460 3a20 5468 6520 7065  napshot`: The pe
-000130c0: 6572 2069 7320 7265 7175 6573 7469 6e67  er is requesting
-000130d0: 2073 6e61 7073 686f 742c 2069 7420 6973   snapshot, it is
-000130e0: 2074 6865 2069 6e64 6578 2074 6861 7420   the index that 
-000130f0: 7468 6520 666f 6c6c 6f77 6572 0a20 2020  the follower.   
-00013100: 2020 2020 206e 6565 6473 2069 7420 746f       needs it to
-00013110: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
-00013120: 6120 736e 6170 7368 6f74 2e0a 2020 2020  a snapshot..    
-00013130: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00013140: 7365 745f 7065 6e64 696e 675f 7265 7175  set_pending_requ
-00013150: 6573 745f 736e 6170 7368 6f74 2873 656c  est_snapshot(sel
-00013160: 662c 2070 656e 6469 6e67 5f72 6571 7565  f, pending_reque
-00013170: 7374 5f73 6e61 7073 686f 743a 2069 6e74  st_snapshot: int
-00013180: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00013190: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-000131a0: 7065 6e64 696e 675f 7265 7175 6573 745f  pending_request_
-000131b0: 736e 6170 7368 6f74 603a 2054 6865 2070  snapshot`: The p
-000131c0: 6565 7220 6973 2072 6571 7565 7374 696e  eer is requestin
-000131d0: 6720 736e 6170 7368 6f74 2c20 6974 2069  g snapshot, it i
-000131e0: 7320 7468 6520 696e 6465 7820 7468 6174  s the index that
-000131f0: 2074 6865 2066 6f6c 6c6f 7765 720a 2020   the follower.  
-00013200: 2020 2020 2020 6e65 6564 7320 6974 2074        needs it t
-00013210: 6f20 6265 2069 6e63 6c75 6465 6420 696e  o be included in
-00013220: 2061 2073 6e61 7073 686f 742e 0a20 2020   a snapshot..   
-00013230: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00013240: 2067 6574 5f69 6428 7365 6c66 2920 2d3e   get_id(self) ->
-00013250: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00013260: 220a 2020 2020 2020 2020 6069 6460 3a20  ".        `id`: 
-00013270: 5468 6520 4944 206f 6620 7468 6973 206e  The ID of this n
-00013280: 6f64 652e 0a20 2020 2020 2020 2022 2222  ode..        """
-00013290: 0a20 2020 2064 6566 2073 6574 5f69 6428  .    def set_id(
-000132a0: 7365 6c66 2c20 6964 3a20 696e 7429 202d  self, id: int) -
-000132b0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-000132c0: 2222 220a 2020 2020 2020 2020 6069 6460  """.        `id`
-000132d0: 3a20 5468 6520 4944 206f 6620 7468 6973  : The ID of this
-000132e0: 206e 6f64 652e 0a20 2020 2020 2020 2022   node..        "
-000132f0: 2222 0a20 2020 2064 6566 2067 6574 5f6d  "".    def get_m
-00013300: 7367 7328 7365 6c66 2920 2d3e 204c 6973  sgs(self) -> Lis
-00013310: 745b 224d 6573 7361 6765 5265 6622 5d3a  t["MessageRef"]:
+00009d90: 745f 7465 726d 2873 656c 6629 202d 3e20  t_term(self) -> 
+00009da0: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+00009db0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00009dc0: 5f74 6572 6d28 7365 6c66 2c20 7465 726d  _term(self, term
+00009dd0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00009de0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+00009df0: 2020 2020 6465 6620 636c 6561 725f 7465      def clear_te
+00009e00: 726d 2873 656c 6629 202d 3e20 4e6f 6e65  rm(self) -> None
+00009e10: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+00009e20: 220a 2020 2020 6465 6620 6765 745f 696e  ".    def get_in
+00009e30: 6465 7828 7365 6c66 2920 2d3e 2069 6e74  dex(self) -> int
+00009e40: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+00009e50: 220a 2020 2020 6465 6620 7365 745f 696e  ".    def set_in
+00009e60: 6465 7828 7365 6c66 2c20 696e 6465 783a  dex(self, index:
+00009e70: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00009e80: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+00009e90: 2020 2064 6566 2063 6c65 6172 5f69 6e64     def clear_ind
+00009ea0: 6578 2873 656c 6629 202d 3e20 4e6f 6e65  ex(self) -> None
+00009eb0: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+00009ec0: 220a 2020 2020 6465 6620 6765 745f 7379  ".    def get_sy
+00009ed0: 6e63 5f6c 6f67 2873 656c 6629 202d 3e20  nc_log(self) -> 
+00009ee0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00009ef0: 220a 2020 2020 2020 2020 4465 7072 6563  ".        Deprec
+00009f00: 6174 6564 2120 4974 2069 7320 6b65 7074  ated! It is kept
+00009f10: 2066 6f72 2062 6163 6b77 6172 6420 636f   for backward co
+00009f20: 6d70 6174 6962 696c 6974 792e 0a20 2020  mpatibility..   
+00009f30: 2020 2020 2054 4f44 4f3a 2072 656d 6f76       TODO: remov
+00009f40: 6520 6974 2069 6e20 7468 6520 6e65 7874  e it in the next
+00009f50: 206d 616a 6f72 2072 656c 6561 7365 2e0a   major release..
+00009f60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009f70: 6465 6620 7365 745f 7379 6e63 5f6c 6f67  def set_sync_log
+00009f80: 2873 656c 662c 2073 796e 635f 6c6f 673a  (self, sync_log:
+00009f90: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a   bool) -> None:.
+00009fa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00009fb0: 2020 2020 4465 7072 6563 6174 6564 2120      Deprecated! 
+00009fc0: 4974 2069 7320 6b65 7074 2066 6f72 2062  It is kept for b
+00009fd0: 6163 6b77 6172 6420 636f 6d70 6174 6962  ackward compatib
+00009fe0: 696c 6974 792e 0a20 2020 2020 2020 2054  ility..        T
+00009ff0: 4f44 4f3a 2072 656d 6f76 6520 6974 2069  ODO: remove it i
+0000a000: 6e20 7468 6520 6e65 7874 206d 616a 6f72  n the next major
+0000a010: 2072 656c 6561 7365 2e0a 2020 2020 2020   release..      
+0000a020: 2020 2222 220a 2020 2020 6465 6620 636c    """.    def cl
+0000a030: 6561 725f 7379 6e63 5f6c 6f67 2873 656c  ear_sync_log(sel
+0000a040: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+0000a050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000a060: 4465 7072 6563 6174 6564 2120 4974 2069  Deprecated! It i
+0000a070: 7320 6b65 7074 2066 6f72 2062 6163 6b77  s kept for backw
+0000a080: 6172 6420 636f 6d70 6174 6962 696c 6974  ard compatibilit
+0000a090: 792e 0a20 2020 2020 2020 2054 4f44 4f3a  y..        TODO:
+0000a0a0: 2072 656d 6f76 6520 6974 2069 6e20 7468   remove it in th
+0000a0b0: 6520 6e65 7874 206d 616a 6f72 2072 656c  e next major rel
+0000a0c0: 6561 7365 2e0a 2020 2020 2020 2020 2222  ease..        ""
+0000a0d0: 220a 0a63 6c61 7373 2045 6e74 7279 285f  "..class Entry(_
+0000a0e0: 5f41 5049 5f45 6e74 7279 293a 0a20 2020  _API_Entry):.   
+0000a0f0: 2022 2222 0a20 2020 2054 6865 2065 6e74   """.    The ent
+0000a100: 7279 2069 7320 6120 7479 7065 206f 6620  ry is a type of 
+0000a110: 6368 616e 6765 2074 6861 7420 6e65 6564  change that need
+0000a120: 7320 746f 2062 6520 6170 706c 6965 642e  s to be applied.
+0000a130: 2049 7420 636f 6e74 6169 6e73 2074 776f   It contains two
+0000a140: 2064 6174 6120 6669 656c 6473 2e0a 2020   data fields..  
+0000a150: 2020 5768 696c 6520 7468 6520 6669 656c    While the fiel
+0000a160: 6473 2061 7265 2062 7569 6c74 2069 6e74  ds are built int
+0000a170: 6f20 7468 6520 6d6f 6465 6c3b 2074 6865  o the model; the
+0000a180: 6972 2075 7361 6765 2069 7320 6465 7465  ir usage is dete
+0000a190: 726d 696e 6564 2062 7920 7468 6520 656e  rmined by the en
+0000a1a0: 7472 795f 7479 7065 2e0a 0a20 2020 2046  try_type...    F
+0000a1b0: 6f72 206e 6f72 6d61 6c20 656e 7472 6965  or normal entrie
+0000a1c0: 732c 2074 6865 2064 6174 6120 6669 656c  s, the data fiel
+0000a1d0: 6420 7368 6f75 6c64 2063 6f6e 7461 696e  d should contain
+0000a1e0: 2074 6865 2064 6174 6120 6368 616e 6765   the data change
+0000a1f0: 2074 6861 7420 7368 6f75 6c64 2062 6520   that should be 
+0000a200: 6170 706c 6965 642e 0a20 2020 2054 6865  applied..    The
+0000a210: 2063 6f6e 7465 7874 2066 6965 6c64 2063   context field c
+0000a220: 616e 2062 6520 7573 6564 2066 6f72 2061  an be used for a
+0000a230: 6e79 2063 6f6e 7465 7874 7561 6c20 6461  ny contextual da
+0000a240: 7461 2074 6861 7420 6d69 6768 7420 6265  ta that might be
+0000a250: 2072 656c 6576 616e 7420 746f 2074 6865   relevant to the
+0000a260: 0a20 2020 2061 7070 6c69 6361 7469 6f6e  .    application
+0000a270: 206f 6620 7468 6520 6461 7461 2e0a 0a20   of the data... 
+0000a280: 2020 2046 6f72 2063 6f6e 6669 6775 7261     For configura
+0000a290: 7469 6f6e 2063 6861 6e67 6573 2c20 7468  tion changes, th
+0000a2a0: 6520 6461 7461 2077 696c 6c20 636f 6e74  e data will cont
+0000a2b0: 6169 6e20 7468 6520 436f 6e66 4368 616e  ain the ConfChan
+0000a2c0: 6765 206d 6573 7361 6765 2061 6e64 2074  ge message and t
+0000a2d0: 6865 0a20 2020 2063 6f6e 7465 7874 2077  he.    context w
+0000a2e0: 696c 6c20 7072 6f76 6964 6520 616e 7974  ill provide anyt
+0000a2f0: 6869 6e67 206e 6565 6465 6420 746f 2061  hing needed to a
+0000a300: 7373 6973 7420 7468 6520 636f 6e66 6967  ssist the config
+0000a310: 7572 6174 696f 6e20 6368 616e 6765 2e20  uration change. 
+0000a320: 5468 6520 636f 6e74 6578 740a 2020 2020  The context.    
+0000a330: 6966 2066 6f72 2074 6865 2075 7365 7220  if for the user 
+0000a340: 746f 2073 6574 2061 6e64 2075 7365 2069  to set and use i
+0000a350: 6e20 7468 6973 2063 6173 652e 0a20 2020  n this case..   
+0000a360: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+0000a370: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
+0000a380: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000a390: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
+0000a3a0: 202d 3e20 2245 6e74 7279 5265 6622 3a20   -> "EntryRef": 
+0000a3b0: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+0000a3c0: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
+0000a3d0: 6661 756c 7428 2920 2d3e 2022 456e 7472  fault() -> "Entr
+0000a3e0: 7922 3a20 2e2e 2e0a 2020 2020 4073 7461  y": ....    @sta
+0000a3f0: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+0000a400: 6620 6465 636f 6465 2876 3a20 6279 7465  f decode(v: byte
+0000a410: 7329 202d 3e20 2245 6e74 7279 223a 202e  s) -> "Entry": .
+0000a420: 2e2e 0a0a 636c 6173 7320 456e 7472 7952  ....class EntryR
+0000a430: 6566 285f 5f41 5049 5f45 6e74 7279 293a  ef(__API_Entry):
+0000a440: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
+0000a450: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
+0000a460: 636c 6173 733a 6045 6e74 7279 602e 0a20  class:`Entry`.. 
+0000a470: 2020 2022 2222 0a0a 636c 6173 7320 5f5f     """..class __
+0000a480: 4150 495f 436f 6e66 5374 6174 6528 5f5f  API_ConfState(__
+0000a490: 436c 6f6e 6561 626c 652c 205f 5f45 6e63  Cloneable, __Enc
+0000a4a0: 6f64 6572 2c20 5f5f 4465 636f 6465 7229  oder, __Decoder)
+0000a4b0: 3a0a 2020 2020 6465 6620 636c 6f6e 6528  :.    def clone(
+0000a4c0: 7365 6c66 2920 2d3e 2022 436f 6e66 5374  self) -> "ConfSt
+0000a4d0: 6174 6522 3a20 2e2e 2e0a 2020 2020 6465  ate": ....    de
+0000a4e0: 6620 6765 745f 6175 746f 5f6c 6561 7665  f get_auto_leave
+0000a4f0: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+0000a500: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000a510: 2020 2020 6465 6620 7365 745f 6175 746f      def set_auto
+0000a520: 5f6c 6561 7665 2873 656c 662c 2061 7574  _leave(self, aut
+0000a530: 6f5f 6c65 6176 653a 2062 6f6f 6c29 202d  o_leave: bool) -
+0000a540: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000a550: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+0000a560: 636c 6561 725f 6175 746f 5f6c 6561 7665  clear_auto_leave
+0000a570: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0000a580: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000a590: 2020 2020 6465 6620 6765 745f 6c65 6172      def get_lear
+0000a5a0: 6e65 7273 2873 656c 6629 202d 3e20 4c69  ners(self) -> Li
+0000a5b0: 7374 5b69 6e74 5d3a 0a20 2020 2020 2020  st[int]:.       
+0000a5c0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000a5d0: 2073 6574 5f6c 6561 726e 6572 7328 7365   set_learners(se
+0000a5e0: 6c66 2c20 6c65 6172 6e65 7273 3a20 4c69  lf, learners: Li
+0000a5f0: 7374 5b69 6e74 5d29 202d 3e20 4e6f 6e65  st[int]) -> None
+0000a600: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+0000a610: 220a 2020 2020 6465 6620 636c 6561 725f  ".    def clear_
+0000a620: 6c65 6172 6e65 7273 2873 656c 6629 202d  learners(self) -
+0000a630: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000a640: 2222 2220 2222 220a 2020 2020 6465 6620  """ """.    def 
+0000a650: 6765 745f 6c65 6172 6e65 7273 5f6e 6578  get_learners_nex
+0000a660: 7428 7365 6c66 2920 2d3e 204c 6973 745b  t(self) -> List[
+0000a670: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
+0000a680: 2220 2222 220a 2020 2020 6465 6620 7365  " """.    def se
+0000a690: 745f 6c65 6172 6e65 7273 5f6e 6578 7428  t_learners_next(
+0000a6a0: 7365 6c66 2c20 6c65 6172 6e65 7273 5f6e  self, learners_n
+0000a6b0: 6578 743a 204c 6973 745b 696e 745d 2920  ext: List[int]) 
+0000a6c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000a6d0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000a6e0: 2063 6c65 6172 5f6c 6561 726e 6572 735f   clear_learners_
+0000a6f0: 6e65 7874 2873 656c 6629 202d 3e20 4e6f  next(self) -> No
+0000a700: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+0000a710: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0000a720: 766f 7465 7273 2873 656c 6629 202d 3e20  voters(self) -> 
+0000a730: 4c69 7374 5b69 6e74 5d3a 0a20 2020 2020  List[int]:.     
+0000a740: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000a750: 6566 2073 6574 5f76 6f74 6572 7328 7365  ef set_voters(se
+0000a760: 6c66 2c20 766f 7465 7273 3a20 4c69 7374  lf, voters: List
+0000a770: 5b69 6e74 5d29 202d 3e20 4e6f 6e65 3a0a  [int]) -> None:.
+0000a780: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000a790: 2020 2020 6465 6620 636c 6561 725f 766f      def clear_vo
+0000a7a0: 7465 7273 2873 656c 6629 202d 3e20 4e6f  ters(self) -> No
+0000a7b0: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+0000a7c0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0000a7d0: 766f 7465 7273 5f6f 7574 676f 696e 6728  voters_outgoing(
+0000a7e0: 7365 6c66 2920 2d3e 204c 6973 745b 696e  self) -> List[in
+0000a7f0: 745d 3a0a 2020 2020 2020 2020 2222 2220  t]:.        """ 
+0000a800: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0000a810: 766f 7465 7273 5f6f 7574 676f 696e 6728  voters_outgoing(
+0000a820: 7365 6c66 2c20 766f 7465 7273 5f6f 7574  self, voters_out
+0000a830: 676f 696e 673a 204c 6973 745b 696e 745d  going: List[int]
+0000a840: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000a850: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000a860: 6566 2063 6c65 6172 5f76 6f74 6572 735f  ef clear_voters_
+0000a870: 6f75 7467 6f69 6e67 2873 656c 6629 202d  outgoing(self) -
+0000a880: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000a890: 2222 2220 2222 220a 0a63 6c61 7373 2043  """ """..class C
+0000a8a0: 6f6e 6653 7461 7465 285f 5f41 5049 5f43  onfState(__API_C
+0000a8b0: 6f6e 6653 7461 7465 293a 0a20 2020 2022  onfState):.    "
+0000a8c0: 2222 2022 2222 0a0a 2020 2020 6465 6620  "" """..    def 
+0000a8d0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0000a8e0: 2020 7365 6c66 2c20 766f 7465 7273 3a20    self, voters: 
+0000a8f0: 4f70 7469 6f6e 616c 5b4c 6973 745b 696e  Optional[List[in
+0000a900: 745d 5d2c 206c 6561 726e 6572 733a 204f  t]], learners: O
+0000a910: 7074 696f 6e61 6c5b 4c69 7374 5b69 6e74  ptional[List[int
+0000a920: 5d5d 0a20 2020 2029 202d 3e20 4e6f 6e65  ]].    ) -> None
+0000a930: 3a20 2e2e 2e0a 2020 2020 6465 6620 6d61  : ....    def ma
+0000a940: 6b65 5f72 6566 2873 656c 6629 202d 3e20  ke_ref(self) -> 
+0000a950: 2243 6f6e 6653 7461 7465 5265 6622 3a20  "ConfStateRef": 
+0000a960: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+0000a970: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
+0000a980: 6661 756c 7428 2920 2d3e 2022 436f 6e66  fault() -> "Conf
+0000a990: 5374 6174 6522 3a20 2e2e 2e0a 2020 2020  State": ....    
+0000a9a0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+0000a9b0: 2020 6465 6620 6465 636f 6465 2876 3a20    def decode(v: 
+0000a9c0: 6279 7465 7329 202d 3e20 2243 6f6e 6653  bytes) -> "ConfS
+0000a9d0: 7461 7465 223a 202e 2e2e 0a0a 636c 6173  tate": .....clas
+0000a9e0: 7320 436f 6e66 5374 6174 6552 6566 285f  s ConfStateRef(_
+0000a9f0: 5f41 5049 5f43 6f6e 6653 7461 7465 293a  _API_ConfState):
+0000aa00: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
+0000aa10: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
+0000aa20: 636c 6173 733a 6043 6f6e 6653 7461 7465  class:`ConfState
+0000aa30: 602e 0a20 2020 2022 2222 0a0a 636c 6173  `..    """..clas
+0000aa40: 7320 5f5f 4150 495f 436f 6e66 4368 616e  s __API_ConfChan
+0000aa50: 6765 5632 285f 5f43 6c6f 6e65 6162 6c65  geV2(__Cloneable
+0000aa60: 2c20 5f5f 456e 636f 6465 722c 205f 5f44  , __Encoder, __D
+0000aa70: 6563 6f64 6572 293a 0a20 2020 2064 6566  ecoder):.    def
+0000aa80: 2063 6c6f 6e65 2873 656c 6629 202d 3e20   clone(self) -> 
+0000aa90: 2243 6f6e 6643 6861 6e67 6556 3222 3a20  "ConfChangeV2": 
+0000aaa0: 2e2e 2e0a 2020 2020 6465 6620 6765 745f  ....    def get_
+0000aab0: 6368 616e 6765 7328 7365 6c66 2920 2d3e  changes(self) ->
+0000aac0: 204c 6973 745b 2243 6f6e 6643 6861 6e67   List["ConfChang
+0000aad0: 6553 696e 676c 6552 6566 225d 3a0a 2020  eSingleRef"]:.  
+0000aae0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+0000aaf0: 2020 6465 6620 7365 745f 6368 616e 6765    def set_change
+0000ab00: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+0000ab10: 2063 6861 6e67 6573 3a20 4c69 7374 5b22   changes: List["
+0000ab20: 436f 6e66 4368 616e 6765 5369 6e67 6c65  ConfChangeSingle
+0000ab30: 225d 207c 204c 6973 745b 2243 6f6e 6643  "] | List["ConfC
+0000ab40: 6861 6e67 6553 696e 676c 6552 6566 225d  hangeSingleRef"]
+0000ab50: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+0000ab60: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000ab70: 2020 2020 6465 6620 636c 6561 725f 6368      def clear_ch
+0000ab80: 616e 6765 7328 7365 6c66 2920 2d3e 204e  anges(self) -> N
+0000ab90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000aba0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+0000abb0: 5f63 6f6e 7465 7874 2873 656c 6629 202d  _context(self) -
+0000abc0: 3e20 6279 7465 733a 0a20 2020 2020 2020  > bytes:.       
+0000abd0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000abe0: 2073 6574 5f63 6f6e 7465 7874 2873 656c   set_context(sel
+0000abf0: 662c 2063 6f6e 7465 7874 3a20 6279 7465  f, context: byte
+0000ac00: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
+0000ac10: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+0000ac20: 6465 6620 636c 6561 725f 636f 6e74 6578  def clear_contex
+0000ac30: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+0000ac40: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+0000ac50: 0a20 2020 2064 6566 2067 6574 5f74 7261  .    def get_tra
+0000ac60: 6e73 6974 696f 6e28 7365 6c66 2920 2d3e  nsition(self) ->
+0000ac70: 2022 436f 6e66 4368 616e 6765 5472 616e   "ConfChangeTran
+0000ac80: 7369 7469 6f6e 223a 0a20 2020 2020 2020  sition":.       
+0000ac90: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000aca0: 2073 6574 5f74 7261 6e73 6974 696f 6e28   set_transition(
+0000acb0: 7365 6c66 2c20 7472 616e 7369 7469 6f6e  self, transition
+0000acc0: 3a20 2243 6f6e 6643 6861 6e67 6554 7261  : "ConfChangeTra
+0000acd0: 6e73 6974 696f 6e22 2920 2d3e 204e 6f6e  nsition") -> Non
+0000ace0: 653a 0a20 2020 2020 2020 2022 2222 2022  e:.        """ "
+0000acf0: 2222 0a20 2020 2064 6566 2063 6c65 6172  "".    def clear
+0000ad00: 5f74 7261 6e73 6974 696f 6e28 7365 6c66  _transition(self
+0000ad10: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000ad20: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000ad30: 6566 2065 6e74 6572 5f6a 6f69 6e74 2873  ef enter_joint(s
+0000ad40: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000ad50: 5b62 6f6f 6c5d 3a0a 2020 2020 2020 2020  [bool]:.        
+0000ad60: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
+0000ad70: 6b73 2069 6620 7573 6573 204a 6f69 6e74  ks if uses Joint
+0000ad80: 2043 6f6e 7365 6e73 7573 2e0a 0a20 2020   Consensus...   
+0000ad90: 2020 2020 2049 7420 7769 6c6c 2072 6574       It will ret
+0000ada0: 7572 6e20 536f 6d65 2069 6620 616e 6420  urn Some if and 
+0000adb0: 6f6e 6c79 2069 6620 7468 6973 2063 6f6e  only if this con
+0000adc0: 6669 6720 6368 616e 6765 2077 696c 6c20  fig change will 
+0000add0: 7573 6520 4a6f 696e 7420 436f 6e73 656e  use Joint Consen
+0000ade0: 7375 732c 0a20 2020 2020 2020 2077 6869  sus,.        whi
+0000adf0: 6368 2069 7320 7468 6520 6361 7365 2069  ch is the case i
+0000ae00: 6620 6974 2063 6f6e 7461 696e 7320 6d6f  f it contains mo
+0000ae10: 7265 2074 6861 6e20 6f6e 6520 6368 616e  re than one chan
+0000ae20: 6765 206f 7220 6966 2074 6865 2075 7365  ge or if the use
+0000ae30: 206f 6620 4a6f 696e 740a 2020 2020 2020   of Joint.      
+0000ae40: 2020 436f 6e73 656e 7375 7320 7761 7320    Consensus was 
+0000ae50: 7265 7175 6573 7465 6420 6578 706c 6963  requested explic
+0000ae60: 6974 6c79 2e20 5468 6520 626f 6f6c 2069  itly. The bool i
+0000ae70: 6e64 6963 6174 6573 2077 6865 7468 6572  ndicates whether
+0000ae80: 2074 6865 204a 6f69 6e74 2053 7461 7465   the Joint State
+0000ae90: 0a20 2020 2020 2020 2077 696c 6c20 6265  .        will be
+0000aea0: 206c 6566 7420 6175 746f 6d61 7469 6361   left automatica
+0000aeb0: 6c6c 792e 0a20 2020 2020 2020 2022 2222  lly..        """
+0000aec0: 0a20 2020 2064 6566 206d 6572 6765 5f66  .    def merge_f
+0000aed0: 726f 6d5f 6279 7465 7328 7365 6c66 2c20  rom_bytes(self, 
+0000aee0: 623a 2062 7974 6573 2920 2d3e 204e 6f6e  b: bytes) -> Non
+0000aef0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0000af00: 2020 2020 2020 2055 7064 6174 6520 7468         Update th
+0000af10: 6973 206d 6573 7361 6765 206f 626a 6563  is message objec
+0000af20: 7420 7769 7468 2066 6965 6c64 7320 7265  t with fields re
+0000af30: 6164 2066 726f 6d20 6769 7665 6e20 7374  ad from given st
+0000af40: 7265 616d 2e0a 2020 2020 2020 2020 2222  ream..        ""
+0000af50: 220a 2020 2020 6465 6620 6c65 6176 655f  ".    def leave_
+0000af60: 6a6f 696e 7428 7365 6c66 2920 2d3e 2062  joint(self) -> b
+0000af70: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+0000af80: 0a20 2020 2020 2020 2043 6865 636b 7320  .        Checks 
+0000af90: 6966 2074 6865 2063 6f6e 6669 6775 7261  if the configura
+0000afa0: 7469 6f6e 2063 6861 6e67 6520 6c65 6176  tion change leav
+0000afb0: 6573 2061 206a 6f69 6e74 2063 6f6e 6669  es a joint confi
+0000afc0: 6775 7261 7469 6f6e 2e0a 0a20 2020 2020  guration...     
+0000afd0: 2020 2054 6869 7320 6973 2074 6865 2063     This is the c
+0000afe0: 6173 6520 6966 2074 6865 2043 6f6e 6643  ase if the ConfC
+0000aff0: 6861 6e67 6556 3220 6973 207a 6572 6f2c  hangeV2 is zero,
+0000b000: 2077 6974 6820 7468 6520 706f 7373 6962   with the possib
+0000b010: 6c65 2065 7863 6570 7469 6f6e 206f 660a  le exception of.
+0000b020: 2020 2020 2020 2020 7468 6520 436f 6e74          the Cont
+0000b030: 6578 7420 6669 656c 642e 0a20 2020 2020  ext field..     
+0000b040: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
+0000b050: 735f 7631 2873 656c 6629 202d 3e20 4f70  s_v1(self) -> Op
+0000b060: 7469 6f6e 616c 5b22 436f 6e66 4368 616e  tional["ConfChan
+0000b070: 6765 5265 6622 5d3a 0a20 2020 2020 2020  geRef"]:.       
+0000b080: 2022 2222 0a20 2020 2020 2020 2043 6f6e   """.        Con
+0000b090: 7665 7274 7320 636f 6e66 2063 6861 6e67  verts conf chang
+0000b0a0: 6520 746f 2060 436f 6e66 4368 616e 6765  e to `ConfChange
+0000b0b0: 602e 0a0a 2020 2020 2020 2020 6043 6f6e  `...        `Con
+0000b0c0: 6643 6861 6e67 6556 3260 2063 616e 2774  fChangeV2` can't
+0000b0d0: 2062 6520 6368 616e 6765 6420 6261 636b   be changed back
+0000b0e0: 2074 6f20 6043 6f6e 6643 6861 6e67 6560   to `ConfChange`
+0000b0f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000b100: 2020 6465 6620 6173 5f76 3228 7365 6c66    def as_v2(self
+0000b110: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
+0000b120: 5632 223a 0a20 2020 2020 2020 2022 2222  V2":.        """
+0000b130: 0a20 2020 2020 2020 2047 6574 7320 636f  .        Gets co
+0000b140: 6e66 2063 6861 6e67 6520 6173 2060 436f  nf change as `Co
+0000b150: 6e66 4368 616e 6765 5632 602e 0a20 2020  nfChangeV2`..   
+0000b160: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000b170: 2069 6e74 6f5f 7632 2873 656c 6629 202d   into_v2(self) -
+0000b180: 3e20 2243 6f6e 6643 6861 6e67 6556 3222  > "ConfChangeV2"
+0000b190: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000b1a0: 2020 2020 2020 436f 6e76 6572 7473 2063        Converts c
+0000b1b0: 6f6e 6620 6368 616e 6765 2074 6f20 6043  onf change to `C
+0000b1c0: 6f6e 6643 6861 6e67 6556 3260 2e0a 2020  onfChangeV2`..  
+0000b1d0: 2020 2020 2020 2222 220a 0a63 6c61 7373        """..class
+0000b1e0: 2043 6f6e 6643 6861 6e67 6556 3228 5f5f   ConfChangeV2(__
+0000b1f0: 4150 495f 436f 6e66 4368 616e 6765 5632  API_ConfChangeV2
+0000b200: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
+0000b210: 6f6e 6643 6861 6e67 6556 3220 6d65 7373  onfChangeV2 mess
+0000b220: 6167 6573 2069 6e69 7469 6174 6520 636f  ages initiate co
+0000b230: 6e66 6967 7572 6174 696f 6e20 6368 616e  nfiguration chan
+0000b240: 6765 732e 2054 6865 7920 7375 7070 6f72  ges. They suppor
+0000b250: 7420 626f 7468 2074 6865 0a20 2020 2073  t both the.    s
+0000b260: 696d 706c 6520 226f 6e65 2061 7420 6120  imple "one at a 
+0000b270: 7469 6d65 2220 6d65 6d62 6572 7368 6970  time" membership
+0000b280: 2063 6861 6e67 6520 7072 6f74 6f63 6f6c   change protocol
+0000b290: 2061 6e64 2066 756c 6c20 4a6f 696e 7420   and full Joint 
+0000b2a0: 436f 6e73 656e 7375 730a 2020 2020 616c  Consensus.    al
+0000b2b0: 6c6f 7769 6e67 2066 6f72 2061 7262 6974  lowing for arbit
+0000b2c0: 7261 7279 2063 6861 6e67 6573 2069 6e20  rary changes in 
+0000b2d0: 6d65 6d62 6572 7368 6970 2e0a 0a20 2020  membership...   
+0000b2e0: 2054 6865 2073 7570 706c 6965 6420 636f   The supplied co
+0000b2f0: 6e74 6578 7420 6973 2074 7265 6174 6564  ntext is treated
+0000b300: 2061 7320 616e 206f 7061 7175 6520 7061   as an opaque pa
+0000b310: 796c 6f61 6420 616e 6420 6361 6e20 6265  yload and can be
+0000b320: 2075 7365 6420 746f 0a20 2020 2061 7474   used to.    att
+0000b330: 6163 6820 616e 2061 6374 696f 6e20 6f6e  ach an action on
+0000b340: 2074 6865 2073 7461 7465 206d 6163 6869   the state machi
+0000b350: 6e65 2074 6f20 7468 6520 6170 706c 6963  ne to the applic
+0000b360: 6174 696f 6e20 6f66 2074 6865 2063 6f6e  ation of the con
+0000b370: 6669 6720 6368 616e 6765 0a20 2020 2070  fig change.    p
+0000b380: 726f 706f 7361 6c2e 204e 6f74 6520 7468  roposal. Note th
+0000b390: 6174 2063 6f6e 7472 6172 7920 746f 204a  at contrary to J
+0000b3a0: 6f69 6e74 2043 6f6e 7365 6e73 7573 2061  oint Consensus a
+0000b3b0: 7320 6f75 746c 696e 6564 2069 6e20 7468  s outlined in th
+0000b3c0: 6520 5261 6674 0a20 2020 2070 6170 6572  e Raft.    paper
+0000b3d0: 5b31 5d2c 2063 6f6e 6669 6775 7261 7469  [1], configurati
+0000b3e0: 6f6e 2063 6861 6e67 6573 2062 6563 6f6d  on changes becom
+0000b3f0: 6520 6163 7469 7665 2077 6865 6e20 7468  e active when th
+0000b400: 6579 2061 7265 202a 6170 706c 6965 642a  ey are *applied*
+0000b410: 2074 6f20 7468 650a 2020 2020 7374 6174   to the.    stat
+0000b420: 6520 6d61 6368 696e 6520 286e 6f74 2077  e machine (not w
+0000b430: 6865 6e20 7468 6579 2061 7265 2061 7070  hen they are app
+0000b440: 656e 6465 6420 746f 2074 6865 206c 6f67  ended to the log
+0000b450: 292e 0a0a 2020 2020 5468 6520 7369 6d70  )...    The simp
+0000b460: 6c65 2070 726f 746f 636f 6c20 6361 6e20  le protocol can 
+0000b470: 6265 2075 7365 6420 7768 656e 6576 6572  be used whenever
+0000b480: 206f 6e6c 7920 6120 7369 6e67 6c65 2063   only a single c
+0000b490: 6861 6e67 6520 6973 206d 6164 652e 0a0a  hange is made...
+0000b4a0: 2020 2020 4e6f 6e2d 7369 6d70 6c65 2063      Non-simple c
+0000b4b0: 6861 6e67 6573 2072 6571 7569 7265 2074  hanges require t
+0000b4c0: 6865 2075 7365 206f 6620 4a6f 696e 7420  he use of Joint 
+0000b4d0: 436f 6e73 656e 7375 732c 2066 6f72 2077  Consensus, for w
+0000b4e0: 6869 6368 2074 776f 0a20 2020 2063 6f6e  hich two.    con
+0000b4f0: 6669 6775 7261 7469 6f6e 2063 6861 6e67  figuration chang
+0000b500: 6573 2061 7265 2072 756e 2e20 5468 6520  es are run. The 
+0000b510: 6669 7273 7420 636f 6e66 6967 7572 6174  first configurat
+0000b520: 696f 6e20 6368 616e 6765 2073 7065 6369  ion change speci
+0000b530: 6669 6573 2074 6865 0a20 2020 2064 6573  fies the.    des
+0000b540: 6972 6564 2063 6861 6e67 6573 2061 6e64  ired changes and
+0000b550: 2074 7261 6e73 6974 696f 6e73 2074 6865   transitions the
+0000b560: 2052 6166 7420 6772 6f75 7020 696e 746f   Raft group into
+0000b570: 2074 6865 206a 6f69 6e74 2063 6f6e 6669   the joint confi
+0000b580: 6775 7261 7469 6f6e 2c0a 2020 2020 696e  guration,.    in
+0000b590: 2077 6869 6368 2071 756f 7275 6d20 7265   which quorum re
+0000b5a0: 7175 6972 6573 2061 206d 616a 6f72 6974  quires a majorit
+0000b5b0: 7920 6f66 2062 6f74 6820 7468 6520 7072  y of both the pr
+0000b5c0: 652d 6368 616e 6765 7320 616e 6420 706f  e-changes and po
+0000b5d0: 7374 2d63 6861 6e67 6573 0a20 2020 2063  st-changes.    c
+0000b5e0: 6f6e 6669 6775 7261 7469 6f6e 2e20 4a6f  onfiguration. Jo
+0000b5f0: 696e 7420 436f 6e73 656e 7375 7320 6176  int Consensus av
+0000b600: 6f69 6473 2065 6e74 6572 696e 6720 6672  oids entering fr
+0000b610: 6167 696c 6520 696e 7465 726d 6564 6961  agile intermedia
+0000b620: 7465 0a20 2020 2063 6f6e 6669 6775 7261  te.    configura
+0000b630: 7469 6f6e 7320 7468 6174 2063 6f75 6c64  tions that could
+0000b640: 2063 6f6d 7072 6f6d 6973 6520 7375 7276   compromise surv
+0000b650: 6976 6162 696c 6974 792e 2046 6f72 2065  ivability. For e
+0000b660: 7861 6d70 6c65 2c20 7769 7468 6f75 7420  xample, without 
+0000b670: 7468 650a 2020 2020 7573 6520 6f66 204a  the.    use of J
+0000b680: 6f69 6e74 2043 6f6e 7365 6e73 7573 2061  oint Consensus a
+0000b690: 6e64 2072 756e 6e69 6e67 2061 6372 6f73  nd running acros
+0000b6a0: 7320 7468 7265 6520 6176 6169 6c61 6269  s three availabi
+0000b6b0: 6c69 7479 207a 6f6e 6573 2077 6974 6820  lity zones with 
+0000b6c0: 610a 2020 2020 7265 706c 6963 6174 696f  a.    replicatio
+0000b6d0: 6e20 6661 6374 6f72 206f 6620 7468 7265  n factor of thre
+0000b6e0: 652c 2069 7420 6973 206e 6f74 2070 6f73  e, it is not pos
+0000b6f0: 7369 626c 6520 746f 2072 6570 6c61 6365  sible to replace
+0000b700: 2061 2076 6f74 6572 2077 6974 686f 7574   a voter without
+0000b710: 0a20 2020 2065 6e74 6572 696e 6720 616e  .    entering an
+0000b720: 2069 6e74 6572 6d65 6469 6174 6520 636f   intermediate co
+0000b730: 6e66 6967 7572 6174 696f 6e20 7468 6174  nfiguration that
+0000b740: 2064 6f65 7320 6e6f 7420 7375 7276 6976   does not surviv
+0000b750: 6520 7468 6520 6f75 7461 6765 206f 660a  e the outage of.
+0000b760: 2020 2020 6f6e 6520 6176 6169 6c61 6269      one availabi
+0000b770: 6c69 7479 207a 6f6e 652e 0a0a 2020 2020  lity zone...    
+0000b780: 5468 6520 7072 6f76 6964 6564 2043 6f6e  The provided Con
+0000b790: 6643 6861 6e67 6554 7261 6e73 6974 696f  fChangeTransitio
+0000b7a0: 6e20 7370 6563 6966 6965 7320 686f 7720  n specifies how 
+0000b7b0: 2861 6e64 2077 6865 7468 6572 2920 4a6f  (and whether) Jo
+0000b7c0: 696e 7420 436f 6e73 656e 7375 730a 2020  int Consensus.  
+0000b7d0: 2020 6973 2075 7365 642c 2061 6e64 2061    is used, and a
+0000b7e0: 7373 6967 6e73 2074 6865 2074 6173 6b20  ssigns the task 
+0000b7f0: 6f66 206c 6561 7669 6e67 2074 6865 206a  of leaving the j
+0000b800: 6f69 6e74 2063 6f6e 6669 6775 7261 7469  oint configurati
+0000b810: 6f6e 2065 6974 6865 7220 746f 0a20 2020  on either to.   
+0000b820: 2052 6166 7420 6f72 2074 6865 2061 7070   Raft or the app
+0000b830: 6c69 6361 7469 6f6e 2e20 4c65 6176 696e  lication. Leavin
+0000b840: 6720 7468 6520 6a6f 696e 7420 636f 6e66  g the joint conf
+0000b850: 6967 7572 6174 696f 6e20 6973 2061 6363  iguration is acc
+0000b860: 6f6d 706c 6973 6865 6420 6279 0a20 2020  omplished by.   
+0000b870: 2070 726f 706f 7369 6e67 2061 2043 6f6e   proposing a Con
+0000b880: 6643 6861 6e67 6556 3220 7769 7468 206f  fChangeV2 with o
+0000b890: 6e6c 7920 616e 6420 6f70 7469 6f6e 616c  nly and optional
+0000b8a0: 6c79 2074 6865 2043 6f6e 7465 7874 2066  ly the Context f
+0000b8b0: 6965 6c64 0a20 2020 2070 6f70 756c 6174  ield.    populat
+0000b8c0: 6564 2e0a 0a20 2020 2046 6f72 2064 6574  ed...    For det
+0000b8d0: 6169 6c73 206f 6e20 5261 6674 206d 656d  ails on Raft mem
+0000b8e0: 6265 7273 6869 7020 6368 616e 6765 732c  bership changes,
+0000b8f0: 2073 6565 3a0a 0a20 2020 205b 315d 3a20   see:..    [1]: 
+0000b900: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000b910: 6f6d 2f6f 6e67 6172 6469 652f 6469 7373  om/ongardie/diss
+0000b920: 6572 7461 7469 6f6e 2f62 6c6f 622f 6d61  ertation/blob/ma
+0000b930: 7374 6572 2f6f 6e6c 696e 652d 7472 696d  ster/online-trim
+0000b940: 2e70 6466 0a20 2020 2022 2222 0a0a 2020  .pdf.    """..  
+0000b950: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000b960: 656c 6629 202d 3e20 4e6f 6e65 3a20 2e2e  elf) -> None: ..
+0000b970: 2e0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0000b980: 686f 640a 2020 2020 6465 6620 6465 6661  hod.    def defa
+0000b990: 756c 7428 2920 2d3e 2022 436f 6e66 4368  ult() -> "ConfCh
+0000b9a0: 616e 6765 5632 223a 202e 2e2e 0a20 2020  angeV2": ....   
+0000b9b0: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
+0000b9c0: 6c66 2920 2d3e 2022 436f 6e66 4368 616e  lf) -> "ConfChan
+0000b9d0: 6765 5632 5265 6622 3a20 2e2e 2e0a 2020  geV2Ref": ....  
+0000b9e0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+0000b9f0: 2020 2020 6465 6620 6465 636f 6465 2876      def decode(v
+0000ba00: 3a20 6279 7465 7329 202d 3e20 2243 6f6e  : bytes) -> "Con
+0000ba10: 6643 6861 6e67 6556 3222 3a20 2e2e 2e0a  fChangeV2": ....
+0000ba20: 0a63 6c61 7373 2043 6f6e 6643 6861 6e67  .class ConfChang
+0000ba30: 6556 3252 6566 285f 5f41 5049 5f43 6f6e  eV2Ref(__API_Con
+0000ba40: 6643 6861 6e67 6556 3229 3a0a 2020 2020  fChangeV2):.    
+0000ba50: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
+0000ba60: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
+0000ba70: 3a60 436f 6e66 4368 616e 6765 5632 602e  :`ConfChangeV2`.
+0000ba80: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
+0000ba90: 5f5f 4150 495f 436f 6e66 4368 616e 6765  __API_ConfChange
+0000baa0: 5369 6e67 6c65 285f 5f43 6c6f 6e65 6162  Single(__Cloneab
+0000bab0: 6c65 2c20 5f5f 456e 636f 6465 722c 205f  le, __Encoder, _
+0000bac0: 5f44 6563 6f64 6572 293a 0a20 2020 2064  _Decoder):.    d
+0000bad0: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
+0000bae0: 3e20 2243 6f6e 6643 6861 6e67 6553 696e  > "ConfChangeSin
+0000baf0: 676c 6522 3a20 2e2e 2e0a 2020 2020 6465  gle": ....    de
+0000bb00: 6620 6765 745f 6e6f 6465 5f69 6428 7365  f get_node_id(se
+0000bb10: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+0000bb20: 2020 2020 2222 2220 2222 220a 2020 2020      """ """.    
+0000bb30: 6465 6620 7365 745f 6e6f 6465 5f69 6428  def set_node_id(
+0000bb40: 7365 6c66 2c20 6e6f 6465 5f69 643a 2069  self, node_id: i
+0000bb50: 6e74 293a 0a20 2020 2020 2020 2022 2222  nt):.        """
+0000bb60: 2022 2222 0a20 2020 2064 6566 2063 6c65   """.    def cle
+0000bb70: 6172 5f6e 6f64 655f 6964 2873 656c 6629  ar_node_id(self)
+0000bb80: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000bb90: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+0000bba0: 6620 6765 745f 6368 616e 6765 5f74 7970  f get_change_typ
+0000bbb0: 6528 7365 6c66 2920 2d3e 2022 436f 6e66  e(self) -> "Conf
+0000bbc0: 4368 616e 6765 5479 7065 223a 0a20 2020  ChangeType":.   
+0000bbd0: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+0000bbe0: 2064 6566 2073 6574 5f63 6861 6e67 655f   def set_change_
+0000bbf0: 7479 7065 2873 656c 662c 2074 7970 3a20  type(self, typ: 
+0000bc00: 2243 6f6e 6643 6861 6e67 6554 7970 6522  "ConfChangeType"
+0000bc10: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000bc20: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+0000bc30: 6566 2063 6c65 6172 5f63 6861 6e67 655f  ef clear_change_
+0000bc40: 7479 7065 2873 656c 6629 202d 3e20 4e6f  type(self) -> No
+0000bc50: 6e65 3a0a 2020 2020 2020 2020 2222 2220  ne:.        """ 
+0000bc60: 2222 220a 0a63 6c61 7373 2043 6f6e 6643  """..class ConfC
+0000bc70: 6861 6e67 6553 696e 676c 6528 5f5f 4150  hangeSingle(__AP
+0000bc80: 495f 436f 6e66 4368 616e 6765 5369 6e67  I_ConfChangeSing
+0000bc90: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
+0000bca0: 2043 6f6e 6643 6861 6e67 6553 696e 676c   ConfChangeSingl
+0000bcb0: 6520 6973 2061 6e20 696e 6469 7669 6475  e is an individu
+0000bcc0: 616c 2063 6f6e 6669 6775 7261 7469 6f6e  al configuration
+0000bcd0: 2063 6861 6e67 6520 6f70 6572 6174 696f   change operatio
+0000bce0: 6e2e 204d 756c 7469 706c 650a 2020 2020  n. Multiple.    
+0000bcf0: 7375 6368 206f 7065 7261 7469 6f6e 7320  such operations 
+0000bd00: 6361 6e20 6265 2063 6172 7269 6564 206f  can be carried o
+0000bd10: 7574 2061 746f 6d69 6361 6c6c 7920 7669  ut atomically vi
+0000bd20: 6120 6120 436f 6e66 4368 616e 6765 5632  a a ConfChangeV2
+0000bd30: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+0000bd40: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000bd50: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+0000bd60: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+0000bd70: 7365 6c66 2920 2d3e 2022 436f 6e66 4368  self) -> "ConfCh
+0000bd80: 616e 6765 5369 6e67 6c65 5265 6622 3a20  angeSingleRef": 
+0000bd90: 2e2e 2e0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+0000bda0: 6574 686f 640a 2020 2020 6465 6620 6465  ethod.    def de
+0000bdb0: 6661 756c 7428 2920 2d3e 2022 436f 6e66  fault() -> "Conf
+0000bdc0: 4368 616e 6765 5369 6e67 6c65 223a 202e  ChangeSingle": .
+0000bdd0: 2e2e 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+0000bde0: 7468 6f64 0a20 2020 2064 6566 2064 6563  thod.    def dec
+0000bdf0: 6f64 6528 763a 2062 7974 6573 2920 2d3e  ode(v: bytes) ->
+0000be00: 2022 436f 6e66 4368 616e 6765 5369 6e67   "ConfChangeSing
+0000be10: 6c65 223a 202e 2e2e 0a0a 636c 6173 7320  le": .....class 
+0000be20: 436f 6e66 4368 616e 6765 5369 6e67 6c65  ConfChangeSingle
+0000be30: 5265 6628 5f5f 4150 495f 436f 6e66 4368  Ref(__API_ConfCh
+0000be40: 616e 6765 5369 6e67 6c65 293a 0a20 2020  angeSingle):.   
+0000be50: 2022 2222 0a20 2020 2052 6566 6572 656e   """.    Referen
+0000be60: 6365 2074 7970 6520 6f66 203a 636c 6173  ce type of :clas
+0000be70: 733a 6043 6f6e 6643 6861 6e67 6553 696e  s:`ConfChangeSin
+0000be80: 676c 6560 2e0a 2020 2020 2222 220a 0a63  gle`..    """..c
+0000be90: 6c61 7373 205f 5f41 5049 5f43 6f6e 6643  lass __API_ConfC
+0000bea0: 6861 6e67 6528 5f5f 436c 6f6e 6561 626c  hange(__Cloneabl
+0000beb0: 652c 205f 5f45 6e63 6f64 6572 2c20 5f5f  e, __Encoder, __
+0000bec0: 4465 636f 6465 7229 3a0a 2020 2020 6465  Decoder):.    de
+0000bed0: 6620 636c 6f6e 6528 7365 6c66 2920 2d3e  f clone(self) ->
+0000bee0: 2022 436f 6e66 4368 616e 6765 223a 202e   "ConfChange": .
+0000bef0: 2e2e 0a20 2020 2064 6566 2067 6574 5f69  ...    def get_i
+0000bf00: 6428 7365 6c66 2920 2d3e 2069 6e74 3a0a  d(self) -> int:.
+0000bf10: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000bf20: 2020 2020 6465 6620 7365 745f 6964 2873      def set_id(s
+0000bf30: 656c 662c 2069 643a 2069 6e74 2920 2d3e  elf, id: int) ->
+0000bf40: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000bf50: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
+0000bf60: 6c65 6172 5f69 6428 7365 6c66 2920 2d3e  lear_id(self) ->
+0000bf70: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000bf80: 2222 2022 2222 0a20 2020 2064 6566 2067  "" """.    def g
+0000bf90: 6574 5f6e 6f64 655f 6964 2873 656c 6629  et_node_id(self)
+0000bfa0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000bfb0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000bfc0: 2073 6574 5f6e 6f64 655f 6964 2873 656c   set_node_id(sel
+0000bfd0: 662c 206e 6f64 655f 6964 3a20 696e 7429  f, node_id: int)
+0000bfe0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+0000bff0: 2020 2222 2220 2222 220a 2020 2020 6465    """ """.    de
+0000c000: 6620 636c 6561 725f 6e6f 6465 5f69 6428  f clear_node_id(
+0000c010: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+0000c020: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
+0000c030: 2020 2064 6566 2067 6574 5f63 6861 6e67     def get_chang
+0000c040: 655f 7479 7065 2873 656c 6629 202d 3e20  e_type(self) -> 
+0000c050: 2243 6f6e 6643 6861 6e67 6554 7970 6522  "ConfChangeType"
+0000c060: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
+0000c070: 220a 2020 2020 6465 6620 7365 745f 6368  ".    def set_ch
+0000c080: 616e 6765 5f74 7970 6528 7365 6c66 2c20  ange_type(self, 
+0000c090: 7479 703a 2022 436f 6e66 4368 616e 6765  typ: "ConfChange
+0000c0a0: 5479 7065 2229 202d 3e20 4e6f 6e65 3a0a  Type") -> None:.
+0000c0b0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000c0c0: 2020 2020 6465 6620 636c 6561 725f 6368      def clear_ch
+0000c0d0: 616e 6765 5f74 7970 6528 7365 6c66 2920  ange_type(self) 
+0000c0e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000c0f0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
+0000c100: 2067 6574 5f63 6f6e 7465 7874 2873 656c   get_context(sel
+0000c110: 6629 202d 3e20 6279 7465 733a 0a20 2020  f) -> bytes:.   
+0000c120: 2020 2020 2022 2222 2022 2222 0a20 2020       """ """.   
+0000c130: 2064 6566 2073 6574 5f63 6f6e 7465 7874   def set_context
+0000c140: 2873 656c 662c 2063 6f6e 7465 7874 3a20  (self, context: 
+0000c150: 6279 7465 7329 202d 3e20 4e6f 6e65 3a0a  bytes) -> None:.
+0000c160: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000c170: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
+0000c180: 6e74 6578 7428 7365 6c66 2920 2d3e 204e  ntext(self) -> N
+0000c190: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000c1a0: 2022 2222 0a20 2020 2064 6566 206d 6572   """.    def mer
+0000c1b0: 6765 5f66 726f 6d5f 6279 7465 7328 7365  ge_from_bytes(se
+0000c1c0: 6c66 2c20 623a 2062 7974 6573 2920 2d3e  lf, b: bytes) ->
+0000c1d0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000c1e0: 2222 0a20 2020 2020 2020 2055 7064 6174  "".        Updat
+0000c1f0: 6520 7468 6973 206d 6573 7361 6765 206f  e this message o
+0000c200: 626a 6563 7420 7769 7468 2066 6965 6c64  bject with field
+0000c210: 7320 7265 6164 2066 726f 6d20 6769 7665  s read from give
+0000c220: 6e20 7374 7265 616d 2e0a 2020 2020 2020  n stream..      
+0000c230: 2020 2222 220a 2020 2020 6465 6620 6173    """.    def as
+0000c240: 5f76 3128 7365 6c66 2920 2d3e 204f 7074  _v1(self) -> Opt
+0000c250: 696f 6e61 6c5b 2243 6f6e 6643 6861 6e67  ional["ConfChang
+0000c260: 6552 6566 225d 3a0a 2020 2020 2020 2020  eRef"]:.        
+0000c270: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
+0000c280: 6572 7473 2063 6f6e 6620 6368 616e 6765  erts conf change
+0000c290: 2074 6f20 6043 6f6e 6643 6861 6e67 6560   to `ConfChange`
+0000c2a0: 2e0a 0a20 2020 2020 2020 2060 436f 6e66  ...        `Conf
+0000c2b0: 4368 616e 6765 5632 6020 6361 6e27 7420  ChangeV2` can't 
+0000c2c0: 6265 2063 6861 6e67 6564 2062 6163 6b20  be changed back 
+0000c2d0: 746f 2060 436f 6e66 4368 616e 6765 602e  to `ConfChange`.
+0000c2e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c2f0: 2064 6566 2061 735f 7632 2873 656c 6629   def as_v2(self)
+0000c300: 202d 3e20 2243 6f6e 6643 6861 6e67 6556   -> "ConfChangeV
+0000c310: 3222 3a0a 2020 2020 2020 2020 2222 220a  2":.        """.
+0000c320: 2020 2020 2020 2020 4765 7473 2063 6f6e          Gets con
+0000c330: 6620 6368 616e 6765 2061 7320 6043 6f6e  f change as `Con
+0000c340: 6643 6861 6e67 6556 3260 2e0a 2020 2020  fChangeV2`..    
+0000c350: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000c360: 696e 746f 5f76 3228 7365 6c66 2920 2d3e  into_v2(self) ->
+0000c370: 2022 436f 6e66 4368 616e 6765 5632 223a   "ConfChangeV2":
+0000c380: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c390: 2020 2020 2043 6f6e 7665 7274 7320 636f       Converts co
+0000c3a0: 6e66 2063 6861 6e67 6520 746f 2060 436f  nf change to `Co
+0000c3b0: 6e66 4368 616e 6765 5632 602e 0a20 2020  nfChangeV2`..   
+0000c3c0: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
+0000c3d0: 436f 6e66 4368 616e 6765 285f 5f41 5049  ConfChange(__API
+0000c3e0: 5f43 6f6e 6643 6861 6e67 6529 3a0a 2020  _ConfChange):.  
+0000c3f0: 2020 2222 2220 2222 220a 0a20 2020 2064    """ """..    d
+0000c400: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000c410: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+0000c420: 2020 2064 6566 206d 616b 655f 7265 6628     def make_ref(
+0000c430: 7365 6c66 2920 2d3e 2022 436f 6e66 4368  self) -> "ConfCh
+0000c440: 616e 6765 5265 6622 3a20 2e2e 2e0a 2020  angeRef": ....  
+0000c450: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+0000c460: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
+0000c470: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
+0000c480: 223a 202e 2e2e 0a20 2020 2040 7374 6174  ": ....    @stat
+0000c490: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0000c4a0: 2064 6563 6f64 6528 763a 2062 7974 6573   decode(v: bytes
+0000c4b0: 2920 2d3e 2022 436f 6e66 4368 616e 6765  ) -> "ConfChange
+0000c4c0: 223a 202e 2e2e 0a0a 636c 6173 7320 436f  ": .....class Co
+0000c4d0: 6e66 4368 616e 6765 5265 6628 5f5f 4150  nfChangeRef(__AP
+0000c4e0: 495f 436f 6e66 4368 616e 6765 293a 0a20  I_ConfChange):. 
+0000c4f0: 2020 2022 2222 0a20 2020 2052 6566 6572     """.    Refer
+0000c500: 656e 6365 2074 7970 6520 6f66 203a 636c  ence type of :cl
+0000c510: 6173 733a 6043 6f6e 6643 6861 6e67 6560  ass:`ConfChange`
+0000c520: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
+0000c530: 205f 5f41 5049 5f55 6e73 7461 626c 653a   __API_Unstable:
+0000c540: 0a20 2020 2064 6566 206d 6179 6265 5f66  .    def maybe_f
+0000c550: 6972 7374 5f69 6e64 6578 2873 656c 6629  irst_index(self)
+0000c560: 202d 3e20 4f70 7469 6f6e 616c 5b69 6e74   -> Optional[int
+0000c570: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000c580: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
+0000c590: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+0000c5a0: 6669 7273 7420 706f 7373 6962 6c65 2065  first possible e
+0000c5b0: 6e74 7279 2069 6e20 656e 7472 6965 730a  ntry in entries.
+0000c5c0: 2020 2020 2020 2020 6966 2069 7420 6861          if it ha
+0000c5d0: 7320 6120 736e 6170 7368 6f74 2e0a 2020  s a snapshot..  
+0000c5e0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+0000c5f0: 6620 6d61 7962 655f 6c61 7374 5f69 6e64  f maybe_last_ind
+0000c600: 6578 2873 656c 6629 202d 3e20 4f70 7469  ex(self) -> Opti
+0000c610: 6f6e 616c 5b69 6e74 5d3a 0a20 2020 2020  onal[int]:.     
+0000c620: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+0000c630: 6574 7572 6e73 2074 6865 206c 6173 7420  eturns the last 
+0000c640: 696e 6465 7820 6966 2069 7420 6861 7320  index if it has 
+0000c650: 6174 206c 6561 7374 206f 6e65 2075 6e73  at least one uns
+0000c660: 7461 626c 6520 656e 7472 7920 6f72 2073  table entry or s
+0000c670: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
+0000c680: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
+0000c690: 6265 5f74 6572 6d28 7365 6c66 2920 2d3e  be_term(self) ->
+0000c6a0: 204f 7074 696f 6e61 6c5b 696e 745d 3a0a   Optional[int]:.
+0000c6b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c6c0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+0000c6d0: 7465 726d 206f 6620 7468 6520 656e 7472  term of the entr
+0000c6e0: 7920 6174 2069 6e64 6578 2069 6478 2c20  y at index idx, 
+0000c6f0: 6966 2074 6865 7265 2069 7320 616e 792e  if there is any.
+0000c700: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c710: 2064 6566 206d 7573 745f 6368 6563 6b5f   def must_check_
+0000c720: 6f75 746f 6662 6f75 6e64 7328 7365 6c66  outofbounds(self
+0000c730: 2c20 6c6f 3a20 696e 742c 2068 693a 2069  , lo: int, hi: i
+0000c740: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+0000c750: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c760: 2041 7373 6572 7473 2074 6865 2060 6869   Asserts the `hi
+0000c770: 6020 616e 6420 606c 6f60 2076 616c 7565  ` and `lo` value
+0000c780: 7320 6167 6169 6e73 7420 6561 6368 206f  s against each o
+0000c790: 7468 6572 2061 6e64 2061 6761 696e 7374  ther and against
+0000c7a0: 2074 6865 0a20 2020 2020 2020 2065 6e74   the.        ent
+0000c7b0: 7269 6573 2074 6865 6d73 656c 7665 732e  ries themselves.
+0000c7c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c7d0: 2064 6566 2073 6c69 6365 2873 656c 662c   def slice(self,
+0000c7e0: 206c 6f3a 2069 6e74 2c20 6869 3a20 696e   lo: int, hi: in
+0000c7f0: 7429 202d 3e20 4c69 7374 5b22 456e 7472  t) -> List["Entr
+0000c800: 7952 6566 225d 3a0a 2020 2020 2020 2020  yRef"]:.        
+0000c810: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000c820: 726e 7320 6120 736c 6963 6520 6f66 2065  rns a slice of e
+0000c830: 6e74 7269 6573 2062 6574 7765 656e 2074  ntries between t
+0000c840: 6865 2068 6967 6820 616e 6420 6c6f 772e  he high and low.
+0000c850: 0a0a 2020 2020 2020 2020 2320 5061 6e69  ..        # Pani
+0000c860: 6373 0a0a 2020 2020 2020 2020 5061 6e69  cs..        Pani
+0000c870: 6373 2069 6620 7468 6520 606c 6f60 206f  cs if the `lo` o
+0000c880: 7220 6068 6960 2061 7265 206f 7574 206f  r `hi` are out o
+0000c890: 6620 626f 756e 6473 2e0a 2020 2020 2020  f bounds..      
+0000c8a0: 2020 5061 6e69 6373 2069 6620 606c 6f20    Panics if `lo 
+0000c8b0: 3e20 6869 602e 0a20 2020 2020 2020 2022  > hi`..        "
+0000c8c0: 2222 0a20 2020 2064 6566 2073 7461 626c  "".    def stabl
+0000c8d0: 655f 736e 6170 2873 656c 662c 2069 6e64  e_snap(self, ind
+0000c8e0: 6578 3a20 696e 7429 202d 3e20 4e6f 6e65  ex: int) -> None
+0000c8f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c900: 2020 2020 2020 436c 6561 7273 2074 6865        Clears the
+0000c910: 2075 6e73 7461 626c 6520 736e 6170 7368   unstable snapsh
+0000c920: 6f74 2e0a 2020 2020 2020 2020 2222 220a  ot..        """.
+0000c930: 2020 2020 6465 6620 7374 6162 6c65 5f65      def stable_e
+0000c940: 6e74 7269 6573 2873 656c 662c 2069 6e64  ntries(self, ind
+0000c950: 6578 3a20 696e 742c 2074 6572 6d3a 2069  ex: int, term: i
+0000c960: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+0000c970: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000c980: 2043 6c65 6172 7320 7468 6520 756e 7374   Clears the unst
+0000c990: 6162 6c65 2065 6e74 7269 6573 2061 6e64  able entries and
+0000c9a0: 206d 6f76 6573 2074 6865 2073 7461 626c   moves the stabl
+0000c9b0: 6520 6f66 6673 6574 2075 7020 746f 2074  e offset up to t
+0000c9c0: 6865 0a20 2020 2020 2020 206c 6173 7420  he.        last 
+0000c9d0: 696e 6465 782c 2069 6620 7468 6572 6520  index, if there 
+0000c9e0: 6973 2061 6e79 2e0a 2020 2020 2020 2020  is any..        
+0000c9f0: 2222 220a 2020 2020 6465 6620 7265 7374  """.    def rest
+0000ca00: 6f72 6528 7365 6c66 2c20 736e 6170 3a20  ore(self, snap: 
+0000ca10: 2253 6e61 7073 686f 7452 6566 2229 202d  "SnapshotRef") -
+0000ca20: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000ca30: 2222 220a 2020 2020 2020 2020 4672 6f6d  """.        From
+0000ca40: 2061 2067 6976 656e 2073 6e61 7073 686f   a given snapsho
+0000ca50: 742c 2072 6573 746f 7265 7320 7468 6520  t, restores the 
+0000ca60: 736e 6170 7368 6f74 2074 6f20 7365 6c66  snapshot to self
+0000ca70: 2c20 6275 7420 646f 6573 6e27 7420 756e  , but doesn't un
+0000ca80: 7061 636b 2e0a 2020 2020 2020 2020 2222  pack..        ""
+0000ca90: 220a 2020 2020 6465 6620 7472 756e 6361  ".    def trunca
+0000caa0: 7465 5f61 6e64 5f61 7070 656e 6428 7365  te_and_append(se
+0000cab0: 6c66 2c20 656e 7473 3a20 4c69 7374 5b22  lf, ents: List["
+0000cac0: 456e 7472 7922 5d20 7c20 4c69 7374 5b22  Entry"] | List["
+0000cad0: 456e 7472 7952 6566 225d 2920 2d3e 204e  EntryRef"]) -> N
+0000cae0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+0000caf0: 0a20 2020 2020 2020 2041 7070 656e 6420  .        Append 
+0000cb00: 656e 7472 6965 7320 746f 2075 6e73 7461  entries to unsta
+0000cb10: 626c 652c 2074 7275 6e63 6174 6520 6c6f  ble, truncate lo
+0000cb20: 6361 6c20 626c 6f63 6b20 6669 7273 7420  cal block first 
+0000cb30: 6966 206f 7665 726c 6170 7065 642e 0a0a  if overlapped...
+0000cb40: 2020 2020 2020 2020 2320 5061 6e69 6373          # Panics
+0000cb50: 0a0a 2020 2020 2020 2020 5061 6e69 6373  ..        Panics
+0000cb60: 2069 6620 7472 756e 6361 7465 206c 6f67   if truncate log
+0000cb70: 7320 746f 2074 6865 2065 6e74 7279 2062  s to the entry b
+0000cb80: 6566 6f72 6520 736e 6170 7368 6f74 0a20  efore snapshot. 
+0000cb90: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000cba0: 6566 2067 6574 5f65 6e74 7269 6573 5f73  ef get_entries_s
+0000cbb0: 697a 6528 7365 6c66 2920 2d3e 2069 6e74  ize(self) -> int
+0000cbc0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000cbd0: 2020 2020 2020 6065 6e74 7269 6573 5f73        `entries_s
+0000cbe0: 697a 6560 3a20 5468 6520 7369 7a65 206f  ize`: The size o
+0000cbf0: 6620 656e 7472 6965 730a 2020 2020 2020  f entries.      
+0000cc00: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+0000cc10: 745f 656e 7472 6965 735f 7369 7a65 2873  t_entries_size(s
+0000cc20: 656c 662c 2065 6e74 7269 6573 5f73 697a  elf, entries_siz
+0000cc30: 653a 2069 6e74 2920 2d3e 204e 6f6e 653a  e: int) -> None:
+0000cc40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cc50: 2020 2020 2060 656e 7472 6965 735f 7369       `entries_si
+0000cc60: 7a65 603a 2054 6865 2073 697a 6520 6f66  ze`: The size of
+0000cc70: 2065 6e74 7269 6573 0a20 2020 2020 2020   entries.       
+0000cc80: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+0000cc90: 5f6f 6666 7365 7428 7365 6c66 2920 2d3e  _offset(self) ->
+0000cca0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+0000ccb0: 220a 2020 2020 2020 2020 606f 6666 7365  ".        `offse
+0000ccc0: 7460 3a20 5468 6520 6f66 6673 6574 2066  t`: The offset f
+0000ccd0: 726f 6d20 7468 6520 7665 6374 6f72 2069  rom the vector i
+0000cce0: 6e64 6578 2e0a 2020 2020 2020 2020 2222  ndex..        ""
+0000ccf0: 220a 2020 2020 6465 6620 7365 745f 6f66  ".    def set_of
+0000cd00: 6673 6574 2873 656c 662c 206f 6666 7365  fset(self, offse
+0000cd10: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
+0000cd20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cd30: 2020 2020 2060 6f66 6673 6574 603a 2054       `offset`: T
+0000cd40: 6865 206f 6666 7365 7420 6672 6f6d 2074  he offset from t
+0000cd50: 6865 2076 6563 746f 7220 696e 6465 782e  he vector index.
+0000cd60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cd70: 2064 6566 2067 6574 5f65 6e74 7269 6573   def get_entries
+0000cd80: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
+0000cd90: 456e 7472 7952 6566 225d 3a0a 2020 2020  EntryRef"]:.    
+0000cda0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cdb0: 6065 6e74 7269 6573 603a 2041 6c6c 2065  `entries`: All e
+0000cdc0: 6e74 7269 6573 2074 6861 7420 6861 7665  ntries that have
+0000cdd0: 206e 6f74 2079 6574 2062 6565 6e20 7772   not yet been wr
+0000cde0: 6974 7465 6e20 746f 2073 746f 7261 6765  itten to storage
+0000cdf0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000ce00: 2020 6465 6620 7365 745f 656e 7472 6965    def set_entrie
+0000ce10: 7328 7365 6c66 2c20 656e 7473 3a20 4c69  s(self, ents: Li
+0000ce20: 7374 5b22 456e 7472 7922 5d20 7c20 4c69  st["Entry"] | Li
+0000ce30: 7374 5b22 456e 7472 7952 6566 225d 2920  st["EntryRef"]) 
+0000ce40: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000ce50: 2022 2222 0a20 2020 2020 2020 2060 656e   """.        `en
+0000ce60: 7472 6965 7360 3a20 416c 6c20 656e 7472  tries`: All entr
+0000ce70: 6965 7320 7468 6174 2068 6176 6520 6e6f  ies that have no
+0000ce80: 7420 7965 7420 6265 656e 2077 7269 7474  t yet been writt
+0000ce90: 656e 2074 6f20 7374 6f72 6167 652e 0a20  en to storage.. 
+0000cea0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000ceb0: 6566 2067 6574 5f6c 6f67 6765 7228 7365  ef get_logger(se
+0000cec0: 6c66 2920 2d3e 2022 4c6f 6767 6572 5265  lf) -> "LoggerRe
+0000ced0: 6622 3a0a 2020 2020 2020 2020 2222 220a  f":.        """.
+0000cee0: 2020 2020 2020 2020 606c 6f67 6765 7260          `logger`
+0000cef0: 3a20 5468 6520 7461 6720 746f 2075 7365  : The tag to use
+0000cf00: 2077 6865 6e20 6c6f 6767 696e 672e 0a20   when logging.. 
+0000cf10: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000cf20: 6566 2073 6574 5f6c 6f67 6765 7228 7365  ef set_logger(se
+0000cf30: 6c66 2c20 6c6f 6767 6572 3a20 224c 6f67  lf, logger: "Log
+0000cf40: 6765 7222 207c 2022 4c6f 6767 6572 5265  ger" | "LoggerRe
+0000cf50: 6622 2920 2d3e 204e 6f6e 653a 0a20 2020  f") -> None:.   
+0000cf60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000cf70: 2060 6c6f 6767 6572 603a 2054 6865 2074   `logger`: The t
+0000cf80: 6167 2074 6f20 7573 6520 7768 656e 206c  ag to use when l
+0000cf90: 6f67 6769 6e67 2e0a 2020 2020 2020 2020  ogging..        
+0000cfa0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0000cfb0: 736e 6170 7368 6f74 2873 656c 6629 202d  snapshot(self) -
+0000cfc0: 3e20 4f70 7469 6f6e 616c 5b22 536e 6170  > Optional["Snap
+0000cfd0: 7368 6f74 5265 6622 5d3a 0a20 2020 2020  shotRef"]:.     
+0000cfe0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+0000cff0: 736e 6170 7368 6f74 603a 2054 6865 2069  snapshot`: The i
+0000d000: 6e63 6f6d 696e 6720 756e 7374 6162 6c65  ncoming unstable
+0000d010: 2073 6e61 7073 686f 742c 2069 6620 616e   snapshot, if an
+0000d020: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+0000d030: 2020 2064 6566 2073 6574 5f73 6e61 7073     def set_snaps
+0000d040: 686f 7428 7365 6c66 2c20 736e 6170 7368  hot(self, snapsh
+0000d050: 6f74 3a20 2253 6e61 7073 686f 7422 207c  ot: "Snapshot" |
+0000d060: 2022 536e 6170 7368 6f74 5265 6622 2920   "SnapshotRef") 
+0000d070: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000d080: 2022 2222 0a20 2020 2020 2020 2060 736e   """.        `sn
+0000d090: 6170 7368 6f74 603a 2054 6865 2069 6e63  apshot`: The inc
+0000d0a0: 6f6d 696e 6720 756e 7374 6162 6c65 2073  oming unstable s
+0000d0b0: 6e61 7073 686f 742c 2069 6620 616e 792e  napshot, if any.
+0000d0c0: 0a20 2020 2020 2020 2022 2222 0a0a 636c  .        """..cl
+0000d0d0: 6173 7320 556e 7374 6162 6c65 285f 5f41  ass Unstable(__A
+0000d0e0: 5049 5f55 6e73 7461 626c 6529 3a0a 2020  PI_Unstable):.  
+0000d0f0: 2020 2222 220a 2020 2020 5468 6520 6075    """.    The `u
+0000d100: 6e73 7461 626c 652e 656e 7472 6965 735b  nstable.entries[
+0000d110: 695d 6020 6861 7320 7261 6674 206c 6f67  i]` has raft log
+0000d120: 2070 6f73 6974 696f 6e20 6069 2b75 6e73   position `i+uns
+0000d130: 7461 626c 652e 6f66 6673 6574 602e 0a20  table.offset`.. 
+0000d140: 2020 204e 6f74 6520 7468 6174 2060 756e     Note that `un
+0000d150: 7374 6162 6c65 2e6f 6666 7365 7460 206d  stable.offset` m
+0000d160: 6179 2062 6520 6c65 7373 2074 6861 6e20  ay be less than 
+0000d170: 7468 6520 6869 6768 6573 7420 6c6f 670a  the highest log.
+0000d180: 2020 2020 706f 7369 7469 6f6e 2069 6e20      position in 
+0000d190: 7374 6f72 6167 653b 2074 6869 7320 6d65  storage; this me
+0000d1a0: 616e 7320 7468 6174 2074 6865 206e 6578  ans that the nex
+0000d1b0: 7420 7772 6974 6520 746f 2073 746f 7261  t write to stora
+0000d1c0: 6765 0a20 2020 206d 6967 6874 206e 6565  ge.    might nee
+0000d1d0: 6420 746f 2074 7275 6e63 6174 6520 7468  d to truncate th
+0000d1e0: 6520 6c6f 6720 6265 666f 7265 2070 6572  e log before per
+0000d1f0: 7369 7374 696e 6720 756e 7374 6162 6c65  sisting unstable
+0000d200: 2e65 6e74 7269 6573 2e0a 2020 2020 2222  .entries..    ""
+0000d210: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+0000d220: 745f 5f28 7365 6c66 2c20 6f66 6673 6574  t__(self, offset
+0000d230: 3a20 696e 742c 206c 6f67 6765 723a 2022  : int, logger: "
+0000d240: 4c6f 6767 6572 2220 7c20 224c 6f67 6765  Logger" | "Logge
+0000d250: 7252 6566 2229 202d 3e20 4e6f 6e65 3a20  rRef") -> None: 
+0000d260: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
+0000d270: 5f72 6566 2873 656c 6629 202d 3e20 2255  _ref(self) -> "U
+0000d280: 6e73 7461 626c 6552 6566 223a 202e 2e2e  nstableRef": ...
+0000d290: 0a0a 636c 6173 7320 556e 7374 6162 6c65  ..class Unstable
+0000d2a0: 5265 6628 5f5f 4150 495f 556e 7374 6162  Ref(__API_Unstab
+0000d2b0: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
+0000d2c0: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+0000d2d0: 6f66 203a 636c 6173 733a 6055 6e73 7461  of :class:`Unsta
+0000d2e0: 626c 6560 2e0a 2020 2020 2222 220a 0a63  ble`..    """..c
+0000d2f0: 6c61 7373 205f 5f41 5049 5f53 6f66 7453  lass __API_SoftS
+0000d300: 7461 7465 3a0a 2020 2020 6465 6620 6765  tate:.    def ge
+0000d310: 745f 6c65 6164 6572 5f69 6428 7365 6c66  t_leader_id(self
+0000d320: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+0000d330: 2020 2222 220a 2020 2020 2020 2020 606c    """.        `l
+0000d340: 6561 6465 725f 6964 603a 2054 6865 2070  eader_id`: The p
+0000d350: 6f74 656e 7469 616c 206c 6561 6465 7220  otential leader 
+0000d360: 6f66 2074 6865 2063 6c75 7374 6572 2e0a  of the cluster..
+0000d370: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d380: 6465 6620 7365 745f 6c65 6164 6572 5f69  def set_leader_i
+0000d390: 6428 7365 6c66 2c20 6c65 6164 6572 5f69  d(self, leader_i
+0000d3a0: 643a 2069 6e74 2920 2d3e 204e 6f6e 653a  d: int) -> None:
+0000d3b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d3c0: 2020 2020 2060 6c65 6164 6572 5f69 6460       `leader_id`
+0000d3d0: 3a20 5468 6520 706f 7465 6e74 6961 6c20  : The potential 
+0000d3e0: 6c65 6164 6572 206f 6620 7468 6520 636c  leader of the cl
+0000d3f0: 7573 7465 722e 0a20 2020 2020 2020 2022  uster..        "
+0000d400: 2222 0a20 2020 2064 6566 2067 6574 5f72  "".    def get_r
+0000d410: 6166 745f 7374 6174 6528 7365 6c66 2920  aft_state(self) 
+0000d420: 2d3e 2022 5374 6174 6552 6f6c 6522 3a0a  -> "StateRole":.
+0000d430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d440: 2020 2020 6072 6166 745f 7374 6174 6560      `raft_state`
+0000d450: 3a20 5468 6520 736f 6674 2072 6f6c 6520  : The soft role 
+0000d460: 7468 6973 206e 6f64 6520 6d61 7920 7461  this node may ta
+0000d470: 6b65 2e0a 2020 2020 2020 2020 2222 220a  ke..        """.
+0000d480: 2020 2020 6465 6620 7365 745f 7261 6674      def set_raft
+0000d490: 5f73 7461 7465 2873 656c 662c 2072 6f6c  _state(self, rol
+0000d4a0: 653a 2022 5374 6174 6552 6f6c 6522 2920  e: "StateRole") 
+0000d4b0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000d4c0: 2022 2222 0a20 2020 2020 2020 2060 7261   """.        `ra
+0000d4d0: 6674 5f73 7461 7465 603a 2054 6865 2073  ft_state`: The s
+0000d4e0: 6f66 7420 726f 6c65 2074 6869 7320 6e6f  oft role this no
+0000d4f0: 6465 206d 6179 2074 616b 652e 0a20 2020  de may take..   
+0000d500: 2020 2020 2022 2222 0a0a 636c 6173 7320       """..class 
+0000d510: 536f 6674 5374 6174 6528 5f5f 4150 495f  SoftState(__API_
+0000d520: 536f 6674 5374 6174 6529 3a0a 2020 2020  SoftState):.    
+0000d530: 2222 220a 2020 2020 536f 6674 5374 6174  """.    SoftStat
+0000d540: 6520 7072 6f76 6964 6573 2073 7461 7465  e provides state
+0000d550: 2074 6861 7420 6973 2075 7365 6675 6c20   that is useful 
+0000d560: 666f 7220 6c6f 6767 696e 6720 616e 6420  for logging and 
+0000d570: 6465 6275 6767 696e 672e 0a20 2020 2054  debugging..    T
+0000d580: 6865 2073 7461 7465 2069 7320 766f 6c61  he state is vola
+0000d590: 7469 6c65 2061 6e64 2064 6f65 7320 6e6f  tile and does no
+0000d5a0: 7420 6e65 6564 2074 6f20 6265 2070 6572  t need to be per
+0000d5b0: 7369 7374 6564 2074 6f20 7468 6520 5741  sisted to the WA
+0000d5c0: 4c2e 0a20 2020 2022 2222 0a0a 2020 2020  L..    """..    
+0000d5d0: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
+0000d5e0: 6629 202d 3e20 2253 6f66 7453 7461 7465  f) -> "SoftState
+0000d5f0: 5265 6622 3a20 2e2e 2e0a 2020 2020 4073  Ref": ....    @s
+0000d600: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+0000d610: 6465 6620 6465 6661 756c 7428 2920 2d3e  def default() ->
+0000d620: 2022 536f 6674 5374 6174 6522 3a20 2e2e   "SoftState": ..
+0000d630: 2e0a 0a63 6c61 7373 2053 6f66 7453 7461  ...class SoftSta
+0000d640: 7465 5265 6628 5f5f 4150 495f 536f 6674  teRef(__API_Soft
+0000d650: 5374 6174 6529 3a0a 2020 2020 2222 220a  State):.    """.
+0000d660: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
+0000d670: 7065 206f 6620 3a63 6c61 7373 3a60 536f  pe of :class:`So
+0000d680: 6674 5374 6174 6560 2e0a 2020 2020 2222  ftState`..    ""
+0000d690: 220a 0a63 6c61 7373 205f 5f41 5049 5f52  "..class __API_R
+0000d6a0: 6561 6453 7461 7465 285f 5f43 6c6f 6e65  eadState(__Clone
+0000d6b0: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
+0000d6c0: 6c6f 6e65 2873 656c 6629 202d 3e20 2252  lone(self) -> "R
+0000d6d0: 6561 6453 7461 7465 223a 202e 2e2e 0a20  eadState": .... 
+0000d6e0: 2020 2064 6566 2067 6574 5f69 6e64 6578     def get_index
+0000d6f0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+0000d700: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d710: 2020 2060 696e 6465 7860 3a20 5468 6520     `index`: The 
+0000d720: 696e 6465 7820 6f66 2074 6865 2072 6561  index of the rea
+0000d730: 6420 7374 6174 652e 0a20 2020 2020 2020  d state..       
+0000d740: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+0000d750: 5f69 6e64 6578 2873 656c 662c 2069 6478  _index(self, idx
+0000d760: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+0000d770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d780: 2020 2020 6069 6e64 6578 603a 2054 6865      `index`: The
+0000d790: 2069 6e64 6578 206f 6620 7468 6520 7265   index of the re
+0000d7a0: 6164 2073 7461 7465 2e0a 2020 2020 2020  ad state..      
+0000d7b0: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
+0000d7c0: 745f 7265 7175 6573 745f 6374 7828 7365  t_request_ctx(se
+0000d7d0: 6c66 2920 2d3e 2062 7974 6573 3a0a 2020  lf) -> bytes:.  
+0000d7e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d7f0: 2020 6072 6571 7565 7374 5f63 7478 603a    `request_ctx`:
+0000d800: 2041 2064 6174 6167 7261 6d20 636f 6e73   A datagram cons
+0000d810: 6973 7469 6e67 206f 6620 636f 6e74 6578  isting of contex
+0000d820: 7420 6162 6f75 7420 7468 6520 7265 7175  t about the requ
+0000d830: 6573 742e 0a20 2020 2020 2020 2022 2222  est..        """
+0000d840: 0a20 2020 2064 6566 2073 6574 5f72 6571  .    def set_req
+0000d850: 7565 7374 5f63 7478 2873 656c 662c 2072  uest_ctx(self, r
+0000d860: 6571 7565 7374 5f63 7478 3a20 6279 7465  equest_ctx: byte
+0000d870: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
+0000d880: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d890: 6072 6571 7565 7374 5f63 7478 603a 2041  `request_ctx`: A
+0000d8a0: 2064 6174 6167 7261 6d20 636f 6e73 6973   datagram consis
+0000d8b0: 7469 6e67 206f 6620 636f 6e74 6578 7420  ting of context 
+0000d8c0: 6162 6f75 7420 7468 6520 7265 7175 6573  about the reques
+0000d8d0: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
+0000d8e0: 636c 6173 7320 5265 6164 5374 6174 6528  class ReadState(
+0000d8f0: 5f5f 4150 495f 5265 6164 5374 6174 6529  __API_ReadState)
+0000d900: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+0000d910: 6164 5374 6174 6520 7072 6f76 6964 6573  adState provides
+0000d920: 2073 7461 7465 2066 6f72 2072 6561 6420   state for read 
+0000d930: 6f6e 6c79 2071 7565 7279 2e0a 2020 2020  only query..    
+0000d940: 4974 2773 2063 616c 6c65 7227 7320 7265  It's caller's re
+0000d950: 7370 6f6e 7369 6269 6c69 7479 2074 6f20  sponsibility to 
+0000d960: 7365 6e64 204d 7367 5265 6164 496e 6465  send MsgReadInde
+0000d970: 7820 6669 7273 7420 6265 666f 7265 2067  x first before g
+0000d980: 6574 7469 6e67 0a20 2020 2074 6869 7320  etting.    this 
+0000d990: 7374 6174 6520 6672 6f6d 2072 6561 6479  state from ready
+0000d9a0: 2e20 4974 2773 2061 6c73 6f20 6361 6c6c  . It's also call
+0000d9b0: 6572 2773 2064 7574 7920 746f 2064 6966  er's duty to dif
+0000d9c0: 6665 7265 6e74 6961 7465 2069 6620 7468  ferentiate if th
+0000d9d0: 6973 0a20 2020 2073 7461 7465 2069 7320  is.    state is 
+0000d9e0: 7768 6174 2069 7420 7265 7175 6573 7473  what it requests
+0000d9f0: 2074 6872 6f75 6768 2072 6571 7565 7374   through request
+0000da00: 5f63 7478 2c20 652e 672e 2067 6976 656e  _ctx, e.g. given
+0000da10: 2061 2075 6e69 7175 6520 6964 2061 730a   a unique id as.
+0000da20: 2020 2020 7265 7175 6573 745f 6374 782e      request_ctx.
+0000da30: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+0000da40: 6620 5f5f 696e 6974 5f5f 2873 656c 6629  f __init__(self)
+0000da50: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+0000da60: 2020 6465 6620 6d61 6b65 5f72 6566 2873    def make_ref(s
+0000da70: 656c 6629 202d 3e20 2252 6561 6453 7461  elf) -> "ReadSta
+0000da80: 7465 5265 6622 3a20 2e2e 2e0a 0a63 6c61  teRef": .....cla
+0000da90: 7373 2052 6561 6453 7461 7465 5265 6628  ss ReadStateRef(
+0000daa0: 5f5f 4150 495f 5265 6164 5374 6174 6529  __API_ReadState)
+0000dab0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+0000dac0: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
+0000dad0: 3a63 6c61 7373 3a60 5265 6164 5374 6174  :class:`ReadStat
+0000dae0: 6560 2e0a 2020 2020 2222 220a 0a63 6c61  e`..    """..cla
+0000daf0: 7373 205f 5f41 5049 5f52 6166 744c 6f67  ss __API_RaftLog
+0000db00: 3a0a 2020 2020 6465 6620 656e 7472 6965  :.    def entrie
+0000db10: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+0000db20: 2069 6478 3a20 696e 742c 2063 6f6e 7465   idx: int, conte
+0000db30: 7874 3a20 2247 6574 456e 7472 6965 7343  xt: "GetEntriesC
+0000db40: 6f6e 7465 7874 5265 6622 2c20 6d61 785f  ontextRef", max_
+0000db50: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
+0000db60: 6e74 5d0a 2020 2020 2920 2d3e 204c 6973  nt].    ) -> Lis
+0000db70: 745b 2245 6e74 7279 225d 3a0a 2020 2020  t["Entry"]:.    
+0000db80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000db90: 5265 7475 726e 7320 656e 7472 6965 7320  Returns entries 
+0000dba0: 7374 6172 7469 6e67 2066 726f 6d20 6120  starting from a 
+0000dbb0: 7061 7274 6963 756c 6172 2069 6e64 6578  particular index
+0000dbc0: 2061 6e64 206e 6f74 2065 7863 6565 6469   and not exceedi
+0000dbd0: 6e67 2061 2062 7974 6573 697a 652e 0a20  ng a bytesize.. 
+0000dbe0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000dbf0: 6566 2061 6c6c 5f65 6e74 7269 6573 2873  ef all_entries(s
+0000dc00: 656c 6629 202d 3e20 4c69 7374 5b22 456e  elf) -> List["En
+0000dc10: 7472 7922 5d3a 0a20 2020 2020 2020 2022  try"]:.        "
+0000dc20: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+0000dc30: 6e73 2061 6c6c 2074 6865 2065 6e74 7269  ns all the entri
+0000dc40: 6573 2e20 4f6e 6c79 2075 7365 6420 6279  es. Only used by
+0000dc50: 2074 6573 7473 2e0a 2020 2020 2020 2020   tests..        
+0000dc60: 2222 220a 2020 2020 6465 6620 6170 7065  """.    def appe
+0000dc70: 6e64 2873 656c 662c 2065 6e74 733a 204c  nd(self, ents: L
+0000dc80: 6973 745b 2245 6e74 7279 225d 207c 204c  ist["Entry"] | L
+0000dc90: 6973 745b 2245 6e74 7279 5265 6622 5d29  ist["EntryRef"])
+0000dca0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000dcb0: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
+0000dcc0: 656e 6473 2061 2073 6574 206f 6620 656e  ends a set of en
+0000dcd0: 7472 6965 7320 746f 2074 6865 2075 6e73  tries to the uns
+0000dce0: 7461 626c 6520 6c69 7374 2e0a 2020 2020  table list..    
+0000dcf0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000dd00: 6170 706c 6965 6428 7365 6c66 2920 2d3e  applied(self) ->
+0000dd10: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+0000dd20: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+0000dd30: 7320 7468 6520 6c61 7374 2061 7070 6c69  s the last appli
+0000dd40: 6564 2069 6e64 6578 2e0a 2020 2020 2020  ed index..      
+0000dd50: 2020 2222 220a 2020 2020 6465 6620 6669    """.    def fi
+0000dd60: 6e64 5f63 6f6e 666c 6963 7428 7365 6c66  nd_conflict(self
+0000dd70: 2c20 656e 7473 3a20 4c69 7374 5b22 456e  , ents: List["En
+0000dd80: 7472 7922 5d20 7c20 4c69 7374 5b22 456e  try"] | List["En
+0000dd90: 7472 7952 6566 225d 2920 2d3e 2069 6e74  tryRef"]) -> int
+0000dda0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000ddb0: 2020 2020 2020 4669 6e64 7320 7468 6520        Finds the 
+0000ddc0: 696e 6465 7820 6f66 2074 6865 2063 6f6e  index of the con
+0000ddd0: 666c 6963 742e 0a0a 2020 2020 2020 2020  flict...        
+0000dde0: 4974 2072 6574 7572 6e73 2074 6865 2066  It returns the f
+0000ddf0: 6972 7374 2069 6e64 6578 206f 6620 636f  irst index of co
+0000de00: 6e66 6c69 6374 696e 6720 656e 7472 6965  nflicting entrie
+0000de10: 7320 6265 7477 6565 6e20 7468 6520 6578  s between the ex
+0000de20: 6973 7469 6e67 0a20 2020 2020 2020 2065  isting.        e
+0000de30: 6e74 7269 6573 2061 6e64 2074 6865 2067  ntries and the g
+0000de40: 6976 656e 2065 6e74 7269 6573 2c20 6966  iven entries, if
+0000de50: 2074 6865 7265 2061 7265 2061 6e79 2e0a   there are any..
+0000de60: 0a20 2020 2020 2020 2049 6620 7468 6572  .        If ther
+0000de70: 6520 6172 6520 6e6f 2063 6f6e 666c 6963  e are no conflic
+0000de80: 7469 6e67 2065 6e74 7269 6573 2c20 616e  ting entries, an
+0000de90: 6420 7468 6520 6578 6973 7469 6e67 2065  d the existing e
+0000dea0: 6e74 7269 6573 2063 6f6e 7461 696e 0a20  ntries contain. 
+0000deb0: 2020 2020 2020 2061 6c6c 2074 6865 2067         all the g
+0000dec0: 6976 656e 2065 6e74 7269 6573 2c20 7a65  iven entries, ze
+0000ded0: 726f 2077 696c 6c20 6265 2072 6574 7572  ro will be retur
+0000dee0: 6e65 642e 0a0a 2020 2020 2020 2020 4966  ned...        If
+0000def0: 2074 6865 7265 2061 7265 206e 6f20 636f   there are no co
+0000df00: 6e66 6c69 6374 696e 6720 656e 7472 6965  nflicting entrie
+0000df10: 732c 2062 7574 2074 6865 2067 6976 656e  s, but the given
+0000df20: 2065 6e74 7269 6573 2063 6f6e 7461 696e   entries contain
+0000df30: 7320 6e65 770a 2020 2020 2020 2020 656e  s new.        en
+0000df40: 7472 6965 732c 2074 6865 2069 6e64 6578  tries, the index
+0000df50: 206f 6620 7468 6520 6669 7273 7420 6e65   of the first ne
+0000df60: 7720 656e 7472 7920 7769 6c6c 2062 6520  w entry will be 
+0000df70: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
+0000df80: 2020 2041 6e20 656e 7472 7920 6973 2063     An entry is c
+0000df90: 6f6e 7369 6465 7265 6420 746f 2062 6520  onsidered to be 
+0000dfa0: 636f 6e66 6c69 6374 696e 6720 6966 2069  conflicting if i
+0000dfb0: 7420 6861 7320 7468 6520 7361 6d65 2069  t has the same i
+0000dfc0: 6e64 6578 2062 7574 0a20 2020 2020 2020  ndex but.       
+0000dfd0: 2061 2064 6966 6665 7265 6e74 2074 6572   a different ter
+0000dfe0: 6d2e 0a0a 2020 2020 2020 2020 5468 6520  m...        The 
+0000dff0: 6669 7273 7420 656e 7472 7920 4d55 5354  first entry MUST
+0000e000: 2068 6176 6520 616e 2069 6e64 6578 2065   have an index e
+0000e010: 7175 616c 2074 6f20 7468 6520 6172 6775  qual to the argu
+0000e020: 6d65 6e74 2027 6672 6f6d 272e 0a20 2020  ment 'from'..   
+0000e030: 2020 2020 2054 6865 2069 6e64 6578 206f       The index o
+0000e040: 6620 7468 6520 6769 7665 6e20 656e 7472  f the given entr
+0000e050: 6965 7320 4d55 5354 2062 6520 636f 6e74  ies MUST be cont
+0000e060: 696e 756f 7573 6c79 2069 6e63 7265 6173  inuously increas
+0000e070: 696e 672e 0a20 2020 2020 2020 2022 2222  ing..        """
+0000e080: 0a20 2020 2064 6566 2066 696e 645f 636f  .    def find_co
+0000e090: 6e66 6c69 6374 5f62 795f 7465 726d 2873  nflict_by_term(s
+0000e0a0: 656c 662c 2069 6e64 6578 3a20 696e 742c  elf, index: int,
+0000e0b0: 2074 6572 6d3a 2069 6e74 2920 2d3e 2054   term: int) -> T
+0000e0c0: 7570 6c65 5b69 6e74 2c20 4f70 7469 6f6e  uple[int, Option
+0000e0d0: 616c 5b69 6e74 5d5d 3a0a 2020 2020 2020  al[int]]:.      
+0000e0e0: 2020 2222 220a 2020 2020 2020 2020 6669    """.        fi
+0000e0f0: 6e64 5f63 6f6e 666c 6963 745f 6279 5f74  nd_conflict_by_t
+0000e100: 6572 6d20 7461 6b65 7320 616e 2028 6069  erm takes an (`i
+0000e110: 6e64 6578 602c 2060 7465 726d 6029 2070  ndex`, `term`) p
+0000e120: 6169 7220 2869 6e64 6963 6174 696e 6720  air (indicating 
+0000e130: 6120 636f 6e66 6c69 6374 696e 6720 6c6f  a conflicting lo
+0000e140: 670a 2020 2020 2020 2020 656e 7472 7920  g.        entry 
+0000e150: 6f6e 2061 206c 6561 6465 722f 666f 6c6c  on a leader/foll
+0000e160: 6f77 6572 2064 7572 696e 6720 616e 2061  ower during an a
+0000e170: 7070 656e 6429 2061 6e64 2066 696e 6473  ppend) and finds
+0000e180: 2074 6865 206c 6172 6765 7374 2069 6e64   the largest ind
+0000e190: 6578 2069 6e0a 2020 2020 2020 2020 6c6f  ex in.        lo
+0000e1a0: 6720 7769 7468 206c 6f67 2e74 6572 6d20  g with log.term 
+0000e1b0: 3c3d 2060 7465 726d 6020 616e 6420 6c6f  <= `term` and lo
+0000e1c0: 672e 696e 6465 7820 3c3d 2060 696e 6465  g.index <= `inde
+0000e1d0: 7860 2e20 4966 206e 6f20 7375 6368 2069  x`. If no such i
+0000e1e0: 6e64 6578 2065 7869 7374 730a 2020 2020  ndex exists.    
+0000e1f0: 2020 2020 696e 2074 6865 206c 6f67 2c20      in the log, 
+0000e200: 7468 6520 6c6f 6727 7320 6669 7273 7420  the log's first 
+0000e210: 696e 6465 7820 6973 2072 6574 7572 6e65  index is returne
+0000e220: 642e 0a0a 2020 2020 2020 2020 5468 6520  d...        The 
+0000e230: 696e 6465 7820 7072 6f76 6964 6564 204d  index provided M
+0000e240: 5553 5420 6265 2065 7175 616c 2074 6f20  UST be equal to 
+0000e250: 6f72 206c 6573 7320 7468 616e 2073 656c  or less than sel
+0000e260: 662e 6c61 7374 5f69 6e64 6578 2829 2e20  f.last_index(). 
+0000e270: 496e 7661 6c69 640a 2020 2020 2020 2020  Invalid.        
+0000e280: 696e 7075 7473 206c 6f67 2061 2077 6172  inputs log a war
+0000e290: 6e69 6e67 2061 6e64 2074 6865 2069 6e70  ning and the inp
+0000e2a0: 7574 2069 6e64 6578 2069 7320 7265 7475  ut index is retu
+0000e2b0: 726e 6564 2e0a 0a20 2020 2020 2020 2052  rned...        R
+0000e2c0: 6574 7572 6e20 2869 6e64 6578 2c20 7465  eturn (index, te
+0000e2d0: 726d 290a 2020 2020 2020 2020 2222 220a  rm).        """.
+0000e2e0: 2020 2020 6465 6620 636f 6d6d 6974 5f74      def commit_t
+0000e2f0: 6f28 7365 6c66 2c20 746f 5f63 6f6d 6d69  o(self, to_commi
+0000e300: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
+0000e310: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000e320: 2020 2020 2053 6574 7320 7468 6520 6c61       Sets the la
+0000e330: 7374 2063 6f6d 6d69 7474 6564 2076 616c  st committed val
+0000e340: 7565 2074 6f20 7468 6520 7061 7373 6564  ue to the passed
+0000e350: 2069 6e20 7661 6c75 652e 0a0a 2020 2020   in value...    
+0000e360: 2020 2020 2320 5061 6e69 6373 0a0a 2020      # Panics..  
+0000e370: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
+0000e380: 7468 6520 696e 6465 7820 676f 6573 2070  the index goes p
+0000e390: 6173 7420 7468 6520 6c61 7374 2069 6e64  ast the last ind
+0000e3a0: 6578 2e0a 2020 2020 2020 2020 2222 220a  ex..        """.
+0000e3b0: 2020 2020 6465 6620 636f 6d6d 6974 5f69      def commit_i
+0000e3c0: 6e66 6f28 7365 6c66 2920 2d3e 2054 7570  nfo(self) -> Tup
+0000e3d0: 6c65 5b69 6e74 2c20 696e 745d 3a0a 2020  le[int, int]:.  
+0000e3e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e3f0: 2020 5265 7475 726e 7320 7468 6520 636f    Returns the co
+0000e400: 6d6d 6974 7465 6420 696e 6465 7820 616e  mmitted index an
+0000e410: 6420 6974 7320 7465 726d 2e0a 2020 2020  d its term..    
+0000e420: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000e430: 7374 6f72 6528 7365 6c66 2920 2d3e 2022  store(self) -> "
+0000e440: 4d65 6d53 746f 7261 6765 5265 6622 3a0a  MemStorageRef":.
+0000e450: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0000e460: 2020 2020 6465 6620 6e65 7874 5f65 6e74      def next_ent
+0000e470: 7269 6573 2873 656c 662c 206d 6178 5f73  ries(self, max_s
+0000e480: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+0000e490: 745d 2920 2d3e 204f 7074 696f 6e61 6c5b  t]) -> Optional[
+0000e4a0: 4c69 7374 5b22 456e 7472 7922 5d5d 3a0a  List["Entry"]]:.
+0000e4b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000e4c0: 2020 2020 5265 7475 726e 7320 616c 6c20      Returns all 
+0000e4d0: 7468 6520 6176 6169 6c61 626c 6520 656e  the available en
+0000e4e0: 7472 6965 7320 666f 7220 6578 6563 7574  tries for execut
+0000e4f0: 696f 6e2e 0a20 2020 2020 2020 2049 6620  ion..        If 
+0000e500: 6170 706c 6965 6420 6973 2073 6d61 6c6c  applied is small
+0000e510: 6572 2074 6861 6e20 7468 6520 696e 6465  er than the inde
+0000e520: 7820 6f66 2073 6e61 7073 686f 742c 2069  x of snapshot, i
+0000e530: 7420 7265 7475 726e 7320 616c 6c20 636f  t returns all co
+0000e540: 6d6d 6974 7465 640a 2020 2020 2020 2020  mmitted.        
+0000e550: 656e 7472 6965 7320 6166 7465 7220 7468  entries after th
+0000e560: 6520 696e 6465 7820 6f66 2073 6e61 7073  e index of snaps
+0000e570: 686f 742e 0a20 2020 2020 2020 2022 2222  hot..        """
+0000e580: 0a20 2020 2064 6566 206e 6578 745f 656e  .    def next_en
+0000e590: 7472 6965 735f 7369 6e63 6528 0a20 2020  tries_since(.   
+0000e5a0: 2020 2020 2073 656c 662c 2073 696e 6365       self, since
+0000e5b0: 5f69 6478 3a20 696e 742c 206d 6178 5f73  _idx: int, max_s
+0000e5c0: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+0000e5d0: 745d 0a20 2020 2029 202d 3e20 4f70 7469  t].    ) -> Opti
+0000e5e0: 6f6e 616c 5b4c 6973 745b 2245 6e74 7279  onal[List["Entry
+0000e5f0: 225d 5d3a 0a20 2020 2020 2020 2022 2222  "]]:.        """
+0000e600: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000e610: 2063 6f6d 6d69 7474 6564 2061 6e64 2070   committed and p
+0000e620: 6572 7369 7374 6564 2065 6e74 7269 6573  ersisted entries
+0000e630: 2073 696e 6365 206d 6178 2860 7369 6e63   since max(`sinc
+0000e640: 655f 6964 7860 202b 2031 2c20 6669 7273  e_idx` + 1, firs
+0000e650: 745f 696e 6465 7829 2e0a 2020 2020 2020  t_index)..      
+0000e660: 2020 2222 220a 2020 2020 6465 6620 6861    """.    def ha
+0000e670: 735f 6e65 7874 5f65 6e74 7269 6573 2873  s_next_entries(s
+0000e680: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+0000e690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e6a0: 2020 5265 7475 726e 7320 7768 6574 6865    Returns whethe
+0000e6b0: 7220 7468 6572 6520 6172 6520 6e65 7720  r there are new 
+0000e6c0: 656e 7472 6965 732e 0a20 2020 2020 2020  entries..       
+0000e6d0: 2022 2222 0a20 2020 2064 6566 2068 6173   """.    def has
+0000e6e0: 5f6e 6578 745f 656e 7472 6965 735f 7369  _next_entries_si
+0000e6f0: 6e63 6528 7365 6c66 2c20 7369 6e63 655f  nce(self, since_
+0000e700: 6964 783a 2069 6e74 2920 2d3e 2062 6f6f  idx: int) -> boo
+0000e710: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+0000e720: 2020 2020 2020 2052 6574 7572 6e73 2077         Returns w
+0000e730: 6865 7468 6572 2074 6865 7265 2061 7265  hether there are
+0000e740: 2063 6f6d 6d69 7474 6564 2061 6e64 2070   committed and p
+0000e750: 6572 7369 7374 6564 2065 6e74 7269 6573  ersisted entries
+0000e760: 2073 696e 6365 0a20 2020 2020 2020 206d   since.        m
+0000e770: 6178 2860 7369 6e63 655f 6964 7860 202b  ax(`since_idx` +
+0000e780: 2031 2c20 6669 7273 745f 696e 6465 7829   1, first_index)
+0000e790: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000e7a0: 2020 6465 6620 6973 5f75 705f 746f 5f64    def is_up_to_d
+0000e7b0: 6174 6528 7365 6c66 2c20 6c61 7374 5f69  ate(self, last_i
+0000e7c0: 6e64 6578 3a20 696e 742c 2074 6572 6d3a  ndex: int, term:
+0000e7d0: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
+0000e7e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000e7f0: 2020 2044 6574 6572 6d69 6e65 7320 6966     Determines if
+0000e800: 2074 6865 2067 6976 656e 2028 6c61 7374   the given (last
+0000e810: 496e 6465 782c 7465 726d 2920 6c6f 6720  Index,term) log 
+0000e820: 6973 206d 6f72 6520 7570 2d74 6f2d 6461  is more up-to-da
+0000e830: 7465 0a20 2020 2020 2020 2062 7920 636f  te.        by co
+0000e840: 6d70 6172 696e 6720 7468 6520 696e 6465  mparing the inde
+0000e850: 7820 616e 6420 7465 726d 206f 6620 7468  x and term of th
+0000e860: 6520 6c61 7374 2065 6e74 7279 2069 6e20  e last entry in 
+0000e870: 7468 6520 6578 6973 7469 6e67 206c 6f67  the existing log
+0000e880: 732e 0a20 2020 2020 2020 2049 6620 7468  s..        If th
+0000e890: 6520 6c6f 6773 2068 6176 6520 6c61 7374  e logs have last
+0000e8a0: 2065 6e74 7279 2077 6974 6820 6469 6666   entry with diff
+0000e8b0: 6572 656e 7420 7465 726d 732c 2074 6865  erent terms, the
+0000e8c0: 6e20 7468 6520 6c6f 6720 7769 7468 2074  n the log with t
+0000e8d0: 6865 0a20 2020 2020 2020 206c 6174 6572  he.        later
+0000e8e0: 2074 6572 6d20 6973 206d 6f72 6520 7570   term is more up
+0000e8f0: 2d74 6f2d 6461 7465 2e20 4966 2074 6865  -to-date. If the
+0000e900: 206c 6f67 7320 656e 6420 7769 7468 2074   logs end with t
+0000e910: 6865 2073 616d 6520 7465 726d 2c20 7468  he same term, th
+0000e920: 656e 0a20 2020 2020 2020 2077 6869 6368  en.        which
+0000e930: 6576 6572 206c 6f67 2068 6173 2074 6865  ever log has the
+0000e940: 206c 6172 6765 7220 6c61 7374 5f69 6e64   larger last_ind
+0000e950: 6578 2069 7320 6d6f 7265 2075 702d 746f  ex is more up-to
+0000e960: 2d64 6174 652e 2049 6620 7468 6520 6c6f  -date. If the lo
+0000e970: 6773 2061 7265 0a20 2020 2020 2020 2074  gs are.        t
+0000e980: 6865 2073 616d 652c 2074 6865 2067 6976  he same, the giv
+0000e990: 656e 206c 6f67 2069 7320 7570 2d74 6f2d  en log is up-to-
+0000e9a0: 6461 7465 2e0a 2020 2020 2020 2020 2222  date..        ""
+0000e9b0: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
+0000e9c0: 636f 6d6d 6974 2873 656c 662c 206d 6178  commit(self, max
+0000e9d0: 5f69 6e64 6578 3a20 696e 742c 2074 6572  _index: int, ter
+0000e9e0: 6d3a 2069 6e74 2920 2d3e 2062 6f6f 6c3a  m: int) -> bool:
+0000e9f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ea00: 2020 2020 2041 7474 656d 7074 7320 746f       Attempts to
+0000ea10: 2063 6f6d 6d69 7420 7468 6520 696e 6465   commit the inde
+0000ea20: 7820 616e 6420 7465 726d 2061 6e64 2072  x and term and r
+0000ea30: 6574 7572 6e73 2077 6865 7468 6572 2069  eturns whether i
+0000ea40: 7420 6469 642e 0a20 2020 2020 2020 2022  t did..        "
+0000ea50: 2222 0a20 2020 2064 6566 206d 6179 6265  "".    def maybe
+0000ea60: 5f70 6572 7369 7374 2873 656c 662c 2069  _persist(self, i
+0000ea70: 6e64 6578 3a20 696e 742c 2074 6572 6d3a  ndex: int, term:
+0000ea80: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
+0000ea90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000eaa0: 2020 2041 7474 656d 7074 7320 746f 2070     Attempts to p
+0000eab0: 6572 7369 7374 2074 6865 2069 6e64 6578  ersist the index
+0000eac0: 2061 6e64 2074 6572 6d20 616e 6420 7265   and term and re
+0000ead0: 7475 726e 7320 7768 6574 6865 7220 6974  turns whether it
+0000eae0: 2064 6964 2e0a 2020 2020 2020 2020 2222   did..        ""
+0000eaf0: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
+0000eb00: 7065 7273 6973 745f 736e 6170 2873 656c  persist_snap(sel
+0000eb10: 662c 2069 6e64 6578 3a20 696e 7429 202d  f, index: int) -
+0000eb20: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000eb30: 2222 220a 2020 2020 2020 2020 4174 7465  """.        Atte
+0000eb40: 6d70 7473 2074 6f20 7065 7273 6973 7420  mpts to persist 
+0000eb50: 7468 6520 736e 6170 7368 6f74 2061 6e64  the snapshot and
+0000eb60: 2072 6574 7572 6e73 2077 6865 7468 6572   returns whether
+0000eb70: 2069 7420 6469 642e 0a20 2020 2020 2020   it did..       
+0000eb80: 2022 2222 0a20 2020 2064 6566 206d 6179   """.    def may
+0000eb90: 6265 5f61 7070 656e 6428 0a20 2020 2020  be_append(.     
+0000eba0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000ebb0: 2069 6478 3a20 696e 742c 0a20 2020 2020   idx: int,.     
+0000ebc0: 2020 2074 6572 6d3a 2069 6e74 2c0a 2020     term: int,.  
+0000ebd0: 2020 2020 2020 636f 6d6d 6974 7465 643a        committed:
+0000ebe0: 2069 6e74 2c0a 2020 2020 2020 2020 656e   int,.        en
+0000ebf0: 7473 3a20 4c69 7374 5b22 456e 7472 7922  ts: List["Entry"
+0000ec00: 5d20 7c20 4c69 7374 5b22 456e 7472 7952  ] | List["EntryR
+0000ec10: 6566 225d 2c0a 2020 2020 2920 2d3e 204f  ef"],.    ) -> O
+0000ec20: 7074 696f 6e61 6c5b 5475 706c 655b 696e  ptional[Tuple[in
+0000ec30: 742c 2069 6e74 5d5d 3a0a 2020 2020 2020  t, int]]:.      
+0000ec40: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000ec50: 7475 726e 7320 4e6f 6e65 2069 6620 7468  turns None if th
+0000ec60: 6520 656e 7472 6965 7320 6361 6e6e 6f74  e entries cannot
+0000ec70: 2062 6520 6170 7065 6e64 6564 2e20 4f74   be appended. Ot
+0000ec80: 6865 7277 6973 652c 0a20 2020 2020 2020  herwise,.       
+0000ec90: 2069 7420 7265 7475 726e 7320 536f 6d65   it returns Some
+0000eca0: 2828 636f 6e66 6c69 6374 5f69 6e64 6578  ((conflict_index
+0000ecb0: 2c20 6c61 7374 5f69 6e64 6578 2929 2e0a  , last_index))..
+0000ecc0: 0a20 2020 2020 2020 2023 2050 616e 6963  .        # Panic
+0000ecd0: 730a 0a20 2020 2020 2020 2050 616e 6963  s..        Panic
+0000ece0: 7320 6966 2069 7420 6669 6e64 7320 6120  s if it finds a 
+0000ecf0: 636f 6e66 6c69 6374 696e 6720 696e 6465  conflicting inde
+0000ed00: 7820 6c65 7373 2074 6861 6e20 636f 6d6d  x less than comm
+0000ed10: 6974 7465 6420 696e 6465 782e 0a20 2020  itted index..   
+0000ed20: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000ed30: 2073 6e61 7073 686f 7428 7365 6c66 2c20   snapshot(self, 
+0000ed40: 7265 7175 6573 745f 696e 6465 783a 2069  request_index: i
+0000ed50: 6e74 2c20 746f 3a20 696e 7429 202d 3e20  nt, to: int) -> 
+0000ed60: 2253 6e61 7073 686f 7452 6566 223a 0a20  "SnapshotRef":. 
+0000ed70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ed80: 2020 2052 6574 7572 6e73 2074 6865 2063     Returns the c
+0000ed90: 7572 7265 6e74 2073 6e61 7073 686f 740a  urrent snapshot.
+0000eda0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000edb0: 6465 6620 7374 6162 6c65 5f65 6e74 7269  def stable_entri
+0000edc0: 6573 2873 656c 662c 2069 6e64 6578 3a20  es(self, index: 
+0000edd0: 696e 742c 2074 6572 6d3a 2069 6e74 2920  int, term: int) 
+0000ede0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000edf0: 2022 2222 0a20 2020 2020 2020 2043 6c65   """.        Cle
+0000ee00: 6172 7320 7468 6520 756e 7374 6162 6c65  ars the unstable
+0000ee10: 2065 6e74 7269 6573 2061 6e64 206d 6f76   entries and mov
+0000ee20: 6573 2074 6865 2073 7461 626c 6520 6f66  es the stable of
+0000ee30: 6673 6574 2075 7020 746f 2074 6865 0a20  fset up to the. 
+0000ee40: 2020 2020 2020 206c 6173 7420 696e 6465         last inde
+0000ee50: 782c 2069 6620 7468 6572 6520 6973 2061  x, if there is a
+0000ee60: 6e79 2e0a 2020 2020 2020 2020 2222 220a  ny..        """.
+0000ee70: 2020 2020 6465 6620 7374 6162 6c65 5f73      def stable_s
+0000ee80: 6e61 7028 7365 6c66 2c20 696e 6465 783a  nap(self, index:
+0000ee90: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+0000eea0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000eeb0: 2020 2043 6c65 6172 7320 7468 6520 756e     Clears the un
+0000eec0: 7374 6162 6c65 2073 6e61 7073 686f 742e  stable snapshot.
+0000eed0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000eee0: 2064 6566 2074 6572 6d28 7365 6c66 2c20   def term(self, 
+0000eef0: 6964 783a 2069 6e74 2920 2d3e 2069 6e74  idx: int) -> int
+0000ef00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000ef10: 2020 2020 2020 466f 7220 6120 6769 7665        For a give
+0000ef20: 6e20 696e 6465 782c 2066 696e 6473 2074  n index, finds t
+0000ef30: 6865 2074 6572 6d20 6173 736f 6369 6174  he term associat
+0000ef40: 6564 2077 6974 6820 6974 2e0a 2020 2020  ed with it..    
+0000ef50: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000ef60: 6c61 7374 5f74 6572 6d28 7365 6c66 2920  last_term(self) 
+0000ef70: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+0000ef80: 2222 220a 2020 2020 2020 2020 4772 6162  """.        Grab
+0000ef90: 7320 7468 6520 7465 726d 2066 726f 6d20  s the term from 
+0000efa0: 7468 6520 6c61 7374 2065 6e74 7279 2e0a  the last entry..
+0000efb0: 0a20 2020 2020 2020 2023 2050 616e 6963  .        # Panic
+0000efc0: 730a 0a20 2020 2020 2020 2050 616e 6963  s..        Panic
+0000efd0: 7320 6966 2074 6865 7265 2061 7265 2065  s if there are e
+0000efe0: 6e74 7269 6573 2062 7574 2074 6865 206c  ntries but the l
+0000eff0: 6173 7420 7465 726d 2068 6173 2062 6565  ast term has bee
+0000f000: 6e20 6469 7363 6172 6465 642e 0a20 2020  n discarded..   
+0000f010: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+0000f020: 206d 6174 6368 5f74 6572 6d28 7365 6c66   match_term(self
+0000f030: 2c20 6964 783a 2069 6e74 2c20 7465 726d  , idx: int, term
+0000f040: 3a20 696e 7429 202d 3e20 626f 6f6c 3a0a  : int) -> bool:.
+0000f050: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f060: 2020 2020 416e 7377 6572 7320 7468 6520      Answers the 
+0000f070: 7175 6573 7469 6f6e 3a20 446f 6573 2074  question: Does t
+0000f080: 6869 7320 696e 6465 7820 6265 6c6f 6e67  his index belong
+0000f090: 2074 6f20 7468 6973 2074 6572 6d3f 0a20   to this term?. 
+0000f0a0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+0000f0b0: 6566 2066 6972 7374 5f69 6e64 6578 2873  ef first_index(s
+0000f0c0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0000f0d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f0e0: 2052 6574 7572 6e73 2074 6820 6669 7273   Returns th firs
+0000f0f0: 7420 696e 6465 7820 696e 2074 6865 2073  t index in the s
+0000f100: 746f 7265 2074 6861 7420 6973 2061 7661  tore that is ava
+0000f110: 696c 6162 6c65 2076 6961 2065 6e74 7269  ilable via entri
+0000f120: 6573 0a0a 2020 2020 2020 2020 2320 5061  es..        # Pa
+0000f130: 6e69 6373 0a0a 2020 2020 2020 2020 5061  nics..        Pa
+0000f140: 6e69 6373 2069 6620 7468 6520 7374 6f72  nics if the stor
+0000f150: 6520 646f 6573 6e27 7420 6861 7665 2061  e doesn't have a
+0000f160: 2066 6972 7374 2069 6e64 6578 2e0a 2020   first index..  
+0000f170: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+0000f180: 6620 6c61 7374 5f69 6e64 6578 2873 656c  f last_index(sel
+0000f190: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+0000f1a0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+0000f1b0: 6574 7572 6e73 2074 6865 206c 6173 7420  eturns the last 
+0000f1c0: 696e 6465 7820 696e 2074 6865 2073 746f  index in the sto
+0000f1d0: 7265 2074 6861 7420 6973 2061 7661 696c  re that is avail
+0000f1e0: 6162 6c65 2076 6961 2065 6e74 7269 6573  able via entries
+0000f1f0: 2e0a 0a20 2020 2020 2020 2023 2050 616e  ...        # Pan
+0000f200: 6963 730a 0a20 2020 2020 2020 2050 616e  ics..        Pan
+0000f210: 6963 7320 6966 2074 6865 2073 746f 7265  ics if the store
+0000f220: 2064 6f65 736e 2774 2068 6176 6520 6120   doesn't have a 
+0000f230: 6c61 7374 2069 6e64 6578 2e0a 2020 2020  last index..    
+0000f240: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000f250: 756e 7374 6162 6c65 2873 656c 6629 202d  unstable(self) -
+0000f260: 3e20 2255 6e73 7461 626c 6552 6566 223a  > "UnstableRef":
+0000f270: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f280: 2020 2020 2052 6574 7572 6e73 2061 2072       Returns a r
+0000f290: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
+0000f2a0: 756e 7374 6162 6c65 206c 6f67 2e0a 2020  unstable log..  
+0000f2b0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+0000f2c0: 6620 756e 7374 6162 6c65 5f65 6e74 7269  f unstable_entri
+0000f2d0: 6573 2873 656c 6629 202d 3e20 4c69 7374  es(self) -> List
+0000f2e0: 5b22 456e 7472 7952 6566 225d 3a0a 2020  ["EntryRef"]:.  
+0000f2f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f300: 2020 5265 7475 726e 7320 736c 6963 6520    Returns slice 
+0000f310: 6f66 2065 6e74 7269 6573 2074 6861 7420  of entries that 
+0000f320: 6172 6520 6e6f 7420 7065 7273 6973 7465  are not persiste
+0000f330: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
+0000f340: 2020 2064 6566 2075 6e73 7461 626c 655f     def unstable_
+0000f350: 736e 6170 7368 6f74 2873 656c 6629 202d  snapshot(self) -
+0000f360: 3e20 4f70 7469 6f6e 616c 5b22 536e 6170  > Optional["Snap
+0000f370: 7368 6f74 5265 6622 5d3a 0a20 2020 2020  shotRef"]:.     
+0000f380: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+0000f390: 6574 7572 6e73 2074 6865 2073 6e61 7073  eturns the snaps
+0000f3a0: 686f 7420 7468 6174 2061 7265 206e 6f74  hot that are not
+0000f3b0: 2070 6572 7369 7374 6564 2e0a 2020 2020   persisted..    
+0000f3c0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+0000f3d0: 6765 745f 6170 706c 6965 6428 7365 6c66  get_applied(self
+0000f3e0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+0000f3f0: 2020 2222 220a 2020 2020 2020 2020 6061    """.        `a
+0000f400: 7070 6c69 6564 603a 2054 6865 2068 6967  pplied`: The hig
+0000f410: 6865 7374 206c 6f67 2070 6f73 6974 696f  hest log positio
+0000f420: 6e20 7468 6174 2074 6865 2061 7070 6c69  n that the appli
+0000f430: 6361 7469 6f6e 2068 6173 2062 6565 6e20  cation has been 
+0000f440: 696e 7374 7275 6374 6564 0a20 2020 2020  instructed.     
+0000f450: 2020 2074 6f20 6170 706c 7920 746f 2069     to apply to i
+0000f460: 7473 2073 7461 7465 206d 6163 6869 6e65  ts state machine
+0000f470: 2e0a 0a20 2020 2020 2020 2049 6e76 6172  ...        Invar
+0000f480: 6961 6e74 3a20 6170 706c 6965 6420 3c3d  iant: applied <=
+0000f490: 206d 696e 2863 6f6d 6d69 7474 6564 2c20   min(committed, 
+0000f4a0: 7065 7273 6973 7465 6429 0a20 2020 2020  persisted).     
+0000f4b0: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
+0000f4c0: 6574 5f61 7070 6c69 6564 2873 656c 662c  et_applied(self,
+0000f4d0: 2061 7070 6c69 6564 3a20 696e 7429 202d   applied: int) -
+0000f4e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000f4f0: 2222 220a 2020 2020 2020 2020 6061 7070  """.        `app
+0000f500: 6c69 6564 603a 2054 6865 2068 6967 6865  lied`: The highe
+0000f510: 7374 206c 6f67 2070 6f73 6974 696f 6e20  st log position 
+0000f520: 7468 6174 2074 6865 2061 7070 6c69 6361  that the applica
+0000f530: 7469 6f6e 2068 6173 2062 6565 6e20 696e  tion has been in
+0000f540: 7374 7275 6374 6564 0a20 2020 2020 2020  structed.       
+0000f550: 2074 6f20 6170 706c 7920 746f 2069 7473   to apply to its
+0000f560: 2073 7461 7465 206d 6163 6869 6e65 2e0a   state machine..
+0000f570: 0a20 2020 2020 2020 2049 6e76 6172 6961  .        Invaria
+0000f580: 6e74 3a20 6170 706c 6965 6420 3c3d 206d  nt: applied <= m
+0000f590: 696e 2863 6f6d 6d69 7474 6564 2c20 7065  in(committed, pe
+0000f5a0: 7273 6973 7465 6429 0a20 2020 2020 2020  rsisted).       
+0000f5b0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+0000f5c0: 5f63 6f6d 6d69 7474 6564 2873 656c 6629  _committed(self)
+0000f5d0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+0000f5e0: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
+0000f5f0: 6d6d 6974 7465 6460 3a20 5468 6520 6869  mmitted`: The hi
+0000f600: 6768 6573 7420 6c6f 6720 706f 7369 7469  ghest log positi
+0000f610: 6f6e 2074 6861 7420 6973 206b 6e6f 776e  on that is known
+0000f620: 2074 6f20 6265 2069 6e20 7374 6162 6c65   to be in stable
+0000f630: 2073 746f 7261 6765 0a20 2020 2020 2020   storage.       
+0000f640: 206f 6e20 6120 7175 6f72 756d 206f 6620   on a quorum of 
+0000f650: 6e6f 6465 732e 0a0a 2020 2020 2020 2020  nodes...        
+0000f660: 496e 7661 7269 616e 743a 2061 7070 6c69  Invariant: appli
+0000f670: 6564 203c 3d20 636f 6d6d 6974 7465 640a  ed <= committed.
+0000f680: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f690: 6465 6620 7365 745f 636f 6d6d 6974 7465  def set_committe
+0000f6a0: 6428 7365 6c66 2c20 636f 6d6d 6974 7465  d(self, committe
+0000f6b0: 643a 2069 6e74 2920 2d3e 204e 6f6e 653a  d: int) -> None:
+0000f6c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f6d0: 2020 2020 2060 636f 6d6d 6974 7465 6460       `committed`
+0000f6e0: 3a20 5468 6520 6869 6768 6573 7420 6c6f  : The highest lo
+0000f6f0: 6720 706f 7369 7469 6f6e 2074 6861 7420  g position that 
+0000f700: 6973 206b 6e6f 776e 2074 6f20 6265 2069  is known to be i
+0000f710: 6e20 7374 6162 6c65 2073 746f 7261 6765  n stable storage
+0000f720: 0a20 2020 2020 2020 206f 6e20 6120 7175  .        on a qu
+0000f730: 6f72 756d 206f 6620 6e6f 6465 732e 0a0a  orum of nodes...
+0000f740: 2020 2020 2020 2020 496e 7661 7269 616e          Invarian
+0000f750: 743a 2061 7070 6c69 6564 203c 3d20 636f  t: applied <= co
+0000f760: 6d6d 6974 7465 640a 2020 2020 2020 2020  mmitted.        
+0000f770: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+0000f780: 7065 7273 6973 7465 6428 7365 6c66 2920  persisted(self) 
+0000f790: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+0000f7a0: 2222 220a 2020 2020 2020 2020 6070 6572  """.        `per
+0000f7b0: 7369 7374 6564 603a 2054 6865 2068 6967  sisted`: The hig
+0000f7c0: 6865 7374 206c 6f67 2070 6f73 6974 696f  hest log positio
+0000f7d0: 6e20 7468 6174 2069 7320 6b6e 6f77 6e20  n that is known 
+0000f7e0: 746f 2062 6520 7065 7273 6973 7465 6420  to be persisted 
+0000f7f0: 696e 2073 7461 626c 650a 2020 2020 2020  in stable.      
+0000f800: 2020 7374 6f72 6167 652e 2049 7427 7320    storage. It's 
+0000f810: 7573 6564 2066 6f72 206c 696d 6974 696e  used for limitin
+0000f820: 6720 7468 6520 7570 7065 7220 626f 756e  g the upper boun
+0000f830: 6420 6f66 2063 6f6d 6d69 7474 6564 2061  d of committed a
+0000f840: 6e64 0a20 2020 2020 2020 2070 6572 7369  nd.        persi
+0000f850: 7374 6564 2065 6e74 7269 6573 2e0a 0a20  sted entries... 
+0000f860: 2020 2020 2020 2049 6e76 6172 6961 6e74         Invariant
+0000f870: 3a20 7065 7273 6973 7465 6420 3c20 756e  : persisted < un
+0000f880: 7374 6162 6c65 2e6f 6666 7365 7420 2626  stable.offset &&
+0000f890: 2061 7070 6c69 6564 203c 3d20 7065 7273   applied <= pers
+0000f8a0: 6973 7465 640a 2020 2020 2020 2020 2222  isted.        ""
+0000f8b0: 220a 2020 2020 6465 6620 7365 745f 7065  ".    def set_pe
+0000f8c0: 7273 6973 7465 6428 7365 6c66 2c20 7065  rsisted(self, pe
+0000f8d0: 7273 6973 7465 643a 2069 6e74 2920 2d3e  rsisted: int) ->
+0000f8e0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+0000f8f0: 2222 0a20 2020 2020 2020 2060 7065 7273  "".        `pers
+0000f900: 6973 7465 6460 3a20 5468 6520 6869 6768  isted`: The high
+0000f910: 6573 7420 6c6f 6720 706f 7369 7469 6f6e  est log position
+0000f920: 2074 6861 7420 6973 206b 6e6f 776e 2074   that is known t
+0000f930: 6f20 6265 2070 6572 7369 7374 6564 2069  o be persisted i
+0000f940: 6e20 7374 6162 6c65 0a20 2020 2020 2020  n stable.       
+0000f950: 2073 746f 7261 6765 2e20 4974 2773 2075   storage. It's u
+0000f960: 7365 6420 666f 7220 6c69 6d69 7469 6e67  sed for limiting
+0000f970: 2074 6865 2075 7070 6572 2062 6f75 6e64   the upper bound
+0000f980: 206f 6620 636f 6d6d 6974 7465 6420 616e   of committed an
+0000f990: 640a 2020 2020 2020 2020 7065 7273 6973  d.        persis
+0000f9a0: 7465 6420 656e 7472 6965 732e 0a0a 2020  ted entries...  
+0000f9b0: 2020 2020 2020 496e 7661 7269 616e 743a        Invariant:
+0000f9c0: 2070 6572 7369 7374 6564 203c 2075 6e73   persisted < uns
+0000f9d0: 7461 626c 652e 6f66 6673 6574 2026 2620  table.offset && 
+0000f9e0: 6170 706c 6965 6420 3c3d 2070 6572 7369  applied <= persi
+0000f9f0: 7374 6564 0a20 2020 2020 2020 2022 2222  sted.        """
+0000fa00: 0a20 2020 2064 6566 2073 6c69 6365 280a  .    def slice(.
+0000fa10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000fa20: 2020 2020 2020 6c6f 773a 2069 6e74 2c0a        low: int,.
+0000fa30: 2020 2020 2020 2020 6869 6768 3a20 696e          high: in
+0000fa40: 742c 0a20 2020 2020 2020 206d 6178 5f73  t,.        max_s
+0000fa50: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+0000fa60: 745d 2c0a 2020 2020 2020 2020 636f 6e74  t],.        cont
+0000fa70: 6578 743a 2022 4765 7445 6e74 7269 6573  ext: "GetEntries
+0000fa80: 436f 6e74 6578 7452 6566 222c 0a20 2020  ContextRef",.   
+0000fa90: 2029 202d 3e20 4c69 7374 5b22 456e 7472   ) -> List["Entr
+0000faa0: 7952 6566 225d 3a0a 2020 2020 2020 2020  yRef"]:.        
+0000fab0: 2222 220a 2020 2020 2020 2020 4772 6162  """.        Grab
+0000fac0: 7320 6120 736c 6963 6520 6f66 2065 6e74  s a slice of ent
+0000fad0: 7269 6573 2066 726f 6d20 7468 6520 7261  ries from the ra
+0000fae0: 6674 2e20 556e 6c69 6b65 2061 2072 7573  ft. Unlike a rus
+0000faf0: 7420 736c 6963 6520 706f 696e 7465 722c  t slice pointer,
+0000fb00: 2074 6865 7365 2061 7265 0a20 2020 2020   these are.     
+0000fb10: 2020 2072 6574 7572 6e65 6420 6279 2076     returned by v
+0000fb20: 616c 7565 2e20 5468 6520 7265 7375 6c74  alue. The result
+0000fb30: 2069 7320 7472 756e 6361 7465 6420 746f   is truncated to
+0000fb40: 2074 6865 206d 6178 5f73 697a 6520 696e   the max_size in
+0000fb50: 2062 7974 6573 2e0a 2020 2020 2020 2020   bytes..        
+0000fb60: 2222 220a 2020 2020 6465 6620 7265 7374  """.    def rest
+0000fb70: 6f72 6528 7365 6c66 2c20 736e 6170 7368  ore(self, snapsh
+0000fb80: 6f74 3a20 2253 6e61 7073 686f 7422 207c  ot: "Snapshot" |
+0000fb90: 2022 536e 6170 7368 6f74 5265 6622 2920   "SnapshotRef") 
+0000fba0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000fbb0: 2022 2222 0a20 2020 2020 2020 2052 6573   """.        Res
+0000fbc0: 746f 7265 7320 7468 6520 6375 7272 656e  tores the curren
+0000fbd0: 7420 6c6f 6720 6672 6f6d 2061 2073 6e61  t log from a sna
+0000fbe0: 7073 686f 742e 0a20 2020 2020 2020 2022  pshot..        "
+0000fbf0: 2222 0a0a 636c 6173 7320 496e 4d65 6d6f  ""..class InMemo
+0000fc00: 7279 5261 6674 4c6f 6728 5f5f 4150 495f  ryRaftLog(__API_
+0000fc10: 5261 6674 4c6f 6729 3a0a 2020 2020 2222  RaftLog):.    ""
+0000fc20: 220a 2020 2020 5261 6674 206c 6f67 2069  ".    Raft log i
+0000fc30: 6d70 6c65 6d65 6e74 6174 696f 6e0a 2020  mplementation.  
+0000fc40: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+0000fc50: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000fc60: 2073 656c 662c 2073 746f 7265 3a20 224d   self, store: "M
+0000fc70: 656d 5374 6f72 6167 6552 6566 222c 206c  emStorageRef", l
+0000fc80: 6f67 6765 723a 2022 4c6f 6767 6572 2220  ogger: "Logger" 
+0000fc90: 7c20 224c 6f67 6765 7252 6566 220a 2020  | "LoggerRef".  
+0000fca0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+0000fcb0: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
+0000fcc0: 6628 7365 6c66 2920 2d3e 2022 496e 4d65  f(self) -> "InMe
+0000fcd0: 6d6f 7279 5261 6674 4c6f 6752 6566 223a  moryRaftLogRef":
+0000fce0: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+0000fcf0: 5f73 746f 7265 2873 656c 6629 202d 3e20  _store(self) -> 
+0000fd00: 224d 656d 5374 6f72 6167 6552 6566 223a  "MemStorageRef":
+0000fd10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fd20: 2020 2020 2047 7261 6220 6120 7265 6164       Grab a read
+0000fd30: 2d6f 6e6c 7920 7265 6665 7265 6e63 6520  -only reference 
+0000fd40: 746f 2074 6865 2075 6e64 6572 6c79 696e  to the underlyin
+0000fd50: 6720 7374 6f72 6167 652e 0a20 2020 2020  g storage..     
+0000fd60: 2020 2022 2222 0a0a 636c 6173 7320 496e     """..class In
+0000fd70: 4d65 6d6f 7279 5261 6674 4c6f 6752 6566  MemoryRaftLogRef
+0000fd80: 285f 5f41 5049 5f52 6166 744c 6f67 293a  (__API_RaftLog):
+0000fd90: 0a20 2020 2022 2222 0a20 2020 2052 6566  .    """.    Ref
+0000fda0: 6572 656e 6365 2074 7970 6520 6f66 203a  erence type of :
+0000fdb0: 636c 6173 733a 6049 6e4d 656d 6f72 7952  class:`InMemoryR
+0000fdc0: 6166 744c 6f67 602e 0a20 2020 2022 2222  aftLog`..    """
+0000fdd0: 0a0a 2020 2020 6465 6620 6765 745f 7374  ..    def get_st
+0000fde0: 6f72 6528 7365 6c66 2920 2d3e 2022 4d65  ore(self) -> "Me
+0000fdf0: 6d53 746f 7261 6765 5265 6622 3a0a 2020  mStorageRef":.  
+0000fe00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000fe10: 2020 4772 6162 2061 2072 6561 642d 6f6e    Grab a read-on
+0000fe20: 6c79 2072 6566 6572 656e 6365 2074 6f20  ly reference to 
+0000fe30: 7468 6520 756e 6465 726c 7969 6e67 2073  the underlying s
+0000fe40: 746f 7261 6765 2e0a 2020 2020 2020 2020  torage..        
+0000fe50: 2222 220a 0a63 6c61 7373 2052 6166 744c  """..class RaftL
+0000fe60: 6f67 285f 5f41 5049 5f52 6166 744c 6f67  og(__API_RaftLog
+0000fe70: 293a 0a20 2020 2022 2222 2022 2222 0a0a  ):.    """ """..
+0000fe80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000fe90: 2873 656c 662c 2073 746f 7265 3a20 2253  (self, store: "S
+0000fea0: 746f 7261 6765 5265 6622 2c20 6c6f 6767  torageRef", logg
+0000feb0: 6572 3a20 224c 6f67 6765 7222 207c 2022  er: "Logger" | "
+0000fec0: 4c6f 6767 6572 5265 6622 2920 2d3e 204e  LoggerRef") -> N
+0000fed0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+0000fee0: 206d 616b 655f 7265 6628 7365 6c66 2920   make_ref(self) 
+0000fef0: 2d3e 2022 5261 6674 4c6f 6752 6566 223a  -> "RaftLogRef":
+0000ff00: 202e 2e2e 0a20 2020 2064 6566 2067 6574   ....    def get
+0000ff10: 5f73 746f 7265 2873 656c 6629 202d 3e20  _store(self) -> 
+0000ff20: 2253 746f 7261 6765 5265 6622 3a0a 2020  "StorageRef":.  
+0000ff30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ff40: 2020 4772 6162 2061 2072 6561 642d 6f6e    Grab a read-on
+0000ff50: 6c79 2072 6566 6572 656e 6365 2074 6f20  ly reference to 
+0000ff60: 7468 6520 756e 6465 726c 7969 6e67 2073  the underlying s
+0000ff70: 746f 7261 6765 2e0a 2020 2020 2020 2020  torage..        
+0000ff80: 2222 220a 0a63 6c61 7373 2052 6166 744c  """..class RaftL
+0000ff90: 6f67 5265 6628 5f5f 4150 495f 5261 6674  ogRef(__API_Raft
+0000ffa0: 4c6f 6729 3a0a 2020 2020 2222 220a 2020  Log):.    """.  
+0000ffb0: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
+0000ffc0: 206f 6620 3a63 6c61 7373 3a60 5261 6674   of :class:`Raft
+0000ffd0: 4c6f 6760 2e0a 2020 2020 2222 220a 0a20  Log`..    """.. 
+0000ffe0: 2020 2064 6566 2067 6574 5f73 746f 7265     def get_store
+0000fff0: 2873 656c 6629 202d 3e20 2253 746f 7261  (self) -> "Stora
+00010000: 6765 5265 6622 3a0a 2020 2020 2020 2020  geRef":.        
+00010010: 2222 220a 2020 2020 2020 2020 4772 6162  """.        Grab
+00010020: 2061 2072 6561 642d 6f6e 6c79 2072 6566   a read-only ref
+00010030: 6572 656e 6365 2074 6f20 7468 6520 756e  erence to the un
+00010040: 6465 726c 7969 6e67 2073 746f 7261 6765  derlying storage
+00010050: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
+00010060: 6c61 7373 205f 5f41 5049 5f52 6166 743a  lass __API_Raft:
+00010070: 0a20 2020 2064 6566 2061 7070 656e 645f  .    def append_
+00010080: 656e 7472 7928 7365 6c66 2c20 656e 7473  entry(self, ents
+00010090: 3a20 4c69 7374 5b22 456e 7472 7922 5d20  : List["Entry"] 
+000100a0: 7c20 4c69 7374 5b22 456e 7472 7952 6566  | List["EntryRef
+000100b0: 225d 2920 2d3e 2062 6f6f 6c3a 0a20 2020  "]) -> bool:.   
+000100c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000100d0: 2041 7070 656e 6473 2061 2073 6c69 6365   Appends a slice
+000100e0: 206f 6620 656e 7472 6965 7320 746f 2074   of entries to t
+000100f0: 6865 206c 6f67 2e0a 2020 2020 2020 2020  he log..        
+00010100: 5468 6520 656e 7472 6965 7320 6172 6520  The entries are 
+00010110: 7570 6461 7465 6420 746f 206d 6174 6368  updated to match
+00010120: 2074 6865 2063 7572 7265 6e74 2069 6e64   the current ind
+00010130: 6578 2061 6e64 2074 6572 6d2e 0a20 2020  ex and term..   
+00010140: 2020 2020 204f 6e6c 7920 6361 6c6c 6564       Only called
+00010150: 2062 7920 6c65 6164 6572 2063 7572 7265   by leader curre
+00010160: 6e74 6c79 0a20 2020 2020 2020 2022 2222  ntly.        """
+00010170: 0a20 2020 2064 6566 2073 656e 645f 6170  .    def send_ap
+00010180: 7065 6e64 2873 656c 662c 2074 6f3a 2069  pend(self, to: i
+00010190: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+000101a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000101b0: 2053 656e 6473 2061 6e20 6170 7065 6e64   Sends an append
+000101c0: 2052 5043 2077 6974 6820 6e65 7720 656e   RPC with new en
+000101d0: 7472 6965 7320 2869 6620 616e 7929 2061  tries (if any) a
+000101e0: 6e64 2074 6865 2063 7572 7265 6e74 2063  nd the current c
+000101f0: 6f6d 6d69 7420 696e 6465 7820 746f 2074  ommit index to t
+00010200: 6865 2067 6976 656e 0a20 2020 2020 2020  he given.       
+00010210: 2070 6565 722e 0a20 2020 2020 2020 2022   peer..        "
+00010220: 2222 0a20 2020 2064 6566 206f 6e5f 7065  "".    def on_pe
+00010230: 7273 6973 745f 656e 7472 6965 7328 7365  rsist_entries(se
+00010240: 6c66 2c20 696e 6465 783a 2069 6e74 2c20  lf, index: int, 
+00010250: 7465 726d 3a20 696e 7429 202d 3e20 4e6f  term: int) -> No
+00010260: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00010270: 2020 2020 2020 2020 4e6f 7469 6669 6573          Notifies
+00010280: 2074 6861 7420 7468 6573 6520 7261 6674   that these raft
+00010290: 206c 6f67 7320 6861 7665 2062 6565 6e20   logs have been 
+000102a0: 7065 7273 6973 7465 642e 0a20 2020 2020  persisted..     
+000102b0: 2020 2022 2222 0a20 2020 2064 6566 2061     """.    def a
+000102c0: 7070 6c79 5f74 6f5f 6375 7272 656e 745f  pply_to_current_
+000102d0: 7465 726d 2873 656c 6629 202d 3e20 626f  term(self) -> bo
+000102e0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
+000102f0: 2020 2020 2020 2020 4368 6563 6b73 2069          Checks i
+00010300: 6620 6c6f 6773 2061 7265 2061 7070 6c69  f logs are appli
+00010310: 6564 2074 6f20 6375 7272 656e 7420 7465  ed to current te
+00010320: 726d 2e0a 2020 2020 2020 2020 2222 220a  rm..        """.
+00010330: 2020 2020 6465 6620 636f 6d6d 6974 5f74      def commit_t
+00010340: 6f5f 6375 7272 656e 745f 7465 726d 2873  o_current_term(s
+00010350: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+00010360: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010370: 2020 4368 6563 6b73 2069 6620 6c6f 6773    Checks if logs
+00010380: 2061 7265 2063 6f6d 6d69 7474 6564 2074   are committed t
+00010390: 6f20 6974 7320 7465 726d 2e0a 0a20 2020  o its term...   
+000103a0: 2020 2020 2054 6865 2063 6865 636b 2069       The check i
+000103b0: 7320 7573 6566 756c 2075 7375 616c 6c79  s useful usually
+000103c0: 2077 6865 6e20 7261 6674 2069 7320 6c65   when raft is le
+000103d0: 6164 6572 2e0a 2020 2020 2020 2020 2222  ader..        ""
+000103e0: 220a 2020 2020 6465 6620 6772 6f75 705f  ".    def group_
+000103f0: 636f 6d6d 6974 2873 656c 6629 202d 3e20  commit(self) -> 
+00010400: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00010410: 220a 2020 2020 2020 2020 5768 6574 6865  ".        Whethe
+00010420: 7220 656e 6162 6c65 2067 726f 7570 2063  r enable group c
+00010430: 6f6d 6d69 742e 0a20 2020 2020 2020 2022  ommit..        "
+00010440: 2222 0a20 2020 2064 6566 2065 6e61 626c  "".    def enabl
+00010450: 655f 6772 6f75 705f 636f 6d6d 6974 2873  e_group_commit(s
+00010460: 656c 662c 2065 6e61 626c 653a 2062 6f6f  elf, enable: boo
+00010470: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+00010480: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010490: 436f 6e66 6967 7572 6573 2067 726f 7570  Configures group
+000104a0: 2063 6f6d 6d69 742e 0a0a 2020 2020 2020   commit...      
+000104b0: 2020 4966 2067 726f 7570 2063 6f6d 6d69    If group commi
+000104c0: 7420 6973 2065 6e61 626c 6564 2c20 6f6e  t is enabled, on
+000104d0: 6c79 206c 6f67 7320 7265 706c 6963 6174  ly logs replicat
+000104e0: 6564 2074 6f20 6174 206c 6561 7374 2074  ed to at least t
+000104f0: 776f 0a20 2020 2020 2020 2064 6966 6665  wo.        diffe
+00010500: 7265 6e74 2067 726f 7570 7320 6172 6520  rent groups are 
+00010510: 636f 6d6d 6974 7465 642e 0a0a 2020 2020  committed...    
+00010520: 2020 2020 596f 7520 7368 6f75 6c64 2075      You should u
+00010530: 7365 2060 6173 7369 676e 5f63 6f6d 6d69  se `assign_commi
+00010540: 745f 6772 6f75 7073 6020 746f 2063 6f6e  t_groups` to con
+00010550: 6669 6775 7265 2070 6565 7220 6772 6f75  figure peer grou
+00010560: 7073 2e0a 2020 2020 2020 2020 2222 220a  ps..        """.
+00010570: 2020 2020 6465 6620 636c 6561 725f 636f      def clear_co
+00010580: 6d6d 6974 5f67 726f 7570 2873 656c 6629  mmit_group(self)
+00010590: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000105a0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+000105b0: 6d6f 7665 7320 616c 6c20 636f 6d6d 6974  moves all commit
+000105c0: 2067 726f 7570 2063 6f6e 6669 6775 7261   group configura
+000105d0: 7469 6f6e 732e 0a20 2020 2020 2020 2022  tions..        "
+000105e0: 2222 0a20 2020 2064 6566 2063 6865 636b  "".    def check
+000105f0: 5f67 726f 7570 5f63 6f6d 6d69 745f 636f  _group_commit_co
+00010600: 6e73 6973 7465 6e74 2873 656c 6629 202d  nsistent(self) -
+00010610: 3e20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  > Optional[bool]
+00010620: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00010630: 2020 2020 2020 4368 6563 6b73 2077 6865        Checks whe
+00010640: 7468 6572 2074 6865 2072 6166 7420 6772  ther the raft gr
+00010650: 6f75 7020 6973 2075 7369 6e67 2067 726f  oup is using gro
+00010660: 7570 2063 6f6d 6d69 7420 616e 6420 636f  up commit and co
+00010670: 6e73 6973 7465 6e74 0a20 2020 2020 2020  nsistent.       
+00010680: 206f 7665 7220 6772 6f75 702e 0a0a 2020   over group...  
+00010690: 2020 2020 2020 4966 2069 7420 6361 6e27        If it can'
+000106a0: 7420 6765 7420 6120 636f 7272 6563 7420  t get a correct 
+000106b0: 616e 7377 6572 2c20 604e 6f6e 6560 2069  answer, `None` i
+000106c0: 7320 7265 7475 726e 6564 2e0a 2020 2020  s returned..    
+000106d0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+000106e0: 6173 7369 676e 5f63 6f6d 6d69 745f 6772  assign_commit_gr
+000106f0: 6f75 7073 2873 656c 662c 2069 6473 3a20  oups(self, ids: 
+00010700: 4c69 7374 5b54 7570 6c65 5b69 6e74 2c20  List[Tuple[int, 
+00010710: 696e 745d 5d29 202d 3e20 4e6f 6e65 3a0a  int]]) -> None:.
+00010720: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010730: 2020 2020 4173 7369 676e 7320 6772 6f75      Assigns grou
+00010740: 7073 2074 6f20 7065 6572 732e 0a0a 2020  ps to peers...  
+00010750: 2020 2020 2020 5468 6520 7475 706c 6520        The tuple 
+00010760: 6973 2028 6070 6565 725f 6964 602c 2060  is (`peer_id`, `
+00010770: 6772 6f75 705f 6964 6029 2e20 6067 726f  group_id`). `gro
+00010780: 7570 5f69 6460 2073 686f 756c 6420 6265  up_id` should be
+00010790: 206c 6172 6765 7220 7468 616e 2030 2e0a   larger than 0..
+000107a0: 0a20 2020 2020 2020 2054 6865 2067 726f  .        The gro
+000107b0: 7570 2069 6e66 6f72 6d61 7469 6f6e 2069  up information i
+000107c0: 7320 6f6e 6c79 2073 746f 7265 6420 696e  s only stored in
+000107d0: 206d 656d 6f72 792e 2053 6f20 796f 7520   memory. So you 
+000107e0: 6e65 6564 2074 6f20 636f 6e66 6967 7572  need to configur
+000107f0: 650a 2020 2020 2020 2020 6974 2065 7665  e.        it eve
+00010800: 7279 2074 696d 6520 6120 7261 6674 2073  ry time a raft s
+00010810: 7461 7465 206d 6163 6869 6e65 2069 7320  tate machine is 
+00010820: 696e 6974 6961 6c69 7a65 6420 6f72 2061  initialized or a
+00010830: 2073 6e61 7073 686f 7420 6973 2061 7070   snapshot is app
+00010840: 6c69 6564 2e0a 2020 2020 2020 2020 2222  lied..        ""
+00010850: 220a 2020 2020 6465 6620 636f 6d6d 6974  ".    def commit
+00010860: 5f61 7070 6c79 2873 656c 662c 2061 7070  _apply(self, app
+00010870: 6c69 6564 3a20 696e 7429 202d 3e20 4e6f  lied: int) -> No
+00010880: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00010890: 2020 2020 2020 2020 436f 6d6d 6974 2074          Commit t
+000108a0: 6861 7420 7468 6520 5261 6674 2070 6565  hat the Raft pee
+000108b0: 7220 6861 7320 6170 706c 6965 6420 7570  r has applied up
+000108c0: 2074 6f20 7468 6520 6769 7665 6e20 696e   to the given in
+000108d0: 6465 782e 0a0a 2020 2020 2020 2020 5265  dex...        Re
+000108e0: 6769 7374 6572 7320 7468 6520 6e65 7720  gisters the new 
+000108f0: 6170 706c 6965 6420 696e 6465 7820 746f  applied index to
+00010900: 2074 6865 2052 6166 7420 6c6f 672e 0a0a   the Raft log...
+00010910: 2020 2020 2020 2020 2320 486f 6f6b 730a          # Hooks.
+00010920: 0a20 2020 2020 2020 202a 2050 6f73 743a  .        * Post:
+00010930: 2043 6865 636b 7320 746f 2073 6565 2069   Checks to see i
+00010940: 6620 6974 2773 2074 696d 6520 746f 2066  f it's time to f
+00010950: 696e 616c 697a 6520 6120 4a6f 696e 7420  inalize a Joint 
+00010960: 436f 6e73 656e 7375 7320 7374 6174 652e  Consensus state.
+00010970: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010980: 2064 6566 206d 6179 6265 5f63 6f6d 6d69   def maybe_commi
+00010990: 7428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  t(self) -> bool:
+000109a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000109b0: 2020 2020 2041 7474 656d 7074 7320 746f       Attempts to
+000109c0: 2061 6476 616e 6365 2074 6865 2063 6f6d   advance the com
+000109d0: 6d69 7420 696e 6465 782e 2052 6574 7572  mit index. Retur
+000109e0: 6e73 2074 7275 6520 6966 2074 6865 2063  ns true if the c
+000109f0: 6f6d 6d69 7420 696e 6465 780a 2020 2020  ommit index.    
+00010a00: 2020 2020 6368 616e 6765 6420 2869 6e20      changed (in 
+00010a10: 7768 6963 6820 6361 7365 2074 6865 2063  which case the c
+00010a20: 616c 6c65 7220 7368 6f75 6c64 2063 616c  aller should cal
+00010a30: 6c20 6072 2e62 6361 7374 5f61 7070 656e  l `r.bcast_appen
+00010a40: 6460 292e 0a20 2020 2020 2020 2022 2222  d`)..        """
+00010a50: 0a20 2020 2064 6566 2075 6e63 6f6d 6d69  .    def uncommi
+00010a60: 7474 6564 5f73 697a 6528 7365 6c66 2920  tted_size(self) 
+00010a70: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00010a80: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+00010a90: 726e 2063 7572 7265 6e74 2075 6e63 6f6d  rn current uncom
+00010aa0: 6d69 7474 6564 2073 697a 6520 7265 636f  mitted size reco
+00010ab0: 7264 6564 2062 7920 756e 636f 6d6d 6974  rded by uncommit
+00010ac0: 7465 645f 7374 6174 650a 2020 2020 2020  ted_state.      
+00010ad0: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
+00010ae0: 7962 655f 696e 6372 6561 7365 5f75 6e63  ybe_increase_unc
+00010af0: 6f6d 6d69 7474 6564 5f73 697a 6528 0a20  ommitted_size(. 
+00010b00: 2020 2020 2020 2073 656c 662c 2065 6e74         self, ent
+00010b10: 733a 204c 6973 745b 2245 6e74 7279 225d  s: List["Entry"]
+00010b20: 207c 204c 6973 745b 2245 6e74 7279 5265   | List["EntryRe
+00010b30: 6622 5d0a 2020 2020 2920 2d3e 2062 6f6f  f"].    ) -> boo
+00010b40: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00010b50: 2020 2020 2020 2049 6e63 7265 6173 6520         Increase 
+00010b60: 7369 7a65 206f 6620 2765 6e74 7327 2074  size of 'ents' t
+00010b70: 6f20 756e 636f 6d6d 6974 7465 6420 7369  o uncommitted si
+00010b80: 7a65 2e20 5265 7475 726e 2074 7275 6520  ze. Return true 
+00010b90: 7768 656e 2073 697a 6520 6c69 6d69 740a  when size limit.
+00010ba0: 2020 2020 2020 2020 6973 2073 6174 6973          is satis
+00010bb0: 6669 6564 2e20 4f74 6865 7277 6973 6520  fied. Otherwise 
+00010bc0: 7265 7475 726e 2066 616c 7365 2061 6e64  return false and
+00010bd0: 2075 6e63 6f6d 6d69 7474 6564 2073 697a   uncommitted siz
+00010be0: 6520 7265 6d61 696e 7320 756e 6368 616e  e remains unchan
+00010bf0: 6765 642e 0a20 2020 2020 2020 2046 6f72  ged..        For
+00010c00: 2072 6166 7420 7769 7468 206e 6f20 6c69   raft with no li
+00010c10: 6d69 7428 6f72 206e 6f6e 2d6c 6561 6465  mit(or non-leade
+00010c20: 7220 7261 6674 292c 2069 7420 616c 7761  r raft), it alwa
+00010c30: 7973 2072 6574 7572 6e20 7472 7565 2e0a  ys return true..
+00010c40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010c50: 6465 6620 7265 6475 6365 5f75 6e63 6f6d  def reduce_uncom
+00010c60: 6d69 7474 6564 5f73 697a 6528 7365 6c66  mitted_size(self
+00010c70: 2c20 656e 7473 3a20 4c69 7374 5b22 456e  , ents: List["En
+00010c80: 7472 7922 5d20 7c20 4c69 7374 5b22 456e  try"] | List["En
+00010c90: 7472 7952 6566 225d 2920 2d3e 204e 6f6e  tryRef"]) -> Non
+00010ca0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00010cb0: 2020 2020 2020 2052 6564 7563 6520 7369         Reduce si
+00010cc0: 7a65 206f 6620 2765 6e74 7327 2066 726f  ze of 'ents' fro
+00010cd0: 6d20 756e 636f 6d6d 6974 7465 6420 7369  m uncommitted si
+00010ce0: 7a65 2e0a 2020 2020 2020 2020 2222 220a  ze..        """.
+00010cf0: 2020 2020 6465 6620 6263 6173 745f 6170      def bcast_ap
+00010d00: 7065 6e64 2873 656c 6629 202d 3e20 4e6f  pend(self) -> No
+00010d10: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00010d20: 2020 2020 2020 2020 5365 6e64 7320 5250          Sends RP
+00010d30: 432c 2077 6974 6820 656e 7472 6965 7320  C, with entries 
+00010d40: 746f 2061 6c6c 2070 6565 7273 2074 6861  to all peers tha
+00010d50: 7420 6172 6520 6e6f 7420 7570 2d74 6f2d  t are not up-to-
+00010d60: 6461 7465 0a20 2020 2020 2020 2061 6363  date.        acc
+00010d70: 6f72 6469 6e67 2074 6f20 7468 6520 7072  ording to the pr
+00010d80: 6f67 7265 7373 2072 6563 6f72 6465 6420  ogress recorded 
+00010d90: 696e 2072 2e70 7273 2829 2e0a 2020 2020  in r.prs()..    
+00010da0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00010db0: 6263 6173 745f 6865 6172 7462 6561 7428  bcast_heartbeat(
+00010dc0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00010dd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010de0: 2020 2053 656e 6473 2052 5043 2c20 7769     Sends RPC, wi
+00010df0: 7468 6f75 7420 656e 7472 6965 7320 746f  thout entries to
+00010e00: 2061 6c6c 2074 6865 2070 6565 7273 2e0a   all the peers..
+00010e10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010e20: 6465 6620 7368 6f75 6c64 5f62 6361 7374  def should_bcast
+00010e30: 5f63 6f6d 6d69 7428 7365 6c66 2920 2d3e  _commit(self) ->
+00010e40: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00010e50: 2222 0a20 2020 2020 2020 2053 7065 6369  "".        Speci
+00010e60: 6669 6573 2069 6620 7468 6520 636f 6d6d  fies if the comm
+00010e70: 6974 2073 686f 756c 6420 6265 2062 726f  it should be bro
+00010e80: 6164 6361 7374 2e0a 2020 2020 2020 2020  adcast..        
+00010e90: 2222 220a 2020 2020 6465 6620 736b 6970  """.    def skip
+00010ea0: 5f62 6361 7374 5f63 6f6d 6d69 7428 7365  _bcast_commit(se
+00010eb0: 6c66 2c20 736b 6970 3a20 626f 6f6c 2920  lf, skip: bool) 
+00010ec0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00010ed0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
+00010ee0: 2077 6865 7468 6572 2073 6b69 7020 6272   whether skip br
+00010ef0: 6f61 6463 6173 7420 656d 7074 7920 636f  oadcast empty co
+00010f00: 6d6d 6974 206d 6573 7361 6765 7320 6174  mmit messages at
+00010f10: 2072 756e 7469 6d65 2e0a 2020 2020 2020   runtime..      
+00010f20: 2020 2222 220a 2020 2020 6465 6620 6265    """.    def be
+00010f30: 636f 6d65 5f6c 6561 6465 7228 7365 6c66  come_leader(self
+00010f40: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00010f50: 2020 2022 2222 0a20 2020 2020 2020 204d     """.        M
+00010f60: 616b 6573 2074 6869 7320 7261 6674 2074  akes this raft t
+00010f70: 6865 206c 6561 6465 722e 0a0a 2020 2020  he leader...    
+00010f80: 2020 2020 2320 5061 6e69 6373 0a0a 2020      # Panics..  
+00010f90: 2020 2020 2020 5061 6e69 6373 2069 6620        Panics if 
+00010fa0: 7468 6973 2069 7320 6120 666f 6c6c 6f77  this is a follow
+00010fb0: 6572 206e 6f64 652e 0a20 2020 2020 2020  er node..       
+00010fc0: 2022 2222 0a20 2020 2064 6566 2062 6563   """.    def bec
+00010fd0: 6f6d 655f 666f 6c6c 6f77 6572 2873 656c  ome_follower(sel
+00010fe0: 662c 2074 6572 6d3a 2069 6e74 2c20 6c65  f, term: int, le
+00010ff0: 6164 6572 5f69 643a 2069 6e74 2920 2d3e  ader_id: int) ->
+00011000: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00011010: 2222 0a20 2020 2020 2020 2043 6f6e 7665  "".        Conve
+00011020: 7274 7320 7468 6973 206e 6f64 6520 746f  rts this node to
+00011030: 2061 2066 6f6c 6c6f 7765 722e 0a20 2020   a follower..   
+00011040: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00011050: 2062 6563 6f6d 655f 7072 655f 6361 6e64   become_pre_cand
+00011060: 6964 6174 6528 7365 6c66 2920 2d3e 204e  idate(self) -> N
+00011070: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00011080: 0a20 2020 2020 2020 2043 6f6e 7665 7274  .        Convert
+00011090: 7320 7468 6973 206e 6f64 6520 746f 2061  s this node to a
+000110a0: 2070 7265 2d63 616e 6469 6461 7465 0a0a   pre-candidate..
+000110b0: 2020 2020 2020 2020 2320 5061 6e69 6373          # Panics
+000110c0: 0a0a 2020 2020 2020 2020 5061 6e69 6373  ..        Panics
+000110d0: 2069 6620 6120 6c65 6164 6572 2061 6c72   if a leader alr
+000110e0: 6561 6479 2065 7869 7374 732e 0a20 2020  eady exists..   
+000110f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00011100: 2062 6563 6f6d 655f 6361 6e64 6964 6174   become_candidat
+00011110: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00011120: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011130: 2020 2020 2043 6f6e 7665 7274 7320 7468       Converts th
+00011140: 6973 206e 6f64 6520 746f 2061 2063 616e  is node to a can
+00011150: 6469 6461 7465 0a0a 2020 2020 2020 2020  didate..        
+00011160: 2320 5061 6e69 6373 0a0a 2020 2020 2020  # Panics..      
+00011170: 2020 5061 6e69 6373 2069 6620 6120 6c65    Panics if a le
+00011180: 6164 6572 2061 6c72 6561 6479 2065 7869  ader already exi
+00011190: 7374 732e 0a20 2020 2020 2020 2022 2222  sts..        """
+000111a0: 0a20 2020 2064 6566 2068 6561 7274 6265  .    def heartbe
+000111b0: 6174 5f74 696d 656f 7574 2873 656c 6629  at_timeout(self)
+000111c0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+000111d0: 2022 2222 0a20 2020 2020 2020 2046 6574   """.        Fet
+000111e0: 6368 2074 6865 206c 656e 6774 6820 6f66  ch the length of
+000111f0: 2074 6865 2068 6561 7274 6265 6174 2074   the heartbeat t
+00011200: 696d 656f 7574 0a20 2020 2020 2020 2022  imeout.        "
+00011210: 2222 0a20 2020 2064 6566 2068 6561 7274  "".    def heart
+00011220: 6265 6174 5f65 6c61 7073 6564 2873 656c  beat_elapsed(sel
+00011230: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00011240: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
+00011250: 6574 6368 2074 6865 206e 756d 6265 7220  etch the number 
+00011260: 6f66 2074 6963 6b73 2065 6c61 7073 6564  of ticks elapsed
+00011270: 2073 696e 6365 206c 6173 7420 6865 6172   since last hear
+00011280: 7462 6561 742e 0a20 2020 2020 2020 2022  tbeat..        "
+00011290: 2222 0a20 2020 2064 6566 2065 6c65 6374  "".    def elect
+000112a0: 696f 6e5f 7469 6d65 6f75 7428 7365 6c66  ion_timeout(self
+000112b0: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+000112c0: 2020 2222 220a 2020 2020 2020 2020 4665    """.        Fe
+000112d0: 7463 6820 7468 6520 6c65 6e67 7468 206f  tch the length o
+000112e0: 6620 7468 6520 656c 6563 7469 6f6e 2074  f the election t
+000112f0: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
+00011300: 2222 220a 2020 2020 6465 6620 7261 6e64  """.    def rand
+00011310: 6f6d 697a 6564 5f65 6c65 6374 696f 6e5f  omized_election_
+00011320: 7469 6d65 6f75 7428 7365 6c66 2920 2d3e  timeout(self) ->
+00011330: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00011340: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00011350: 2074 6865 206c 656e 6774 6820 6f66 2074   the length of t
+00011360: 6865 2063 7572 7265 6e74 2072 616e 646f  he current rando
+00011370: 6d69 7a65 6420 656c 6563 7469 6f6e 2074  mized election t
+00011380: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
+00011390: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+000113a0: 7261 6e64 6f6d 697a 6564 5f65 6c65 6374  randomized_elect
+000113b0: 696f 6e5f 7469 6d65 6f75 7428 7365 6c66  ion_timeout(self
+000113c0: 2c20 7261 6e64 6f6d 697a 6564 5f65 6c65  , randomized_ele
+000113d0: 6374 696f 6e5f 7469 6d65 6f75 743a 2069  ction_timeout: i
+000113e0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+000113f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011400: 2046 6f72 2074 6573 7469 6e67 206c 6561   For testing lea
+00011410: 6465 7220 6c65 6173 650a 2020 2020 2020  der lease.      
+00011420: 2020 2222 220a 2020 2020 6465 6620 7265    """.    def re
+00011430: 7365 745f 7261 6e64 6f6d 697a 6564 5f65  set_randomized_e
+00011440: 6c65 6374 696f 6e5f 7469 6d65 6f75 7428  lection_timeout(
+00011450: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00011460: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011470: 2020 2052 6567 656e 6572 6174 6573 2061     Regenerates a
+00011480: 6e64 2073 746f 7265 7320 7468 6520 656c  nd stores the el
+00011490: 6563 7469 6f6e 2074 696d 656f 7574 2e0a  ection timeout..
+000114a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000114b0: 6465 6620 7061 7373 5f65 6c65 6374 696f  def pass_electio
+000114c0: 6e5f 7469 6d65 6f75 7428 7365 6c66 2920  n_timeout(self) 
+000114d0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+000114e0: 2022 2222 0a20 2020 2020 2020 2060 7061   """.        `pa
+000114f0: 7373 5f65 6c65 6374 696f 6e5f 7469 6d65  ss_election_time
+00011500: 6f75 7460 2072 6574 7572 6e73 2074 7275  out` returns tru
+00011510: 6520 6966 2060 656c 6563 7469 6f6e 5f65  e if `election_e
+00011520: 6c61 7073 6564 6020 6973 2067 7265 6174  lapsed` is great
+00011530: 6572 0a20 2020 2020 2020 2074 6861 6e20  er.        than 
+00011540: 6f72 2065 7175 616c 2074 6f20 7468 6520  or equal to the 
+00011550: 7261 6e64 6f6d 697a 6564 2065 6c65 6374  randomized elect
+00011560: 696f 6e20 7469 6d65 6f75 7420 696e 0a20  ion timeout in. 
+00011570: 2020 2020 2020 205b 6065 6c65 6374 696f         [`electio
+00011580: 6e5f 7469 6d65 6f75 7460 2c20 3220 2a20  n_timeout`, 2 * 
+00011590: 6065 6c65 6374 696f 6e5f 7469 6d65 6f75  `election_timeou
+000115a0: 7460 202d 2031 5d2e 0a20 2020 2020 2020  t` - 1]..       
+000115b0: 2022 2222 0a20 2020 2064 6566 2073 656e   """.    def sen
+000115c0: 645f 7469 6d65 6f75 745f 6e6f 7728 7365  d_timeout_now(se
+000115d0: 6c66 2c20 746f 3a20 696e 7429 202d 3e20  lf, to: int) -> 
+000115e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000115f0: 220a 2020 2020 2020 2020 4973 7375 6573  ".        Issues
+00011600: 2061 206d 6573 7361 6765 2074 6f20 7469   a message to ti
+00011610: 6d65 6f75 7420 696d 6d65 6469 6174 656c  meout immediatel
+00011620: 792e 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
+00011630: 2020 2064 6566 2072 6561 6479 5f72 6561     def ready_rea
+00011640: 645f 636f 756e 7428 7365 6c66 2920 2d3e  d_count(self) ->
+00011650: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00011660: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00011670: 7320 686f 7720 6d61 6e79 2072 6561 6420  s how many read 
+00011680: 7374 6174 6573 2065 7869 7374 2e0a 2020  states exist..  
+00011690: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+000116a0: 6620 7065 6e64 696e 675f 7265 6164 5f63  f pending_read_c
+000116b0: 6f75 6e74 2873 656c 6629 202d 3e20 696e  ount(self) -> in
+000116c0: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+000116d0: 2020 2020 2020 2052 6574 7572 6e73 2074         Returns t
+000116e0: 6865 206e 756d 6265 7220 6f66 2070 656e  he number of pen
+000116f0: 6469 6e67 2072 6561 642d 6f6e 6c79 206d  ding read-only m
+00011700: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
+00011710: 2022 2222 0a20 2020 2064 6566 206c 6f61   """.    def loa
+00011720: 645f 7374 6174 6528 7365 6c66 2c20 6873  d_state(self, hs
+00011730: 3a20 2248 6172 6453 7461 7465 2220 7c20  : "HardState" | 
+00011740: 2248 6172 6453 7461 7465 5265 6622 2920  "HardStateRef") 
+00011750: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00011760: 2022 2222 0a20 2020 2020 2020 2046 6f72   """.        For
+00011770: 2061 2067 6976 656e 2068 6172 6473 7461   a given hardsta
+00011780: 7465 2c20 6c6f 6164 2074 6865 2073 7461  te, load the sta
+00011790: 7465 2069 6e74 6f20 7365 6c66 2e0a 2020  te into self..  
+000117a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+000117b0: 6620 736f 6674 5f73 7461 7465 2873 656c  f soft_state(sel
+000117c0: 6629 202d 3e20 2253 6f66 7453 7461 7465  f) -> "SoftState
+000117d0: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+000117e0: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
+000117f0: 2076 616c 7565 2072 6570 7265 7365 6e74   value represent
+00011800: 696e 6720 7468 6520 736f 6674 7374 6174  ing the softstat
+00011810: 6520 6174 2074 6865 2074 696d 6520 6f66  e at the time of
+00011820: 2063 616c 6c69 6e67 2e0a 2020 2020 2020   calling..      
+00011830: 2020 2222 220a 2020 2020 6465 6620 6861    """.    def ha
+00011840: 7264 5f73 7461 7465 2873 656c 6629 202d  rd_state(self) -
+00011850: 3e20 2248 6172 6453 7461 7465 223a 0a20  > "HardState":. 
+00011860: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011870: 2020 2052 6574 7572 6e73 2061 2076 616c     Returns a val
+00011880: 7565 2072 6570 7265 7365 6e74 696e 6720  ue representing 
+00011890: 7468 6520 6861 7264 7374 6174 6520 6174  the hardstate at
+000118a0: 2074 6865 2074 696d 6520 6f66 2063 616c   the time of cal
+000118b0: 6c69 6e67 2e0a 2020 2020 2020 2020 2222  ling..        ""
+000118c0: 220a 2020 2020 6465 6620 7069 6e67 2873  ".    def ping(s
+000118d0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000118e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000118f0: 2020 4272 6f61 6463 6173 7473 2068 6561    Broadcasts hea
+00011900: 7274 6265 6174 7320 746f 2061 6c6c 2074  rtbeats to all t
+00011910: 6865 2066 6f6c 6c6f 7765 7273 2069 6620  he followers if 
+00011920: 6974 2773 206c 6561 6465 722e 0a20 2020  it's leader..   
+00011930: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00011940: 2074 6963 6b28 7365 6c66 2920 2d3e 2062   tick(self) -> b
+00011950: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00011960: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00011970: 2074 7275 6520 746f 2069 6e64 6963 6174   true to indicat
+00011980: 6520 7468 6174 2074 6865 7265 2077 696c  e that there wil
+00011990: 6c20 7072 6f62 6162 6c79 2062 6520 736f  l probably be so
+000119a0: 6d65 2072 6561 6469 6e65 7373 206e 6565  me readiness nee
+000119b0: 6420 746f 2062 6520 6861 6e64 6c65 642e  d to be handled.
+000119c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000119d0: 2064 6566 2074 6963 6b5f 656c 6563 7469   def tick_electi
+000119e0: 6f6e 2873 656c 6629 202d 3e20 626f 6f6c  on(self) -> bool
+000119f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00011a00: 2020 2020 2020 5275 6e20 6279 2066 6f6c        Run by fol
+00011a10: 6c6f 7765 7273 2061 6e64 2063 616e 6469  lowers and candi
+00011a20: 6461 7465 7320 6166 7465 7220 7365 6c66  dates after self
+00011a30: 2e65 6c65 6374 696f 6e5f 7469 6d65 6f75  .election_timeou
+00011a40: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
+00011a50: 726e 7320 7472 7565 2074 6f20 696e 6469  rns true to indi
+00011a60: 6361 7465 2074 6861 7420 7468 6572 6520  cate that there 
+00011a70: 7769 6c6c 2070 726f 6261 626c 7920 6265  will probably be
+00011a80: 2073 6f6d 6520 7265 6164 696e 6573 7320   some readiness 
+00011a90: 6e65 6564 2074 6f20 6265 2068 616e 646c  need to be handl
+00011aa0: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
+00011ab0: 2020 2020 6465 6620 7374 6570 2873 656c      def step(sel
+00011ac0: 662c 206d 7367 3a20 224d 6573 7361 6765  f, msg: "Message
+00011ad0: 2220 7c20 224d 6573 7361 6765 5265 6622  " | "MessageRef"
+00011ae0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00011af0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00011b00: 7465 7073 2074 6865 2072 6166 7420 616c  teps the raft al
+00011b10: 6f6e 6720 7669 6120 6120 6d65 7373 6167  ong via a messag
+00011b20: 652e 2054 6869 7320 7368 6f75 6c64 2062  e. This should b
+00011b30: 6520 6361 6c6c 6564 2065 7665 7279 7469  e called everyti
+00011b40: 6d65 2079 6f75 7220 7261 6674 2072 6563  me your raft rec
+00011b50: 6569 7665 7320 610a 2020 2020 2020 2020  eives a.        
+00011b60: 6d65 7373 6167 6520 6672 6f6d 2061 2070  message from a p
+00011b70: 6565 722e 0a20 2020 2020 2020 2022 2222  eer..        """
+00011b80: 0a20 2020 2064 6566 2068 6173 5f70 656e  .    def has_pen
+00011b90: 6469 6e67 5f63 6f6e 6628 7365 6c66 2920  ding_conf(self) 
+00011ba0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00011bb0: 2022 2222 0a20 2020 2020 2020 2043 6865   """.        Che
+00011bc0: 636b 2069 6620 7468 6572 6520 6973 2061  ck if there is a
+00011bd0: 6e79 2070 656e 6469 6e67 2063 6f6e 6663  ny pending confc
+00011be0: 6861 6e67 652e 0a0a 2020 2020 2020 2020  hange...        
+00011bf0: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
+00011c00: 6265 2066 616c 7365 2070 6f73 6974 6976  be false positiv
+00011c10: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00011c20: 2020 2064 6566 2070 726f 6d6f 7461 626c     def promotabl
+00011c30: 6528 7365 6c66 2920 2d3e 2062 6f6f 6c3a  e(self) -> bool:
+00011c40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011c50: 2020 2020 2049 6e64 6963 6174 6573 2077       Indicates w
+00011c60: 6865 7468 6572 2073 7461 7465 206d 6163  hether state mac
+00011c70: 6869 6e65 2063 616e 2062 6520 7072 6f6d  hine can be prom
+00011c80: 6f74 6564 2074 6f20 6c65 6164 6572 2c0a  oted to leader,.
+00011c90: 2020 2020 2020 2020 7768 6963 6820 6973          which is
+00011ca0: 2074 7275 6520 7768 656e 2069 7427 7320   true when it's 
+00011cb0: 6120 766f 7465 7220 616e 6420 6974 7320  a voter and its 
+00011cc0: 6f77 6e20 6964 2069 7320 696e 2070 726f  own id is in pro
+00011cd0: 6772 6573 7320 6c69 7374 2e0a 2020 2020  gress list..    
+00011ce0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00011cf0: 706f 7374 5f63 6f6e 665f 6368 616e 6765  post_conf_change
+00011d00: 2873 656c 6629 202d 3e20 2243 6f6e 6653  (self) -> "ConfS
+00011d10: 7461 7465 5265 6622 3a0a 2020 2020 2020  tateRef":.      
+00011d20: 2020 2222 220a 2020 2020 2020 2020 5570    """.        Up
+00011d30: 6461 7465 7320 7468 6520 696e 2d6d 656d  dates the in-mem
+00011d40: 6f72 7920 7374 6174 6520 616e 642c 2077  ory state and, w
+00011d50: 6865 6e20 6e65 6365 7373 6172 792c 2063  hen necessary, c
+00011d60: 6172 7269 6573 206f 7574 2061 6464 6974  arries out addit
+00011d70: 696f 6e61 6c20 6163 7469 6f6e 730a 2020  ional actions.  
+00011d80: 2020 2020 2020 7375 6368 2061 7320 7265        such as re
+00011d90: 6163 7469 6e67 2074 6f20 7468 6520 7265  acting to the re
+00011da0: 6d6f 7661 6c20 6f66 206e 6f64 6573 206f  moval of nodes o
+00011db0: 7220 6368 616e 6765 6420 7175 6f72 756d  r changed quorum
+00011dc0: 2072 6571 7569 7265 6d65 6e74 732e 0a20   requirements.. 
+00011dd0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00011de0: 6566 2069 6e5f 6c65 6173 6528 7365 6c66  ef in_lease(self
+00011df0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00011e00: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00011e10: 6574 7572 6e73 2077 6865 7468 6572 2074  eturns whether t
+00011e20: 6865 2063 7572 7265 6e74 2072 6166 7420  he current raft 
+00011e30: 6973 2069 6e20 6c65 6173 652e 0a20 2020  is in lease..   
+00011e40: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00011e50: 2068 616e 646c 655f 6865 6172 7462 6561   handle_heartbea
+00011e60: 7428 7365 6c66 2c20 6d73 673a 2022 4d65  t(self, msg: "Me
+00011e70: 7373 6167 6522 207c 2022 4d65 7373 6167  ssage" | "Messag
+00011e80: 6552 6566 2229 202d 3e20 4e6f 6e65 3a0a  eRef") -> None:.
+00011e90: 2020 2020 2020 2020 2222 2246 6f72 2061          """For a
+00011ea0: 206d 6573 7361 6765 2c20 636f 6d6d 6974   message, commit
+00011eb0: 2061 6e64 2073 656e 6420 6f75 7420 6865   and send out he
+00011ec0: 6172 7462 6561 742e 2222 220a 2020 2020  artbeat.""".    
+00011ed0: 6465 6620 6861 6e64 6c65 5f61 7070 656e  def handle_appen
+00011ee0: 645f 656e 7472 6965 7328 7365 6c66 2c20  d_entries(self, 
+00011ef0: 6d73 673a 2022 4d65 7373 6167 6522 207c  msg: "Message" |
+00011f00: 2022 4d65 7373 6167 6552 6566 2229 202d   "MessageRef") -
+00011f10: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00011f20: 2222 2246 6f72 2061 2067 6976 656e 206d  """For a given m
+00011f30: 6573 7361 6765 2c20 6170 7065 6e64 2074  essage, append t
+00011f40: 6865 2065 6e74 7269 6573 2074 6f20 7468  he entries to th
+00011f50: 6520 6c6f 672e 2222 220a 2020 2020 6465  e log.""".    de
+00011f60: 6620 7265 7175 6573 745f 736e 6170 7368  f request_snapsh
+00011f70: 6f74 2873 656c 6629 202d 3e20 4e6f 6e65  ot(self) -> None
+00011f80: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00011f90: 2020 2020 2020 5265 7175 6573 7420 6120        Request a 
+00011fa0: 736e 6170 7368 6f74 2066 726f 6d20 6120  snapshot from a 
+00011fb0: 6c65 6164 6572 2e0a 2020 2020 2020 2020  leader..        
+00011fc0: 2222 220a 2020 2020 6465 6620 7072 7328  """.    def prs(
+00011fd0: 7365 6c66 2920 2d3e 2022 5072 6f67 7265  self) -> "Progre
+00011fe0: 7373 5472 6163 6b65 7252 6566 223a 0a20  ssTrackerRef":. 
+00011ff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012000: 2020 2052 6574 7572 6e73 2061 2072 6561     Returns a rea
+00012010: 642d 6f6e 6c79 2072 6566 6572 656e 6365  d-only reference
+00012020: 2074 6f20 7468 6520 7072 6f67 7265 7373   to the progress
+00012030: 2073 6574 2e0a 2020 2020 2020 2020 2222   set..        ""
+00012040: 220a 2020 2020 6465 6620 7265 7365 7428  ".    def reset(
+00012050: 7365 6c66 2c20 7465 726d 3a20 696e 7429  self, term: int)
+00012060: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00012070: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+00012080: 7365 7473 2074 6865 2063 7572 7265 6e74  sets the current
+00012090: 206e 6f64 6520 746f 2061 2067 6976 656e   node to a given
+000120a0: 2074 6572 6d2e 0a20 2020 2020 2020 2022   term..        "
+000120b0: 2222 0a20 2020 2064 6566 2072 6573 746f  "".    def resto
+000120c0: 7265 2873 656c 662c 2073 6e61 7073 686f  re(self, snapsho
+000120d0: 743a 2022 536e 6170 7368 6f74 2220 7c20  t: "Snapshot" | 
+000120e0: 2253 6e61 7073 686f 7452 6566 2229 202d  "SnapshotRef") -
+000120f0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00012100: 2222 220a 2020 2020 2020 2020 5265 636f  """.        Reco
+00012110: 7665 7273 2074 6865 2073 7461 7465 206d  vers the state m
+00012120: 6163 6869 6e65 2066 726f 6d20 6120 736e  achine from a sn
+00012130: 6170 7368 6f74 2e20 4974 2072 6573 746f  apshot. It resto
+00012140: 7265 7320 7468 6520 6c6f 6720 616e 6420  res the log and 
+00012150: 7468 650a 2020 2020 2020 2020 636f 6e66  the.        conf
+00012160: 6967 7572 6174 696f 6e20 6f66 2073 7461  iguration of sta
+00012170: 7465 206d 6163 6869 6e65 2e0a 2020 2020  te machine..    
+00012180: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00012190: 736e 6170 2873 656c 6629 202d 3e20 4f70  snap(self) -> Op
+000121a0: 7469 6f6e 616c 5b22 536e 6170 7368 6f74  tional["Snapshot
+000121b0: 5265 6622 5d3a 0a20 2020 2020 2020 2022  Ref"]:.        "
+000121c0: 2222 0a20 2020 2020 2020 2047 7261 6273  "".        Grabs
+000121d0: 2061 2072 6566 6572 656e 6365 2074 6f20   a reference to 
+000121e0: 7468 6520 736e 6170 7368 6f74 0a20 2020  the snapshot.   
+000121f0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00012200: 2073 746f 7265 2873 656c 6629 202d 3e20   store(self) -> 
+00012210: 224d 656d 5374 6f72 6167 6552 6566 223a  "MemStorageRef":
+00012220: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012230: 2020 2020 2047 7261 6273 2061 6e20 696d       Grabs an im
+00012240: 6d75 7461 626c 6520 7265 6665 7265 6e63  mutable referenc
+00012250: 6520 746f 2074 6865 2073 746f 7265 2e0a  e to the store..
+00012260: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012270: 6465 6620 6f6e 5f70 6572 7369 7374 5f73  def on_persist_s
+00012280: 6e61 7028 7365 6c66 2c20 696e 6465 783a  nap(self, index:
+00012290: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+000122a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000122b0: 2020 204e 6f74 6966 6965 7320 7468 6174     Notifies that
+000122c0: 2074 6865 2073 6e61 7073 686f 7420 6861   the snapshot ha
+000122d0: 7665 2062 6565 6e20 7065 7273 6973 7465  ve been persiste
+000122e0: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
+000122f0: 2020 2064 6566 2061 626f 7274 5f6c 6561     def abort_lea
+00012300: 6465 725f 7472 616e 7366 6572 2873 656c  der_transfer(sel
+00012310: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00012320: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012330: 5374 6f70 7320 7468 6520 7472 616e 7366  Stops the transf
+00012340: 6572 206f 6620 6120 6c65 6164 6572 2e0a  er of a leader..
+00012350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012360: 6465 6620 6361 6d70 6169 676e 2873 656c  def campaign(sel
+00012370: 662c 2074 7970 3a20 7374 7229 202d 3e20  f, typ: str) -> 
+00012380: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00012390: 220a 2020 2020 2020 2020 4361 6d70 6169  ".        Campai
+000123a0: 676e 2074 6f20 6174 7465 6d70 7420 746f  gn to attempt to
+000123b0: 2062 6563 6f6d 6520 6120 6c65 6164 6572   become a leader
+000123c0: 2e0a 0a20 2020 2020 2020 2049 6620 7072  ...        If pr
+000123d0: 6576 6f74 6520 6973 2065 6e61 626c 6564  evote is enabled
+000123e0: 2c20 7468 6973 2069 7320 6861 6e64 6c65  , this is handle
+000123f0: 6420 6173 2077 656c 6c2e 0a20 2020 2020  d as well..     
+00012400: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00012410: 6574 5f6c 6561 645f 7472 616e 7366 6572  et_lead_transfer
+00012420: 6565 2873 656c 6629 202d 3e20 4f70 7469  ee(self) -> Opti
+00012430: 6f6e 616c 5b69 6e74 5d3a 0a20 2020 2020  onal[int]:.     
+00012440: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00012450: 6c65 6164 5f74 7261 6e73 6665 7265 6560  lead_transferee`
+00012460: 3a20 4944 206f 6620 7468 6520 6c65 6164  : ID of the lead
+00012470: 6572 2074 7261 6e73 6665 7220 7461 7267  er transfer targ
+00012480: 6574 2077 6865 6e20 6974 7320 7661 6c75  et when its valu
+00012490: 6520 6973 206e 6f74 204e 6f6e 652e 0a0a  e is not None...
+000124a0: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
+000124b0: 6973 2053 6f6d 6528 6964 292c 2077 6520  is Some(id), we 
+000124c0: 666f 6c6c 6f77 2074 6865 2070 726f 6365  follow the proce
+000124d0: 6475 7265 2064 6566 696e 6564 2069 6e20  dure defined in 
+000124e0: 7261 6674 2074 6865 7369 7320 332e 3130  raft thesis 3.10
+000124f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00012500: 2020 6465 6620 7365 745f 6c65 6164 5f74    def set_lead_t
+00012510: 7261 6e73 6665 7265 6528 7365 6c66 2c20  ransferee(self, 
+00012520: 6c65 6164 5f74 7261 6e73 6665 7265 653a  lead_transferee:
+00012530: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00012540: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012550: 2020 2060 6c65 6164 5f74 7261 6e73 6665     `lead_transfe
+00012560: 7265 6560 3a20 4944 206f 6620 7468 6520  ree`: ID of the 
+00012570: 6c65 6164 6572 2074 7261 6e73 6665 7220  leader transfer 
+00012580: 7461 7267 6574 2077 6865 6e20 6974 7320  target when its 
+00012590: 7661 6c75 6520 6973 206e 6f74 204e 6f6e  value is not Non
+000125a0: 652e 0a0a 2020 2020 2020 2020 4966 2074  e...        If t
+000125b0: 6869 7320 6973 2053 6f6d 6528 6964 292c  his is Some(id),
+000125c0: 2077 6520 666f 6c6c 6f77 2074 6865 2070   we follow the p
+000125d0: 726f 6365 6475 7265 2064 6566 696e 6564  rocedure defined
+000125e0: 2069 6e20 7261 6674 2074 6865 7369 7320   in raft thesis 
+000125f0: 332e 3130 2e0a 2020 2020 2020 2020 2222  3.10..        ""
+00012600: 220a 2020 2020 6465 6620 6765 745f 7465  ".    def get_te
+00012610: 726d 2873 656c 6629 202d 3e20 696e 743a  rm(self) -> int:
+00012620: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012630: 2020 2020 2060 7465 726d 603a 2054 6865       `term`: The
+00012640: 2063 7572 7265 6e74 2065 6c65 6374 696f   current electio
+00012650: 6e20 7465 726d 2e0a 2020 2020 2020 2020  n term..        
+00012660: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00012670: 7465 726d 2873 656c 662c 2074 6572 6d3a  term(self, term:
+00012680: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+00012690: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000126a0: 2020 2060 7465 726d 603a 2054 6865 2063     `term`: The c
+000126b0: 7572 7265 6e74 2065 6c65 6374 696f 6e20  urrent election 
+000126c0: 7465 726d 2e0a 2020 2020 2020 2020 2222  term..        ""
+000126d0: 220a 2020 2020 6465 6620 6765 745f 766f  ".    def get_vo
+000126e0: 7465 2873 656c 6629 202d 3e20 696e 743a  te(self) -> int:
+000126f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012700: 2020 2020 2060 766f 7465 603a 2057 6869       `vote`: Whi
+00012710: 6368 2070 6565 7220 7468 6973 2072 6166  ch peer this raf
+00012720: 7420 6973 2076 6f74 696e 6720 666f 722e  t is voting for.
+00012730: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012740: 2064 6566 2073 6574 5f76 6f74 6528 7365   def set_vote(se
+00012750: 6c66 2c20 766f 7465 3a20 696e 7429 202d  lf, vote: int) -
+00012760: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00012770: 2222 220a 2020 2020 2020 2020 6076 6f74  """.        `vot
+00012780: 6560 3a20 5768 6963 6820 7065 6572 2074  e`: Which peer t
+00012790: 6869 7320 7261 6674 2069 7320 766f 7469  his raft is voti
+000127a0: 6e67 2066 6f72 2e0a 2020 2020 2020 2020  ng for..        
+000127b0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+000127c0: 7072 696f 7269 7479 2873 656c 6629 202d  priority(self) -
+000127d0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+000127e0: 2222 0a20 2020 2020 2020 2060 7072 696f  "".        `prio
+000127f0: 7269 7479 603a 2054 6865 2065 6c65 6374  rity`: The elect
+00012800: 696f 6e20 7072 696f 7269 7479 206f 6620  ion priority of 
+00012810: 7468 6973 206e 6f64 652e 0a20 2020 2020  this node..     
+00012820: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
+00012830: 6574 5f70 7269 6f72 6974 7928 7365 6c66  et_priority(self
+00012840: 2c20 7072 696f 7269 7479 3a20 696e 7429  , priority: int)
+00012850: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00012860: 2020 2222 220a 2020 2020 2020 2020 6070    """.        `p
+00012870: 7269 6f72 6974 7960 3a20 5468 6520 656c  riority`: The el
+00012880: 6563 7469 6f6e 2070 7269 6f72 6974 7920  ection priority 
+00012890: 6f66 2074 6869 7320 6e6f 6465 2e0a 2020  of this node..  
+000128a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+000128b0: 6620 6765 745f 6c65 6164 6572 5f69 6428  f get_leader_id(
+000128c0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+000128d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000128e0: 2020 606c 6561 6465 725f 6964 603a 2054    `leader_id`: T
+000128f0: 6865 206c 6561 6465 7220 6964 0a20 2020  he leader id.   
+00012900: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00012910: 2073 6574 5f6c 6561 6465 725f 6964 2873   set_leader_id(s
+00012920: 656c 662c 206c 6561 6465 725f 6964 3a20  elf, leader_id: 
+00012930: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00012940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012950: 2020 606c 6561 6465 725f 6964 603a 2054    `leader_id`: T
+00012960: 6865 206c 6561 6465 7220 6964 0a20 2020  he leader id.   
+00012970: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00012980: 2067 6574 5f6d 6178 5f6d 7367 5f73 697a   get_max_msg_siz
+00012990: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0a  e(self) -> int:.
+000129a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000129b0: 2020 2020 606d 6178 5f6d 7367 5f73 697a      `max_msg_siz
+000129c0: 6560 3a20 5468 6520 6d61 7869 6d75 6d20  e`: The maximum 
+000129d0: 6c65 6e67 7468 2028 696e 2062 7974 6573  length (in bytes
+000129e0: 2920 6f66 2061 6c6c 2074 6865 2065 6e74  ) of all the ent
+000129f0: 7269 6573 2e0a 2020 2020 2020 2020 2222  ries..        ""
+00012a00: 220a 2020 2020 6465 6620 7365 745f 6d61  ".    def set_ma
+00012a10: 785f 6d73 675f 7369 7a65 2873 656c 662c  x_msg_size(self,
+00012a20: 206d 6178 5f6d 7367 5f73 697a 653a 2069   max_msg_size: i
+00012a30: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00012a40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012a50: 2060 6d61 785f 6d73 675f 7369 7a65 603a   `max_msg_size`:
+00012a60: 2054 6865 206d 6178 696d 756d 206c 656e   The maximum len
+00012a70: 6774 6820 2869 6e20 6279 7465 7329 206f  gth (in bytes) o
+00012a80: 6620 616c 6c20 7468 6520 656e 7472 6965  f all the entrie
+00012a90: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00012aa0: 2020 2064 6566 2067 6574 5f70 656e 6469     def get_pendi
+00012ab0: 6e67 5f63 6f6e 665f 696e 6465 7828 7365  ng_conf_index(se
+00012ac0: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00012ad0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012ae0: 6070 656e 6469 6e67 5f63 6f6e 665f 696e  `pending_conf_in
+00012af0: 6465 7860 3a20 4f6e 6c79 206f 6e65 2063  dex`: Only one c
+00012b00: 6f6e 6620 6368 616e 6765 206d 6179 2062  onf change may b
+00012b10: 6520 7065 6e64 696e 6720 2869 6e20 7468  e pending (in th
+00012b20: 6520 6c6f 672c 2062 7574 206e 6f74 2079  e log, but not y
+00012b30: 6574 0a20 2020 2020 2020 2061 7070 6c69  et.        appli
+00012b40: 6564 2920 6174 2061 2074 696d 652e 2054  ed) at a time. T
+00012b50: 6869 7320 6973 2065 6e66 6f72 6365 6420  his is enforced 
+00012b60: 7669 6120 6070 656e 6469 6e67 5f63 6f6e  via `pending_con
+00012b70: 665f 696e 6465 7860 2c20 7768 6963 680a  f_index`, which.
+00012b80: 2020 2020 2020 2020 6973 2073 6574 2074          is set t
+00012b90: 6f20 6120 7661 6c75 6520 3e3d 2074 6865  o a value >= the
+00012ba0: 206c 6f67 2069 6e64 6578 206f 6620 7468   log index of th
+00012bb0: 6520 6c61 7465 7374 2070 656e 6469 6e67  e latest pending
+00012bc0: 0a20 2020 2020 2020 2063 6f6e 6669 6775  .        configu
+00012bd0: 7261 7469 6f6e 2063 6861 6e67 6520 2869  ration change (i
+00012be0: 6620 616e 7929 2e20 436f 6e66 6967 2063  f any). Config c
+00012bf0: 6861 6e67 6573 2061 7265 206f 6e6c 7920  hanges are only 
+00012c00: 616c 6c6f 7765 6420 746f 0a20 2020 2020  allowed to.     
+00012c10: 2020 2062 6520 7072 6f70 6f73 6564 2069     be proposed i
+00012c20: 6620 7468 6520 6c65 6164 6572 2773 2061  f the leader's a
+00012c30: 7070 6c69 6564 2069 6e64 6578 2069 7320  pplied index is 
+00012c40: 6772 6561 7465 7220 7468 616e 2074 6869  greater than thi
+00012c50: 730a 2020 2020 2020 2020 7661 6c75 652e  s.        value.
+00012c60: 0a0a 2020 2020 2020 2020 5468 6973 2076  ..        This v
+00012c70: 616c 7565 2069 7320 636f 6e73 6572 7661  alue is conserva
+00012c80: 7469 7665 6c79 2073 6574 2069 6e20 6361  tively set in ca
+00012c90: 7365 7320 7768 6572 6520 7468 6572 6520  ses where there 
+00012ca0: 6d61 7920 6265 2061 2063 6f6e 6669 6775  may be a configu
+00012cb0: 7261 7469 6f6e 2063 6861 6e67 6520 7065  ration change pe
+00012cc0: 6e64 696e 672c 0a20 2020 2020 2020 2062  nding,.        b
+00012cd0: 7574 2073 6361 6e6e 696e 6720 7468 6520  ut scanning the 
+00012ce0: 6c6f 6720 6973 2070 6f73 7369 626c 7920  log is possibly 
+00012cf0: 6578 7065 6e73 6976 652e 2054 6869 7320  expensive. This 
+00012d00: 696d 706c 6965 7320 7468 6174 2074 6865  implies that the
+00012d10: 2069 6e64 6578 2073 7461 7465 6420 6865   index stated he
+00012d20: 7265 206d 6179 206e 6f74 0a20 2020 2020  re may not.     
+00012d30: 2020 206e 6563 6573 7361 7269 6c79 2062     necessarily b
+00012d40: 6520 6120 636f 6e66 6967 2063 6861 6e67  e a config chang
+00012d50: 6520 656e 7472 792c 2061 6e64 2069 7420  e entry, and it 
+00012d60: 6d61 7920 6e6f 7420 6265 2061 2060 4265  may not be a `Be
+00012d70: 6769 6e4d 656d 6265 7273 6869 7043 6861  ginMembershipCha
+00012d80: 6e67 6560 2065 6e74 7279 2c20 6576 656e  nge` entry, even
+00012d90: 2069 660a 2020 2020 2020 2020 7765 2073   if.        we s
+00012da0: 6574 2074 6869 7320 746f 206f 6e65 2e0a  et this to one..
+00012db0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012dc0: 6465 6620 7365 745f 7065 6e64 696e 675f  def set_pending_
+00012dd0: 636f 6e66 5f69 6e64 6578 2873 656c 662c  conf_index(self,
+00012de0: 2070 656e 6469 6e67 5f63 6f6e 665f 696e   pending_conf_in
+00012df0: 6465 783a 2069 6e74 2920 2d3e 204e 6f6e  dex: int) -> Non
+00012e00: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00012e10: 2020 2020 2020 2060 7065 6e64 696e 675f         `pending_
+00012e20: 636f 6e66 5f69 6e64 6578 603a 204f 6e6c  conf_index`: Onl
+00012e30: 7920 6f6e 6520 636f 6e66 2063 6861 6e67  y one conf chang
+00012e40: 6520 6d61 7920 6265 2070 656e 6469 6e67  e may be pending
+00012e50: 2028 696e 2074 6865 206c 6f67 2c20 6275   (in the log, bu
+00012e60: 7420 6e6f 7420 7965 740a 2020 2020 2020  t not yet.      
+00012e70: 2020 6170 706c 6965 6429 2061 7420 6120    applied) at a 
+00012e80: 7469 6d65 2e20 5468 6973 2069 7320 656e  time. This is en
+00012e90: 666f 7263 6564 2076 6961 2060 7065 6e64  forced via `pend
+00012ea0: 696e 675f 636f 6e66 5f69 6e64 6578 602c  ing_conf_index`,
+00012eb0: 2077 6869 6368 0a20 2020 2020 2020 2069   which.        i
+00012ec0: 7320 7365 7420 746f 2061 2076 616c 7565  s set to a value
+00012ed0: 203e 3d20 7468 6520 6c6f 6720 696e 6465   >= the log inde
+00012ee0: 7820 6f66 2074 6865 206c 6174 6573 7420  x of the latest 
+00012ef0: 7065 6e64 696e 670a 2020 2020 2020 2020  pending.        
+00012f00: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
+00012f10: 616e 6765 2028 6966 2061 6e79 292e 2043  ange (if any). C
+00012f20: 6f6e 6669 6720 6368 616e 6765 7320 6172  onfig changes ar
+00012f30: 6520 6f6e 6c79 2061 6c6c 6f77 6564 2074  e only allowed t
+00012f40: 6f0a 2020 2020 2020 2020 6265 2070 726f  o.        be pro
+00012f50: 706f 7365 6420 6966 2074 6865 206c 6561  posed if the lea
+00012f60: 6465 7227 7320 6170 706c 6965 6420 696e  der's applied in
+00012f70: 6465 7820 6973 2067 7265 6174 6572 2074  dex is greater t
+00012f80: 6861 6e20 7468 6973 0a20 2020 2020 2020  han this.       
+00012f90: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+00012fa0: 2054 6869 7320 7661 6c75 6520 6973 2063   This value is c
+00012fb0: 6f6e 7365 7276 6174 6976 656c 7920 7365  onservatively se
+00012fc0: 7420 696e 2063 6173 6573 2077 6865 7265  t in cases where
+00012fd0: 2074 6865 7265 206d 6179 2062 6520 6120   there may be a 
+00012fe0: 636f 6e66 6967 7572 6174 696f 6e20 6368  configuration ch
+00012ff0: 616e 6765 2070 656e 6469 6e67 2c0a 2020  ange pending,.  
+00013000: 2020 2020 2020 6275 7420 7363 616e 6e69        but scanni
+00013010: 6e67 2074 6865 206c 6f67 2069 7320 706f  ng the log is po
+00013020: 7373 6962 6c79 2065 7870 656e 7369 7665  ssibly expensive
+00013030: 2e20 5468 6973 2069 6d70 6c69 6573 2074  . This implies t
+00013040: 6861 7420 7468 6520 696e 6465 7820 7374  hat the index st
+00013050: 6174 6564 2068 6572 6520 6d61 7920 6e6f  ated here may no
+00013060: 740a 2020 2020 2020 2020 6e65 6365 7373  t.        necess
+00013070: 6172 696c 7920 6265 2061 2063 6f6e 6669  arily be a confi
+00013080: 6720 6368 616e 6765 2065 6e74 7279 2c20  g change entry, 
+00013090: 616e 6420 6974 206d 6179 206e 6f74 2062  and it may not b
+000130a0: 6520 6120 6042 6567 696e 4d65 6d62 6572  e a `BeginMember
+000130b0: 7368 6970 4368 616e 6765 6020 656e 7472  shipChange` entr
+000130c0: 792c 2065 7665 6e20 6966 0a20 2020 2020  y, even if.     
+000130d0: 2020 2077 6520 7365 7420 7468 6973 2074     we set this t
+000130e0: 6f20 6f6e 652e 0a20 2020 2020 2020 2022  o one..        "
+000130f0: 2222 0a20 2020 2064 6566 2067 6574 5f70  "".    def get_p
+00013100: 656e 6469 6e67 5f72 6571 7565 7374 5f73  ending_request_s
+00013110: 6e61 7073 686f 7428 7365 6c66 2920 2d3e  napshot(self) ->
+00013120: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00013130: 220a 2020 2020 2020 2020 6070 656e 6469  ".        `pendi
+00013140: 6e67 5f72 6571 7565 7374 5f73 6e61 7073  ng_request_snaps
+00013150: 686f 7460 3a20 5468 6520 7065 6572 2069  hot`: The peer i
+00013160: 7320 7265 7175 6573 7469 6e67 2073 6e61  s requesting sna
+00013170: 7073 686f 742c 2069 7420 6973 2074 6865  pshot, it is the
+00013180: 2069 6e64 6578 2074 6861 7420 7468 6520   index that the 
+00013190: 666f 6c6c 6f77 6572 0a20 2020 2020 2020  follower.       
+000131a0: 206e 6565 6473 2069 7420 746f 2062 6520   needs it to be 
+000131b0: 696e 636c 7564 6564 2069 6e20 6120 736e  included in a sn
+000131c0: 6170 7368 6f74 2e0a 2020 2020 2020 2020  apshot..        
+000131d0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+000131e0: 7065 6e64 696e 675f 7265 7175 6573 745f  pending_request_
+000131f0: 736e 6170 7368 6f74 2873 656c 662c 2070  snapshot(self, p
+00013200: 656e 6469 6e67 5f72 6571 7565 7374 5f73  ending_request_s
+00013210: 6e61 7073 686f 743a 2069 6e74 2920 2d3e  napshot: int) ->
+00013220: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00013230: 2222 0a20 2020 2020 2020 2060 7065 6e64  "".        `pend
+00013240: 696e 675f 7265 7175 6573 745f 736e 6170  ing_request_snap
+00013250: 7368 6f74 603a 2054 6865 2070 6565 7220  shot`: The peer 
+00013260: 6973 2072 6571 7565 7374 696e 6720 736e  is requesting sn
+00013270: 6170 7368 6f74 2c20 6974 2069 7320 7468  apshot, it is th
+00013280: 6520 696e 6465 7820 7468 6174 2074 6865  e index that the
+00013290: 2066 6f6c 6c6f 7765 720a 2020 2020 2020   follower.      
+000132a0: 2020 6e65 6564 7320 6974 2074 6f20 6265    needs it to be
+000132b0: 2069 6e63 6c75 6465 6420 696e 2061 2073   included in a s
+000132c0: 6e61 7073 686f 742e 0a20 2020 2020 2020  napshot..       
+000132d0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+000132e0: 5f69 6428 7365 6c66 2920 2d3e 2069 6e74  _id(self) -> int
+000132f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013300: 2020 2020 2020 6069 6460 3a20 5468 6520        `id`: The 
+00013310: 4944 206f 6620 7468 6973 206e 6f64 652e  ID of this node.
 00013320: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013330: 2020 2020 2060 6d73 6773 603a 2054 6865       `msgs`: The
-00013340: 206c 6973 7420 6f66 206d 6573 7361 6765   list of message
-00013350: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00013360: 2020 2064 6566 2073 6574 5f6d 7367 7328     def set_msgs(
-00013370: 7365 6c66 2c20 6d73 6773 3a20 4c69 7374  self, msgs: List
-00013380: 5b22 4d65 7373 6167 6522 207c 2022 4d65  ["Message" | "Me
-00013390: 7373 6167 6552 6566 225d 2920 2d3e 204e  ssageRef"]) -> N
-000133a0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000133b0: 0a20 2020 2020 2020 2060 6d73 6773 603a  .        `msgs`:
-000133c0: 2054 6865 206c 6973 7420 6f66 206d 6573   The list of mes
-000133d0: 7361 6765 732e 0a20 2020 2020 2020 2022  sages..        "
-000133e0: 2222 0a20 2020 2064 6566 2074 616b 655f  "".    def take_
-000133f0: 6d73 6773 2873 656c 6629 202d 3e20 4c69  msgs(self) -> Li
-00013400: 7374 5b22 4d65 7373 6167 6522 5d3a 0a20  st["Message"]:. 
-00013410: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013420: 2020 2060 6d73 6773 603a 2054 6865 206c     `msgs`: The l
-00013430: 6973 7420 6f66 206d 6573 7361 6765 732e  ist of messages.
+00013330: 2064 6566 2073 6574 5f69 6428 7365 6c66   def set_id(self
+00013340: 2c20 6964 3a20 696e 7429 202d 3e20 4e6f  , id: int) -> No
+00013350: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00013360: 2020 2020 2020 2020 6069 6460 3a20 5468          `id`: Th
+00013370: 6520 4944 206f 6620 7468 6973 206e 6f64  e ID of this nod
+00013380: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00013390: 2020 2064 6566 2067 6574 5f6d 7367 7328     def get_msgs(
+000133a0: 7365 6c66 2920 2d3e 204c 6973 745b 224d  self) -> List["M
+000133b0: 6573 7361 6765 5265 6622 5d3a 0a20 2020  essageRef"]:.   
+000133c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000133d0: 2060 6d73 6773 603a 2054 6865 206c 6973   `msgs`: The lis
+000133e0: 7420 6f66 206d 6573 7361 6765 732e 0a20  t of messages.. 
+000133f0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00013400: 6566 2073 6574 5f6d 7367 7328 7365 6c66  ef set_msgs(self
+00013410: 2c20 6d73 6773 3a20 4c69 7374 5b22 4d65  , msgs: List["Me
+00013420: 7373 6167 6522 207c 2022 4d65 7373 6167  ssage" | "Messag
+00013430: 6552 6566 225d 2920 2d3e 204e 6f6e 653a  eRef"]) -> None:
 00013440: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013450: 2064 6566 2067 6574 5f6d 6178 5f69 6e66   def get_max_inf
-00013460: 6c69 6768 7428 7365 6c66 2920 2d3e 2069  light(self) -> i
-00013470: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-00013480: 2020 2020 2020 2020 606d 6178 5f69 6e66          `max_inf
-00013490: 6c69 6768 7460 3a20 5468 6520 6d61 7869  light`: The maxi
-000134a0: 6d75 6d20 6e75 6d62 6572 206f 6620 6d65  mum number of me
-000134b0: 7373 6167 6573 2074 6861 7420 6361 6e20  ssages that can 
-000134c0: 6265 2069 6e66 6c69 6768 742e 0a20 2020  be inflight..   
-000134d0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-000134e0: 2073 6574 5f6d 6178 5f69 6e66 6c69 6768   set_max_infligh
-000134f0: 7428 7365 6c66 2c20 6d61 785f 696e 666c  t(self, max_infl
-00013500: 6967 6874 3a20 696e 7429 202d 3e20 4e6f  ight: int) -> No
-00013510: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00013520: 2020 2020 2020 2020 606d 6178 5f69 6e66          `max_inf
-00013530: 6c69 6768 7460 3a20 5468 6520 6d61 7869  light`: The maxi
-00013540: 6d75 6d20 6e75 6d62 6572 206f 6620 6d65  mum number of me
-00013550: 7373 6167 6573 2074 6861 7420 6361 6e20  ssages that can 
-00013560: 6265 2069 6e66 6c69 6768 742e 0a20 2020  be inflight..   
-00013570: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00013580: 2067 6574 5f73 7461 7465 2873 656c 6629   get_state(self)
-00013590: 202d 3e20 2253 7461 7465 526f 6c65 223a   -> "StateRole":
-000135a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000135b0: 2020 2020 2060 7374 6174 6560 3a20 5468       `state`: Th
-000135c0: 6520 6375 7272 656e 7420 726f 6c65 206f  e current role o
-000135d0: 6620 7468 6973 206e 6f64 652e 0a20 2020  f this node..   
-000135e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-000135f0: 2073 6574 5f73 7461 7465 2873 656c 662c   set_state(self,
-00013600: 2073 7461 7465 5f72 6f6c 653a 2022 5374   state_role: "St
-00013610: 6174 6552 6f6c 6522 2920 2d3e 204e 6f6e  ateRole") -> Non
-00013620: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00013630: 2020 2020 2020 2060 7374 6174 6560 3a20         `state`: 
-00013640: 5468 6520 6375 7272 656e 7420 726f 6c65  The current role
-00013650: 206f 6620 7468 6973 206e 6f64 652e 0a20   of this node.. 
-00013660: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00013670: 6566 2067 6574 5f65 6c65 6374 696f 6e5f  ef get_election_
-00013680: 656c 6170 7365 6428 7365 6c66 2920 2d3e  elapsed(self) ->
-00013690: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-000136a0: 220a 2020 2020 2020 2020 6065 6c65 6374  ".        `elect
-000136b0: 696f 6e5f 656c 6170 7365 6460 3a20 5469  ion_elapsed`: Ti
-000136c0: 636b 7320 7369 6e63 6520 6974 2072 6561  cks since it rea
-000136d0: 6368 6564 206c 6173 7420 656c 6563 7469  ched last electi
-000136e0: 6f6e 5469 6d65 6f75 7420 7768 656e 2069  onTimeout when i
-000136f0: 7420 6973 206c 6561 6465 7220 6f72 2063  t is leader or c
-00013700: 616e 6469 6461 7465 2e0a 2020 2020 2020  andidate..      
-00013710: 2020 4e75 6d62 6572 206f 6620 7469 636b    Number of tick
-00013720: 7320 7369 6e63 6520 6974 2072 6561 6368  s since it reach
-00013730: 6564 206c 6173 7420 656c 6563 7469 6f6e  ed last election
-00013740: 5469 6d65 6f75 7420 6f72 2072 6563 6569  Timeout or recei
-00013750: 7665 6420 610a 2020 2020 2020 2020 7661  ved a.        va
-00013760: 6c69 6420 6d65 7373 6167 6520 6672 6f6d  lid message from
-00013770: 2063 7572 7265 6e74 206c 6561 6465 7220   current leader 
-00013780: 7768 656e 2069 7420 6973 2061 2066 6f6c  when it is a fol
-00013790: 6c6f 7765 722e 0a20 2020 2020 2020 2022  lower..        "
-000137a0: 2222 0a20 2020 2064 6566 2073 6574 5f65  "".    def set_e
-000137b0: 6c65 6374 696f 6e5f 656c 6170 7365 6428  lection_elapsed(
-000137c0: 7365 6c66 2c20 656c 6563 7469 6f6e 5f65  self, election_e
-000137d0: 6c61 7073 6564 3a20 696e 7429 202d 3e20  lapsed: int) -> 
-000137e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000137f0: 220a 2020 2020 2020 2020 6065 6c65 6374  ".        `elect
-00013800: 696f 6e5f 656c 6170 7365 6460 3a20 5469  ion_elapsed`: Ti
-00013810: 636b 7320 7369 6e63 6520 6974 2072 6561  cks since it rea
-00013820: 6368 6564 206c 6173 7420 656c 6563 7469  ched last electi
-00013830: 6f6e 5469 6d65 6f75 7420 7768 656e 2069  onTimeout when i
-00013840: 7420 6973 206c 6561 6465 7220 6f72 2063  t is leader or c
-00013850: 616e 6469 6461 7465 2e0a 2020 2020 2020  andidate..      
-00013860: 2020 4e75 6d62 6572 206f 6620 7469 636b    Number of tick
-00013870: 7320 7369 6e63 6520 6974 2072 6561 6368  s since it reach
-00013880: 6564 206c 6173 7420 656c 6563 7469 6f6e  ed last election
-00013890: 5469 6d65 6f75 7420 6f72 2072 6563 6569  Timeout or recei
-000138a0: 7665 6420 610a 2020 2020 2020 2020 7661  ved a.        va
-000138b0: 6c69 6420 6d65 7373 6167 6520 6672 6f6d  lid message from
-000138c0: 2063 7572 7265 6e74 206c 6561 6465 7220   current leader 
-000138d0: 7768 656e 2069 7420 6973 2061 2066 6f6c  when it is a fol
-000138e0: 6c6f 7765 722e 0a20 2020 2020 2020 2022  lower..        "
-000138f0: 2222 0a20 2020 2064 6566 2067 6574 5f63  "".    def get_c
-00013900: 6865 636b 5f71 756f 7275 6d28 7365 6c66  heck_quorum(self
-00013910: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00013920: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00013930: 6368 6563 6b5f 7175 6f72 756d 603a 2057  check_quorum`: W
-00013940: 6865 7468 6572 2074 6f20 6368 6563 6b20  hether to check 
-00013950: 7468 6520 7175 6f72 756d 0a20 2020 2020  the quorum.     
-00013960: 2020 2022 2222 0a20 2020 2064 6566 2073     """.    def s
-00013970: 6574 5f63 6865 636b 5f71 756f 7275 6d28  et_check_quorum(
-00013980: 7365 6c66 2c20 6368 6563 6b5f 7175 6f72  self, check_quor
-00013990: 756d 3a20 626f 6f6c 2920 2d3e 204e 6f6e  um: bool) -> Non
-000139a0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000139b0: 2020 2020 2020 2060 6368 6563 6b5f 7175         `check_qu
-000139c0: 6f72 756d 603a 2057 6865 7468 6572 2074  orum`: Whether t
-000139d0: 6f20 6368 6563 6b20 7468 6520 7175 6f72  o check the quor
-000139e0: 756d 0a20 2020 2020 2020 2022 2222 0a20  um.        """. 
-000139f0: 2020 2064 6566 2067 6574 5f70 7265 5f76     def get_pre_v
-00013a00: 6f74 6528 7365 6c66 2920 2d3e 2062 6f6f  ote(self) -> boo
-00013a10: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-00013a20: 2020 2020 2020 2060 7072 655f 766f 7465         `pre_vote
-00013a30: 603a 2045 6e61 626c 6520 7468 6520 7072  `: Enable the pr
-00013a40: 6576 6f74 6520 616c 676f 7269 7468 6d2e  evote algorithm.
-00013a50: 0a0a 2020 2020 2020 2020 5468 6973 2065  ..        This e
-00013a60: 6e61 626c 6573 2061 2070 7265 2d65 6c65  nables a pre-ele
-00013a70: 6374 696f 6e20 766f 7465 2072 6f75 6e64  ction vote round
-00013a80: 206f 6e20 4361 6e64 6964 6174 6573 2070   on Candidates p
-00013a90: 7269 6f72 2074 6f20 6469 7372 7570 7469  rior to disrupti
-00013aa0: 6e67 2074 6865 2063 6c75 7374 6572 2e0a  ng the cluster..
-00013ab0: 0a20 2020 2020 2020 2045 6e61 626c 6520  .        Enable 
-00013ac0: 7468 6973 2069 6620 6772 6561 7465 7220  this if greater 
-00013ad0: 636c 7573 7465 7220 7374 6162 696c 6974  cluster stabilit
-00013ae0: 7920 6973 2070 7265 6665 7272 6564 206f  y is preferred o
-00013af0: 7665 7220 6661 7374 6572 2065 6c65 6374  ver faster elect
-00013b00: 696f 6e73 2e0a 2020 2020 2020 2020 2222  ions..        ""
-00013b10: 220a 2020 2020 6465 6620 7365 745f 7072  ".    def set_pr
-00013b20: 655f 766f 7465 2873 656c 662c 2070 7265  e_vote(self, pre
-00013b30: 5f76 6f74 653a 2062 6f6f 6c29 202d 3e20  _vote: bool) -> 
-00013b40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00013b50: 220a 2020 2020 2020 2020 6070 7265 5f76  ".        `pre_v
-00013b60: 6f74 6560 3a20 456e 6162 6c65 2074 6865  ote`: Enable the
-00013b70: 2070 7265 766f 7465 2061 6c67 6f72 6974   prevote algorit
-00013b80: 686d 2e0a 0a20 2020 2020 2020 2054 6869  hm...        Thi
-00013b90: 7320 656e 6162 6c65 7320 6120 7072 652d  s enables a pre-
-00013ba0: 656c 6563 7469 6f6e 2076 6f74 6520 726f  election vote ro
-00013bb0: 756e 6420 6f6e 2043 616e 6469 6461 7465  und on Candidate
-00013bc0: 7320 7072 696f 7220 746f 2064 6973 7275  s prior to disru
-00013bd0: 7074 696e 6720 7468 6520 636c 7573 7465  pting the cluste
-00013be0: 722e 0a0a 2020 2020 2020 2020 456e 6162  r...        Enab
-00013bf0: 6c65 2074 6869 7320 6966 2067 7265 6174  le this if great
-00013c00: 6572 2063 6c75 7374 6572 2073 7461 6269  er cluster stabi
-00013c10: 6c69 7479 2069 7320 7072 6566 6572 7265  lity is preferre
-00013c20: 6420 6f76 6572 2066 6173 7465 7220 656c  d over faster el
-00013c30: 6563 7469 6f6e 732e 0a20 2020 2020 2020  ections..       
-00013c40: 2022 2222 0a20 2020 2064 6566 2061 7070   """.    def app
-00013c50: 6c79 5f63 6f6e 665f 6368 616e 6765 2873  ly_conf_change(s
-00013c60: 656c 662c 2063 6f6e 665f 6368 616e 6765  elf, conf_change
-00013c70: 3a20 2243 6f6e 6643 6861 6e67 6556 3252  : "ConfChangeV2R
-00013c80: 6566 2229 202d 3e20 2243 6f6e 6643 6861  ef") -> "ConfCha
-00013c90: 6e67 6552 6566 223a 0a20 2020 2020 2020  ngeRef":.       
-00013ca0: 2022 2222 2022 2222 0a20 2020 2064 6566   """ """.    def
-00013cb0: 2067 6574 5f72 6561 645f 7374 6174 6573   get_read_states
-00013cc0: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
-00013cd0: 5265 6164 5374 6174 6522 5d3a 0a20 2020  ReadState"]:.   
-00013ce0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013cf0: 2060 7265 6164 5f73 7461 7465 7360 3a20   `read_states`: 
-00013d00: 5468 6520 6375 7272 656e 7420 7265 6164  The current read
-00013d10: 2073 7461 7465 732e 0a20 2020 2020 2020   states..       
-00013d20: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-00013d30: 5f72 6561 645f 7374 6174 6573 280a 2020  _read_states(.  
-00013d40: 2020 2020 2020 7365 6c66 2c20 7265 6164        self, read
-00013d50: 5f73 7461 7465 733a 204c 6973 745b 2252  _states: List["R
-00013d60: 6561 6453 7461 7465 225d 207c 204c 6973  eadState"] | Lis
-00013d70: 745b 2252 6561 6453 7461 7465 5265 6622  t["ReadStateRef"
-00013d80: 5d0a 2020 2020 2920 2d3e 204e 6f6e 653a  ].    ) -> None:
-00013d90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013da0: 2020 2020 2060 7265 6164 5f73 7461 7465       `read_state
-00013db0: 7360 3a20 5468 6520 6375 7272 656e 7420  s`: The current 
-00013dc0: 7265 6164 2073 7461 7465 732e 0a20 2020  read states..   
-00013dd0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00013de0: 2067 6574 5f72 6561 645f 6f6e 6c79 5f6f   get_read_only_o
-00013df0: 7074 696f 6e28 7365 6c66 2920 2d3e 2022  ption(self) -> "
-00013e00: 5265 6164 4f6e 6c79 4f70 7469 6f6e 223a  ReadOnlyOption":
-00013e10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013e20: 2020 2020 2060 7265 6164 5f6f 6e6c 795f       `read_only_
-00013e30: 6f70 7469 6f6e 603a 2043 686f 6f73 6520  option`: Choose 
-00013e40: 7468 6520 6c69 6e65 6172 697a 6162 696c  the linearizabil
-00013e50: 6974 7920 6d6f 6465 206f 7220 7468 6520  ity mode or the 
-00013e60: 6c65 6173 6520 6d6f 6465 2074 6f20 7265  lease mode to re
-00013e70: 6164 2064 6174 612e 2049 6620 796f 7520  ad data. If you 
-00013e80: 646f 6ee2 8099 7420 6361 7265 2061 626f  don...t care abo
-00013e90: 7574 2074 6865 2072 6561 6420 636f 6e73  ut the read cons
-00013ea0: 6973 7465 6e63 7920 616e 6420 7761 6e74  istency and want
-00013eb0: 2061 2068 6967 6865 7220 7265 6164 2070   a higher read p
-00013ec0: 6572 666f 726d 616e 6365 2c20 796f 7520  erformance, you 
-00013ed0: 6361 6e20 7573 6520 7468 6520 6c65 6173  can use the leas
-00013ee0: 6520 6d6f 6465 2e0a 2020 2020 2020 2020  e mode..        
-00013ef0: 5365 7474 696e 6720 7468 6973 2074 6f20  Setting this to 
-00013f00: 604c 6561 7365 4261 7365 6460 2072 6571  `LeaseBased` req
-00013f10: 7569 7265 7320 6063 6865 636b 5f71 756f  uires `check_quo
-00013f20: 7275 6d20 3d20 7472 7565 602e 0a20 2020  rum = true`..   
-00013f30: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00013f40: 2073 6574 5f72 6561 645f 6f6e 6c79 5f6f   set_read_only_o
-00013f50: 7074 696f 6e28 7365 6c66 2c20 6f70 7469  ption(self, opti
-00013f60: 6f6e 3a20 2252 6561 644f 6e6c 794f 7074  on: "ReadOnlyOpt
-00013f70: 696f 6e22 2920 2d3e 204e 6f6e 653a 0a20  ion") -> None:. 
-00013f80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013f90: 2020 2060 7265 6164 5f6f 6e6c 795f 6f70     `read_only_op
-00013fa0: 7469 6f6e 603a 2043 686f 6f73 6520 7468  tion`: Choose th
-00013fb0: 6520 6c69 6e65 6172 697a 6162 696c 6974  e linearizabilit
-00013fc0: 7920 6d6f 6465 206f 7220 7468 6520 6c65  y mode or the le
-00013fd0: 6173 6520 6d6f 6465 2074 6f20 7265 6164  ase mode to read
-00013fe0: 2064 6174 612e 2049 6620 796f 7520 646f   data. If you do
-00013ff0: 6ee2 8099 7420 6361 7265 2061 626f 7574  n...t care about
-00014000: 2074 6865 2072 6561 6420 636f 6e73 6973   the read consis
-00014010: 7465 6e63 7920 616e 6420 7761 6e74 2061  tency and want a
-00014020: 2068 6967 6865 7220 7265 6164 2070 6572   higher read per
-00014030: 666f 726d 616e 6365 2c20 796f 7520 6361  formance, you ca
-00014040: 6e20 7573 6520 7468 6520 6c65 6173 6520  n use the lease 
-00014050: 6d6f 6465 2e0a 2020 2020 2020 2020 5365  mode..        Se
-00014060: 7474 696e 6720 7468 6973 2074 6f20 604c  tting this to `L
-00014070: 6561 7365 4261 7365 6460 2072 6571 7569  easeBased` requi
-00014080: 7265 7320 6063 6865 636b 5f71 756f 7275  res `check_quoru
-00014090: 6d20 3d20 7472 7565 602e 0a20 2020 2020  m = true`..     
-000140a0: 2020 2022 2222 0a20 2020 2064 6566 2069     """.    def i
-000140b0: 6e66 6c69 6768 745f 6275 6666 6572 735f  nflight_buffers_
-000140c0: 7369 7a65 2873 656c 6629 202d 3e20 696e  size(self) -> in
-000140d0: 743a 0a20 2020 2020 2020 2022 2222 4765  t:.        """Ge
-000140e0: 7420 7468 6520 696e 666c 6967 6874 2062  t the inflight b
-000140f0: 7566 6665 7220 7369 7a65 2e22 2222 0a20  uffer size.""". 
-00014100: 2020 2064 6566 206d 6179 6265 5f66 7265     def maybe_fre
-00014110: 655f 696e 666c 6967 6874 5f62 7566 6665  e_inflight_buffe
-00014120: 7273 2873 656c 6629 202d 3e20 4e6f 6e65  rs(self) -> None
-00014130: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00014140: 2020 2020 2020 4120 5261 6674 206c 6561        A Raft lea
-00014150: 6465 7220 616c 6c6f 6361 7465 7320 6120  der allocates a 
-00014160: 7665 6374 6f72 2077 6974 6820 6361 7061  vector with capa
-00014170: 6369 7479 2060 6d61 785f 696e 666c 6967  city `max_inflig
-00014180: 6874 5f6d 7367 7360 2066 6f72 2065 7665  ht_msgs` for eve
-00014190: 7279 2070 6565 722e 0a20 2020 2020 2020  ry peer..       
-000141a0: 2049 7420 7461 6b65 7320 6120 6c6f 7420   It takes a lot 
-000141b0: 6f66 206d 656d 6f72 7920 6966 2074 6865  of memory if the
-000141c0: 7265 2061 7265 2074 6f6f 206d 616e 7920  re are too many 
-000141d0: 5261 6674 2067 726f 7570 732e 2060 6d61  Raft groups. `ma
-000141e0: 7962 655f 6672 6565 5f69 6e66 6c69 6768  ybe_free_infligh
-000141f0: 745f 6275 6666 6572 7360 0a20 2020 2020  t_buffers`.     
-00014200: 2020 2069 7320 7573 6564 2074 6f20 6672     is used to fr
-00014210: 6565 206d 656d 6f72 7920 6966 206e 6563  ee memory if nec
-00014220: 6573 7361 7279 2e0a 2020 2020 2020 2020  essary..        
-00014230: 2222 220a 2020 2020 6465 6620 6164 6a75  """.    def adju
-00014240: 7374 5f6d 6178 5f69 6e66 6c69 6768 745f  st_max_inflight_
-00014250: 6d73 6773 2873 656c 662c 2074 6172 6765  msgs(self, targe
-00014260: 743a 2069 6e74 2c20 6361 703a 2069 6e74  t: int, cap: int
-00014270: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00014280: 2020 2022 2222 0a20 2020 2020 2020 2054     """.        T
-00014290: 6f20 6164 6a75 7374 2060 6d61 785f 696e  o adjust `max_in
-000142a0: 666c 6967 6874 5f6d 7367 7360 2066 6f72  flight_msgs` for
-000142b0: 2074 6865 2073 7065 6369 6669 6564 2070   the specified p
-000142c0: 6565 722e 0a20 2020 2020 2020 2053 6574  eer..        Set
-000142d0: 2074 6f20 6030 6020 7769 6c6c 2064 6973   to `0` will dis
-000142e0: 6162 6c65 2074 6865 2070 726f 6772 6573  able the progres
-000142f0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00014300: 2020 2064 6566 2067 6574 5f72 6561 646f     def get_reado
-00014310: 6e6c 795f 7265 6164 5f69 6e64 6578 5f71  nly_read_index_q
-00014320: 7565 7565 2873 656c 6629 202d 3e20 4c69  ueue(self) -> Li
-00014330: 7374 5b4c 6973 745b 696e 745d 5d3a 0a20  st[List[int]]:. 
-00014340: 2020 2020 2020 2022 2222 2022 2222 0a20         """ """. 
-00014350: 2020 2064 6566 2073 6574 5f62 6174 6368     def set_batch
-00014360: 5f61 7070 656e 6428 7365 6c66 2c20 6261  _append(self, ba
-00014370: 7463 685f 6170 7065 6e64 3a20 626f 6f6c  tch_append: bool
-00014380: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00014390: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-000143a0: 6574 2077 6865 7468 6572 2062 6174 6368  et whether batch
-000143b0: 2061 7070 656e 6420 6d73 6720 6174 2072   append msg at r
-000143c0: 756e 7469 6d65 2e0a 2020 2020 2020 2020  untime..        
-000143d0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-000143e0: 6d61 785f 636f 6d6d 6974 7465 645f 7369  max_committed_si
-000143f0: 7a65 5f70 6572 5f72 6561 6479 2873 656c  ze_per_ready(sel
-00014400: 662c 2073 697a 653a 2069 6e74 2920 2d3e  f, size: int) ->
-00014410: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00014420: 2222 0a20 2020 2020 2020 2053 6574 2060  "".        Set `
-00014430: 6d61 785f 636f 6d6d 6974 7465 645f 7369  max_committed_si
-00014440: 7a65 5f70 6572 5f72 6561 6479 6020 746f  ze_per_ready` to
-00014450: 2060 7369 7a65 602e 0a20 2020 2020 2020   `size`..       
-00014460: 2022 2222 0a0a 636c 6173 7320 496e 4d65   """..class InMe
-00014470: 6d6f 7279 5261 6674 285f 5f41 5049 5f52  moryRaft(__API_R
-00014480: 6166 7429 3a0a 2020 2020 2222 220a 2020  aft):.    """.  
-00014490: 2020 4120 7374 7275 6374 2074 6861 7420    A struct that 
-000144a0: 7265 7072 6573 656e 7473 2074 6865 2072  represents the r
-000144b0: 6166 7420 636f 6e73 656e 7375 7320 6974  aft consensus it
-000144c0: 7365 6c66 2e20 5374 6f72 6573 2064 6574  self. Stores det
-000144d0: 6169 6c73 2063 6f6e 6365 726e 696e 6720  ails concerning 
-000144e0: 7468 6520 6375 7272 656e 740a 2020 2020  the current.    
-000144f0: 616e 6420 706f 7373 6962 6c65 2073 7461  and possible sta
-00014500: 7465 2074 6865 2073 7973 7465 6d20 6361  te the system ca
-00014510: 6e20 7461 6b65 2e0a 2020 2020 2222 220a  n take..    """.
-00014520: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00014530: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00014540: 0a20 2020 2020 2020 2063 6667 3a20 2243  .        cfg: "C
-00014550: 6f6e 6669 6722 207c 2022 436f 6e66 6967  onfig" | "Config
-00014560: 5265 6622 2c0a 2020 2020 2020 2020 7374  Ref",.        st
-00014570: 6f72 653a 2022 4d65 6d53 746f 7261 6765  ore: "MemStorage
-00014580: 2220 7c20 224d 656d 5374 6f72 6167 6552  " | "MemStorageR
-00014590: 6566 222c 0a20 2020 2020 2020 206c 6f67  ef",.        log
-000145a0: 6765 723a 2022 4c6f 6767 6572 2220 7c20  ger: "Logger" | 
-000145b0: 224c 6f67 6765 7252 6566 222c 0a20 2020  "LoggerRef",.   
-000145c0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-000145d0: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
-000145e0: 2873 656c 6629 202d 3e20 2249 6e4d 656d  (self) -> "InMem
-000145f0: 6f72 7952 6166 7452 6566 223a 202e 2e2e  oryRaftRef": ...
-00014600: 0a20 2020 2064 6566 2067 6574 5f72 6166  .    def get_raf
-00014610: 745f 6c6f 6728 7365 6c66 2920 2d3e 2022  t_log(self) -> "
-00014620: 496e 4d65 6d6f 7279 5261 6674 4c6f 6752  InMemoryRaftLogR
-00014630: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
-00014640: 2022 2222 0a0a 636c 6173 7320 496e 4d65   """..class InMe
-00014650: 6d6f 7279 5261 6674 5265 6628 5f5f 4150  moryRaftRef(__AP
-00014660: 495f 5261 6674 293a 0a20 2020 2022 2222  I_Raft):.    """
-00014670: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
-00014680: 7970 6520 6f66 203a 636c 6173 733a 6049  ype of :class:`I
-00014690: 6e4d 656d 6f72 7952 6166 7460 2e0a 2020  nMemoryRaft`..  
-000146a0: 2020 2222 220a 0a20 2020 2064 6566 2067    """..    def g
-000146b0: 6574 5f72 6166 745f 6c6f 6728 7365 6c66  et_raft_log(self
-000146c0: 2920 2d3e 2022 496e 4d65 6d6f 7279 5261  ) -> "InMemoryRa
-000146d0: 6674 4c6f 6752 6566 223a 0a20 2020 2020  ftLogRef":.     
-000146e0: 2020 2022 2222 2022 2222 0a0a 636c 6173     """ """..clas
-000146f0: 7320 5261 6674 285f 5f41 5049 5f52 6166  s Raft(__API_Raf
-00014700: 7429 3a0a 2020 2020 2222 220a 2020 2020  t):.    """.    
-00014710: 4120 7374 7275 6374 2074 6861 7420 7265  A struct that re
-00014720: 7072 6573 656e 7473 2074 6865 2072 6166  presents the raf
-00014730: 7420 636f 6e73 656e 7375 7320 6974 7365  t consensus itse
-00014740: 6c66 2e20 5374 6f72 6573 2064 6574 6169  lf. Stores detai
-00014750: 6c73 2063 6f6e 6365 726e 696e 6720 7468  ls concerning th
-00014760: 6520 6375 7272 656e 740a 2020 2020 616e  e current.    an
-00014770: 6420 706f 7373 6962 6c65 2073 7461 7465  d possible state
-00014780: 2074 6865 2073 7973 7465 6d20 6361 6e20   the system can 
-00014790: 7461 6b65 2e0a 2020 2020 2222 220a 0a20  take..    """.. 
-000147a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000147b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000147c0: 2020 2020 2020 2063 6667 3a20 2243 6f6e         cfg: "Con
-000147d0: 6669 6722 207c 2022 436f 6e66 6967 5265  fig" | "ConfigRe
-000147e0: 6622 2c0a 2020 2020 2020 2020 7374 6f72  f",.        stor
-000147f0: 653a 2022 5374 6f72 6167 6522 207c 2022  e: "Storage" | "
-00014800: 5374 6f72 6167 6552 6566 222c 0a20 2020  StorageRef",.   
-00014810: 2020 2020 206c 6f67 6765 723a 2022 4c6f       logger: "Lo
-00014820: 6767 6572 2220 7c20 224c 6f67 6765 7252  gger" | "LoggerR
-00014830: 6566 222c 0a20 2020 2029 202d 3e20 4e6f  ef",.    ) -> No
-00014840: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00014850: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-00014860: 3e20 2252 6166 7452 6566 223a 202e 2e2e  > "RaftRef": ...
-00014870: 0a20 2020 2064 6566 2067 6574 5f72 6166  .    def get_raf
-00014880: 745f 6c6f 6728 7365 6c66 2920 2d3e 2022  t_log(self) -> "
-00014890: 5261 6674 4c6f 6752 6566 223a 0a20 2020  RaftLogRef":.   
-000148a0: 2020 2020 2022 2222 2022 2222 0a0a 636c       """ """..cl
-000148b0: 6173 7320 5261 6674 5265 6628 5f5f 4150  ass RaftRef(__AP
-000148c0: 495f 5261 6674 293a 0a20 2020 2022 2222  I_Raft):.    """
-000148d0: 0a20 2020 2052 6566 6572 656e 6365 2074  .    Reference t
-000148e0: 7970 6520 6f66 203a 636c 6173 733a 6052  ype of :class:`R
-000148f0: 6166 7460 2e0a 2020 2020 2222 220a 0a20  aft`..    """.. 
-00014900: 2020 2064 6566 2067 6574 5f72 6166 745f     def get_raft_
-00014910: 6c6f 6728 7365 6c66 2920 2d3e 2022 5261  log(self) -> "Ra
-00014920: 6674 4c6f 6752 6566 223a 0a20 2020 2020  ftLogRef":.     
-00014930: 2020 2022 2222 2022 2222 0a0a 636c 6173     """ """..clas
-00014940: 7320 5072 6f67 7265 7373 4d61 7049 7465  s ProgressMapIte
-00014950: 6d3a 0a20 2020 2064 6566 2069 6428 7365  m:.    def id(se
-00014960: 6c66 2920 2d3e 2069 6e74 3a20 2e2e 2e0a  lf) -> int: ....
-00014970: 2020 2020 6465 6620 7072 6f67 7265 7373      def progress
-00014980: 2873 656c 6629 202d 3e20 2250 726f 6772  (self) -> "Progr
-00014990: 6573 7322 3a20 2e2e 2e0a 0a63 6c61 7373  ess": .....class
-000149a0: 205f 5f41 5049 5f50 726f 6772 6573 7354   __API_ProgressT
-000149b0: 7261 636b 6572 285f 5f43 6c6f 6e65 6162  racker(__Cloneab
-000149c0: 6c65 293a 0a20 2020 2064 6566 2063 6c6f  le):.    def clo
-000149d0: 6e65 2873 656c 6629 202d 3e20 2250 726f  ne(self) -> "Pro
-000149e0: 6772 6573 7354 7261 636b 6572 223a 202e  gressTracker": .
-000149f0: 2e2e 0a20 2020 2064 6566 2067 6574 2873  ...    def get(s
-00014a00: 656c 662c 2069 643a 2069 6e74 2920 2d3e  elf, id: int) ->
-00014a10: 204f 7074 696f 6e61 6c5b 2250 726f 6772   Optional["Progr
-00014a20: 6573 7352 6566 225d 3a0a 2020 2020 2020  essRef"]:.      
-00014a30: 2020 2222 2222 2222 0a20 2020 2064 6566    """""".    def
-00014a40: 2067 726f 7570 5f63 6f6d 6d69 7428 7365   group_commit(se
-00014a50: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00014a60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014a70: 2057 6865 7468 6572 2065 6e61 626c 6520   Whether enable 
-00014a80: 6772 6f75 7020 636f 6d6d 6974 2e0a 2020  group commit..  
-00014a90: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00014aa0: 6620 656e 6162 6c65 5f67 726f 7570 5f63  f enable_group_c
-00014ab0: 6f6d 6d69 7428 7365 6c66 2c20 656e 6162  ommit(self, enab
-00014ac0: 6c65 3a20 626f 6f6c 2920 2d3e 204e 6f6e  le: bool) -> Non
-00014ad0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00014ae0: 2020 2020 2020 2043 6f6e 6669 6775 7265         Configure
-00014af0: 7320 6772 6f75 7020 636f 6d6d 6974 2e0a  s group commit..
-00014b00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014b10: 6465 6620 6861 735f 7175 6f72 756d 2873  def has_quorum(s
-00014b20: 656c 662c 2070 6f74 656e 7469 616c 5f71  elf, potential_q
-00014b30: 756f 7275 6d3a 2053 6574 5b69 6e74 5d29  uorum: Set[int])
-00014b40: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00014b50: 2020 2222 220a 2020 2020 2020 2020 4465    """.        De
-00014b60: 7465 726d 696e 6520 6966 2061 2071 756f  termine if a quo
-00014b70: 7275 6d20 6973 2066 6f72 6d65 6420 6672  rum is formed fr
-00014b80: 6f6d 2074 6865 2067 6976 656e 2073 6574  om the given set
-00014b90: 206f 6620 6e6f 6465 732e 0a0a 2020 2020   of nodes...    
-00014ba0: 2020 2020 5468 6973 2069 7320 7468 6520      This is the 
-00014bb0: 6f6e 6c79 2063 6f72 7265 6374 2077 6179  only correct way
-00014bc0: 2074 6f20 7665 7269 6679 2079 6f75 2068   to verify you h
-00014bd0: 6176 6520 7265 6163 6865 6420 6120 7175  ave reached a qu
-00014be0: 6f72 756d 2066 6f72 2074 6865 2077 686f  orum for the who
-00014bf0: 6c65 2067 726f 7570 2e0a 2020 2020 2020  le group..      
-00014c00: 2020 2222 220a 2020 2020 6465 6620 6973    """.    def is
-00014c10: 5f73 696e 676c 6574 6f6e 2873 656c 6629  _singleton(self)
-00014c20: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-00014c30: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-00014c40: 7475 726e 7320 7472 7565 2069 6620 2861  turns true if (a
-00014c50: 6e64 206f 6e6c 7920 6966 2920 7468 6572  nd only if) ther
-00014c60: 6520 6973 206f 6e6c 7920 6f6e 6520 766f  e is only one vo
-00014c70: 7469 6e67 206d 656d 6265 720a 2020 2020  ting member.    
-00014c80: 2020 2020 2869 2e65 2e20 7468 6520 6c65      (i.e. the le
-00014c90: 6164 6572 2920 696e 2074 6865 2063 7572  ader) in the cur
-00014ca0: 7265 6e74 2063 6f6e 6669 6775 7261 7469  rent configurati
-00014cb0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-00014cc0: 2020 2020 6465 6620 7175 6f72 756d 5f72      def quorum_r
-00014cd0: 6563 656e 746c 795f 6163 7469 7665 2873  ecently_active(s
-00014ce0: 656c 662c 2070 6572 7370 6563 7469 7665  elf, perspective
-00014cf0: 5f6f 663a 2069 6e74 2920 2d3e 2062 6f6f  _of: int) -> boo
-00014d00: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-00014d10: 2020 2020 2020 2044 6574 6572 6d69 6e65         Determine
-00014d20: 7320 6966 2074 6865 2063 7572 7265 6e74  s if the current
-00014d30: 2071 756f 7275 6d20 6973 2061 6374 6976   quorum is activ
-00014d40: 6520 6163 636f 7264 696e 6720 746f 2074  e according to t
-00014d50: 6865 2074 6869 7320 7261 6674 206e 6f64  he this raft nod
-00014d60: 652e 0a20 2020 2020 2020 2044 6f69 6e67  e..        Doing
-00014d70: 2074 6869 7320 7769 6c6c 2073 6574 2074   this will set t
-00014d80: 6865 2060 7265 6365 6e74 5f61 6374 6976  he `recent_activ
-00014d90: 6560 206f 6620 6561 6368 2070 6565 7220  e` of each peer 
-00014da0: 746f 2066 616c 7365 2e0a 0a20 2020 2020  to false...     
-00014db0: 2020 2054 6869 7320 7368 6f75 6c64 206f     This should o
-00014dc0: 6e6c 7920 6265 2063 616c 6c65 6420 6279  nly be called by
-00014dd0: 2074 6865 206c 6561 6465 722e 0a20 2020   the leader..   
-00014de0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00014df0: 206d 6178 696d 616c 5f63 6f6d 6d69 7474   maximal_committ
-00014e00: 6564 5f69 6e64 6578 2873 656c 6629 202d  ed_index(self) -
-00014e10: 3e20 5475 706c 655b 696e 742c 2062 6f6f  > Tuple[int, boo
-00014e20: 6c5d 3a0a 2020 2020 2020 2020 2222 220a  l]:.        """.
-00014e30: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-00014e40: 7468 6520 6d61 7869 6d61 6c20 636f 6d6d  the maximal comm
-00014e50: 6974 7465 6420 696e 6465 7820 666f 7220  itted index for 
-00014e60: 7468 6520 636c 7573 7465 722e 2054 6865  the cluster. The
-00014e70: 2062 6f6f 6c20 666c 6167 2069 6e64 6963   bool flag indic
-00014e80: 6174 6573 2077 6865 7468 6572 0a20 2020  ates whether.   
-00014e90: 2020 2020 2074 6865 2069 6e64 6578 2069       the index i
-00014ea0: 7320 636f 6d70 7574 6564 2062 7920 6772  s computed by gr
-00014eb0: 6f75 7020 636f 6d6d 6974 2061 6c67 6f72  oup commit algor
-00014ec0: 6974 686d 2073 7563 6365 7373 6675 6c6c  ithm successfull
-00014ed0: 790a 0a20 2020 2020 2020 2045 672e 2049  y..        Eg. I
-00014ee0: 6620 7468 6520 6d61 7463 6865 6420 696e  f the matched in
-00014ef0: 6465 7865 7320 6172 6520 605b 322c 322c  dexes are `[2,2,
-00014f00: 322c 342c 355d 602c 2069 7420 7769 6c6c  2,4,5]`, it will
-00014f10: 2072 6574 7572 6e20 6032 602e 0a20 2020   return `2`..   
-00014f20: 2020 2020 2049 6620 7468 6520 6d61 7463       If the matc
-00014f30: 6865 6420 696e 6465 7865 7320 616e 6420  hed indexes and 
-00014f40: 6772 6f75 7073 2061 7265 2060 5b28 312c  groups are `[(1,
-00014f50: 2031 292c 2028 322c 2032 292c 2028 332c   1), (2, 2), (3,
-00014f60: 2032 295d 602c 2069 7420 7769 6c6c 2072   2)]`, it will r
-00014f70: 6574 7572 6e20 6031 602e 0a20 2020 2020  eturn `1`..     
-00014f80: 2020 2022 2222 0a20 2020 2064 6566 2072     """.    def r
-00014f90: 6563 6f72 645f 766f 7465 2873 656c 662c  ecord_vote(self,
-00014fa0: 2069 643a 2069 6e74 2c20 766f 7465 3a20   id: int, vote: 
-00014fb0: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
-00014fc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014fd0: 2020 2052 6563 6f72 6473 2074 6861 7420     Records that 
-00014fe0: 7468 6520 6e6f 6465 2077 6974 6820 7468  the node with th
-00014ff0: 6520 6769 7665 6e20 6964 2076 6f74 6564  e given id voted
-00015000: 2066 6f72 2074 6869 7320 5261 6674 0a20   for this Raft. 
-00015010: 2020 2020 2020 2069 6e73 7461 6e63 6520         instance 
-00015020: 6966 2076 203d 3d20 7472 7565 2028 616e  if v == true (an
-00015030: 6420 6465 636c 696e 6564 2069 7420 6f74  d declined it ot
-00015040: 6865 7277 6973 6529 2e0a 2020 2020 2020  herwise)..      
-00015050: 2020 2222 220a 2020 2020 6465 6620 7265    """.    def re
-00015060: 7365 745f 766f 7465 7328 7365 6c66 2920  set_votes(self) 
-00015070: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00015080: 2022 2222 0a20 2020 2020 2020 2050 7265   """.        Pre
-00015090: 7061 7265 7320 666f 7220 6120 6e65 7720  pares for a new 
-000150a0: 726f 756e 6420 6f66 2076 6f74 6520 636f  round of vote co
-000150b0: 756e 7469 6e67 2076 6961 2072 6563 6f72  unting via recor
-000150c0: 6456 6f74 652e 0a20 2020 2020 2020 2022  dVote..        "
-000150d0: 2222 0a20 2020 2064 6566 2063 6f6e 665f  "".    def conf_
-000150e0: 766f 7465 7273 2873 656c 6629 202d 3e20  voters(self) -> 
-000150f0: 224a 6f69 6e74 436f 6e66 6967 5265 6622  "JointConfigRef"
-00015100: 3a0a 2020 2020 2020 2020 2222 2220 2222  :.        """ ""
-00015110: 220a 2020 2020 6465 6620 636f 6e66 5f6c  ".    def conf_l
-00015120: 6561 726e 6572 7328 7365 6c66 2920 2d3e  earners(self) ->
-00015130: 2053 6574 5b69 6e74 5d3a 0a20 2020 2020   Set[int]:.     
-00015140: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
-00015150: 6566 2063 6f6c 6c65 6374 2873 656c 6629  ef collect(self)
-00015160: 202d 3e20 4c69 7374 5b22 5072 6f67 7265   -> List["Progre
-00015170: 7373 4d61 7049 7465 6d22 5d3a 0a20 2020  ssMapItem"]:.   
-00015180: 2020 2020 2022 2222 2022 2222 0a0a 636c       """ """..cl
-00015190: 6173 7320 5072 6f67 7265 7373 5472 6163  ass ProgressTrac
-000151a0: 6b65 7228 5f5f 4150 495f 5072 6f67 7265  ker(__API_Progre
-000151b0: 7373 5472 6163 6b65 7229 3a0a 2020 2020  ssTracker):.    
-000151c0: 2222 220a 2020 2020 6050 726f 6772 6573  """.    `Progres
-000151d0: 7354 7261 636b 6572 6020 636f 6e74 6169  sTracker` contai
-000151e0: 6e73 2073 6576 6572 616c 2060 5072 6f67  ns several `Prog
-000151f0: 7265 7373 6065 732c 0a20 2020 2077 6869  ress`es,.    whi
-00015200: 6368 2063 6f75 6c64 2062 6520 604c 6561  ch could be `Lea
-00015210: 6465 7260 2c20 6046 6f6c 6c6f 7765 7260  der`, `Follower`
-00015220: 2061 6e64 2060 4c65 6172 6e65 7260 2e0a   and `Learner`..
-00015230: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00015240: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00015250: 6d61 785f 696e 666c 6967 6874 3a20 696e  max_inflight: in
-00015260: 7429 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  t) -> None: ....
-00015270: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
-00015280: 2873 656c 6629 202d 3e20 2250 726f 6772  (self) -> "Progr
-00015290: 6573 7354 7261 636b 6572 5265 6622 3a20  essTrackerRef": 
-000152a0: 2e2e 2e0a 0a63 6c61 7373 2050 726f 6772  .....class Progr
-000152b0: 6573 7354 7261 636b 6572 5265 6628 5f5f  essTrackerRef(__
-000152c0: 4150 495f 5072 6f67 7265 7373 5472 6163  API_ProgressTrac
-000152d0: 6b65 7229 3a0a 2020 2020 2222 220a 2020  ker):.    """.  
-000152e0: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
-000152f0: 206f 6620 3a63 6c61 7373 3a60 5072 6f67   of :class:`Prog
-00015300: 7265 7373 5472 6163 6b65 7260 2e0a 2020  ressTracker`..  
-00015310: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
-00015320: 5049 5f50 726f 6772 6573 7328 5f5f 436c  PI_Progress(__Cl
-00015330: 6f6e 6561 626c 6529 3a0a 2020 2020 6465  oneable):.    de
-00015340: 6620 636c 6f6e 6528 7365 6c66 2920 2d3e  f clone(self) ->
-00015350: 2022 5072 6f67 7265 7373 223a 202e 2e2e   "Progress": ...
-00015360: 0a20 2020 2064 6566 2062 6563 6f6d 655f  .    def become_
-00015370: 7072 6f62 6528 7365 6c66 2920 2d3e 204e  probe(self) -> N
-00015380: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00015390: 4368 616e 6765 7320 7468 6520 7072 6f67  Changes the prog
-000153a0: 7265 7373 2074 6f20 6120 7072 6f62 652e  ress to a probe.
-000153b0: 2222 220a 2020 2020 6465 6620 6265 636f  """.    def beco
-000153c0: 6d65 5f72 6570 6c69 6361 7465 2873 656c  me_replicate(sel
-000153d0: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
-000153e0: 2020 2020 2222 2243 6861 6e67 6573 2074      """Changes t
-000153f0: 6865 2070 726f 6772 6573 7320 746f 2061  he progress to a
-00015400: 2052 6570 6c69 6361 7465 2e22 2222 0a20   Replicate.""". 
-00015410: 2020 2064 6566 2062 6563 6f6d 655f 736e     def become_sn
-00015420: 6170 7368 6f74 2873 656c 662c 2073 6e61  apshot(self, sna
-00015430: 7073 686f 745f 6964 783a 2069 6e74 2920  pshot_idx: int) 
-00015440: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00015450: 2022 2222 4368 616e 6765 7320 7468 6520   """Changes the 
-00015460: 7072 6f67 7265 7373 2074 6f20 6120 736e  progress to a sn
-00015470: 6170 7368 6f74 2e22 2222 0a20 2020 2064  apshot.""".    d
-00015480: 6566 206d 6179 6265 5f75 7064 6174 6528  ef maybe_update(
-00015490: 7365 6c66 2c20 6e3a 2069 6e74 2920 2d3e  self, n: int) ->
-000154a0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-000154b0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-000154c0: 6e73 2066 616c 7365 2069 6620 7468 6520  ns false if the 
-000154d0: 6769 7665 6e20 6e20 696e 6465 7820 636f  given n index co
-000154e0: 6d65 7320 6672 6f6d 2061 6e20 6f75 7464  mes from an outd
-000154f0: 6174 6564 206d 6573 7361 6765 2e0a 2020  ated message..  
-00015500: 2020 2020 2020 4f74 6865 7277 6973 6520        Otherwise 
-00015510: 6974 2075 7064 6174 6573 2074 6865 2070  it updates the p
-00015520: 726f 6772 6573 7320 616e 6420 7265 7475  rogress and retu
-00015530: 726e 7320 7472 7565 2e0a 2020 2020 2020  rns true..      
-00015540: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
-00015550: 7962 655f 6465 6372 5f74 6f28 0a20 2020  ybe_decr_to(.   
-00015560: 2020 2020 2073 656c 662c 2072 656a 6563       self, rejec
-00015570: 7465 643a 2069 6e74 2c20 6d61 7463 685f  ted: int, match_
-00015580: 6869 6e74 3a20 696e 742c 2072 6571 7565  hint: int, reque
-00015590: 7374 5f73 6e61 7073 686f 743a 2069 6e74  st_snapshot: int
-000155a0: 0a20 2020 2029 202d 3e20 626f 6f6c 3a0a  .    ) -> bool:.
-000155b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000155c0: 2020 2020 5265 7475 726e 7320 6661 6c73      Returns fals
-000155d0: 6520 6966 2074 6865 2067 6976 656e 2069  e if the given i
-000155e0: 6e64 6578 2063 6f6d 6573 2066 726f 6d20  ndex comes from 
-000155f0: 616e 206f 7574 206f 6620 6f72 6465 7220  an out of order 
-00015600: 6d65 7373 6167 652e 0a20 2020 2020 2020  message..       
-00015610: 204f 7468 6572 7769 7365 2069 7420 6465   Otherwise it de
-00015620: 6372 6561 7365 7320 7468 6520 7072 6f67  creases the prog
-00015630: 7265 7373 206e 6578 7420 696e 6465 7820  ress next index 
-00015640: 746f 206d 696e 2872 656a 6563 7465 642c  to min(rejected,
-00015650: 206c 6173 7429 0a20 2020 2020 2020 2061   last).        a
-00015660: 6e64 2072 6574 7572 6e73 2074 7275 652e  nd returns true.
-00015670: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015680: 2064 6566 2073 6e61 7073 686f 745f 6661   def snapshot_fa
-00015690: 696c 7572 6528 7365 6c66 2920 2d3e 204e  ilure(self) -> N
-000156a0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000156b0: 0a20 2020 2020 2020 2053 6574 7320 7468  .        Sets th
-000156c0: 6520 736e 6170 7368 6f74 2074 6f20 6661  e snapshot to fa
-000156d0: 696c 7572 652e 0a20 2020 2020 2020 2022  ilure..        "
-000156e0: 2222 0a20 2020 2064 6566 2070 6175 7365  "".    def pause
-000156f0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00015700: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015710: 2020 2020 5061 7573 6520 7072 6f67 7265      Pause progre
-00015720: 7373 2e0a 2020 2020 2020 2020 2222 220a  ss..        """.
-00015730: 2020 2020 6465 6620 6973 5f70 6175 7365      def is_pause
-00015740: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
-00015750: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015760: 2020 2020 2044 6574 6572 6d69 6e65 2077       Determine w
-00015770: 6865 7468 6572 2070 726f 6772 6573 7320  hether progress 
-00015780: 6973 2070 6175 7365 642e 0a20 2020 2020  is paused..     
-00015790: 2020 2022 2222 0a20 2020 2064 6566 2069     """.    def i
-000157a0: 735f 736e 6170 7368 6f74 5f63 6175 6768  s_snapshot_caugh
-000157b0: 745f 7570 2873 656c 6629 202d 3e20 626f  t_up(self) -> bo
-000157c0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-000157d0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-000157e0: 7472 7565 2069 6620 4d61 7463 6820 6973  true if Match is
-000157f0: 2065 7175 616c 206f 7220 6869 6768 6572   equal or higher
-00015800: 2074 6861 6e20 7468 6520 7065 6e64 696e   than the pendin
-00015810: 6753 6e61 7073 686f 742e 0a20 2020 2020  gSnapshot..     
-00015820: 2020 2022 2222 0a20 2020 2064 6566 2072     """.    def r
-00015830: 6573 756d 6528 7365 6c66 2920 2d3e 204e  esume(self) -> N
-00015840: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-00015850: 0a20 2020 2020 2020 2052 6573 756d 6520  .        Resume 
-00015860: 7072 6f67 7265 7373 0a20 2020 2020 2020  progress.       
-00015870: 2022 2222 0a20 2020 2064 6566 2075 7064   """.    def upd
-00015880: 6174 655f 7374 6174 6528 7365 6c66 2c20  ate_state(self, 
-00015890: 6c61 7374 3a20 696e 7429 202d 3e20 4e6f  last: int) -> No
-000158a0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-000158b0: 2020 2020 2020 2020 5570 6461 7465 2069          Update i
-000158c0: 6e66 6c69 6768 7420 6d73 6773 2061 6e64  nflight msgs and
-000158d0: 206e 6578 745f 6964 780a 2020 2020 2020   next_idx.      
-000158e0: 2020 2222 220a 2020 2020 6465 6620 7570    """.    def up
-000158f0: 6461 7465 5f63 6f6d 6d69 7474 6564 2873  date_committed(s
-00015900: 656c 662c 2063 6f6d 6d69 7474 6564 5f69  elf, committed_i
-00015910: 6e64 6578 3a20 696e 7429 202d 3e20 4e6f  ndex: int) -> No
-00015920: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00015930: 2020 2020 2020 2020 5570 6461 7465 2063          Update c
-00015940: 6f6d 6d69 7474 6564 5f69 6e64 6578 2e0a  ommitted_index..
-00015950: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015960: 6465 6620 6f70 7469 6d69 7374 6963 5f75  def optimistic_u
-00015970: 7064 6174 6528 7365 6c66 2c20 6e3a 2069  pdate(self, n: i
-00015980: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
-00015990: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000159a0: 204f 7074 696d 6973 7469 6361 6c6c 7920   Optimistically 
-000159b0: 6164 7661 6e63 6520 7468 6520 696e 6465  advance the inde
-000159c0: 780a 2020 2020 2020 2020 2222 220a 2020  x.        """.  
-000159d0: 2020 6465 6620 6765 745f 696e 7328 7365    def get_ins(se
-000159e0: 6c66 2920 2d3e 2022 496e 666c 6967 6874  lf) -> "Inflight
-000159f0: 7352 6566 223a 0a20 2020 2020 2020 2022  sRef":.        "
-00015a00: 2222 0a20 2020 2020 2020 2060 696e 7360  "".        `ins`
-00015a10: 3a20 496e 666c 6967 6874 7320 6973 2061  : Inflights is a
-00015a20: 2073 6c69 6469 6e67 2077 696e 646f 7720   sliding window 
-00015a30: 666f 7220 7468 6520 696e 666c 6967 6874  for the inflight
-00015a40: 206d 6573 7361 6765 732e 0a20 2020 2020   messages..     
-00015a50: 2020 2057 6865 6e20 696e 666c 6967 6874     When inflight
-00015a60: 7320 6973 2066 756c 6c2c 206e 6f20 6d6f  s is full, no mo
-00015a70: 7265 206d 6573 7361 6765 2073 686f 756c  re message shoul
-00015a80: 6420 6265 2073 656e 742e 0a20 2020 2020  d be sent..     
-00015a90: 2020 2057 6865 6e20 6120 6c65 6164 6572     When a leader
-00015aa0: 2073 656e 6473 206f 7574 2061 206d 6573   sends out a mes
-00015ab0: 7361 6765 2c20 7468 6520 696e 6465 7820  sage, the index 
-00015ac0: 6f66 2074 6865 206c 6173 740a 2020 2020  of the last.    
-00015ad0: 2020 2020 656e 7472 7920 7368 6f75 6c64      entry should
-00015ae0: 2062 6520 6164 6465 6420 746f 2069 6e66   be added to inf
-00015af0: 6c69 6768 7473 2e20 5468 6520 696e 6465  lights. The inde
-00015b00: 7820 4d55 5354 2062 6520 6164 6465 640a  x MUST be added.
-00015b10: 2020 2020 2020 2020 696e 746f 2069 6e66          into inf
-00015b20: 6c69 6768 7473 2069 6e20 6f72 6465 722e  lights in order.
-00015b30: 0a20 2020 2020 2020 2057 6865 6e20 6120  .        When a 
-00015b40: 6c65 6164 6572 2072 6563 6569 7665 7320  leader receives 
-00015b50: 6120 7265 706c 792c 2074 6865 2070 7265  a reply, the pre
-00015b60: 7669 6f75 7320 696e 666c 6967 6874 7320  vious inflights 
-00015b70: 7368 6f75 6c64 0a20 2020 2020 2020 2062  should.        b
-00015b80: 6520 6672 6565 6420 6279 2063 616c 6c69  e freed by calli
-00015b90: 6e67 2069 6e66 6c69 6768 7473 2e66 7265  ng inflights.fre
-00015ba0: 6554 6f2e 0a20 2020 2020 2020 2022 2222  eTo..        """
-00015bb0: 0a20 2020 2064 6566 2073 6574 5f69 6e73  .    def set_ins
-00015bc0: 2873 656c 662c 2069 6e66 6c69 6768 7473  (self, inflights
-00015bd0: 3a20 2249 6e66 6c69 6768 7473 2220 7c20  : "Inflights" | 
-00015be0: 2249 6e66 6c69 6768 7473 5265 6622 2920  "InflightsRef") 
-00015bf0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00015c00: 2022 2222 0a20 2020 2020 2020 2060 696e   """.        `in
-00015c10: 7360 3a20 496e 666c 6967 6874 7320 6973  s`: Inflights is
-00015c20: 2061 2073 6c69 6469 6e67 2077 696e 646f   a sliding windo
-00015c30: 7720 666f 7220 7468 6520 696e 666c 6967  w for the inflig
-00015c40: 6874 206d 6573 7361 6765 732e 0a20 2020  ht messages..   
-00015c50: 2020 2020 2057 6865 6e20 696e 666c 6967       When inflig
-00015c60: 6874 7320 6973 2066 756c 6c2c 206e 6f20  hts is full, no 
-00015c70: 6d6f 7265 206d 6573 7361 6765 2073 686f  more message sho
-00015c80: 756c 6420 6265 2073 656e 742e 0a20 2020  uld be sent..   
-00015c90: 2020 2020 2057 6865 6e20 6120 6c65 6164       When a lead
-00015ca0: 6572 2073 656e 6473 206f 7574 2061 206d  er sends out a m
-00015cb0: 6573 7361 6765 2c20 7468 6520 696e 6465  essage, the inde
-00015cc0: 7820 6f66 2074 6865 206c 6173 740a 2020  x of the last.  
-00015cd0: 2020 2020 2020 656e 7472 7920 7368 6f75        entry shou
-00015ce0: 6c64 2062 6520 6164 6465 6420 746f 2069  ld be added to i
-00015cf0: 6e66 6c69 6768 7473 2e20 5468 6520 696e  nflights. The in
-00015d00: 6465 7820 4d55 5354 2062 6520 6164 6465  dex MUST be adde
-00015d10: 640a 2020 2020 2020 2020 696e 746f 2069  d.        into i
-00015d20: 6e66 6c69 6768 7473 2069 6e20 6f72 6465  nflights in orde
-00015d30: 722e 0a20 2020 2020 2020 2057 6865 6e20  r..        When 
-00015d40: 6120 6c65 6164 6572 2072 6563 6569 7665  a leader receive
-00015d50: 7320 6120 7265 706c 792c 2074 6865 2070  s a reply, the p
-00015d60: 7265 7669 6f75 7320 696e 666c 6967 6874  revious inflight
-00015d70: 7320 7368 6f75 6c64 0a20 2020 2020 2020  s should.       
-00015d80: 2062 6520 6672 6565 6420 6279 2063 616c   be freed by cal
-00015d90: 6c69 6e67 2069 6e66 6c69 6768 7473 2e66  ling inflights.f
-00015da0: 7265 6554 6f2e 0a20 2020 2020 2020 2022  reeTo..        "
-00015db0: 2222 0a20 2020 2064 6566 2067 6574 5f63  "".    def get_c
-00015dc0: 6f6d 6d69 745f 6772 6f75 705f 6964 2873  ommit_group_id(s
-00015dd0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-00015de0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015df0: 2060 636f 6d6d 6974 5f67 726f 7570 5f69   `commit_group_i
-00015e00: 6460 3a20 4f6e 6c79 206c 6f67 7320 7265  d`: Only logs re
-00015e10: 706c 6963 6174 6564 2074 6f20 6469 6666  plicated to diff
-00015e20: 6572 656e 7420 6772 6f75 7020 7769 6c6c  erent group will
-00015e30: 2062 6520 636f 6d6d 6974 7465 6420 6966   be committed if
-00015e40: 2061 6e79 2067 726f 7570 2069 7320 636f   any group is co
-00015e50: 6e66 6967 7572 6564 2e0a 2020 2020 2020  nfigured..      
-00015e60: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00015e70: 745f 636f 6d6d 6974 5f67 726f 7570 5f69  t_commit_group_i
-00015e80: 6428 7365 6c66 2c20 636f 6d6d 6974 5f67  d(self, commit_g
-00015e90: 726f 7570 5f69 643a 2069 6e74 2920 2d3e  roup_id: int) ->
-00015ea0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-00015eb0: 2222 0a20 2020 2020 2020 2060 636f 6d6d  "".        `comm
-00015ec0: 6974 5f67 726f 7570 5f69 6460 3a20 4f6e  it_group_id`: On
-00015ed0: 6c79 206c 6f67 7320 7265 706c 6963 6174  ly logs replicat
-00015ee0: 6564 2074 6f20 6469 6666 6572 656e 7420  ed to different 
-00015ef0: 6772 6f75 7020 7769 6c6c 2062 6520 636f  group will be co
-00015f00: 6d6d 6974 7465 6420 6966 2061 6e79 2067  mmitted if any g
-00015f10: 726f 7570 2069 7320 636f 6e66 6967 7572  roup is configur
-00015f20: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
-00015f30: 2020 2020 6465 6620 6765 745f 636f 6d6d      def get_comm
-00015f40: 6974 7465 645f 696e 6465 7828 7365 6c66  itted_index(self
-00015f50: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00015f60: 2020 2222 220a 2020 2020 2020 2020 6063    """.        `c
-00015f70: 6f6d 6d69 7474 6564 5f69 6e64 6578 603a  ommitted_index`:
-00015f80: 2043 6f6d 6d69 7474 6564 2069 6e64 6578   Committed index
-00015f90: 2069 6e20 7261 6674 5f6c 6f67 0a20 2020   in raft_log.   
-00015fa0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00015fb0: 2073 6574 5f63 6f6d 6d69 7474 6564 5f69   set_committed_i
-00015fc0: 6e64 6578 2873 656c 662c 2063 6f6d 6d69  ndex(self, commi
-00015fd0: 7474 6564 5f69 6e64 6578 3a20 696e 7429  tted_index: int)
-00015fe0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00015ff0: 2020 2222 220a 2020 2020 2020 2020 6063    """.        `c
-00016000: 6f6d 6d69 7474 6564 5f69 6e64 6578 603a  ommitted_index`:
-00016010: 2043 6f6d 6d69 7474 6564 2069 6e64 6578   Committed index
-00016020: 2069 6e20 7261 6674 5f6c 6f67 0a20 2020   in raft_log.   
-00016030: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
-00016040: 2067 6574 5f6d 6174 6368 6564 2873 656c   get_matched(sel
-00016050: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00016060: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00016070: 6d61 7463 6865 6460 3a20 486f 7720 6d75  matched`: How mu
-00016080: 6368 2073 7461 7465 2069 7320 6d61 7463  ch state is matc
-00016090: 6865 642e 0a20 2020 2020 2020 2022 2222  hed..        """
-000160a0: 0a20 2020 2064 6566 2073 6574 5f6d 6174  .    def set_mat
-000160b0: 6368 6564 2873 656c 662c 206d 6174 6368  ched(self, match
-000160c0: 6564 3a20 696e 7429 202d 3e20 4e6f 6e65  ed: int) -> None
-000160d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000160e0: 2020 2020 2020 606d 6174 6368 6564 603a        `matched`:
-000160f0: 2048 6f77 206d 7563 6820 7374 6174 6520   How much state 
-00016100: 6973 206d 6174 6368 6564 2e0a 2020 2020  is matched..    
-00016110: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00016120: 6765 745f 6e65 7874 5f69 6478 2873 656c  get_next_idx(sel
-00016130: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00016140: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00016150: 6e65 7874 5f69 6478 603a 2054 6865 206e  next_idx`: The n
-00016160: 6578 7420 696e 6465 7820 746f 2061 7070  ext index to app
-00016170: 6c79 0a20 2020 2020 2020 2022 2222 0a20  ly.        """. 
-00016180: 2020 2064 6566 2073 6574 5f6e 6578 745f     def set_next_
-00016190: 6964 7828 7365 6c66 2c20 6e65 7874 5f69  idx(self, next_i
-000161a0: 6478 3a20 696e 7429 202d 3e20 4e6f 6e65  dx: int) -> None
-000161b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000161c0: 2020 2020 2020 606e 6578 745f 6964 7860        `next_idx`
-000161d0: 3a20 5468 6520 6e65 7874 2069 6e64 6578  : The next index
-000161e0: 2074 6f20 6170 706c 790a 2020 2020 2020   to apply.      
-000161f0: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-00016200: 745f 7065 6e64 696e 675f 736e 6170 7368  t_pending_snapsh
-00016210: 6f74 2873 656c 6629 202d 3e20 696e 743a  ot(self) -> int:
-00016220: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016230: 2020 2020 2060 7065 6e64 696e 675f 736e       `pending_sn
-00016240: 6170 7368 6f74 603a 2054 6869 7320 6669  apshot`: This fi
-00016250: 656c 6420 6973 2075 7365 6420 696e 2050  eld is used in P
-00016260: 726f 6772 6573 7353 7461 7465 536e 6170  rogressStateSnap
-00016270: 7368 6f74 2e0a 2020 2020 2020 2020 4966  shot..        If
-00016280: 2074 6865 7265 2069 7320 6120 7065 6e64   there is a pend
-00016290: 696e 6720 736e 6170 7368 6f74 2c20 7468  ing snapshot, th
-000162a0: 6520 7065 6e64 696e 6753 6e61 7073 686f  e pendingSnapsho
-000162b0: 7420 7769 6c6c 2062 6520 7365 7420 746f  t will be set to
-000162c0: 2074 6865 0a20 2020 2020 2020 2069 6e64   the.        ind
-000162d0: 6578 206f 6620 7468 6520 736e 6170 7368  ex of the snapsh
-000162e0: 6f74 2e20 4966 2070 656e 6469 6e67 536e  ot. If pendingSn
-000162f0: 6170 7368 6f74 2069 7320 7365 742c 2074  apshot is set, t
-00016300: 6865 2072 6570 6c69 6361 7469 6f6e 2070  he replication p
-00016310: 726f 6365 7373 206f 660a 2020 2020 2020  rocess of.      
-00016320: 2020 7468 6973 2050 726f 6772 6573 7320    this Progress 
-00016330: 7769 6c6c 2062 6520 7061 7573 6564 2e20  will be paused. 
-00016340: 7261 6674 2077 696c 6c20 6e6f 7420 7265  raft will not re
-00016350: 7365 6e64 2073 6e61 7073 686f 7420 756e  send snapshot un
-00016360: 7469 6c20 7468 6520 7065 6e64 696e 6720  til the pending 
-00016370: 6f6e 650a 2020 2020 2020 2020 6973 2072  one.        is r
-00016380: 6570 6f72 7465 6420 746f 2062 6520 6661  eported to be fa
-00016390: 696c 6564 2e0a 2020 2020 2020 2020 2222  iled..        ""
-000163a0: 220a 2020 2020 6465 6620 7365 745f 7065  ".    def set_pe
-000163b0: 6e64 696e 675f 736e 6170 7368 6f74 2873  nding_snapshot(s
-000163c0: 656c 662c 2070 656e 6469 6e67 5f73 6e61  elf, pending_sna
-000163d0: 7073 686f 743a 2069 6e74 2920 2d3e 204e  pshot: int) -> N
-000163e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
-000163f0: 0a20 2020 2020 2020 2060 7065 6e64 696e  .        `pendin
-00016400: 675f 736e 6170 7368 6f74 603a 2054 6869  g_snapshot`: Thi
-00016410: 7320 6669 656c 6420 6973 2075 7365 6420  s field is used 
-00016420: 696e 2050 726f 6772 6573 7353 7461 7465  in ProgressState
-00016430: 536e 6170 7368 6f74 2e0a 2020 2020 2020  Snapshot..      
-00016440: 2020 4966 2074 6865 7265 2069 7320 6120    If there is a 
-00016450: 7065 6e64 696e 6720 736e 6170 7368 6f74  pending snapshot
-00016460: 2c20 7468 6520 7065 6e64 696e 6753 6e61  , the pendingSna
-00016470: 7073 686f 7420 7769 6c6c 2062 6520 7365  pshot will be se
-00016480: 7420 746f 2074 6865 0a20 2020 2020 2020  t to the.       
-00016490: 2069 6e64 6578 206f 6620 7468 6520 736e   index of the sn
-000164a0: 6170 7368 6f74 2e20 4966 2070 656e 6469  apshot. If pendi
-000164b0: 6e67 536e 6170 7368 6f74 2069 7320 7365  ngSnapshot is se
-000164c0: 742c 2074 6865 2072 6570 6c69 6361 7469  t, the replicati
-000164d0: 6f6e 2070 726f 6365 7373 206f 660a 2020  on process of.  
-000164e0: 2020 2020 2020 7468 6973 2050 726f 6772        this Progr
-000164f0: 6573 7320 7769 6c6c 2062 6520 7061 7573  ess will be paus
-00016500: 6564 2e20 7261 6674 2077 696c 6c20 6e6f  ed. raft will no
-00016510: 7420 7265 7365 6e64 2073 6e61 7073 686f  t resend snapsho
-00016520: 7420 756e 7469 6c20 7468 6520 7065 6e64  t until the pend
-00016530: 696e 6720 6f6e 650a 2020 2020 2020 2020  ing one.        
-00016540: 6973 2072 6570 6f72 7465 6420 746f 2062  is reported to b
-00016550: 6520 6661 696c 6564 2e0a 2020 2020 2020  e failed..      
-00016560: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-00016570: 745f 7065 6e64 696e 675f 7265 7175 6573  t_pending_reques
-00016580: 745f 736e 6170 7368 6f74 2873 656c 6629  t_snapshot(self)
-00016590: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-000165a0: 2022 2222 0a20 2020 2020 2020 2060 7065   """.        `pe
-000165b0: 6e64 696e 675f 7265 7175 6573 745f 736e  nding_request_sn
-000165c0: 6170 7368 6f74 603a 2054 6869 7320 6669  apshot`: This fi
-000165d0: 656c 6420 6973 2075 7365 6420 696e 2072  eld is used in r
-000165e0: 6571 7565 7374 2073 6e61 7073 686f 742e  equest snapshot.
-000165f0: 0a20 2020 2020 2020 2049 6620 7468 6572  .        If ther
-00016600: 6520 6973 2061 2070 656e 6469 6e67 2072  e is a pending r
-00016610: 6571 7565 7374 2073 6e61 7073 686f 742c  equest snapshot,
-00016620: 2074 6869 7320 7769 6c6c 2062 6520 7365   this will be se
-00016630: 7420 746f 2074 6865 2072 6571 7565 7374  t to the request
-00016640: 0a20 2020 2020 2020 2069 6e64 6578 206f  .        index o
-00016650: 6620 7468 6520 736e 6170 7368 6f74 2e0a  f the snapshot..
-00016660: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00016670: 6465 6620 7365 745f 7065 6e64 696e 675f  def set_pending_
-00016680: 7265 7175 6573 745f 736e 6170 7368 6f74  request_snapshot
-00016690: 2873 656c 662c 2070 656e 6469 6e67 5f72  (self, pending_r
-000166a0: 6571 7565 7374 5f73 6e61 7073 686f 743a  equest_snapshot:
-000166b0: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-000166c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000166d0: 2020 2060 7065 6e64 696e 675f 7265 7175     `pending_requ
-000166e0: 6573 745f 736e 6170 7368 6f74 603a 2054  est_snapshot`: T
-000166f0: 6869 7320 6669 656c 6420 6973 2075 7365  his field is use
-00016700: 6420 696e 2072 6571 7565 7374 2073 6e61  d in request sna
-00016710: 7073 686f 742e 0a20 2020 2020 2020 2049  pshot..        I
-00016720: 6620 7468 6572 6520 6973 2061 2070 656e  f there is a pen
-00016730: 6469 6e67 2072 6571 7565 7374 2073 6e61  ding request sna
-00016740: 7073 686f 742c 2074 6869 7320 7769 6c6c  pshot, this will
-00016750: 2062 6520 7365 7420 746f 2074 6865 2072   be set to the r
-00016760: 6571 7565 7374 0a20 2020 2020 2020 2069  equest.        i
-00016770: 6e64 6578 206f 6620 7468 6520 736e 6170  ndex of the snap
-00016780: 7368 6f74 2e0a 2020 2020 2020 2020 2222  shot..        ""
-00016790: 220a 2020 2020 6465 6620 6765 745f 7265  ".    def get_re
-000167a0: 6365 6e74 5f61 6374 6976 6528 7365 6c66  cent_active(self
-000167b0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-000167c0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-000167d0: 7265 6365 6e74 5f61 6374 6976 6560 3a20  recent_active`: 
-000167e0: 5468 6973 2069 7320 7472 7565 2069 6620  This is true if 
-000167f0: 7468 6520 7072 6f67 7265 7373 2069 7320  the progress is 
-00016800: 7265 6365 6e74 6c79 2061 6374 6976 652e  recently active.
-00016810: 2052 6563 6569 7669 6e67 2061 6e79 206d   Receiving any m
-00016820: 6573 7361 6765 730a 2020 2020 2020 2020  essages.        
-00016830: 6672 6f6d 2074 6865 2063 6f72 7265 7370  from the corresp
-00016840: 6f6e 6469 6e67 2066 6f6c 6c6f 7765 7220  onding follower 
-00016850: 696e 6469 6361 7465 7320 7468 6520 7072  indicates the pr
-00016860: 6f67 7265 7373 2069 7320 6163 7469 7665  ogress is active
-00016870: 2e0a 2020 2020 2020 2020 5265 6365 6e74  ..        Recent
-00016880: 4163 7469 7665 2063 616e 2062 6520 7265  Active can be re
-00016890: 7365 7420 746f 2066 616c 7365 2061 6674  set to false aft
-000168a0: 6572 2061 6e20 656c 6563 7469 6f6e 2074  er an election t
-000168b0: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
-000168c0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-000168d0: 7265 6365 6e74 5f61 6374 6976 6528 7365  recent_active(se
-000168e0: 6c66 2c20 7265 6365 6e74 5f61 6374 6976  lf, recent_activ
-000168f0: 653a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  e: bool) -> None
-00016900: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00016910: 2020 2020 2020 6072 6563 656e 745f 6163        `recent_ac
-00016920: 7469 7665 603a 2054 6869 7320 6973 2074  tive`: This is t
-00016930: 7275 6520 6966 2074 6865 2070 726f 6772  rue if the progr
-00016940: 6573 7320 6973 2072 6563 656e 746c 7920  ess is recently 
-00016950: 6163 7469 7665 2e20 5265 6365 6976 696e  active. Receivin
-00016960: 6720 616e 7920 6d65 7373 6167 6573 0a20  g any messages. 
-00016970: 2020 2020 2020 2066 726f 6d20 7468 6520         from the 
-00016980: 636f 7272 6573 706f 6e64 696e 6720 666f  corresponding fo
-00016990: 6c6c 6f77 6572 2069 6e64 6963 6174 6573  llower indicates
-000169a0: 2074 6865 2070 726f 6772 6573 7320 6973   the progress is
-000169b0: 2061 6374 6976 652e 0a20 2020 2020 2020   active..       
-000169c0: 2052 6563 656e 7441 6374 6976 6520 6361   RecentActive ca
-000169d0: 6e20 6265 2072 6573 6574 2074 6f20 6661  n be reset to fa
-000169e0: 6c73 6520 6166 7465 7220 616e 2065 6c65  lse after an ele
-000169f0: 6374 696f 6e20 7469 6d65 6f75 742e 0a20  ction timeout.. 
-00016a00: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-00016a10: 6566 2067 6574 5f70 6175 7365 6428 7365  ef get_paused(se
-00016a20: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
-00016a30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00016a40: 2060 7061 7573 6564 603a 2050 6175 7365   `paused`: Pause
-00016a50: 6420 6973 2075 7365 6420 696e 2050 726f  d is used in Pro
-00016a60: 6772 6573 7353 7461 7465 5072 6f62 652e  gressStateProbe.
-00016a70: 0a20 2020 2020 2020 2057 6865 6e20 5061  .        When Pa
-00016a80: 7573 6564 2069 7320 7472 7565 2c20 7261  used is true, ra
-00016a90: 6674 2073 686f 756c 6420 7061 7573 6520  ft should pause 
-00016aa0: 7365 6e64 696e 6720 7265 706c 6963 6174  sending replicat
-00016ab0: 696f 6e20 6d65 7373 6167 6520 746f 2074  ion message to t
-00016ac0: 6869 7320 7065 6572 2e0a 2020 2020 2020  his peer..      
-00016ad0: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
-00016ae0: 745f 7061 7573 6564 2873 656c 662c 2070  t_paused(self, p
-00016af0: 6175 7365 643a 2062 6f6f 6c29 202d 3e20  aused: bool) -> 
-00016b00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00016b10: 220a 2020 2020 2020 2020 6070 6175 7365  ".        `pause
-00016b20: 6460 3a20 5061 7573 6564 2069 7320 7573  d`: Paused is us
-00016b30: 6564 2069 6e20 5072 6f67 7265 7373 5374  ed in ProgressSt
-00016b40: 6174 6550 726f 6265 2e0a 2020 2020 2020  ateProbe..      
-00016b50: 2020 5768 656e 2050 6175 7365 6420 6973    When Paused is
-00016b60: 2074 7275 652c 2072 6166 7420 7368 6f75   true, raft shou
-00016b70: 6c64 2070 6175 7365 2073 656e 6469 6e67  ld pause sending
-00016b80: 2072 6570 6c69 6361 7469 6f6e 206d 6573   replication mes
-00016b90: 7361 6765 2074 6f20 7468 6973 2070 6565  sage to this pee
-00016ba0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-00016bb0: 2020 2064 6566 2067 6574 5f73 7461 7465     def get_state
-00016bc0: 2873 656c 6629 202d 3e20 2250 726f 6772  (self) -> "Progr
-00016bd0: 6573 7353 7461 7465 223a 0a20 2020 2020  essState":.     
-00016be0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00016bf0: 7374 6174 6560 3a20 5768 656e 2069 6e20  state`: When in 
-00016c00: 5072 6f67 7265 7373 5374 6174 6550 726f  ProgressStatePro
-00016c10: 6265 2c20 6c65 6164 6572 2073 656e 6473  be, leader sends
-00016c20: 2061 7420 6d6f 7374 206f 6e65 2072 6570   at most one rep
-00016c30: 6c69 6361 7469 6f6e 206d 6573 7361 6765  lication message
-00016c40: 0a20 2020 2020 2020 2070 6572 2068 6561  .        per hea
-00016c50: 7274 6265 6174 2069 6e74 6572 7661 6c2e  rtbeat interval.
-00016c60: 2049 7420 616c 736f 2070 726f 6265 7320   It also probes 
-00016c70: 6163 7475 616c 2070 726f 6772 6573 7320  actual progress 
-00016c80: 6f66 2074 6865 2066 6f6c 6c6f 7765 722e  of the follower.
-00016c90: 0a0a 2020 2020 2020 2020 5768 656e 2069  ..        When i
-00016ca0: 6e20 5072 6f67 7265 7373 5374 6174 6552  n ProgressStateR
-00016cb0: 6570 6c69 6361 7465 2c20 6c65 6164 6572  eplicate, leader
-00016cc0: 206f 7074 696d 6973 7469 6361 6c6c 7920   optimistically 
-00016cd0: 696e 6372 6561 7365 7320 6e65 7874 0a20  increases next. 
-00016ce0: 2020 2020 2020 2074 6f20 7468 6520 6c61         to the la
-00016cf0: 7465 7374 2065 6e74 7279 2073 656e 7420  test entry sent 
-00016d00: 6166 7465 7220 7365 6e64 696e 6720 7265  after sending re
-00016d10: 706c 6963 6174 696f 6e20 6d65 7373 6167  plication messag
-00016d20: 652e 2054 6869 7320 6973 0a20 2020 2020  e. This is.     
-00016d30: 2020 2061 6e20 6f70 7469 6d69 7a65 6420     an optimized 
-00016d40: 7374 6174 6520 666f 7220 6661 7374 2072  state for fast r
-00016d50: 6570 6c69 6361 7469 6e67 206c 6f67 2065  eplicating log e
-00016d60: 6e74 7269 6573 2074 6f20 7468 6520 666f  ntries to the fo
-00016d70: 6c6c 6f77 6572 2e0a 0a20 2020 2020 2020  llower...       
-00016d80: 2057 6865 6e20 696e 2050 726f 6772 6573   When in Progres
-00016d90: 7353 7461 7465 536e 6170 7368 6f74 2c20  sStateSnapshot, 
-00016da0: 6c65 6164 6572 2073 686f 756c 6420 6861  leader should ha
-00016db0: 7665 2073 656e 7420 6f75 7420 736e 6170  ve sent out snap
-00016dc0: 7368 6f74 0a20 2020 2020 2020 2062 6566  shot.        bef
-00016dd0: 6f72 6520 616e 6420 7374 6f70 2073 656e  ore and stop sen
-00016de0: 6469 6e67 2061 6e79 2072 6570 6c69 6361  ding any replica
-00016df0: 7469 6f6e 206d 6573 7361 6765 2e0a 2020  tion message..  
-00016e00: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00016e10: 6620 7365 745f 7374 6174 6528 7365 6c66  f set_state(self
-00016e20: 2c20 7374 6174 653a 2022 5072 6f67 7265  , state: "Progre
-00016e30: 7373 5374 6174 6522 2920 2d3e 204e 6f6e  ssState") -> Non
-00016e40: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00016e50: 2020 2020 2020 2060 7374 6174 6560 3a20         `state`: 
-00016e60: 5768 656e 2069 6e20 5072 6f67 7265 7373  When in Progress
-00016e70: 5374 6174 6550 726f 6265 2c20 6c65 6164  StateProbe, lead
-00016e80: 6572 2073 656e 6473 2061 7420 6d6f 7374  er sends at most
-00016e90: 206f 6e65 2072 6570 6c69 6361 7469 6f6e   one replication
-00016ea0: 206d 6573 7361 6765 0a20 2020 2020 2020   message.       
-00016eb0: 2070 6572 2068 6561 7274 6265 6174 2069   per heartbeat i
-00016ec0: 6e74 6572 7661 6c2e 2049 7420 616c 736f  nterval. It also
-00016ed0: 2070 726f 6265 7320 6163 7475 616c 2070   probes actual p
-00016ee0: 726f 6772 6573 7320 6f66 2074 6865 2066  rogress of the f
-00016ef0: 6f6c 6c6f 7765 722e 0a0a 2020 2020 2020  ollower...      
-00016f00: 2020 5768 656e 2069 6e20 5072 6f67 7265    When in Progre
-00016f10: 7373 5374 6174 6552 6570 6c69 6361 7465  ssStateReplicate
-00016f20: 2c20 6c65 6164 6572 206f 7074 696d 6973  , leader optimis
-00016f30: 7469 6361 6c6c 7920 696e 6372 6561 7365  tically increase
-00016f40: 7320 6e65 7874 0a20 2020 2020 2020 2074  s next.        t
-00016f50: 6f20 7468 6520 6c61 7465 7374 2065 6e74  o the latest ent
-00016f60: 7279 2073 656e 7420 6166 7465 7220 7365  ry sent after se
-00016f70: 6e64 696e 6720 7265 706c 6963 6174 696f  nding replicatio
-00016f80: 6e20 6d65 7373 6167 652e 2054 6869 7320  n message. This 
-00016f90: 6973 0a20 2020 2020 2020 2061 6e20 6f70  is.        an op
-00016fa0: 7469 6d69 7a65 6420 7374 6174 6520 666f  timized state fo
-00016fb0: 7220 6661 7374 2072 6570 6c69 6361 7469  r fast replicati
-00016fc0: 6e67 206c 6f67 2065 6e74 7269 6573 2074  ng log entries t
-00016fd0: 6f20 7468 6520 666f 6c6c 6f77 6572 2e0a  o the follower..
-00016fe0: 0a20 2020 2020 2020 2057 6865 6e20 696e  .        When in
-00016ff0: 2050 726f 6772 6573 7353 7461 7465 536e   ProgressStateSn
-00017000: 6170 7368 6f74 2c20 6c65 6164 6572 2073  apshot, leader s
-00017010: 686f 756c 6420 6861 7665 2073 656e 7420  hould have sent 
-00017020: 6f75 7420 736e 6170 7368 6f74 0a20 2020  out snapshot.   
-00017030: 2020 2020 2062 6566 6f72 6520 616e 6420       before and 
-00017040: 7374 6f70 2073 656e 6469 6e67 2061 6e79  stop sending any
-00017050: 2072 6570 6c69 6361 7469 6f6e 206d 6573   replication mes
-00017060: 7361 6765 2e0a 2020 2020 2020 2020 2222  sage..        ""
-00017070: 220a 0a63 6c61 7373 2050 726f 6772 6573  "..class Progres
-00017080: 7328 5f5f 4150 495f 5072 6f67 7265 7373  s(__API_Progress
-00017090: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
-000170a0: 6865 2070 726f 6772 6573 7320 6f66 2063  he progress of c
-000170b0: 6174 6368 696e 6720 7570 2066 726f 6d20  atching up from 
-000170c0: 6120 7265 7374 6172 742e 0a20 2020 2022  a restart..    "
-000170d0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-000170e0: 6974 5f5f 2873 656c 662c 206e 6578 745f  it__(self, next_
-000170f0: 6964 783a 2069 6e74 2c20 696e 735f 7369  idx: int, ins_si
-00017100: 7a65 3a20 696e 7429 202d 3e20 4e6f 6e65  ze: int) -> None
-00017110: 3a20 2e2e 2e0a 2020 2020 6465 6620 6d61  : ....    def ma
-00017120: 6b65 5f72 6566 2873 656c 6629 202d 3e20  ke_ref(self) -> 
-00017130: 2250 726f 6772 6573 7352 6566 223a 202e  "ProgressRef": .
-00017140: 2e2e 0a0a 636c 6173 7320 5072 6f67 7265  ....class Progre
-00017150: 7373 5265 6628 5f5f 4150 495f 5072 6f67  ssRef(__API_Prog
-00017160: 7265 7373 293a 0a20 2020 2022 2222 0a20  ress):.    """. 
-00017170: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
-00017180: 6520 6f66 203a 636c 6173 733a 6050 726f  e of :class:`Pro
-00017190: 6772 6573 7360 2e0a 2020 2020 2222 220a  gress`..    """.
-000171a0: 0a63 6c61 7373 205f 5f41 5049 5f4a 6f69  .class __API_Joi
-000171b0: 6e74 436f 6e66 6967 285f 5f43 6c6f 6e65  ntConfig(__Clone
-000171c0: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
-000171d0: 6c6f 6e65 2873 656c 6629 202d 3e20 224a  lone(self) -> "J
-000171e0: 6f69 6e74 436f 6e66 6967 223a 202e 2e2e  ointConfig": ...
-000171f0: 0a20 2020 2064 6566 2063 6c65 6172 2873  .    def clear(s
-00017200: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00017210: 2020 2020 2020 2222 2243 6c65 6172 7320        """Clears 
-00017220: 616c 6c20 4944 732e 2222 220a 2020 2020  all IDs.""".    
-00017230: 6465 6620 636f 6e74 6169 6e73 2873 656c  def contains(sel
-00017240: 662c 2069 643a 2069 6e74 2920 2d3e 2062  f, id: int) -> b
-00017250: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00017260: 4368 6563 6b20 6966 2061 6e20 6964 2069  Check if an id i
-00017270: 7320 6120 766f 7465 722e 2222 220a 2020  s a voter.""".  
-00017280: 2020 6465 6620 6964 7328 2920 2d3e 2053    def ids() -> S
-00017290: 6574 5b69 6e74 5d3a 0a20 2020 2020 2020  et[int]:.       
-000172a0: 2022 2222 5265 7475 726e 7320 616e 2069   """Returns an i
-000172b0: 7465 7261 746f 7220 6f76 6572 2074 776f  terator over two
-000172c0: 2068 6173 6820 7365 7420 7769 7468 6f75   hash set withou
-000172d0: 7420 636c 6f6e 696e 672e 2222 220a 2020  t cloning.""".  
-000172e0: 2020 6465 6620 6973 5f73 696e 676c 6574    def is_singlet
-000172f0: 6f6e 2873 656c 6629 202d 3e20 626f 6f6c  on(self) -> bool
-00017300: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00017310: 2020 2020 2020 5265 7475 726e 7320 7472        Returns tr
-00017320: 7565 2069 6620 2861 6e64 206f 6e6c 7920  ue if (and only 
-00017330: 6966 2920 7468 6572 6520 6973 206f 6e6c  if) there is onl
-00017340: 7920 6f6e 6520 766f 7469 6e67 206d 656d  y one voting mem
-00017350: 6265 720a 2020 2020 2020 2020 2869 2e65  ber.        (i.e
-00017360: 2e20 7468 6520 6c65 6164 6572 2920 696e  . the leader) in
-00017370: 2074 6865 2063 7572 7265 6e74 2063 6f6e   the current con
-00017380: 6669 6775 7261 7469 6f6e 2e0a 2020 2020  figuration..    
-00017390: 2020 2020 2222 220a 0a63 6c61 7373 204a      """..class J
-000173a0: 6f69 6e74 436f 6e66 6967 285f 5f41 5049  ointConfig(__API
-000173b0: 5f4a 6f69 6e74 436f 6e66 6967 293a 0a20  _JointConfig):. 
-000173c0: 2020 2022 2222 0a20 2020 2041 2063 6f6e     """.    A con
-000173d0: 6669 6775 7261 7469 6f6e 206f 6620 7477  figuration of tw
-000173e0: 6f20 6772 6f75 7073 206f 6620 2870 6f73  o groups of (pos
-000173f0: 7369 626c 7920 6f76 6572 6c61 7070 696e  sibly overlappin
-00017400: 6729 206d 616a 6f72 6974 7920 636f 6e66  g) majority conf
-00017410: 6967 7572 6174 696f 6e73 2e0a 2020 2020  igurations..    
-00017420: 4465 6369 7369 6f6e 7320 7265 7175 6972  Decisions requir
-00017430: 6520 7468 6520 7375 7070 6f72 7420 6f66  e the support of
-00017440: 2062 6f74 6820 6d61 6a6f 7269 7469 6573   both majorities
-00017450: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00017460: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00017470: 2c20 766f 7465 7273 3a20 5365 745b 696e  , voters: Set[in
-00017480: 745d 2920 2d3e 204e 6f6e 653a 202e 2e2e  t]) -> None: ...
-00017490: 0a20 2020 2064 6566 206d 616b 655f 7265  .    def make_re
-000174a0: 6628 7365 6c66 2920 2d3e 2022 4a6f 696e  f(self) -> "Join
-000174b0: 7443 6f6e 6669 6752 6566 223a 202e 2e2e  tConfigRef": ...
-000174c0: 0a0a 636c 6173 7320 4a6f 696e 7443 6f6e  ..class JointCon
-000174d0: 6669 6752 6566 285f 5f41 5049 5f4a 6f69  figRef(__API_Joi
-000174e0: 6e74 436f 6e66 6967 293a 0a20 2020 2022  ntConfig):.    "
-000174f0: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
-00017500: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
-00017510: 604a 6f69 6e74 436f 6e66 6967 602e 0a20  `JointConfig`.. 
-00017520: 2020 2022 2222 0a0a 636c 6173 7320 5f5f     """..class __
-00017530: 4150 495f 4d61 6a6f 7269 7479 436f 6e66  API_MajorityConf
-00017540: 6967 285f 5f43 6c6f 6e65 6162 6c65 293a  ig(__Cloneable):
-00017550: 0a20 2020 2064 6566 2063 6c6f 6e65 2873  .    def clone(s
-00017560: 656c 6629 202d 3e20 224d 616a 6f72 6974  elf) -> "Majorit
-00017570: 7943 6f6e 6669 6722 3a20 2e2e 2e0a 2020  yConfig": ....  
-00017580: 2020 6465 6620 7261 775f 736c 6963 6528    def raw_slice(
-00017590: 7365 6c66 2920 2d3e 204c 6973 745b 696e  self) -> List[in
-000175a0: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-000175b0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-000175c0: 7468 6520 4d61 6a6f 7269 7479 436f 6e66  the MajorityConf
-000175d0: 6967 2061 7320 6120 736c 6963 652e 0a20  ig as a slice.. 
-000175e0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
-000175f0: 6566 2063 6170 6163 6974 7928 7365 6c66  ef capacity(self
-00017600: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00017610: 2020 2222 2222 2222 0a20 2020 2064 6566    """""".    def
-00017620: 2065 7874 656e 6428 7365 6c66 2c20 6f74   extend(self, ot
-00017630: 6865 725f 7365 743a 2053 6574 5b69 6e74  her_set: Set[int
-00017640: 5d29 202d 3e20 4e6f 6e65 3a0a 2020 2020  ]) -> None:.    
-00017650: 2020 2020 2222 2222 2222 0a20 2020 2064      """""".    d
-00017660: 6566 2067 6574 2873 656c 662c 2069 6e64  ef get(self, ind
-00017670: 6578 3a20 696e 7429 202d 3e20 4f70 7469  ex: int) -> Opti
-00017680: 6f6e 616c 5b69 6e74 5d3a 0a20 2020 2020  onal[int]:.     
-00017690: 2020 2022 2222 2222 220a 2020 2020 6465     """""".    de
-000176a0: 6620 696e 7365 7274 2873 656c 662c 2076  f insert(self, v
-000176b0: 616c 7565 3a20 696e 7429 202d 3e20 626f  alue: int) -> bo
-000176c0: 6f6c 3a0a 2020 2020 2020 2020 2222 2222  ol:.        """"
-000176d0: 2222 0a20 2020 2064 6566 2072 6570 6c61  "".    def repla
-000176e0: 6365 2873 656c 662c 2076 616c 7565 3a20  ce(self, value: 
-000176f0: 696e 7429 202d 3e20 696e 743a 0a20 2020  int) -> int:.   
-00017700: 2020 2020 2022 2222 2222 220a 2020 2020       """""".    
-00017710: 6465 6620 6973 5f64 6973 6a6f 696e 7428  def is_disjoint(
-00017720: 7365 6c66 2c20 6f74 6865 723a 2053 6574  self, other: Set
-00017730: 5b69 6e74 5d29 202d 3e20 626f 6f6c 3a0a  [int]) -> bool:.
-00017740: 2020 2020 2020 2020 2222 2222 2222 0a20          """""". 
-00017750: 2020 2064 6566 2069 735f 7375 7065 7273     def is_supers
-00017760: 6574 2873 656c 662c 206f 7468 6572 3a20  et(self, other: 
-00017770: 5365 745b 696e 745d 2920 2d3e 2062 6f6f  Set[int]) -> boo
-00017780: 6c3a 0a20 2020 2020 2020 2022 2222 2222  l:.        """""
-00017790: 220a 2020 2020 6465 6620 6973 5f73 7562  ".    def is_sub
-000177a0: 7365 7428 7365 6c66 2c20 6f74 6865 723a  set(self, other:
-000177b0: 2053 6574 5b69 6e74 5d29 202d 3e20 626f   Set[int]) -> bo
-000177c0: 6f6c 3a0a 2020 2020 2020 2020 2222 2222  ol:.        """"
-000177d0: 2222 0a20 2020 2064 6566 2072 6573 6572  "".    def reser
-000177e0: 7665 2873 656c 662c 2061 6464 6974 696f  ve(self, additio
-000177f0: 6e61 6c3a 2069 6e74 2920 2d3e 204e 6f6e  nal: int) -> Non
-00017800: 653a 0a20 2020 2020 2020 2022 2222 2222  e:.        """""
-00017810: 220a 2020 2020 6465 6620 7265 6d6f 7665  ".    def remove
-00017820: 2873 656c 662c 2076 616c 7565 3a20 696e  (self, value: in
-00017830: 7429 202d 3e20 626f 6f6c 3a0a 2020 2020  t) -> bool:.    
-00017840: 2020 2020 2222 2222 2222 0a20 2020 2064      """""".    d
-00017850: 6566 2073 6872 696e 6b5f 746f 2873 656c  ef shrink_to(sel
-00017860: 662c 206d 696e 5f63 6170 6163 6974 793a  f, min_capacity:
-00017870: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
-00017880: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
-00017890: 2020 6465 6620 7368 7269 6e6b 5f74 6f5f    def shrink_to_
-000178a0: 6669 7428 7365 6c66 2920 2d3e 204e 6f6e  fit(self) -> Non
-000178b0: 653a 0a20 2020 2020 2020 2022 2222 2222  e:.        """""
-000178c0: 220a 2020 2020 6465 6620 7472 795f 7265  ".    def try_re
-000178d0: 7365 7276 6528 7365 6c66 2c20 6164 6469  serve(self, addi
-000178e0: 7469 6f6e 616c 3a20 696e 7429 202d 3e20  tional: int) -> 
-000178f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00017900: 2222 2222 0a0a 636c 6173 7320 4d61 6a6f  """"..class Majo
-00017910: 7269 7479 436f 6e66 6967 285f 5f41 5049  rityConfig(__API
-00017920: 5f4d 616a 6f72 6974 7943 6f6e 6669 6729  _MajorityConfig)
-00017930: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
-00017940: 7365 7420 6f66 2049 4473 2074 6861 7420  set of IDs that 
-00017950: 7573 6573 206d 616a 6f72 6974 7920 7175  uses majority qu
-00017960: 6f72 756d 7320 746f 206d 616b 6520 6465  orums to make de
-00017970: 6369 7369 6f6e 732e 0a20 2020 2022 2222  cisions..    """
-00017980: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-00017990: 5f5f 2873 656c 662c 2076 6f74 6572 733a  __(self, voters:
-000179a0: 2053 6574 5b69 6e74 5d29 202d 3e20 4e6f   Set[int]) -> No
-000179b0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-000179c0: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-000179d0: 3e20 224d 616a 6f72 6974 7943 6f6e 6669  > "MajorityConfi
-000179e0: 6752 6566 223a 202e 2e2e 0a0a 636c 6173  gRef": .....clas
-000179f0: 7320 4d61 6a6f 7269 7479 436f 6e66 6967  s MajorityConfig
-00017a00: 5265 6628 5f5f 4150 495f 4d61 6a6f 7269  Ref(__API_Majori
-00017a10: 7479 436f 6e66 6967 293a 0a20 2020 2022  tyConfig):.    "
-00017a20: 2222 0a20 2020 2052 6566 6572 656e 6365  "".    Reference
-00017a30: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
-00017a40: 604d 616a 6f72 6974 7943 6f6e 6669 6760  `MajorityConfig`
-00017a50: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
-00017a60: 205f 5f41 5049 5f49 6e66 6c69 6768 7473   __API_Inflights
-00017a70: 285f 5f43 6c6f 6e65 6162 6c65 293a 0a20  (__Cloneable):. 
-00017a80: 2020 2064 6566 2063 6c6f 6e65 2873 656c     def clone(sel
-00017a90: 6629 202d 3e20 2249 6e66 6c69 6768 7473  f) -> "Inflights
-00017aa0: 223a 202e 2e2e 0a20 2020 2064 6566 2061  ": ....    def a
-00017ab0: 6464 2873 656c 662c 2069 6e66 6c69 6768  dd(self, infligh
-00017ac0: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
-00017ad0: 0a20 2020 2020 2020 2022 2222 4164 6473  .        """Adds
-00017ae0: 2061 6e20 696e 666c 6967 6874 2069 6e74   an inflight int
-00017af0: 6f20 696e 666c 6967 6874 7322 2222 0a20  o inflights""". 
-00017b00: 2020 2064 6566 2066 756c 6c28 7365 6c66     def full(self
-00017b10: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00017b20: 2020 2022 2222 5265 7475 726e 7320 7472     """Returns tr
-00017b30: 7565 2069 6620 7468 6520 696e 666c 6967  ue if the inflig
-00017b40: 6874 7320 6973 2066 756c 6c2e 2222 220a  hts is full.""".
-00017b50: 2020 2020 6465 6620 7265 7365 7428 7365      def reset(se
-00017b60: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00017b70: 2020 2020 2022 2222 4672 6565 7320 616c       """Frees al
-00017b80: 6c20 696e 666c 6967 6874 732e 2222 220a  l inflights.""".
-00017b90: 2020 2020 6465 6620 6672 6565 5f74 6f28      def free_to(
-00017ba0: 7365 6c66 2c20 746f 3a20 696e 7429 202d  self, to: int) -
-00017bb0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00017bc0: 2222 2246 7265 6573 2074 6865 2069 6e66  """Frees the inf
-00017bd0: 6c69 6768 7473 2073 6d61 6c6c 6572 206f  lights smaller o
-00017be0: 7220 6571 7561 6c20 746f 2074 6865 2067  r equal to the g
-00017bf0: 6976 656e 2060 746f 6020 666c 6967 6874  iven `to` flight
-00017c00: 2e22 2222 0a20 2020 2064 6566 2066 7265  .""".    def fre
-00017c10: 655f 6669 7273 745f 6f6e 6528 7365 6c66  e_first_one(self
-00017c20: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00017c30: 2020 2022 2222 4672 6565 7320 7468 6520     """Frees the 
-00017c40: 6669 7273 7420 6275 6666 6572 2065 6e74  first buffer ent
-00017c50: 7279 2e22 2222 0a20 2020 2064 6566 206d  ry.""".    def m
-00017c60: 6179 6265 5f66 7265 655f 6275 6666 6572  aybe_free_buffer
-00017c70: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-00017c80: 2020 2020 2020 2020 2222 2246 7265 6520          """Free 
-00017c90: 756e 7573 6564 206d 656d 6f72 7922 2222  unused memory"""
-00017ca0: 0a20 2020 2064 6566 2062 7566 6665 725f  .    def buffer_
-00017cb0: 6361 7061 6369 7479 2873 656c 6629 202d  capacity(self) -
-00017cc0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
-00017cd0: 2222 4361 7061 6369 7479 206f 6620 7468  ""Capacity of th
-00017ce0: 6520 696e 7465 726e 616c 2062 7566 6665  e internal buffe
-00017cf0: 722e 2222 220a 2020 2020 6465 6620 6275  r.""".    def bu
-00017d00: 6666 6572 5f69 735f 616c 6c6f 6361 7465  ffer_is_allocate
-00017d10: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
-00017d20: 0a20 2020 2020 2020 2022 2222 5768 6574  .        """Whet
-00017d30: 6865 7220 6275 6666 6572 2069 7320 616c  her buffer is al
-00017d40: 6c6f 6361 7465 6420 6f72 206e 6f74 2e20  located or not. 
-00017d50: 4974 2773 2066 6f72 2074 6573 7473 2e22  It's for tests."
-00017d60: 2222 0a20 2020 2064 6566 2063 6f75 6e74  "".    def count
-00017d70: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00017d80: 2020 2020 2020 2022 2222 4e75 6d62 6572         """Number
-00017d90: 206f 6620 696e 666c 6967 6874 206d 6573   of inflight mes
-00017da0: 7361 6765 732e 2049 7427 7320 666f 7220  sages. It's for 
-00017db0: 7465 7374 732e 2222 220a 2020 2020 6465  tests.""".    de
-00017dc0: 6620 7365 745f 6361 7028 7365 6c66 2c20  f set_cap(self, 
-00017dd0: 696e 636f 6d69 6e67 5f63 6170 3a20 696e  incoming_cap: in
-00017de0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-00017df0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00017e00: 4164 6a75 7374 2069 6e66 6c69 6768 7420  Adjust inflight 
-00017e10: 6275 6666 6572 2063 6170 6163 6974 792e  buffer capacity.
-00017e20: 2053 6574 2069 7420 746f 2060 3060 2077   Set it to `0` w
-00017e30: 696c 6c20 6469 7361 626c 6520 7468 6520  ill disable the 
-00017e40: 7072 6f67 7265 7373 2e0a 2020 2020 2020  progress..      
-00017e50: 2020 4361 6c6c 696e 6720 6974 2062 6574    Calling it bet
-00017e60: 7765 656e 2060 7365 6c66 2e66 756c 6c28  ween `self.full(
-00017e70: 2960 2061 6e64 2060 7365 6c66 2e61 6464  )` and `self.add
-00017e80: 2829 6020 6361 6e20 6361 7573 6520 6120  ()` can cause a 
-00017e90: 7061 6e69 632e 0a20 2020 2020 2020 2022  panic..        "
-00017ea0: 2222 0a0a 636c 6173 7320 496e 666c 6967  ""..class Inflig
-00017eb0: 6874 7328 5f5f 4150 495f 496e 666c 6967  hts(__API_Inflig
-00017ec0: 6874 7329 3a0a 2020 2020 2222 220a 2020  hts):.    """.  
-00017ed0: 2020 4120 6275 6666 6572 206f 6620 696e    A buffer of in
-00017ee0: 666c 6967 6874 206d 6573 7361 6765 732e  flight messages.
-00017ef0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-00017f00: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00017f10: 2063 6170 3a20 696e 7429 202d 3e20 4e6f   cap: int) -> No
-00017f20: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00017f30: 6d61 6b65 5f72 6566 2873 656c 6629 202d  make_ref(self) -
-00017f40: 3e20 2249 6e66 6c69 6768 7473 5265 6622  > "InflightsRef"
-00017f50: 3a20 2e2e 2e0a 0a63 6c61 7373 2049 6e66  : .....class Inf
-00017f60: 6c69 6768 7473 5265 6628 5f5f 4150 495f  lightsRef(__API_
-00017f70: 496e 666c 6967 6874 7329 3a0a 2020 2020  Inflights):.    
-00017f80: 2222 220a 2020 2020 5265 6665 7265 6e63  """.    Referenc
-00017f90: 6520 7479 7065 206f 6620 3a63 6c61 7373  e type of :class
-00017fa0: 3a60 496e 666c 6967 6874 7352 6566 602e  :`InflightsRef`.
-00017fb0: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-00017fc0: 5f5f 4150 495f 436f 6e66 6967 285f 5f43  __API_Config(__C
-00017fd0: 6c6f 6e65 6162 6c65 293a 0a20 2020 2064  loneable):.    d
-00017fe0: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
-00017ff0: 3e20 2243 6f6e 6669 6722 3a20 2e2e 2e0a  > "Config": ....
-00018000: 2020 2020 6465 6620 6d69 6e5f 656c 6563      def min_elec
-00018010: 7469 6f6e 5f74 6963 6b28 7365 6c66 2920  tion_tick(self) 
-00018020: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00018030: 2222 220a 2020 2020 2020 2020 606d 696e  """.        `min
-00018040: 5f65 6c65 6374 696f 6e5f 7469 636b 603a  _election_tick`:
-00018050: 2054 6865 206d 696e 696d 756d 206e 756d   The minimum num
-00018060: 6265 7220 6f66 2074 6963 6b73 2062 6566  ber of ticks bef
-00018070: 6f72 6520 616e 2065 6c65 6374 696f 6e2e  ore an election.
-00018080: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00018090: 2064 6566 2073 6574 5f6d 696e 5f65 6c65   def set_min_ele
-000180a0: 6374 696f 6e5f 7469 636b 2873 656c 662c  ction_tick(self,
-000180b0: 206d 696e 5f65 6c65 6374 696f 6e5f 7469   min_election_ti
-000180c0: 636b 3a20 696e 7429 202d 3e20 4e6f 6e65  ck: int) -> None
-000180d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000180e0: 2020 2020 2020 606d 696e 5f65 6c65 6374        `min_elect
-000180f0: 696f 6e5f 7469 636b 603a 2054 6865 206d  ion_tick`: The m
-00018100: 696e 696d 756d 206e 756d 6265 7220 6f66  inimum number of
-00018110: 2074 6963 6b73 2062 6566 6f72 6520 616e   ticks before an
-00018120: 2065 6c65 6374 696f 6e2e 0a20 2020 2020   election..     
-00018130: 2020 2022 2222 0a20 2020 2064 6566 206d     """.    def m
-00018140: 6178 5f65 6c65 6374 696f 6e5f 7469 636b  ax_election_tick
-00018150: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00018160: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00018170: 2020 2060 6d61 785f 656c 6563 7469 6f6e     `max_election
-00018180: 5f74 6963 6b60 3a20 5468 6520 6d61 7869  _tick`: The maxi
-00018190: 6d75 6d20 6e75 6d62 6572 206f 6620 7469  mum number of ti
-000181a0: 636b 7320 6265 666f 7265 2061 6e20 656c  cks before an el
-000181b0: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-000181c0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-000181d0: 6d61 785f 656c 6563 7469 6f6e 5f74 6963  max_election_tic
-000181e0: 6b28 7365 6c66 2c20 6d61 785f 656c 6563  k(self, max_elec
-000181f0: 7469 6f6e 5f74 6963 6b3a 2069 6e74 2920  tion_tick: int) 
-00018200: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00018210: 2022 2222 0a20 2020 2020 2020 2060 6d61   """.        `ma
-00018220: 785f 656c 6563 7469 6f6e 5f74 6963 6b60  x_election_tick`
-00018230: 3a20 5468 6520 6d61 7869 6d75 6d20 6e75  : The maximum nu
-00018240: 6d62 6572 206f 6620 7469 636b 7320 6265  mber of ticks be
-00018250: 666f 7265 2061 6e20 656c 6563 7469 6f6e  fore an election
-00018260: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00018270: 2020 6465 6620 6765 745f 7265 6164 5f6f    def get_read_o
-00018280: 6e6c 795f 6f70 7469 6f6e 2873 656c 6629  nly_option(self)
-00018290: 202d 3e20 2252 6561 644f 6e6c 794f 7074   -> "ReadOnlyOpt
-000182a0: 696f 6e22 3a0a 2020 2020 2020 2020 2222  ion":.        ""
-000182b0: 220a 2020 2020 2020 2020 6072 6561 645f  ".        `read_
-000182c0: 6f6e 6c79 5f6f 7074 696f 6e60 3a20 4368  only_option`: Ch
-000182d0: 6f6f 7365 2074 6865 206c 696e 6561 7269  oose the lineari
-000182e0: 7a61 6269 6c69 7479 206d 6f64 6520 6f72  zability mode or
-000182f0: 2074 6865 206c 6561 7365 206d 6f64 6520   the lease mode 
-00018300: 746f 2072 6561 6420 6461 7461 2e20 4966  to read data. If
-00018310: 2079 6f75 2064 6f6e e280 9974 2063 6172   you don...t car
-00018320: 6520 6162 6f75 7420 7468 6520 7265 6164  e about the read
-00018330: 2063 6f6e 7369 7374 656e 6379 2061 6e64   consistency and
-00018340: 2077 616e 7420 6120 6869 6768 6572 2072   want a higher r
-00018350: 6561 6420 7065 7266 6f72 6d61 6e63 652c  ead performance,
-00018360: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00018370: 206c 6561 7365 206d 6f64 652e 0a20 2020   lease mode..   
-00018380: 2020 2020 2053 6574 7469 6e67 2074 6869       Setting thi
-00018390: 7320 746f 2060 4c65 6173 6542 6173 6564  s to `LeaseBased
-000183a0: 6020 7265 7175 6972 6573 2060 6368 6563  ` requires `chec
-000183b0: 6b5f 7175 6f72 756d 203d 2074 7275 6560  k_quorum = true`
-000183c0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000183d0: 2020 6465 6620 7365 745f 7265 6164 5f6f    def set_read_o
-000183e0: 6e6c 795f 6f70 7469 6f6e 2873 656c 662c  nly_option(self,
-000183f0: 2072 6561 645f 6f6e 6c79 5f6f 7074 696f   read_only_optio
-00018400: 6e3a 2022 5265 6164 4f6e 6c79 4f70 7469  n: "ReadOnlyOpti
-00018410: 6f6e 2229 202d 3e20 4e6f 6e65 3a0a 2020  on") -> None:.  
-00018420: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00018430: 2020 6072 6561 645f 6f6e 6c79 5f6f 7074    `read_only_opt
-00018440: 696f 6e60 3a20 4368 6f6f 7365 2074 6865  ion`: Choose the
-00018450: 206c 696e 6561 7269 7a61 6269 6c69 7479   linearizability
-00018460: 206d 6f64 6520 6f72 2074 6865 206c 6561   mode or the lea
-00018470: 7365 206d 6f64 6520 746f 2072 6561 6420  se mode to read 
-00018480: 6461 7461 2e20 4966 2079 6f75 2064 6f6e  data. If you don
-00018490: e280 9974 2063 6172 6520 6162 6f75 7420  ...t care about 
-000184a0: 7468 6520 7265 6164 2063 6f6e 7369 7374  the read consist
-000184b0: 656e 6379 2061 6e64 2077 616e 7420 6120  ency and want a 
-000184c0: 6869 6768 6572 2072 6561 6420 7065 7266  higher read perf
-000184d0: 6f72 6d61 6e63 652c 2079 6f75 2063 616e  ormance, you can
-000184e0: 2075 7365 2074 6865 206c 6561 7365 206d   use the lease m
-000184f0: 6f64 652e 0a20 2020 2020 2020 2053 6574  ode..        Set
-00018500: 7469 6e67 2074 6869 7320 746f 2060 4c65  ting this to `Le
-00018510: 6173 6542 6173 6564 6020 7265 7175 6972  aseBased` requir
-00018520: 6573 2060 6368 6563 6b5f 7175 6f72 756d  es `check_quorum
-00018530: 203d 2074 7275 6560 2e0a 2020 2020 2020   = true`..      
-00018540: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
-00018550: 745f 6964 2873 656c 6629 202d 3e20 696e  t_id(self) -> in
-00018560: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-00018570: 2020 2020 2020 2060 6964 603a 2054 6865         `id`: The
-00018580: 2069 6465 6e74 6974 7920 6f66 2074 6865   identity of the
-00018590: 206c 6f63 616c 2072 6166 742e 2049 7420   local raft. It 
-000185a0: 6361 6e6e 6f74 2062 6520 302c 2061 6e64  cannot be 0, and
-000185b0: 206d 7573 7420 6265 2075 6e69 7175 6520   must be unique 
-000185c0: 696e 2074 6865 2067 726f 7570 2e0a 2020  in the group..  
-000185d0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-000185e0: 6620 7365 745f 6964 2873 656c 662c 2069  f set_id(self, i
-000185f0: 643a 2069 6e74 2920 2d3e 204e 6f6e 653a  d: int) -> None:
-00018600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00018610: 2020 2020 2060 6964 603a 2054 6865 2069       `id`: The i
-00018620: 6465 6e74 6974 7920 6f66 2074 6865 206c  dentity of the l
-00018630: 6f63 616c 2072 6166 742e 2049 7420 6361  ocal raft. It ca
-00018640: 6e6e 6f74 2062 6520 302c 2061 6e64 206d  nnot be 0, and m
-00018650: 7573 7420 6265 2075 6e69 7175 6520 696e  ust be unique in
-00018660: 2074 6865 2067 726f 7570 2e0a 2020 2020   the group..    
-00018670: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00018680: 6765 745f 656c 6563 7469 6f6e 5f74 6963  get_election_tic
-00018690: 6b28 7365 6c66 2920 2d3e 2069 6e74 3a0a  k(self) -> int:.
-000186a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000186b0: 2020 2020 6065 6c65 6374 696f 6e5f 7469      `election_ti
-000186c0: 636b 603a 2054 6865 206e 756d 6265 7220  ck`: The number 
-000186d0: 6f66 206e 6f64 652e 7469 636b 2069 6e76  of node.tick inv
-000186e0: 6f63 6174 696f 6e73 2074 6861 7420 6d75  ocations that mu
-000186f0: 7374 2070 6173 7320 6265 7477 6565 6e0a  st pass between.
-00018700: 2020 2020 2020 2020 656c 6563 7469 6f6e          election
-00018710: 732e 2054 6861 7420 6973 2c20 6966 2061  s. That is, if a
-00018720: 2066 6f6c 6c6f 7765 7220 646f 6573 206e   follower does n
-00018730: 6f74 2072 6563 6569 7665 2061 6e79 206d  ot receive any m
-00018740: 6573 7361 6765 2066 726f 6d20 7468 650a  essage from the.
-00018750: 2020 2020 2020 2020 6c65 6164 6572 206f          leader o
-00018760: 6620 6375 7272 656e 7420 7465 726d 2062  f current term b
-00018770: 6566 6f72 6520 456c 6563 7469 6f6e 5469  efore ElectionTi
-00018780: 636b 2068 6173 2065 6c61 7073 6564 2c20  ck has elapsed, 
-00018790: 6974 2077 696c 6c20 6265 636f 6d65 0a20  it will become. 
-000187a0: 2020 2020 2020 2063 616e 6469 6461 7465         candidate
-000187b0: 2061 6e64 2073 7461 7274 2061 6e20 656c   and start an el
-000187c0: 6563 7469 6f6e 2e20 656c 6563 7469 6f6e  ection. election
-000187d0: 5f74 6963 6b20 6d75 7374 2062 6520 6772  _tick must be gr
-000187e0: 6561 7465 7220 7468 616e 0a20 2020 2020  eater than.     
-000187f0: 2020 2048 6561 7274 6265 6174 5469 636b     HeartbeatTick
-00018800: 2e20 5765 2073 7567 6765 7374 2065 6c65  . We suggest ele
-00018810: 6374 696f 6e5f 7469 636b 203d 2031 3020  ction_tick = 10 
-00018820: 2a20 4865 6172 7462 6561 7454 6963 6b20  * HeartbeatTick 
-00018830: 746f 2061 766f 6964 0a20 2020 2020 2020  to avoid.       
-00018840: 2075 6e6e 6563 6573 7361 7279 206c 6561   unnecessary lea
-00018850: 6465 7220 7377 6974 6368 696e 670a 2020  der switching.  
-00018860: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-00018870: 6620 7365 745f 656c 6563 7469 6f6e 5f74  f set_election_t
-00018880: 6963 6b28 7365 6c66 2c20 656c 6563 7469  ick(self, electi
-00018890: 6f6e 5f74 6963 6b3a 2069 6e74 2920 2d3e  on_tick: int) ->
-000188a0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000188b0: 2222 0a20 2020 2020 2020 2060 656c 6563  "".        `elec
-000188c0: 7469 6f6e 5f74 6963 6b60 3a20 5468 6520  tion_tick`: The 
-000188d0: 6e75 6d62 6572 206f 6620 6e6f 6465 2e74  number of node.t
-000188e0: 6963 6b20 696e 766f 6361 7469 6f6e 7320  ick invocations 
-000188f0: 7468 6174 206d 7573 7420 7061 7373 2062  that must pass b
-00018900: 6574 7765 656e 0a20 2020 2020 2020 2065  etween.        e
-00018910: 6c65 6374 696f 6e73 2e20 5468 6174 2069  lections. That i
-00018920: 732c 2069 6620 6120 666f 6c6c 6f77 6572  s, if a follower
-00018930: 2064 6f65 7320 6e6f 7420 7265 6365 6976   does not receiv
-00018940: 6520 616e 7920 6d65 7373 6167 6520 6672  e any message fr
-00018950: 6f6d 2074 6865 0a20 2020 2020 2020 206c  om the.        l
-00018960: 6561 6465 7220 6f66 2063 7572 7265 6e74  eader of current
-00018970: 2074 6572 6d20 6265 666f 7265 2045 6c65   term before Ele
-00018980: 6374 696f 6e54 6963 6b20 6861 7320 656c  ctionTick has el
-00018990: 6170 7365 642c 2069 7420 7769 6c6c 2062  apsed, it will b
-000189a0: 6563 6f6d 650a 2020 2020 2020 2020 6361  ecome.        ca
-000189b0: 6e64 6964 6174 6520 616e 6420 7374 6172  ndidate and star
-000189c0: 7420 616e 2065 6c65 6374 696f 6e2e 2065  t an election. e
-000189d0: 6c65 6374 696f 6e5f 7469 636b 206d 7573  lection_tick mus
-000189e0: 7420 6265 2067 7265 6174 6572 2074 6861  t be greater tha
-000189f0: 6e0a 2020 2020 2020 2020 4865 6172 7462  n.        Heartb
-00018a00: 6561 7454 6963 6b2e 2057 6520 7375 6767  eatTick. We sugg
-00018a10: 6573 7420 656c 6563 7469 6f6e 5f74 6963  est election_tic
-00018a20: 6b20 3d20 3130 202a 2048 6561 7274 6265  k = 10 * Heartbe
-00018a30: 6174 5469 636b 2074 6f20 6176 6f69 640a  atTick to avoid.
-00018a40: 2020 2020 2020 2020 756e 6e65 6365 7373          unnecess
-00018a50: 6172 7920 6c65 6164 6572 2073 7769 7463  ary leader switc
-00018a60: 6869 6e67 0a20 2020 2020 2020 2022 2222  hing.        """
-00018a70: 0a20 2020 2064 6566 2067 6574 5f68 6561  .    def get_hea
-00018a80: 7274 6265 6174 5f74 6963 6b28 7365 6c66  rtbeat_tick(self
-00018a90: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00018aa0: 2020 2222 220a 2020 2020 2020 2020 6068    """.        `h
-00018ab0: 6561 7274 6265 6174 5f74 6963 6b60 3a20  eartbeat_tick`: 
-00018ac0: 4865 6172 7462 6561 7454 6963 6b20 6973  HeartbeatTick is
-00018ad0: 2074 6865 206e 756d 6265 7220 6f66 206e   the number of n
-00018ae0: 6f64 652e 7469 636b 2069 6e76 6f63 6174  ode.tick invocat
-00018af0: 696f 6e73 2074 6861 7420 6d75 7374 2070  ions that must p
-00018b00: 6173 7320 6265 7477 6565 6e0a 2020 2020  ass between.    
-00018b10: 2020 2020 6865 6172 7462 6561 7473 2e20      heartbeats. 
-00018b20: 5468 6174 2069 732c 2061 206c 6561 6465  That is, a leade
-00018b30: 7220 7365 6e64 7320 6865 6172 7462 6561  r sends heartbea
-00018b40: 7420 6d65 7373 6167 6573 2074 6f20 6d61  t messages to ma
-00018b50: 696e 7461 696e 2069 7473 0a20 2020 2020  intain its.     
-00018b60: 2020 206c 6561 6465 7273 6869 7020 6576     leadership ev
-00018b70: 6572 7920 6865 6172 7462 6561 7420 7469  ery heartbeat ti
-00018b80: 636b 732e 0a20 2020 2020 2020 2022 2222  cks..        """
-00018b90: 0a20 2020 2064 6566 2073 6574 5f68 6561  .    def set_hea
-00018ba0: 7274 6265 6174 5f74 6963 6b28 7365 6c66  rtbeat_tick(self
-00018bb0: 2c20 6865 6172 7462 6561 745f 7469 636b  , heartbeat_tick
-00018bc0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
-00018bd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00018be0: 2020 2020 6068 6561 7274 6265 6174 5f74      `heartbeat_t
-00018bf0: 6963 6b60 3a20 4865 6172 7462 6561 7454  ick`: HeartbeatT
-00018c00: 6963 6b20 6973 2074 6865 206e 756d 6265  ick is the numbe
-00018c10: 7220 6f66 206e 6f64 652e 7469 636b 2069  r of node.tick i
-00018c20: 6e76 6f63 6174 696f 6e73 2074 6861 7420  nvocations that 
-00018c30: 6d75 7374 2070 6173 7320 6265 7477 6565  must pass betwee
-00018c40: 6e0a 2020 2020 2020 2020 6865 6172 7462  n.        heartb
-00018c50: 6561 7473 2e20 5468 6174 2069 732c 2061  eats. That is, a
-00018c60: 206c 6561 6465 7220 7365 6e64 7320 6865   leader sends he
-00018c70: 6172 7462 6561 7420 6d65 7373 6167 6573  artbeat messages
-00018c80: 2074 6f20 6d61 696e 7461 696e 2069 7473   to maintain its
-00018c90: 0a20 2020 2020 2020 206c 6561 6465 7273  .        leaders
-00018ca0: 6869 7020 6576 6572 7920 6865 6172 7462  hip every heartb
-00018cb0: 6561 7420 7469 636b 732e 0a20 2020 2020  eat ticks..     
-00018cc0: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
-00018cd0: 6574 5f6d 6178 5f73 697a 655f 7065 725f  et_max_size_per_
-00018ce0: 6d73 6728 7365 6c66 2920 2d3e 2069 6e74  msg(self) -> int
-00018cf0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00018d00: 2020 2020 2020 606d 6178 5f73 697a 655f        `max_size_
-00018d10: 7065 725f 6d73 6760 3a20 4c69 6d69 7420  per_msg`: Limit 
-00018d20: 7468 6520 6d61 7820 7369 7a65 206f 6620  the max size of 
-00018d30: 6561 6368 2061 7070 656e 6420 6d65 7373  each append mess
-00018d40: 6167 652e 2053 6d61 6c6c 6572 2076 616c  age. Smaller val
-00018d50: 7565 206c 6f77 6572 730a 2020 2020 2020  ue lowers.      
-00018d60: 2020 7468 6520 7261 6674 2072 6563 6f76    the raft recov
-00018d70: 6572 7920 636f 7374 2869 6e69 7469 616c  ery cost(initial
-00018d80: 2070 726f 6269 6e67 2061 6e64 206d 6573   probing and mes
-00018d90: 7361 6765 206c 6f73 7420 6475 7269 6e67  sage lost during
-00018da0: 206e 6f72 6d61 6c20 6f70 6572 6174 696f   normal operatio
-00018db0: 6e29 2e0a 2020 2020 2020 2020 4f6e 2074  n)..        On t
-00018dc0: 6865 206f 7468 6572 2073 6964 652c 2069  he other side, i
-00018dd0: 7420 6d69 6768 7420 6166 6665 6374 2074  t might affect t
-00018de0: 6865 2074 6872 6f75 6768 7075 7420 6475  he throughput du
-00018df0: 7269 6e67 206e 6f72 6d61 6c20 7265 706c  ring normal repl
-00018e00: 6963 6174 696f 6e2e 0a20 2020 2020 2020  ication..       
-00018e10: 204e 6f74 653a 206d 6174 682e 4d61 7855   Note: math.MaxU
-00018e20: 7573 697a 6536 3420 666f 7220 756e 6c69  usize64 for unli
-00018e30: 6d69 7465 642c 2030 2066 6f72 2061 7420  mited, 0 for at 
-00018e40: 6d6f 7374 206f 6e65 2065 6e74 7279 2070  most one entry p
-00018e50: 6572 206d 6573 7361 6765 2e0a 2020 2020  er message..    
-00018e60: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00018e70: 7365 745f 6d61 785f 7369 7a65 5f70 6572  set_max_size_per
-00018e80: 5f6d 7367 2873 656c 662c 206d 6178 5f73  _msg(self, max_s
-00018e90: 697a 655f 7065 725f 6d73 673a 2069 6e74  ize_per_msg: int
-00018ea0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00018eb0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00018ec0: 6d61 785f 7369 7a65 5f70 6572 5f6d 7367  max_size_per_msg
-00018ed0: 603a 204c 696d 6974 2074 6865 206d 6178  `: Limit the max
-00018ee0: 2073 697a 6520 6f66 2065 6163 6820 6170   size of each ap
-00018ef0: 7065 6e64 206d 6573 7361 6765 2e20 536d  pend message. Sm
-00018f00: 616c 6c65 7220 7661 6c75 6520 6c6f 7765  aller value lowe
-00018f10: 7273 0a20 2020 2020 2020 2074 6865 2072  rs.        the r
-00018f20: 6166 7420 7265 636f 7665 7279 2063 6f73  aft recovery cos
-00018f30: 7428 696e 6974 6961 6c20 7072 6f62 696e  t(initial probin
-00018f40: 6720 616e 6420 6d65 7373 6167 6520 6c6f  g and message lo
-00018f50: 7374 2064 7572 696e 6720 6e6f 726d 616c  st during normal
-00018f60: 206f 7065 7261 7469 6f6e 292e 0a20 2020   operation)..   
-00018f70: 2020 2020 204f 6e20 7468 6520 6f74 6865       On the othe
-00018f80: 7220 7369 6465 2c20 6974 206d 6967 6874  r side, it might
-00018f90: 2061 6666 6563 7420 7468 6520 7468 726f   affect the thro
-00018fa0: 7567 6870 7574 2064 7572 696e 6720 6e6f  ughput during no
-00018fb0: 726d 616c 2072 6570 6c69 6361 7469 6f6e  rmal replication
-00018fc0: 2e0a 2020 2020 2020 2020 4e6f 7465 3a20  ..        Note: 
-00018fd0: 6d61 7468 2e4d 6178 5575 7369 7a65 3634  math.MaxUusize64
-00018fe0: 2066 6f72 2075 6e6c 696d 6974 6564 2c20   for unlimited, 
-00018ff0: 3020 666f 7220 6174 206d 6f73 7420 6f6e  0 for at most on
-00019000: 6520 656e 7472 7920 7065 7220 6d65 7373  e entry per mess
-00019010: 6167 652e 0a20 2020 2020 2020 2022 2222  age..        """
-00019020: 0a20 2020 2064 6566 2067 6574 5f6d 6178  .    def get_max
-00019030: 5f69 6e66 6c69 6768 745f 6d73 6773 2873  _inflight_msgs(s
-00019040: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
-00019050: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00019060: 2060 6d61 785f 696e 666c 6967 6874 5f6d   `max_inflight_m
-00019070: 7367 7360 3a20 4c69 6d69 7420 7468 6520  sgs`: Limit the 
-00019080: 6d61 7820 6e75 6d62 6572 206f 6620 696e  max number of in
-00019090: 2d66 6c69 6768 7420 6170 7065 6e64 206d  -flight append m
-000190a0: 6573 7361 6765 7320 6475 7269 6e67 206f  essages during o
-000190b0: 7074 696d 6973 7469 630a 2020 2020 2020  ptimistic.      
-000190c0: 2020 7265 706c 6963 6174 696f 6e20 7068    replication ph
-000190d0: 6173 652e 2054 6865 2061 7070 6c69 6361  ase. The applica
-000190e0: 7469 6f6e 2074 7261 6e73 706f 7274 6174  tion transportat
-000190f0: 696f 6e20 6c61 7965 7220 7573 7561 6c6c  ion layer usuall
-00019100: 7920 6861 7320 6974 7320 6f77 6e20 7365  y has its own se
-00019110: 6e64 696e 670a 2020 2020 2020 2020 6275  nding.        bu
-00019120: 6666 6572 206f 7665 7220 5443 502f 5544  ffer over TCP/UD
-00019130: 502e 2053 6574 2074 6f20 6176 6f69 6420  P. Set to avoid 
-00019140: 6f76 6572 666c 6f77 696e 6720 7468 6174  overflowing that
-00019150: 2073 656e 6469 6e67 2062 7566 6665 722e   sending buffer.
-00019160: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019170: 2064 6566 2073 6574 5f6d 6178 5f69 6e66   def set_max_inf
-00019180: 6c69 6768 745f 6d73 6773 2873 656c 662c  light_msgs(self,
-00019190: 206d 6178 5f69 6e66 6c69 6768 745f 6d73   max_inflight_ms
-000191a0: 6773 3a20 696e 7429 202d 3e20 4e6f 6e65  gs: int) -> None
-000191b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000191c0: 2020 2020 2020 606d 6178 5f69 6e66 6c69        `max_infli
-000191d0: 6768 745f 6d73 6773 603a 204c 696d 6974  ght_msgs`: Limit
-000191e0: 2074 6865 206d 6178 206e 756d 6265 7220   the max number 
-000191f0: 6f66 2069 6e2d 666c 6967 6874 2061 7070  of in-flight app
-00019200: 656e 6420 6d65 7373 6167 6573 2064 7572  end messages dur
-00019210: 696e 6720 6f70 7469 6d69 7374 6963 0a20  ing optimistic. 
-00019220: 2020 2020 2020 2072 6570 6c69 6361 7469         replicati
-00019230: 6f6e 2070 6861 7365 2e20 5468 6520 6170  on phase. The ap
-00019240: 706c 6963 6174 696f 6e20 7472 616e 7370  plication transp
-00019250: 6f72 7461 7469 6f6e 206c 6179 6572 2075  ortation layer u
-00019260: 7375 616c 6c79 2068 6173 2069 7473 206f  sually has its o
-00019270: 776e 2073 656e 6469 6e67 0a20 2020 2020  wn sending.     
-00019280: 2020 2062 7566 6665 7220 6f76 6572 2054     buffer over T
-00019290: 4350 2f55 4450 2e20 5365 7420 746f 2061  CP/UDP. Set to a
-000192a0: 766f 6964 206f 7665 7266 6c6f 7769 6e67  void overflowing
-000192b0: 2074 6861 7420 7365 6e64 696e 6720 6275   that sending bu
-000192c0: 6666 6572 2e0a 2020 2020 2020 2020 2222  ffer..        ""
-000192d0: 220a 2020 2020 6465 6620 6765 745f 6170  ".    def get_ap
-000192e0: 706c 6965 6428 7365 6c66 2920 2d3e 2069  plied(self) -> i
-000192f0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
-00019300: 2020 2020 2020 2020 6061 7070 6c69 6564          `applied
-00019310: 603a 2041 7070 6c69 6564 2069 7320 7468  `: Applied is th
-00019320: 6520 6c61 7374 2061 7070 6c69 6564 2069  e last applied i
-00019330: 6e64 6578 2e20 4974 2073 686f 756c 6420  ndex. It should 
-00019340: 6f6e 6c79 2062 6520 7365 7420 7768 656e  only be set when
-00019350: 2072 6573 7461 7274 696e 670a 2020 2020   restarting.    
-00019360: 2020 2020 7261 6674 2e20 7261 6674 2077      raft. raft w
-00019370: 696c 6c20 6e6f 7420 7265 7475 726e 2065  ill not return e
-00019380: 6e74 7269 6573 2074 6f20 7468 6520 6170  ntries to the ap
-00019390: 706c 6963 6174 696f 6e20 736d 616c 6c65  plication smalle
-000193a0: 7220 6f72 2065 7175 616c 2074 6f20 4170  r or equal to Ap
-000193b0: 706c 6965 642e 0a20 2020 2020 2020 2049  plied..        I
-000193c0: 6620 4170 706c 6965 6420 6973 2075 6e73  f Applied is uns
-000193d0: 6574 2077 6865 6e20 7265 7374 6172 7469  et when restarti
-000193e0: 6e67 2c20 7261 6674 206d 6967 6874 2072  ng, raft might r
-000193f0: 6574 7572 6e20 7072 6576 696f 7573 2061  eturn previous a
-00019400: 7070 6c69 6564 2065 6e74 7269 6573 2e0a  pplied entries..
-00019410: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-00019420: 6120 7665 7279 2061 7070 6c69 6361 7469  a very applicati
-00019430: 6f6e 2064 6570 656e 6465 6e74 2063 6f6e  on dependent con
-00019440: 6669 6775 7261 7469 6f6e 2e0a 2020 2020  figuration..    
-00019450: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00019460: 7365 745f 6170 706c 6965 6428 7365 6c66  set_applied(self
-00019470: 2c20 6170 706c 6965 643a 2069 6e74 2920  , applied: int) 
-00019480: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00019490: 2022 2222 0a20 2020 2020 2020 2060 6170   """.        `ap
-000194a0: 706c 6965 6460 3a20 4170 706c 6965 6420  plied`: Applied 
-000194b0: 6973 2074 6865 206c 6173 7420 6170 706c  is the last appl
-000194c0: 6965 6420 696e 6465 782e 2049 7420 7368  ied index. It sh
-000194d0: 6f75 6c64 206f 6e6c 7920 6265 2073 6574  ould only be set
-000194e0: 2077 6865 6e20 7265 7374 6172 7469 6e67   when restarting
-000194f0: 0a20 2020 2020 2020 2072 6166 742e 2072  .        raft. r
-00019500: 6166 7420 7769 6c6c 206e 6f74 2072 6574  aft will not ret
-00019510: 7572 6e20 656e 7472 6965 7320 746f 2074  urn entries to t
-00019520: 6865 2061 7070 6c69 6361 7469 6f6e 2073  he application s
-00019530: 6d61 6c6c 6572 206f 7220 6571 7561 6c20  maller or equal 
-00019540: 746f 2041 7070 6c69 6564 2e0a 2020 2020  to Applied..    
-00019550: 2020 2020 4966 2041 7070 6c69 6564 2069      If Applied i
-00019560: 7320 756e 7365 7420 7768 656e 2072 6573  s unset when res
-00019570: 7461 7274 696e 672c 2072 6166 7420 6d69  tarting, raft mi
-00019580: 6768 7420 7265 7475 726e 2070 7265 7669  ght return previ
-00019590: 6f75 7320 6170 706c 6965 6420 656e 7472  ous applied entr
-000195a0: 6965 732e 0a20 2020 2020 2020 2054 6869  ies..        Thi
-000195b0: 7320 6973 2061 2076 6572 7920 6170 706c  s is a very appl
-000195c0: 6963 6174 696f 6e20 6465 7065 6e64 656e  ication dependen
-000195d0: 7420 636f 6e66 6967 7572 6174 696f 6e2e  t configuration.
-000195e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000195f0: 2064 6566 2067 6574 5f63 6865 636b 5f71   def get_check_q
-00019600: 756f 7275 6d28 7365 6c66 2920 2d3e 2062  uorum(self) -> b
-00019610: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00019620: 0a20 2020 2020 2020 2060 6368 6563 6b5f  .        `check_
-00019630: 7175 6f72 756d 603a 2053 7065 6369 6679  quorum`: Specify
-00019640: 2069 6620 7468 6520 6c65 6164 6572 2073   if the leader s
-00019650: 686f 756c 6420 6368 6563 6b20 7175 6f72  hould check quor
-00019660: 756d 2061 6374 6976 6974 792e 204c 6561  um activity. Lea
-00019670: 6465 7220 7374 6570 7320 646f 776e 2077  der steps down w
-00019680: 6865 6e0a 2020 2020 2020 2020 7175 6f72  hen.        quor
-00019690: 756d 2069 7320 6e6f 7420 6163 7469 7665  um is not active
-000196a0: 2066 6f72 2061 6e20 656c 6563 7469 6f6e   for an election
-000196b0: 5469 6d65 6f75 742e 0a20 2020 2020 2020  Timeout..       
-000196c0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
-000196d0: 5f63 6865 636b 5f71 756f 7275 6d28 7365  _check_quorum(se
-000196e0: 6c66 2c20 6368 6563 6b5f 7175 6f72 756d  lf, check_quorum
-000196f0: 3a20 626f 6f6c 2920 2d3e 204e 6f6e 653a  : bool) -> None:
-00019700: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019710: 2020 2020 2060 6368 6563 6b5f 7175 6f72       `check_quor
-00019720: 756d 603a 2053 7065 6369 6679 2069 6620  um`: Specify if 
-00019730: 7468 6520 6c65 6164 6572 2073 686f 756c  the leader shoul
-00019740: 6420 6368 6563 6b20 7175 6f72 756d 2061  d check quorum a
-00019750: 6374 6976 6974 792e 204c 6561 6465 7220  ctivity. Leader 
-00019760: 7374 6570 7320 646f 776e 2077 6865 6e0a  steps down when.
-00019770: 2020 2020 2020 2020 7175 6f72 756d 2069          quorum i
-00019780: 7320 6e6f 7420 6163 7469 7665 2066 6f72  s not active for
-00019790: 2061 6e20 656c 6563 7469 6f6e 5469 6d65   an electionTime
-000197a0: 6f75 742e 0a20 2020 2020 2020 2022 2222  out..        """
-000197b0: 0a20 2020 2064 6566 2067 6574 5f70 7265  .    def get_pre
-000197c0: 5f76 6f74 6528 7365 6c66 2920 2d3e 2062  _vote(self) -> b
-000197d0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-000197e0: 0a20 2020 2020 2020 2060 7072 655f 766f  .        `pre_vo
-000197f0: 7465 603a 2045 6e61 626c 6573 2074 6865  te`: Enables the
-00019800: 2050 7265 2d56 6f74 6520 616c 676f 7269   Pre-Vote algori
-00019810: 7468 6d20 6465 7363 7269 6265 6420 696e  thm described in
-00019820: 2072 6166 7420 7468 6573 6973 2073 6563   raft thesis sec
-00019830: 7469 6f6e 0a20 2020 2020 2020 2039 2e36  tion.        9.6
-00019840: 2e20 5468 6973 2070 7265 7665 6e74 7320  . This prevents 
-00019850: 6469 7372 7570 7469 6f6e 2077 6865 6e20  disruption when 
-00019860: 6120 6e6f 6465 2074 6861 7420 6861 7320  a node that has 
-00019870: 6265 656e 2070 6172 7469 7469 6f6e 6564  been partitioned
-00019880: 2061 7761 790a 2020 2020 2020 2020 7265   away.        re
-00019890: 6a6f 696e 7320 7468 6520 636c 7573 7465  joins the cluste
-000198a0: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-000198b0: 2020 2064 6566 2073 6574 5f70 7265 5f76     def set_pre_v
-000198c0: 6f74 6528 7365 6c66 2c20 7072 655f 766f  ote(self, pre_vo
-000198d0: 7465 3a20 626f 6f6c 2920 2d3e 204e 6f6e  te: bool) -> Non
-000198e0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-000198f0: 2020 2020 2020 2060 7072 655f 766f 7465         `pre_vote
-00019900: 603a 2045 6e61 626c 6573 2074 6865 2050  `: Enables the P
-00019910: 7265 2d56 6f74 6520 616c 676f 7269 7468  re-Vote algorith
-00019920: 6d20 6465 7363 7269 6265 6420 696e 2072  m described in r
-00019930: 6166 7420 7468 6573 6973 2073 6563 7469  aft thesis secti
-00019940: 6f6e 0a20 2020 2020 2020 2039 2e36 2e20  on.        9.6. 
-00019950: 5468 6973 2070 7265 7665 6e74 7320 6469  This prevents di
-00019960: 7372 7570 7469 6f6e 2077 6865 6e20 6120  sruption when a 
-00019970: 6e6f 6465 2074 6861 7420 6861 7320 6265  node that has be
-00019980: 656e 2070 6172 7469 7469 6f6e 6564 2061  en partitioned a
-00019990: 7761 790a 2020 2020 2020 2020 7265 6a6f  way.        rejo
-000199a0: 696e 7320 7468 6520 636c 7573 7465 722e  ins the cluster.
-000199b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000199c0: 2064 6566 2067 6574 5f62 6174 6368 5f61   def get_batch_a
-000199d0: 7070 656e 6428 7365 6c66 2920 2d3e 2062  ppend(self) -> b
-000199e0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-000199f0: 0a20 2020 2020 2020 2060 6261 7463 685f  .        `batch_
-00019a00: 6170 7065 6e64 603a 2042 6174 6368 6573  append`: Batches
-00019a10: 2065 7665 7279 2061 7070 656e 6420 6d73   every append ms
-00019a20: 6720 6966 2061 6e79 2061 7070 656e 6420  g if any append 
-00019a30: 6d73 6720 616c 7265 6164 7920 6578 6973  msg already exis
-00019a40: 7473 0a20 2020 2020 2020 2022 2222 0a20  ts.        """. 
-00019a50: 2020 2064 6566 2073 6574 5f62 6174 6368     def set_batch
-00019a60: 5f61 7070 656e 6428 7365 6c66 2c20 6261  _append(self, ba
-00019a70: 7463 685f 6170 7065 6e64 3a20 626f 6f6c  tch_append: bool
-00019a80: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00019a90: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
-00019aa0: 6261 7463 685f 6170 7065 6e64 603a 2042  batch_append`: B
-00019ab0: 6174 6368 6573 2065 7665 7279 2061 7070  atches every app
-00019ac0: 656e 6420 6d73 6720 6966 2061 6e79 2061  end msg if any a
-00019ad0: 7070 656e 6420 6d73 6720 616c 7265 6164  ppend msg alread
-00019ae0: 7920 6578 6973 7473 0a20 2020 2020 2020  y exists.       
-00019af0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
-00019b00: 5f73 6b69 705f 6263 6173 745f 636f 6d6d  _skip_bcast_comm
-00019b10: 6974 2873 656c 6629 202d 3e20 626f 6f6c  it(self) -> bool
-00019b20: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00019b30: 2020 2020 2020 6073 6b69 705f 6263 6173        `skip_bcas
-00019b40: 745f 636f 6d6d 6974 603a 2044 6f6e 2774  t_commit`: Don't
-00019b50: 2062 726f 6164 6361 7374 2061 6e20 656d   broadcast an em
-00019b60: 7074 7920 7261 6674 2065 6e74 7279 2074  pty raft entry t
-00019b70: 6f20 6e6f 7469 6679 2066 6f6c 6c6f 7765  o notify followe
-00019b80: 7220 746f 2063 6f6d 6d69 7420 616e 2065  r to commit an e
-00019b90: 6e74 7279 2e0a 2020 2020 2020 2020 5468  ntry..        Th
-00019ba0: 6973 206d 6179 206d 616b 6520 666f 6c6c  is may make foll
-00019bb0: 6f77 6572 2077 6169 7420 6120 6c6f 6e67  ower wait a long
-00019bc0: 6572 2074 696d 6520 746f 2061 7070 6c79  er time to apply
-00019bd0: 2061 6e20 656e 7472 792e 2054 6869 7320   an entry. This 
-00019be0: 636f 6e66 6967 7572 6174 696f 6e0a 2020  configuration.  
-00019bf0: 2020 2020 2020 4d61 7920 6166 6665 6374        May affect
-00019c00: 2070 726f 706f 7361 6c20 666f 7277 6172   proposal forwar
-00019c10: 6469 6e67 2061 6e64 2066 6f6c 6c6f 7765  ding and followe
-00019c20: 7220 7265 6164 2e0a 2020 2020 2020 2020  r read..        
-00019c30: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
-00019c40: 736b 6970 5f62 6361 7374 5f63 6f6d 6d69  skip_bcast_commi
-00019c50: 7428 7365 6c66 2c20 736b 6970 5f62 6361  t(self, skip_bca
-00019c60: 7374 5f63 6f6d 6d69 743a 2062 6f6f 6c29  st_commit: bool)
-00019c70: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00019c80: 2020 2222 220a 2020 2020 2020 2020 6073    """.        `s
-00019c90: 6b69 705f 6263 6173 745f 636f 6d6d 6974  kip_bcast_commit
-00019ca0: 603a 2044 6f6e 2774 2062 726f 6164 6361  `: Don't broadca
-00019cb0: 7374 2061 6e20 656d 7074 7920 7261 6674  st an empty raft
-00019cc0: 2065 6e74 7279 2074 6f20 6e6f 7469 6679   entry to notify
-00019cd0: 2066 6f6c 6c6f 7765 7220 746f 2063 6f6d   follower to com
-00019ce0: 6d69 7420 616e 2065 6e74 7279 2e0a 2020  mit an entry..  
-00019cf0: 2020 2020 2020 5468 6973 206d 6179 206d        This may m
-00019d00: 616b 6520 666f 6c6c 6f77 6572 2077 6169  ake follower wai
-00019d10: 7420 6120 6c6f 6e67 6572 2074 696d 6520  t a longer time 
-00019d20: 746f 2061 7070 6c79 2061 6e20 656e 7472  to apply an entr
-00019d30: 792e 2054 6869 7320 636f 6e66 6967 7572  y. This configur
-00019d40: 6174 696f 6e0a 2020 2020 2020 2020 4d61  ation.        Ma
-00019d50: 7920 6166 6665 6374 2070 726f 706f 7361  y affect proposa
-00019d60: 6c20 666f 7277 6172 6469 6e67 2061 6e64  l forwarding and
-00019d70: 2066 6f6c 6c6f 7765 7220 7265 6164 2e0a   follower read..
-00019d80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00019d90: 6465 6620 6765 745f 7072 696f 7269 7479  def get_priority
-00019da0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
-00019db0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00019dc0: 2020 2060 7072 696f 7269 7479 603a 2054     `priority`: T
-00019dd0: 6865 2065 6c65 6374 696f 6e20 7072 696f  he election prio
-00019de0: 7269 7479 206f 6620 7468 6973 206e 6f64  rity of this nod
-00019df0: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00019e00: 2020 2064 6566 2073 6574 5f70 7269 6f72     def set_prior
-00019e10: 6974 7928 7365 6c66 2c20 7072 696f 7269  ity(self, priori
-00019e20: 7479 3a20 696e 7429 202d 3e20 4e6f 6e65  ty: int) -> None
-00019e30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00019e40: 2020 2020 2020 6070 7269 6f72 6974 7960        `priority`
-00019e50: 3a20 5468 6520 656c 6563 7469 6f6e 2070  : The election p
-00019e60: 7269 6f72 6974 7920 6f66 2074 6869 7320  riority of this 
-00019e70: 6e6f 6465 2e0a 2020 2020 2020 2020 2222  node..        ""
-00019e80: 220a 2020 2020 6465 6620 6765 745f 6d61  ".    def get_ma
-00019e90: 785f 756e 636f 6d6d 6974 7465 645f 7369  x_uncommitted_si
-00019ea0: 7a65 2873 656c 6629 202d 3e20 696e 743a  ze(self) -> int:
-00019eb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019ec0: 2020 2020 2060 6d61 785f 756e 636f 6d6d       `max_uncomm
-00019ed0: 6974 7465 645f 7369 7a65 603a 2053 7065  itted_size`: Spe
-00019ee0: 6369 6679 206d 6178 696d 756d 206f 6620  cify maximum of 
-00019ef0: 756e 636f 6d6d 6974 7465 6420 656e 7472  uncommitted entr
-00019f00: 7920 7369 7a65 2e0a 2020 2020 2020 2020  y size..        
-00019f10: 5768 656e 2074 6869 7320 6c69 6d69 7420  When this limit 
-00019f20: 6973 2072 6561 6368 6564 2c20 616c 6c20  is reached, all 
-00019f30: 7072 6f70 6f73 616c 7320 746f 2061 7070  proposals to app
-00019f40: 656e 6420 6e65 7720 6c6f 6720 7769 6c6c  end new log will
-00019f50: 2062 6520 6472 6f70 7065 640a 2020 2020   be dropped.    
-00019f60: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
-00019f70: 7365 745f 6d61 785f 756e 636f 6d6d 6974  set_max_uncommit
-00019f80: 7465 645f 7369 7a65 2873 656c 662c 206d  ted_size(self, m
-00019f90: 6178 5f75 6e63 6f6d 6d69 7474 6564 5f73  ax_uncommitted_s
-00019fa0: 697a 653a 2069 6e74 2920 2d3e 204e 6f6e  ize: int) -> Non
-00019fb0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00019fc0: 2020 2020 2020 2060 6d61 785f 756e 636f         `max_unco
-00019fd0: 6d6d 6974 7465 645f 7369 7a65 603a 2053  mmitted_size`: S
-00019fe0: 7065 6369 6679 206d 6178 696d 756d 206f  pecify maximum o
-00019ff0: 6620 756e 636f 6d6d 6974 7465 6420 656e  f uncommitted en
-0001a000: 7472 7920 7369 7a65 2e0a 2020 2020 2020  try size..      
-0001a010: 2020 5768 656e 2074 6869 7320 6c69 6d69    When this limi
-0001a020: 7420 6973 2072 6561 6368 6564 2c20 616c  t is reached, al
-0001a030: 6c20 7072 6f70 6f73 616c 7320 746f 2061  l proposals to a
-0001a040: 7070 656e 6420 6e65 7720 6c6f 6720 7769  ppend new log wi
-0001a050: 6c6c 2062 6520 6472 6f70 7065 640a 2020  ll be dropped.  
-0001a060: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0001a070: 6620 6765 745f 6d61 785f 636f 6d6d 6974  f get_max_commit
-0001a080: 7465 645f 7369 7a65 5f70 6572 5f72 6561  ted_size_per_rea
-0001a090: 6479 2873 656c 6629 202d 3e20 696e 743a  dy(self) -> int:
-0001a0a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0001a0b0: 2020 2020 2060 6d61 785f 636f 6d6d 6974       `max_commit
-0001a0c0: 7465 645f 7369 7a65 5f70 6572 5f72 6561  ted_size_per_rea
-0001a0d0: 6479 603a 204d 6178 2073 697a 6520 666f  dy`: Max size fo
-0001a0e0: 7220 636f 6d6d 6974 7465 6420 656e 7472  r committed entr
-0001a0f0: 6965 7320 696e 2061 2060 5265 6164 7960  ies in a `Ready`
-0001a100: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0001a110: 2020 6465 6620 7365 745f 6d61 785f 636f    def set_max_co
-0001a120: 6d6d 6974 7465 645f 7369 7a65 5f70 6572  mmitted_size_per
-0001a130: 5f72 6561 6479 280a 2020 2020 2020 2020  _ready(.        
-0001a140: 7365 6c66 2c20 6d61 785f 636f 6d6d 6974  self, max_commit
-0001a150: 7465 645f 7369 7a65 5f70 6572 5f72 6561  ted_size_per_rea
-0001a160: 6479 3a20 696e 740a 2020 2020 2920 2d3e  dy: int.    ) ->
-0001a170: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0001a180: 2222 0a20 2020 2020 2020 2060 6d61 785f  "".        `max_
-0001a190: 636f 6d6d 6974 7465 645f 7369 7a65 5f70  committed_size_p
-0001a1a0: 6572 5f72 6561 6479 603a 204d 6178 2073  er_ready`: Max s
-0001a1b0: 697a 6520 666f 7220 636f 6d6d 6974 7465  ize for committe
-0001a1c0: 6420 656e 7472 6965 7320 696e 2061 2060  d entries in a `
-0001a1d0: 5265 6164 7960 2e0a 2020 2020 2020 2020  Ready`..        
-0001a1e0: 2222 220a 2020 2020 6465 6620 7661 6c69  """.    def vali
-0001a1f0: 6461 7465 2873 656c 6629 202d 3e20 4e6f  date(self) -> No
-0001a200: 6e65 3a0a 2020 2020 2020 2020 2222 2252  ne:.        """R
-0001a210: 756e 7320 7661 6c69 6461 7469 6f6e 7320  uns validations 
-0001a220: 6167 6169 6e73 7420 7468 6520 636f 6e66  against the conf
-0001a230: 6967 2e22 2222 0a0a 636c 6173 7320 436f  ig."""..class Co
-0001a240: 6e66 6967 285f 5f41 5049 5f43 6f6e 6669  nfig(__API_Confi
-0001a250: 6729 3a0a 2020 2020 2222 220a 2020 2020  g):.    """.    
-0001a260: 436f 6e66 6967 2063 6f6e 7461 696e 7320  Config contains 
-0001a270: 7468 6520 7061 7261 6d65 7465 7273 2074  the parameters t
-0001a280: 6f20 7374 6172 7420 6120 7261 6674 2e0a  o start a raft..
-0001a290: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-0001a2a0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-0001a2b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0001a2c0: 202a 2c0a 2020 2020 2020 2020 6964 3a20   *,.        id: 
-0001a2d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-0001a2e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656c  None,.        el
-0001a2f0: 6563 7469 6f6e 5f74 6963 6b3a 204f 7074  ection_tick: Opt
-0001a300: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-0001a310: 652c 0a20 2020 2020 2020 2068 6561 7274  e,.        heart
-0001a320: 6265 6174 5f74 6963 6b3a 204f 7074 696f  beat_tick: Optio
-0001a330: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0001a340: 0a20 2020 2020 2020 2061 7070 6c69 6564  .        applied
-0001a350: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0001a360: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0001a370: 6d61 785f 7369 7a65 5f70 6572 5f6d 7367  max_size_per_msg
-0001a380: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0001a390: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0001a3a0: 6d61 785f 696e 666c 6967 6874 5f6d 7367  max_inflight_msg
-0001a3b0: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-0001a3c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0001a3d0: 2063 6865 636b 5f71 756f 7275 6d3a 204f   check_quorum: O
-0001a3e0: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-0001a3f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
-0001a400: 655f 766f 7465 3a20 4f70 7469 6f6e 616c  e_vote: Optional
-0001a410: 5b62 6f6f 6c5d 203d 204e 6f6e 652c 0a20  [bool] = None,. 
-0001a420: 2020 2020 2020 206d 696e 5f65 6c65 6374         min_elect
-0001a430: 696f 6e5f 7469 636b 3a20 4f70 7469 6f6e  ion_tick: Option
-0001a440: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-0001a450: 2020 2020 2020 2020 6d61 785f 656c 6563          max_elec
-0001a460: 7469 6f6e 5f74 6963 6b3a 204f 7074 696f  tion_tick: Optio
-0001a470: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0001a480: 0a20 2020 2020 2020 2072 6561 645f 6f6e  .        read_on
-0001a490: 6c79 5f6f 7074 696f 6e3a 204f 7074 696f  ly_option: Optio
-0001a4a0: 6e61 6c5b 2252 6561 644f 6e6c 794f 7074  nal["ReadOnlyOpt
-0001a4b0: 696f 6e22 5d20 3d20 4e6f 6e65 2c0a 2020  ion"] = None,.  
-0001a4c0: 2020 2020 2020 736b 6970 5f62 6361 7374        skip_bcast
-0001a4d0: 5f63 6f6d 6d69 743a 204f 7074 696f 6e61  _commit: Optiona
-0001a4e0: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
-0001a4f0: 2020 2020 2020 2020 6261 7463 685f 6170          batch_ap
-0001a500: 7065 6e64 3a20 4f70 7469 6f6e 616c 5b62  pend: Optional[b
-0001a510: 6f6f 6c5d 203d 204e 6f6e 652c 0a20 2020  ool] = None,.   
-0001a520: 2020 2020 2070 7269 6f72 6974 793a 204f       priority: O
-0001a530: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0001a540: 6f6e 652c 0a20 2020 2020 2020 206d 6178  one,.        max
-0001a550: 5f75 6e63 6f6d 6d69 7474 6564 5f73 697a  _uncommitted_siz
-0001a560: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-0001a570: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0001a580: 206d 6178 5f63 6f6d 6d69 7474 6564 5f73   max_committed_s
-0001a590: 697a 655f 7065 725f 7265 6164 793a 204f  ize_per_ready: O
-0001a5a0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-0001a5b0: 6f6e 652c 0a20 2020 2029 202d 3e20 4e6f  one,.    ) -> No
-0001a5c0: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-0001a5d0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-0001a5e0: 643a 2054 6865 2069 6465 6e74 6974 7920  d: The identity 
-0001a5f0: 6f66 2074 6865 206c 6f63 616c 2072 6166  of the local raf
-0001a600: 742e 2049 7420 6361 6e6e 6f74 2062 6520  t. It cannot be 
-0001a610: 302c 2061 6e64 206d 7573 7420 6265 2075  0, and must be u
-0001a620: 6e69 7175 6520 696e 2074 6865 2067 726f  nique in the gro
-0001a630: 7570 2e0a 0a20 2020 2020 2020 203a 7061  up...        :pa
-0001a640: 7261 6d20 656c 6563 7469 6f6e 5f74 6963  ram election_tic
-0001a650: 6b3a 2054 6865 206e 756d 6265 7220 6f66  k: The number of
-0001a660: 206e 6f64 652e 7469 636b 2069 6e76 6f63   node.tick invoc
-0001a670: 6174 696f 6e73 2074 6861 7420 6d75 7374  ations that must
-0001a680: 2070 6173 7320 6265 7477 6565 6e0a 2020   pass between.  
-0001a690: 2020 2020 2020 656c 6563 7469 6f6e 732e        elections.
-0001a6a0: 2054 6861 7420 6973 2c20 6966 2061 2066   That is, if a f
-0001a6b0: 6f6c 6c6f 7765 7220 646f 6573 206e 6f74  ollower does not
-0001a6c0: 2072 6563 6569 7665 2061 6e79 206d 6573   receive any mes
-0001a6d0: 7361 6765 2066 726f 6d20 7468 650a 2020  sage from the.  
-0001a6e0: 2020 2020 2020 6c65 6164 6572 206f 6620        leader of 
-0001a6f0: 6375 7272 656e 7420 7465 726d 2062 6566  current term bef
-0001a700: 6f72 6520 456c 6563 7469 6f6e 5469 636b  ore ElectionTick
-0001a710: 2068 6173 2065 6c61 7073 6564 2c20 6974   has elapsed, it
-0001a720: 2077 696c 6c20 6265 636f 6d65 0a20 2020   will become.   
-0001a730: 2020 2020 2063 616e 6469 6461 7465 2061       candidate a
-0001a740: 6e64 2073 7461 7274 2061 6e20 656c 6563  nd start an elec
-0001a750: 7469 6f6e 2e20 656c 6563 7469 6f6e 5f74  tion. election_t
-0001a760: 6963 6b20 6d75 7374 2062 6520 6772 6561  ick must be grea
-0001a770: 7465 7220 7468 616e 0a20 2020 2020 2020  ter than.       
-0001a780: 2048 6561 7274 6265 6174 5469 636b 2e20   HeartbeatTick. 
-0001a790: 5765 2073 7567 6765 7374 2065 6c65 6374  We suggest elect
-0001a7a0: 696f 6e5f 7469 636b 203d 2031 3020 2a20  ion_tick = 10 * 
-0001a7b0: 4865 6172 7462 6561 7454 6963 6b20 746f  HeartbeatTick to
-0001a7c0: 2061 766f 6964 0a20 2020 2020 2020 2075   avoid.        u
-0001a7d0: 6e6e 6563 6573 7361 7279 206c 6561 6465  nnecessary leade
-0001a7e0: 7220 7377 6974 6368 696e 670a 0a20 2020  r switching..   
-0001a7f0: 2020 2020 203a 7061 7261 6d20 6865 6172       :param hear
-0001a800: 7462 6561 745f 7469 636b 3a20 4865 6172  tbeat_tick: Hear
-0001a810: 7462 6561 7454 6963 6b20 6973 2074 6865  tbeatTick is the
-0001a820: 206e 756d 6265 7220 6f66 206e 6f64 652e   number of node.
-0001a830: 7469 636b 2069 6e76 6f63 6174 696f 6e73  tick invocations
-0001a840: 2074 6861 7420 6d75 7374 2070 6173 7320   that must pass 
-0001a850: 6265 7477 6565 6e0a 2020 2020 2020 2020  between.        
-0001a860: 6865 6172 7462 6561 7473 2e20 5468 6174  heartbeats. That
-0001a870: 2069 732c 2061 206c 6561 6465 7220 7365   is, a leader se
-0001a880: 6e64 7320 6865 6172 7462 6561 7420 6d65  nds heartbeat me
-0001a890: 7373 6167 6573 2074 6f20 6d61 696e 7461  ssages to mainta
-0001a8a0: 696e 2069 7473 0a20 2020 2020 2020 206c  in its.        l
-0001a8b0: 6561 6465 7273 6869 7020 6576 6572 7920  eadership every 
-0001a8c0: 6865 6172 7462 6561 7420 7469 636b 732e  heartbeat ticks.
-0001a8d0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0001a8e0: 2061 7070 6c69 6564 3a20 4170 706c 6965   applied: Applie
-0001a8f0: 6420 6973 2074 6865 206c 6173 7420 6170  d is the last ap
-0001a900: 706c 6965 6420 696e 6465 782e 2049 7420  plied index. It 
-0001a910: 7368 6f75 6c64 206f 6e6c 7920 6265 2073  should only be s
-0001a920: 6574 2077 6865 6e20 7265 7374 6172 7469  et when restarti
-0001a930: 6e67 0a20 2020 2020 2020 2072 6166 742e  ng.        raft.
-0001a940: 2072 6166 7420 7769 6c6c 206e 6f74 2072   raft will not r
-0001a950: 6574 7572 6e20 656e 7472 6965 7320 746f  eturn entries to
-0001a960: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
-0001a970: 2073 6d61 6c6c 6572 206f 7220 6571 7561   smaller or equa
-0001a980: 6c20 746f 2041 7070 6c69 6564 2e0a 2020  l to Applied..  
-0001a990: 2020 2020 2020 4966 2041 7070 6c69 6564        If Applied
-0001a9a0: 2069 7320 756e 7365 7420 7768 656e 2072   is unset when r
-0001a9b0: 6573 7461 7274 696e 672c 2072 6166 7420  estarting, raft 
-0001a9c0: 6d69 6768 7420 7265 7475 726e 2070 7265  might return pre
-0001a9d0: 7669 6f75 7320 6170 706c 6965 6420 656e  vious applied en
-0001a9e0: 7472 6965 732e 0a20 2020 2020 2020 2054  tries..        T
-0001a9f0: 6869 7320 6973 2061 2076 6572 7920 6170  his is a very ap
-0001aa00: 706c 6963 6174 696f 6e20 6465 7065 6e64  plication depend
-0001aa10: 656e 7420 636f 6e66 6967 7572 6174 696f  ent configuratio
-0001aa20: 6e2e 0a0a 2020 2020 2020 2020 3a70 6172  n...        :par
-0001aa30: 616d 206d 6178 5f73 697a 655f 7065 725f  am max_size_per_
-0001aa40: 6d73 673a 204c 696d 6974 2074 6865 206d  msg: Limit the m
-0001aa50: 6178 2073 697a 6520 6f66 2065 6163 6820  ax size of each 
-0001aa60: 6170 7065 6e64 206d 6573 7361 6765 2e20  append message. 
-0001aa70: 536d 616c 6c65 7220 7661 6c75 6520 6c6f  Smaller value lo
-0001aa80: 7765 7273 0a20 2020 2020 2020 2074 6865  wers.        the
-0001aa90: 2072 6166 7420 7265 636f 7665 7279 2063   raft recovery c
-0001aaa0: 6f73 7428 696e 6974 6961 6c20 7072 6f62  ost(initial prob
-0001aab0: 696e 6720 616e 6420 6d65 7373 6167 6520  ing and message 
-0001aac0: 6c6f 7374 2064 7572 696e 6720 6e6f 726d  lost during norm
-0001aad0: 616c 206f 7065 7261 7469 6f6e 292e 0a20  al operation).. 
-0001aae0: 2020 2020 2020 204f 6e20 7468 6520 6f74         On the ot
-0001aaf0: 6865 7220 7369 6465 2c20 6974 206d 6967  her side, it mig
-0001ab00: 6874 2061 6666 6563 7420 7468 6520 7468  ht affect the th
-0001ab10: 726f 7567 6870 7574 2064 7572 696e 6720  roughput during 
-0001ab20: 6e6f 726d 616c 2072 6570 6c69 6361 7469  normal replicati
-0001ab30: 6f6e 2e0a 2020 2020 2020 2020 4e6f 7465  on..        Note
-0001ab40: 3a20 6d61 7468 2e4d 6178 5575 7369 7a65  : math.MaxUusize
-0001ab50: 3634 2066 6f72 2075 6e6c 696d 6974 6564  64 for unlimited
-0001ab60: 2c20 3020 666f 7220 6174 206d 6f73 7420  , 0 for at most 
-0001ab70: 6f6e 6520 656e 7472 7920 7065 7220 6d65  one entry per me
-0001ab80: 7373 6167 652e 0a0a 2020 2020 2020 2020  ssage...        
-0001ab90: 3a70 6172 616d 206d 6178 5f69 6e66 6c69  :param max_infli
-0001aba0: 6768 745f 6d73 6773 3a20 4c69 6d69 7420  ght_msgs: Limit 
-0001abb0: 7468 6520 6d61 7820 6e75 6d62 6572 206f  the max number o
-0001abc0: 6620 696e 2d66 6c69 6768 7420 6170 7065  f in-flight appe
-0001abd0: 6e64 206d 6573 7361 6765 7320 6475 7269  nd messages duri
-0001abe0: 6e67 206f 7074 696d 6973 7469 630a 2020  ng optimistic.  
-0001abf0: 2020 2020 2020 7265 706c 6963 6174 696f        replicatio
-0001ac00: 6e20 7068 6173 652e 2054 6865 2061 7070  n phase. The app
-0001ac10: 6c69 6361 7469 6f6e 2074 7261 6e73 706f  lication transpo
-0001ac20: 7274 6174 696f 6e20 6c61 7965 7220 7573  rtation layer us
-0001ac30: 7561 6c6c 7920 6861 7320 6974 7320 6f77  ually has its ow
-0001ac40: 6e20 7365 6e64 696e 670a 2020 2020 2020  n sending.      
-0001ac50: 2020 6275 6666 6572 206f 7665 7220 5443    buffer over TC
-0001ac60: 502f 5544 502e 2053 6574 2074 6f20 6176  P/UDP. Set to av
-0001ac70: 6f69 6420 6f76 6572 666c 6f77 696e 6720  oid overflowing 
-0001ac80: 7468 6174 2073 656e 6469 6e67 2062 7566  that sending buf
-0001ac90: 6665 722e 0a0a 2020 2020 2020 2020 3a70  fer...        :p
-0001aca0: 6172 616d 2063 6865 636b 5f71 756f 7275  aram check_quoru
-0001acb0: 6d3a 2053 7065 6369 6679 2069 6620 7468  m: Specify if th
-0001acc0: 6520 6c65 6164 6572 2073 686f 756c 6420  e leader should 
-0001acd0: 6368 6563 6b20 7175 6f72 756d 2061 6374  check quorum act
-0001ace0: 6976 6974 792e 204c 6561 6465 7220 7374  ivity. Leader st
-0001acf0: 6570 7320 646f 776e 2077 6865 6e0a 2020  eps down when.  
-0001ad00: 2020 2020 2020 7175 6f72 756d 2069 7320        quorum is 
-0001ad10: 6e6f 7420 6163 7469 7665 2066 6f72 2061  not active for a
-0001ad20: 6e20 656c 6563 7469 6f6e 5469 6d65 6f75  n electionTimeou
-0001ad30: 742e 0a0a 2020 2020 2020 2020 3a70 6172  t...        :par
-0001ad40: 616d 2070 7265 5f76 6f74 653a 2045 6e61  am pre_vote: Ena
-0001ad50: 626c 6573 2074 6865 2050 7265 2d56 6f74  bles the Pre-Vot
-0001ad60: 6520 616c 676f 7269 7468 6d20 6465 7363  e algorithm desc
-0001ad70: 7269 6265 6420 696e 2072 6166 7420 7468  ribed in raft th
-0001ad80: 6573 6973 2073 6563 7469 6f6e 0a20 2020  esis section.   
-0001ad90: 2020 2020 2039 2e36 2e20 5468 6973 2070       9.6. This p
-0001ada0: 7265 7665 6e74 7320 6469 7372 7570 7469  revents disrupti
-0001adb0: 6f6e 2077 6865 6e20 6120 6e6f 6465 2074  on when a node t
-0001adc0: 6861 7420 6861 7320 6265 656e 2070 6172  hat has been par
-0001add0: 7469 7469 6f6e 6564 2061 7761 790a 2020  titioned away.  
-0001ade0: 2020 2020 2020 7265 6a6f 696e 7320 7468        rejoins th
-0001adf0: 6520 636c 7573 7465 722e 0a0a 2020 2020  e cluster...    
-0001ae00: 2020 2020 3a70 6172 616d 206d 696e 5f65      :param min_e
-0001ae10: 6c65 6374 696f 6e5f 7469 636b 3a20 5468  lection_tick: Th
-0001ae20: 6520 7261 6e67 6520 6f66 2065 6c65 6374  e range of elect
-0001ae30: 696f 6e20 7469 6d65 6f75 742e 2049 6e20  ion timeout. In 
-0001ae40: 736f 6d65 2063 6173 6573 2c20 7765 2068  some cases, we h
-0001ae50: 6f70 6520 736f 6d65 206e 6f64 6573 2068  ope some nodes h
-0001ae60: 6173 206c 6573 7320 706f 7373 6962 696c  as less possibil
-0001ae70: 6974 790a 2020 2020 2020 2020 746f 2062  ity.        to b
-0001ae80: 6563 6f6d 6520 6c65 6164 6572 2e20 5468  ecome leader. Th
-0001ae90: 6973 2063 6f6e 6669 6775 7261 7469 6f6e  is configuration
-0001aea0: 2065 6e73 7572 6573 2074 6861 7420 7468   ensures that th
-0001aeb0: 6520 7261 6e64 6f6d 697a 6564 2065 6c65  e randomized ele
-0001aec0: 6374 696f 6e5f 7469 6d65 6f75 740a 2020  ction_timeout.  
-0001aed0: 2020 2020 2020 7769 6c6c 2061 6c77 6179        will alway
-0001aee0: 7320 6265 2073 7569 7420 696e 205b 6d69  s be suit in [mi
-0001aef0: 6e5f 656c 6563 7469 6f6e 5f74 6963 6b2c  n_election_tick,
-0001af00: 206d 6178 5f65 6c65 6374 696f 6e5f 7469   max_election_ti
-0001af10: 636b 292e 0a20 2020 2020 2020 2049 6620  ck)..        If 
-0001af20: 6974 2069 7320 302c 2074 6865 6e20 656c  it is 0, then el
-0001af30: 6563 7469 6f6e 5f74 6963 6b20 7769 6c6c  ection_tick will
-0001af40: 2062 6520 6368 6f73 656e 2e0a 0a20 2020   be chosen...   
-0001af50: 2020 2020 203a 7061 7261 6d20 6d61 785f       :param max_
-0001af60: 656c 6563 7469 6f6e 5f74 6963 6b3a 2049  election_tick: I
-0001af70: 6620 6974 2069 7320 302c 2074 6865 6e20  f it is 0, then 
-0001af80: 3220 2a20 656c 6563 7469 6f6e 5f74 6963  2 * election_tic
-0001af90: 6b20 7769 6c6c 2062 6520 6368 6f73 656e  k will be chosen
-0001afa0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-0001afb0: 6d20 7265 6164 5f6f 6e6c 795f 6f70 7469  m read_only_opti
-0001afc0: 6f6e 3a20 4368 6f6f 7365 2074 6865 206c  on: Choose the l
-0001afd0: 696e 6561 7269 7a61 6269 6c69 7479 206d  inearizability m
-0001afe0: 6f64 6520 6f72 2074 6865 206c 6561 7365  ode or the lease
-0001aff0: 206d 6f64 6520 746f 2072 6561 6420 6461   mode to read da
-0001b000: 7461 2e20 4966 2079 6f75 2064 6f6e e280  ta. If you don..
-0001b010: 9974 2063 6172 6520 6162 6f75 7420 7468  .t care about th
-0001b020: 6520 7265 6164 2063 6f6e 7369 7374 656e  e read consisten
-0001b030: 6379 2061 6e64 2077 616e 7420 6120 6869  cy and want a hi
-0001b040: 6768 6572 2072 6561 6420 7065 7266 6f72  gher read perfor
-0001b050: 6d61 6e63 652c 2079 6f75 2063 616e 2075  mance, you can u
-0001b060: 7365 2074 6865 206c 6561 7365 206d 6f64  se the lease mod
-0001b070: 652e 0a20 2020 2020 2020 2053 6574 7469  e..        Setti
-0001b080: 6e67 2074 6869 7320 746f 2060 4c65 6173  ng this to `Leas
-0001b090: 6542 6173 6564 6020 7265 7175 6972 6573  eBased` requires
-0001b0a0: 2060 6368 6563 6b5f 7175 6f72 756d 203d   `check_quorum =
-0001b0b0: 2074 7275 6560 2e0a 0a20 2020 2020 2020   true`...       
-0001b0c0: 203a 7061 7261 6d20 736b 6970 5f62 6361   :param skip_bca
-0001b0d0: 7374 5f63 6f6d 6d69 743a 2044 6f6e 2774  st_commit: Don't
-0001b0e0: 2062 726f 6164 6361 7374 2061 6e20 656d   broadcast an em
-0001b0f0: 7074 7920 7261 6674 2065 6e74 7279 2074  pty raft entry t
-0001b100: 6f20 6e6f 7469 6679 2066 6f6c 6c6f 7765  o notify followe
-0001b110: 7220 746f 2063 6f6d 6d69 7420 616e 2065  r to commit an e
-0001b120: 6e74 7279 2e0a 2020 2020 2020 2020 5468  ntry..        Th
-0001b130: 6973 206d 6179 206d 616b 6520 666f 6c6c  is may make foll
-0001b140: 6f77 6572 2077 6169 7420 6120 6c6f 6e67  ower wait a long
-0001b150: 6572 2074 696d 6520 746f 2061 7070 6c79  er time to apply
-0001b160: 2061 6e20 656e 7472 792e 2054 6869 7320   an entry. This 
-0001b170: 636f 6e66 6967 7572 6174 696f 6e0a 2020  configuration.  
-0001b180: 2020 2020 2020 4d61 7920 6166 6665 6374        May affect
-0001b190: 2070 726f 706f 7361 6c20 666f 7277 6172   proposal forwar
-0001b1a0: 6469 6e67 2061 6e64 2066 6f6c 6c6f 7765  ding and followe
-0001b1b0: 7220 7265 6164 2e0a 0a20 2020 2020 2020  r read...       
-0001b1c0: 203a 7061 7261 6d20 6261 7463 685f 6170   :param batch_ap
-0001b1d0: 7065 6e64 3a20 4261 7463 6865 7320 6576  pend: Batches ev
-0001b1e0: 6572 7920 6170 7065 6e64 206d 7367 2069  ery append msg i
-0001b1f0: 6620 616e 7920 6170 7065 6e64 206d 7367  f any append msg
-0001b200: 2061 6c72 6561 6479 2065 7869 7374 730a   already exists.
-0001b210: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0001b220: 7072 696f 7269 7479 3a20 5468 6520 656c  priority: The el
-0001b230: 6563 7469 6f6e 2070 7269 6f72 6974 7920  ection priority 
-0001b240: 6f66 2074 6869 7320 6e6f 6465 2e0a 0a20  of this node... 
-0001b250: 2020 2020 2020 203a 7061 7261 6d20 6d61         :param ma
-0001b260: 785f 756e 636f 6d6d 6974 7465 645f 7369  x_uncommitted_si
-0001b270: 7a65 3a20 5370 6563 6966 7920 6d61 7869  ze: Specify maxi
-0001b280: 6d75 6d20 6f66 2075 6e63 6f6d 6d69 7474  mum of uncommitt
-0001b290: 6564 2065 6e74 7279 2073 697a 652e 0a20  ed entry size.. 
-0001b2a0: 2020 2020 2020 2057 6865 6e20 7468 6973         When this
-0001b2b0: 206c 696d 6974 2069 7320 7265 6163 6865   limit is reache
-0001b2c0: 642c 2061 6c6c 2070 726f 706f 7361 6c73  d, all proposals
-0001b2d0: 2074 6f20 6170 7065 6e64 206e 6577 206c   to append new l
-0001b2e0: 6f67 2077 696c 6c20 6265 2064 726f 7070  og will be dropp
-0001b2f0: 6564 0a0a 2020 2020 2020 2020 3a70 6172  ed..        :par
-0001b300: 616d 206d 6178 5f63 6f6d 6d69 7474 6564  am max_committed
-0001b310: 5f73 697a 655f 7065 725f 7265 6164 793a  _size_per_ready:
-0001b320: 204d 6178 2073 697a 6520 666f 7220 636f   Max size for co
-0001b330: 6d6d 6974 7465 6420 656e 7472 6965 7320  mmitted entries 
-0001b340: 696e 2061 2060 5265 6164 7960 2e0a 2020  in a `Ready`..  
-0001b350: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
-0001b360: 6620 6d61 6b65 5f72 6566 2873 656c 6629  f make_ref(self)
-0001b370: 202d 3e20 2243 6f6e 6669 6752 6566 223a   -> "ConfigRef":
-0001b380: 202e 2e2e 0a20 2020 2040 7374 6174 6963   ....    @static
-0001b390: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-0001b3a0: 6566 6175 6c74 2829 202d 3e20 2243 6f6e  efault() -> "Con
-0001b3b0: 6669 6722 3a20 2e2e 2e0a 0a63 6c61 7373  fig": .....class
-0001b3c0: 2043 6f6e 6669 6752 6566 285f 5f41 5049   ConfigRef(__API
-0001b3d0: 5f43 6f6e 6669 6729 3a0a 2020 2020 2222  _Config):.    ""
-0001b3e0: 220a 2020 2020 5265 6665 7265 6e63 6520  ".    Reference 
-0001b3f0: 7479 7065 206f 6620 3a63 6c61 7373 3a60  type of :class:`
-0001b400: 496e 666c 6967 6874 7352 6566 602e 0a20  InflightsRef`.. 
-0001b410: 2020 2022 2222 0a0a 2320 544f 444f 3a20     """..# TODO: 
-0001b420: 4164 6420 6265 6c6f 7720 696d 706c 656d  Add below implem
-0001b430: 656e 7461 7469 6f6e 2069 6620 6e65 6564  entation if need
-0001b440: 6564 2c20 6f74 6865 7277 6973 6520 7265  ed, otherwise re
-0001b450: 6d6f 7665 2062 656c 6f77 2063 6f64 6573  move below codes
-0001b460: 2e0a 2320 636c 6173 7320 5f5f 4150 495f  ..# class __API_
-0001b470: 5374 6174 7573 3a0a 2320 2020 2020 6465  Status:.#     de
-0001b480: 6620 6765 745f 6170 706c 6965 6428 7365  f get_applied(se
-0001b490: 6c66 2920 2d3e 2069 6e74 3a0a 2320 2020  lf) -> int:.#   
-0001b4a0: 2020 2020 2020 2222 2220 2222 220a 2320        """ """.# 
-0001b4b0: 2020 2020 6465 6620 7365 745f 6170 706c      def set_appl
-0001b4c0: 6965 6428 7365 6c66 2c20 6170 706c 6965  ied(self, applie
-0001b4d0: 643a 2069 6e74 2920 2d3e 204e 6f6e 653a  d: int) -> None:
-0001b4e0: 0a23 2020 2020 2020 2020 2022 2222 2022  .#         """ "
-0001b4f0: 2222 0a23 2020 2020 2064 6566 2067 6574  "".#     def get
-0001b500: 5f69 6428 7365 6c66 2920 2d3e 2069 6e74  _id(self) -> int
-0001b510: 3a0a 2320 2020 2020 2020 2020 2222 2220  :.#         """ 
-0001b520: 2222 220a 2320 2020 2020 6465 6620 7365  """.#     def se
-0001b530: 745f 6964 2873 656c 662c 2069 643a 2069  t_id(self, id: i
-0001b540: 6e74 2920 2d3e 204e 6f6e 653a 0a23 2020  nt) -> None:.#  
-0001b550: 2020 2020 2020 2022 2222 2022 2222 0a23         """ """.#
-0001b560: 2020 2020 2064 6566 2067 6574 5f68 7328       def get_hs(
-0001b570: 7365 6c66 2920 2d3e 2048 6172 6453 7461  self) -> HardSta
-0001b580: 7465 5265 663a 0a23 2020 2020 2020 2020  teRef:.#        
-0001b590: 2022 2222 2022 2222 0a23 2020 2020 2064   """ """.#     d
-0001b5a0: 6566 2073 6574 5f68 7328 7365 6c66 2c20  ef set_hs(self, 
-0001b5b0: 6873 3a20 4861 7264 5374 6174 6552 6566  hs: HardStateRef
-0001b5c0: 2920 2d3e 204e 6f6e 653a 0a23 2020 2020  ) -> None:.#    
-0001b5d0: 2020 2020 2022 2222 2022 2222 0a23 2020       """ """.#  
-0001b5e0: 2020 2064 6566 2067 6574 5f73 7328 7365     def get_ss(se
-0001b5f0: 6c66 2920 2d3e 2053 6f66 7453 7461 7465  lf) -> SoftState
-0001b600: 5265 663a 0a23 2020 2020 2020 2020 2022  Ref:.#         "
-0001b610: 2222 2022 2222 0a23 2020 2020 2064 6566  "" """.#     def
-0001b620: 2073 6574 5f73 7328 7365 6c66 2c20 7373   set_ss(self, ss
-0001b630: 3a20 536f 6674 5374 6174 6552 6566 2920  : SoftStateRef) 
-0001b640: 2d3e 204e 6f6e 653a 0a23 2020 2020 2020  -> None:.#      
-0001b650: 2020 2022 2222 2022 2222 0a23 2020 2020     """ """.#    
-0001b660: 2064 6566 2067 6574 5f70 726f 6772 6573   def get_progres
-0001b670: 7328 7365 6c66 2920 2d3e 204f 7074 696f  s(self) -> Optio
-0001b680: 6e61 6c5b 5072 6f67 7265 7373 5472 6163  nal[ProgressTrac
-0001b690: 6b65 7252 6566 5d3a 0a23 2020 2020 2020  kerRef]:.#      
-0001b6a0: 2020 2022 2222 2022 2222 0a23 2020 2020     """ """.#    
-0001b6b0: 2064 6566 2073 6574 5f70 726f 6772 6573   def set_progres
-0001b6c0: 7328 0a23 2020 2020 2020 2020 2073 656c  s(.#         sel
-0001b6d0: 662c 2074 7261 636b 6572 3a20 4f70 7469  f, tracker: Opti
-0001b6e0: 6f6e 616c 5b50 726f 6772 6573 7354 7261  onal[ProgressTra
-0001b6f0: 636b 6572 5d20 7c20 4f70 7469 6f6e 616c  cker] | Optional
-0001b700: 5b50 726f 6772 6573 7354 7261 636b 6572  [ProgressTracker
-0001b710: 5265 665d 0a23 2020 2020 2029 202d 3e20  Ref].#     ) -> 
-0001b720: 4e6f 6e65 3a0a 2320 2020 2020 2020 2020  None:.#         
-0001b730: 2222 2220 2222 220a 0a23 2063 6c61 7373  """ """..# class
-0001b740: 2049 6e4d 656d 6f72 7953 7461 7475 7328   InMemoryStatus(
-0001b750: 5f5f 4150 495f 5374 6174 7573 293a 0a23  __API_Status):.#
-0001b760: 2020 2020 2022 2222 0a23 2020 2020 2052       """.#     R
-0001b770: 6570 7265 7365 6e74 7320 7468 6520 6375  epresents the cu
-0001b780: 7272 656e 7420 7374 6174 7573 206f 6620  rrent status of 
-0001b790: 7468 6520 7261 6674 0a23 2020 2020 2022  the raft.#     "
-0001b7a0: 2222 0a0a 2320 2020 2020 6465 6620 5f5f  ""..#     def __
-0001b7b0: 696e 6974 5f5f 2873 656c 662c 2072 6166  init__(self, raf
-0001b7c0: 743a 2049 6e4d 656d 6f72 7952 6166 7429  t: InMemoryRaft)
-0001b7d0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2320   -> None: ....# 
-0001b7e0: 2020 2020 6465 6620 6d61 6b65 5f72 6566      def make_ref
-0001b7f0: 2873 656c 6629 202d 3e20 5374 6174 7573  (self) -> Status
-0001b800: 5f5f 4d65 6d73 746f 7261 6765 5265 663a  __MemstorageRef:
-0001b810: 202e 2e2e 0a0a 2320 636c 6173 7320 496e   .....# class In
-0001b820: 4d65 6d6f 7279 5374 6174 7573 5265 6628  MemoryStatusRef(
-0001b830: 5f5f 4150 495f 5374 6174 7573 293a 0a23  __API_Status):.#
-0001b840: 2020 2020 2022 2222 0a23 2020 2020 2052       """.#     R
-0001b850: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
-0001b860: 203a 636c 6173 733a 6053 7461 7475 735f   :class:`Status_
-0001b870: 5f4d 656d 7374 6f72 6167 6560 2e0a 2320  _Memstorage`..# 
-0001b880: 2020 2020 2222 220a 0a63 6c61 7373 2044      """..class D
-0001b890: 6573 7472 6f79 6564 5265 6655 7365 6445  estroyedRefUsedE
-0001b8a0: 7272 6f72 2845 7863 6570 7469 6f6e 293a  rror(Exception):
-0001b8b0: 0a20 2020 2022 2222 2022 2222 0a0a 636c  .    """ """..cl
-0001b8c0: 6173 7320 5261 6674 4572 726f 7228 4578  ass RaftError(Ex
-0001b8d0: 6365 7074 696f 6e29 3a0a 2020 2020 2222  ception):.    ""
-0001b8e0: 2220 2222 220a 0a63 6c61 7373 2045 7869  " """..class Exi
-0001b8f0: 7374 7345 7272 6f72 2852 6166 7445 7272  stsError(RaftErr
-0001b900: 6f72 293a 0a20 2020 2022 2222 0a20 2020  or):.    """.   
-0001b910: 2054 6865 206e 6f64 6520 7b69 647d 2061   The node {id} a
-0001b920: 6c72 6561 6479 2065 7869 7374 7320 696e  lready exists in
-0001b930: 2074 6865 207b 7365 747d 2073 6574 2e0a   the {set} set..
-0001b940: 2020 2020 2222 220a 0a20 2020 2069 643a      """..    id:
-0001b950: 2069 6e74 0a20 2020 2073 6574 3a20 7374   int.    set: st
-0001b960: 720a 0a63 6c61 7373 204e 6f74 4578 6973  r..class NotExis
-0001b970: 7473 2852 6166 7445 7272 6f72 293a 0a20  ts(RaftError):. 
-0001b980: 2020 2022 2222 0a20 2020 2054 6865 206e     """.    The n
-0001b990: 6f64 6520 7b69 647d 2069 7320 6e6f 7420  ode {id} is not 
-0001b9a0: 696e 2074 6865 207b 7365 747d 2073 6574  in the {set} set
-0001b9b0: 2e0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
-0001b9c0: 643a 2069 6e74 0a20 2020 2073 6574 3a20  d: int.    set: 
-0001b9d0: 7374 720a 0a63 6c61 7373 2043 6f64 6563  str..class Codec
-0001b9e0: 4572 726f 7228 5261 6674 4572 726f 7229  Error(RaftError)
-0001b9f0: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
-0001ba00: 7072 6f74 6f62 7566 206d 6573 7361 6765  protobuf message
-0001ba10: 2063 6f64 6563 2066 6169 6c65 6420 696e   codec failed in
-0001ba20: 2073 6f6d 6520 6d61 6e6e 6572 2e0a 2020   some manner..  
-0001ba30: 2020 2222 220a 0a63 6c61 7373 2043 6f6e    """..class Con
-0001ba40: 6669 6749 6e76 616c 6964 4572 726f 7228  figInvalidError(
-0001ba50: 5261 6674 4572 726f 7229 3a0a 2020 2020  RaftError):.    
-0001ba60: 2222 220a 2020 2020 5468 6520 636f 6e66  """.    The conf
-0001ba70: 6967 7572 6174 696f 6e20 6973 2069 6e76  iguration is inv
-0001ba80: 616c 6964 2e0a 2020 2020 2222 220a 0a63  alid..    """..c
-0001ba90: 6c61 7373 2050 726f 706f 7361 6c44 726f  lass ProposalDro
-0001baa0: 7070 6564 4572 726f 7228 5261 6674 4572  ppedError(RaftEr
-0001bab0: 726f 7229 3a0a 2020 2020 2222 220a 2020  ror):.    """.  
-0001bac0: 2020 5468 6520 7072 6f70 6f73 616c 206f    The proposal o
-0001bad0: 6620 6368 616e 6765 7320 7761 7320 6472  f changes was dr
-0001bae0: 6f70 7065 642e 0a20 2020 2022 2222 0a0a  opped..    """..
-0001baf0: 636c 6173 7320 5265 7175 6573 7453 6e61  class RequestSna
-0001bb00: 7073 686f 7444 726f 7070 6564 4572 726f  pshotDroppedErro
-0001bb10: 7228 5261 6674 4572 726f 7229 3a0a 2020  r(RaftError):.  
-0001bb20: 2020 2222 220a 2020 2020 5468 6520 7265    """.    The re
-0001bb30: 7175 6573 7420 736e 6170 7368 6f74 2069  quest snapshot i
-0001bb40: 7320 6472 6f70 7065 642e 0a20 2020 2022  s dropped..    "
-0001bb50: 2222 0a0a 636c 6173 7320 436f 6e66 4368  ""..class ConfCh
-0001bb60: 616e 6765 4572 726f 7228 5261 6674 4572  angeError(RaftEr
-0001bb70: 726f 7229 3a0a 2020 2020 2222 220a 2020  ror):.    """.  
-0001bb80: 2020 436f 6e66 4368 616e 6765 2070 726f    ConfChange pro
-0001bb90: 706f 7361 6c20 6973 2069 6e76 616c 6964  posal is invalid
-0001bba0: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
-0001bbb0: 2049 6f45 7272 6f72 2852 6166 7445 7272   IoError(RaftErr
-0001bbc0: 6f72 293a 0a20 2020 2022 2222 0a20 2020  or):.    """.   
-0001bbd0: 2041 6e20 494f 2065 7272 6f72 206f 6363   An IO error occ
-0001bbe0: 7572 7265 642e 0a20 2020 2022 2222 0a0a  urred..    """..
-0001bbf0: 636c 6173 7320 5374 6f72 6545 7272 6f72  class StoreError
-0001bc00: 2852 6166 7445 7272 6f72 293a 0a20 2020  (RaftError):.   
-0001bc10: 2022 2222 0a20 2020 2041 2073 746f 7261   """.    A stora
-0001bc20: 6765 2065 7272 6f72 206f 6363 7572 7265  ge error occurre
-0001bc30: 642e 0a20 2020 2022 2222 0a0a 636c 6173  d..    """..clas
-0001bc40: 7320 5374 6570 4c6f 6361 6c4d 7367 2852  s StepLocalMsg(R
-0001bc50: 6166 7445 7272 6f72 293a 0a20 2020 2022  aftError):.    "
-0001bc60: 2222 0a20 2020 2052 6166 7420 6361 6e6e  "".    Raft cann
-0001bc70: 6f74 2073 7465 7020 7468 6520 6c6f 6361  ot step the loca
-0001bc80: 6c20 6d65 7373 6167 652e 0a20 2020 2022  l message..    "
-0001bc90: 2222 0a0a 636c 6173 7320 5374 6570 5065  ""..class StepPe
-0001bca0: 6572 4e6f 7446 6f75 6e64 2852 6166 7445  erNotFound(RaftE
-0001bcb0: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
-0001bcc0: 2020 2054 6865 2072 6166 7420 7065 6572     The raft peer
-0001bcd0: 2069 7320 6e6f 7420 666f 756e 6420 616e   is not found an
-0001bce0: 6420 7468 7573 2063 616e 6e6f 7420 7374  d thus cannot st
-0001bcf0: 6570 2e0a 2020 2020 2222 220a 0a63 6c61  ep..    """..cla
-0001bd00: 7373 2052 6166 7453 746f 7261 6765 4572  ss RaftStorageEr
-0001bd10: 726f 7228 4578 6365 7074 696f 6e29 3a0a  ror(Exception):.
-0001bd20: 2020 2020 2222 220a 2020 2020 416e 2065      """.    An e
-0001bd30: 7272 6f72 2077 6974 6820 7468 6520 7374  rror with the st
-0001bd40: 6f72 6167 652e 0a20 2020 2022 2222 0a0a  orage..    """..
-0001bd50: 636c 6173 7320 436f 6d70 6163 7465 6445  class CompactedE
-0001bd60: 7272 6f72 2852 6166 7453 746f 7261 6765  rror(RaftStorage
-0001bd70: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
-0001bd80: 2020 2020 5468 6520 7374 6f72 6167 6520      The storage 
-0001bd90: 7761 7320 636f 6d70 6163 7465 6420 616e  was compacted an
-0001bda0: 6420 6e6f 7420 6163 6365 7373 6962 6c65  d not accessible
-0001bdb0: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-0001bdc0: 556e 6176 6169 6c61 626c 6545 7272 6f72  UnavailableError
-0001bdd0: 2852 6166 7453 746f 7261 6765 4572 726f  (RaftStorageErro
-0001bde0: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
-0001bdf0: 5468 6520 6c6f 6720 6973 206e 6f74 2061  The log is not a
-0001be00: 7661 696c 6162 6c65 2e0a 2020 2020 2222  vailable..    ""
-0001be10: 220a 0a63 6c61 7373 204c 6f67 5465 6d70  "..class LogTemp
-0001be20: 6f72 6172 696c 7955 6e61 7661 696c 6162  orarilyUnavailab
-0001be30: 6c65 4572 726f 7228 5261 6674 5374 6f72  leError(RaftStor
-0001be40: 6167 6545 7272 6f72 293a 0a20 2020 2022  ageError):.    "
-0001be50: 2222 0a20 2020 2054 6865 206c 6f67 2069  "".    The log i
-0001be60: 7320 6265 696e 6720 6665 7463 6865 642e  s being fetched.
-0001be70: 0a20 2020 2022 2222 0a0a 636c 6173 7320  .    """..class 
-0001be80: 536e 6170 7368 6f74 4f75 744f 6644 6174  SnapshotOutOfDat
-0001be90: 6545 7272 6f72 2852 6166 7453 746f 7261  eError(RaftStora
-0001bea0: 6765 4572 726f 7229 3a0a 2020 2020 2222  geError):.    ""
-0001beb0: 220a 2020 2020 5468 6520 736e 6170 7368  ".    The snapsh
-0001bec0: 6f74 2069 7320 6f75 7420 6f66 2064 6174  ot is out of dat
-0001bed0: 652e 0a20 2020 2022 2222 0a0a 636c 6173  e..    """..clas
-0001bee0: 7320 536e 6170 7368 6f74 5465 6d70 6f72  s SnapshotTempor
-0001bef0: 6172 696c 7955 6e61 7661 696c 6162 6c65  arilyUnavailable
-0001bf00: 2852 6166 7453 746f 7261 6765 4572 726f  (RaftStorageErro
-0001bf10: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
-0001bf20: 5468 6520 736e 6170 7368 6f74 2069 7320  The snapshot is 
-0001bf30: 6265 696e 6720 6372 6561 7465 642e 0a20  being created.. 
-0001bf40: 2020 2022 2222 0a0a 636c 6173 7320 4f74     """..class Ot
-0001bf50: 6865 7245 7272 6f72 2852 6166 7453 746f  herError(RaftSto
-0001bf60: 7261 6765 4572 726f 7229 3a0a 2020 2020  rageError):.    
-0001bf70: 2222 220a 2020 2020 536f 6d65 206f 7468  """.    Some oth
-0001bf80: 6572 2065 7272 6f72 206f 6363 7572 7265  er error occurre
-0001bf90: 642e 0a20 2020 2022 2222 0a              d..    """.
+00013450: 2020 2020 2060 6d73 6773 603a 2054 6865       `msgs`: The
+00013460: 206c 6973 7420 6f66 206d 6573 7361 6765   list of message
+00013470: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00013480: 2020 2064 6566 2074 616b 655f 6d73 6773     def take_msgs
+00013490: 2873 656c 6629 202d 3e20 4c69 7374 5b22  (self) -> List["
+000134a0: 4d65 7373 6167 6522 5d3a 0a20 2020 2020  Message"]:.     
+000134b0: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+000134c0: 6d73 6773 603a 2054 6865 206c 6973 7420  msgs`: The list 
+000134d0: 6f66 206d 6573 7361 6765 732e 0a20 2020  of messages..   
+000134e0: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+000134f0: 2067 6574 5f6d 6178 5f69 6e66 6c69 6768   get_max_infligh
+00013500: 7428 7365 6c66 2920 2d3e 2069 6e74 3a0a  t(self) -> int:.
+00013510: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013520: 2020 2020 606d 6178 5f69 6e66 6c69 6768      `max_infligh
+00013530: 7460 3a20 5468 6520 6d61 7869 6d75 6d20  t`: The maximum 
+00013540: 6e75 6d62 6572 206f 6620 6d65 7373 6167  number of messag
+00013550: 6573 2074 6861 7420 6361 6e20 6265 2069  es that can be i
+00013560: 6e66 6c69 6768 742e 0a20 2020 2020 2020  nflight..       
+00013570: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00013580: 5f6d 6178 5f69 6e66 6c69 6768 7428 7365  _max_inflight(se
+00013590: 6c66 2c20 6d61 785f 696e 666c 6967 6874  lf, max_inflight
+000135a0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+000135b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000135c0: 2020 2020 606d 6178 5f69 6e66 6c69 6768      `max_infligh
+000135d0: 7460 3a20 5468 6520 6d61 7869 6d75 6d20  t`: The maximum 
+000135e0: 6e75 6d62 6572 206f 6620 6d65 7373 6167  number of messag
+000135f0: 6573 2074 6861 7420 6361 6e20 6265 2069  es that can be i
+00013600: 6e66 6c69 6768 742e 0a20 2020 2020 2020  nflight..       
+00013610: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00013620: 5f73 7461 7465 2873 656c 6629 202d 3e20  _state(self) -> 
+00013630: 2253 7461 7465 526f 6c65 223a 0a20 2020  "StateRole":.   
+00013640: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013650: 2060 7374 6174 6560 3a20 5468 6520 6375   `state`: The cu
+00013660: 7272 656e 7420 726f 6c65 206f 6620 7468  rrent role of th
+00013670: 6973 206e 6f64 652e 0a20 2020 2020 2020  is node..       
+00013680: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00013690: 5f73 7461 7465 2873 656c 662c 2073 7461  _state(self, sta
+000136a0: 7465 5f72 6f6c 653a 2022 5374 6174 6552  te_role: "StateR
+000136b0: 6f6c 6522 2920 2d3e 204e 6f6e 653a 0a20  ole") -> None:. 
+000136c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000136d0: 2020 2060 7374 6174 6560 3a20 5468 6520     `state`: The 
+000136e0: 6375 7272 656e 7420 726f 6c65 206f 6620  current role of 
+000136f0: 7468 6973 206e 6f64 652e 0a20 2020 2020  this node..     
+00013700: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00013710: 6574 5f65 6c65 6374 696f 6e5f 656c 6170  et_election_elap
+00013720: 7365 6428 7365 6c66 2920 2d3e 2069 6e74  sed(self) -> int
+00013730: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013740: 2020 2020 2020 6065 6c65 6374 696f 6e5f        `election_
+00013750: 656c 6170 7365 6460 3a20 5469 636b 7320  elapsed`: Ticks 
+00013760: 7369 6e63 6520 6974 2072 6561 6368 6564  since it reached
+00013770: 206c 6173 7420 656c 6563 7469 6f6e 5469   last electionTi
+00013780: 6d65 6f75 7420 7768 656e 2069 7420 6973  meout when it is
+00013790: 206c 6561 6465 7220 6f72 2063 616e 6469   leader or candi
+000137a0: 6461 7465 2e0a 2020 2020 2020 2020 4e75  date..        Nu
+000137b0: 6d62 6572 206f 6620 7469 636b 7320 7369  mber of ticks si
+000137c0: 6e63 6520 6974 2072 6561 6368 6564 206c  nce it reached l
+000137d0: 6173 7420 656c 6563 7469 6f6e 5469 6d65  ast electionTime
+000137e0: 6f75 7420 6f72 2072 6563 6569 7665 6420  out or received 
+000137f0: 610a 2020 2020 2020 2020 7661 6c69 6420  a.        valid 
+00013800: 6d65 7373 6167 6520 6672 6f6d 2063 7572  message from cur
+00013810: 7265 6e74 206c 6561 6465 7220 7768 656e  rent leader when
+00013820: 2069 7420 6973 2061 2066 6f6c 6c6f 7765   it is a followe
+00013830: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+00013840: 2020 2064 6566 2073 6574 5f65 6c65 6374     def set_elect
+00013850: 696f 6e5f 656c 6170 7365 6428 7365 6c66  ion_elapsed(self
+00013860: 2c20 656c 6563 7469 6f6e 5f65 6c61 7073  , election_elaps
+00013870: 6564 3a20 696e 7429 202d 3e20 4e6f 6e65  ed: int) -> None
+00013880: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013890: 2020 2020 2020 6065 6c65 6374 696f 6e5f        `election_
+000138a0: 656c 6170 7365 6460 3a20 5469 636b 7320  elapsed`: Ticks 
+000138b0: 7369 6e63 6520 6974 2072 6561 6368 6564  since it reached
+000138c0: 206c 6173 7420 656c 6563 7469 6f6e 5469   last electionTi
+000138d0: 6d65 6f75 7420 7768 656e 2069 7420 6973  meout when it is
+000138e0: 206c 6561 6465 7220 6f72 2063 616e 6469   leader or candi
+000138f0: 6461 7465 2e0a 2020 2020 2020 2020 4e75  date..        Nu
+00013900: 6d62 6572 206f 6620 7469 636b 7320 7369  mber of ticks si
+00013910: 6e63 6520 6974 2072 6561 6368 6564 206c  nce it reached l
+00013920: 6173 7420 656c 6563 7469 6f6e 5469 6d65  ast electionTime
+00013930: 6f75 7420 6f72 2072 6563 6569 7665 6420  out or received 
+00013940: 610a 2020 2020 2020 2020 7661 6c69 6420  a.        valid 
+00013950: 6d65 7373 6167 6520 6672 6f6d 2063 7572  message from cur
+00013960: 7265 6e74 206c 6561 6465 7220 7768 656e  rent leader when
+00013970: 2069 7420 6973 2061 2066 6f6c 6c6f 7765   it is a followe
+00013980: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
+00013990: 2020 2064 6566 2067 6574 5f63 6865 636b     def get_check
+000139a0: 5f71 756f 7275 6d28 7365 6c66 2920 2d3e  _quorum(self) ->
+000139b0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+000139c0: 2222 0a20 2020 2020 2020 2060 6368 6563  "".        `chec
+000139d0: 6b5f 7175 6f72 756d 603a 2057 6865 7468  k_quorum`: Wheth
+000139e0: 6572 2074 6f20 6368 6563 6b20 7468 6520  er to check the 
+000139f0: 7175 6f72 756d 0a20 2020 2020 2020 2022  quorum.        "
+00013a00: 2222 0a20 2020 2064 6566 2073 6574 5f63  "".    def set_c
+00013a10: 6865 636b 5f71 756f 7275 6d28 7365 6c66  heck_quorum(self
+00013a20: 2c20 6368 6563 6b5f 7175 6f72 756d 3a20  , check_quorum: 
+00013a30: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
+00013a40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013a50: 2020 2060 6368 6563 6b5f 7175 6f72 756d     `check_quorum
+00013a60: 603a 2057 6865 7468 6572 2074 6f20 6368  `: Whether to ch
+00013a70: 6563 6b20 7468 6520 7175 6f72 756d 0a20  eck the quorum. 
+00013a80: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00013a90: 6566 2067 6574 5f70 7265 5f76 6f74 6528  ef get_pre_vote(
+00013aa0: 7365 6c66 2920 2d3e 2062 6f6f 6c3a 0a20  self) -> bool:. 
+00013ab0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013ac0: 2020 2060 7072 655f 766f 7465 603a 2045     `pre_vote`: E
+00013ad0: 6e61 626c 6520 7468 6520 7072 6576 6f74  nable the prevot
+00013ae0: 6520 616c 676f 7269 7468 6d2e 0a0a 2020  e algorithm...  
+00013af0: 2020 2020 2020 5468 6973 2065 6e61 626c        This enabl
+00013b00: 6573 2061 2070 7265 2d65 6c65 6374 696f  es a pre-electio
+00013b10: 6e20 766f 7465 2072 6f75 6e64 206f 6e20  n vote round on 
+00013b20: 4361 6e64 6964 6174 6573 2070 7269 6f72  Candidates prior
+00013b30: 2074 6f20 6469 7372 7570 7469 6e67 2074   to disrupting t
+00013b40: 6865 2063 6c75 7374 6572 2e0a 0a20 2020  he cluster...   
+00013b50: 2020 2020 2045 6e61 626c 6520 7468 6973       Enable this
+00013b60: 2069 6620 6772 6561 7465 7220 636c 7573   if greater clus
+00013b70: 7465 7220 7374 6162 696c 6974 7920 6973  ter stability is
+00013b80: 2070 7265 6665 7272 6564 206f 7665 7220   preferred over 
+00013b90: 6661 7374 6572 2065 6c65 6374 696f 6e73  faster elections
+00013ba0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00013bb0: 2020 6465 6620 7365 745f 7072 655f 766f    def set_pre_vo
+00013bc0: 7465 2873 656c 662c 2070 7265 5f76 6f74  te(self, pre_vot
+00013bd0: 653a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  e: bool) -> None
+00013be0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013bf0: 2020 2020 2020 6070 7265 5f76 6f74 6560        `pre_vote`
+00013c00: 3a20 456e 6162 6c65 2074 6865 2070 7265  : Enable the pre
+00013c10: 766f 7465 2061 6c67 6f72 6974 686d 2e0a  vote algorithm..
+00013c20: 0a20 2020 2020 2020 2054 6869 7320 656e  .        This en
+00013c30: 6162 6c65 7320 6120 7072 652d 656c 6563  ables a pre-elec
+00013c40: 7469 6f6e 2076 6f74 6520 726f 756e 6420  tion vote round 
+00013c50: 6f6e 2043 616e 6469 6461 7465 7320 7072  on Candidates pr
+00013c60: 696f 7220 746f 2064 6973 7275 7074 696e  ior to disruptin
+00013c70: 6720 7468 6520 636c 7573 7465 722e 0a0a  g the cluster...
+00013c80: 2020 2020 2020 2020 456e 6162 6c65 2074          Enable t
+00013c90: 6869 7320 6966 2067 7265 6174 6572 2063  his if greater c
+00013ca0: 6c75 7374 6572 2073 7461 6269 6c69 7479  luster stability
+00013cb0: 2069 7320 7072 6566 6572 7265 6420 6f76   is preferred ov
+00013cc0: 6572 2066 6173 7465 7220 656c 6563 7469  er faster electi
+00013cd0: 6f6e 732e 0a20 2020 2020 2020 2022 2222  ons..        """
+00013ce0: 0a20 2020 2064 6566 2061 7070 6c79 5f63  .    def apply_c
+00013cf0: 6f6e 665f 6368 616e 6765 2873 656c 662c  onf_change(self,
+00013d00: 2063 6f6e 665f 6368 616e 6765 3a20 2243   conf_change: "C
+00013d10: 6f6e 6643 6861 6e67 6556 3252 6566 2229  onfChangeV2Ref")
+00013d20: 202d 3e20 2243 6f6e 6643 6861 6e67 6552   -> "ConfChangeR
+00013d30: 6566 223a 0a20 2020 2020 2020 2022 2222  ef":.        """
+00013d40: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00013d50: 5f72 6561 645f 7374 6174 6573 2873 656c  _read_states(sel
+00013d60: 6629 202d 3e20 4c69 7374 5b22 5265 6164  f) -> List["Read
+00013d70: 5374 6174 6522 5d3a 0a20 2020 2020 2020  State"]:.       
+00013d80: 2022 2222 0a20 2020 2020 2020 2060 7265   """.        `re
+00013d90: 6164 5f73 7461 7465 7360 3a20 5468 6520  ad_states`: The 
+00013da0: 6375 7272 656e 7420 7265 6164 2073 7461  current read sta
+00013db0: 7465 732e 0a20 2020 2020 2020 2022 2222  tes..        """
+00013dc0: 0a20 2020 2064 6566 2073 6574 5f72 6561  .    def set_rea
+00013dd0: 645f 7374 6174 6573 280a 2020 2020 2020  d_states(.      
+00013de0: 2020 7365 6c66 2c20 7265 6164 5f73 7461    self, read_sta
+00013df0: 7465 733a 204c 6973 745b 2252 6561 6453  tes: List["ReadS
+00013e00: 7461 7465 225d 207c 204c 6973 745b 2252  tate"] | List["R
+00013e10: 6561 6453 7461 7465 5265 6622 5d0a 2020  eadStateRef"].  
+00013e20: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+00013e30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013e40: 2060 7265 6164 5f73 7461 7465 7360 3a20   `read_states`: 
+00013e50: 5468 6520 6375 7272 656e 7420 7265 6164  The current read
+00013e60: 2073 7461 7465 732e 0a20 2020 2020 2020   states..       
+00013e70: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+00013e80: 5f72 6561 645f 6f6e 6c79 5f6f 7074 696f  _read_only_optio
+00013e90: 6e28 7365 6c66 2920 2d3e 2022 5265 6164  n(self) -> "Read
+00013ea0: 4f6e 6c79 4f70 7469 6f6e 223a 0a20 2020  OnlyOption":.   
+00013eb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013ec0: 2060 7265 6164 5f6f 6e6c 795f 6f70 7469   `read_only_opti
+00013ed0: 6f6e 603a 2043 686f 6f73 6520 7468 6520  on`: Choose the 
+00013ee0: 6c69 6e65 6172 697a 6162 696c 6974 7920  linearizability 
+00013ef0: 6d6f 6465 206f 7220 7468 6520 6c65 6173  mode or the leas
+00013f00: 6520 6d6f 6465 2074 6f20 7265 6164 2064  e mode to read d
+00013f10: 6174 612e 2049 6620 796f 7520 646f 6ee2  ata. If you don.
+00013f20: 8099 7420 6361 7265 2061 626f 7574 2074  ..t care about t
+00013f30: 6865 2072 6561 6420 636f 6e73 6973 7465  he read consiste
+00013f40: 6e63 7920 616e 6420 7761 6e74 2061 2068  ncy and want a h
+00013f50: 6967 6865 7220 7265 6164 2070 6572 666f  igher read perfo
+00013f60: 726d 616e 6365 2c20 796f 7520 6361 6e20  rmance, you can 
+00013f70: 7573 6520 7468 6520 6c65 6173 6520 6d6f  use the lease mo
+00013f80: 6465 2e0a 2020 2020 2020 2020 5365 7474  de..        Sett
+00013f90: 696e 6720 7468 6973 2074 6f20 604c 6561  ing this to `Lea
+00013fa0: 7365 4261 7365 6460 2072 6571 7569 7265  seBased` require
+00013fb0: 7320 6063 6865 636b 5f71 756f 7275 6d20  s `check_quorum 
+00013fc0: 3d20 7472 7565 602e 0a20 2020 2020 2020  = true`..       
+00013fd0: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00013fe0: 5f72 6561 645f 6f6e 6c79 5f6f 7074 696f  _read_only_optio
+00013ff0: 6e28 7365 6c66 2c20 6f70 7469 6f6e 3a20  n(self, option: 
+00014000: 2252 6561 644f 6e6c 794f 7074 696f 6e22  "ReadOnlyOption"
+00014010: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014020: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00014030: 7265 6164 5f6f 6e6c 795f 6f70 7469 6f6e  read_only_option
+00014040: 603a 2043 686f 6f73 6520 7468 6520 6c69  `: Choose the li
+00014050: 6e65 6172 697a 6162 696c 6974 7920 6d6f  nearizability mo
+00014060: 6465 206f 7220 7468 6520 6c65 6173 6520  de or the lease 
+00014070: 6d6f 6465 2074 6f20 7265 6164 2064 6174  mode to read dat
+00014080: 612e 2049 6620 796f 7520 646f 6ee2 8099  a. If you don...
+00014090: 7420 6361 7265 2061 626f 7574 2074 6865  t care about the
+000140a0: 2072 6561 6420 636f 6e73 6973 7465 6e63   read consistenc
+000140b0: 7920 616e 6420 7761 6e74 2061 2068 6967  y and want a hig
+000140c0: 6865 7220 7265 6164 2070 6572 666f 726d  her read perform
+000140d0: 616e 6365 2c20 796f 7520 6361 6e20 7573  ance, you can us
+000140e0: 6520 7468 6520 6c65 6173 6520 6d6f 6465  e the lease mode
+000140f0: 2e0a 2020 2020 2020 2020 5365 7474 696e  ..        Settin
+00014100: 6720 7468 6973 2074 6f20 604c 6561 7365  g this to `Lease
+00014110: 4261 7365 6460 2072 6571 7569 7265 7320  Based` requires 
+00014120: 6063 6865 636b 5f71 756f 7275 6d20 3d20  `check_quorum = 
+00014130: 7472 7565 602e 0a20 2020 2020 2020 2022  true`..        "
+00014140: 2222 0a20 2020 2064 6566 2069 6e66 6c69  "".    def infli
+00014150: 6768 745f 6275 6666 6572 735f 7369 7a65  ght_buffers_size
+00014160: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00014170: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
+00014180: 6520 696e 666c 6967 6874 2062 7566 6665  e inflight buffe
+00014190: 7220 7369 7a65 2e22 2222 0a20 2020 2064  r size.""".    d
+000141a0: 6566 206d 6179 6265 5f66 7265 655f 696e  ef maybe_free_in
+000141b0: 666c 6967 6874 5f62 7566 6665 7273 2873  flight_buffers(s
+000141c0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+000141d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000141e0: 2020 4120 5261 6674 206c 6561 6465 7220    A Raft leader 
+000141f0: 616c 6c6f 6361 7465 7320 6120 7665 6374  allocates a vect
+00014200: 6f72 2077 6974 6820 6361 7061 6369 7479  or with capacity
+00014210: 2060 6d61 785f 696e 666c 6967 6874 5f6d   `max_inflight_m
+00014220: 7367 7360 2066 6f72 2065 7665 7279 2070  sgs` for every p
+00014230: 6565 722e 0a20 2020 2020 2020 2049 7420  eer..        It 
+00014240: 7461 6b65 7320 6120 6c6f 7420 6f66 206d  takes a lot of m
+00014250: 656d 6f72 7920 6966 2074 6865 7265 2061  emory if there a
+00014260: 7265 2074 6f6f 206d 616e 7920 5261 6674  re too many Raft
+00014270: 2067 726f 7570 732e 2060 6d61 7962 655f   groups. `maybe_
+00014280: 6672 6565 5f69 6e66 6c69 6768 745f 6275  free_inflight_bu
+00014290: 6666 6572 7360 0a20 2020 2020 2020 2069  ffers`.        i
+000142a0: 7320 7573 6564 2074 6f20 6672 6565 206d  s used to free m
+000142b0: 656d 6f72 7920 6966 206e 6563 6573 7361  emory if necessa
+000142c0: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
+000142d0: 2020 2020 6465 6620 6164 6a75 7374 5f6d      def adjust_m
+000142e0: 6178 5f69 6e66 6c69 6768 745f 6d73 6773  ax_inflight_msgs
+000142f0: 2873 656c 662c 2074 6172 6765 743a 2069  (self, target: i
+00014300: 6e74 2c20 6361 703a 2069 6e74 2920 2d3e  nt, cap: int) ->
+00014310: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00014320: 2222 0a20 2020 2020 2020 2054 6f20 6164  "".        To ad
+00014330: 6a75 7374 2060 6d61 785f 696e 666c 6967  just `max_inflig
+00014340: 6874 5f6d 7367 7360 2066 6f72 2074 6865  ht_msgs` for the
+00014350: 2073 7065 6369 6669 6564 2070 6565 722e   specified peer.
+00014360: 0a20 2020 2020 2020 2053 6574 2074 6f20  .        Set to 
+00014370: 6030 6020 7769 6c6c 2064 6973 6162 6c65  `0` will disable
+00014380: 2074 6865 2070 726f 6772 6573 732e 0a20   the progress.. 
+00014390: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+000143a0: 6566 2067 6574 5f72 6561 646f 6e6c 795f  ef get_readonly_
+000143b0: 7265 6164 5f69 6e64 6578 5f71 7565 7565  read_index_queue
+000143c0: 2873 656c 6629 202d 3e20 4c69 7374 5b4c  (self) -> List[L
+000143d0: 6973 745b 696e 745d 5d3a 0a20 2020 2020  ist[int]]:.     
+000143e0: 2020 2022 2222 2022 2222 0a20 2020 2064     """ """.    d
+000143f0: 6566 2073 6574 5f62 6174 6368 5f61 7070  ef set_batch_app
+00014400: 656e 6428 7365 6c66 2c20 6261 7463 685f  end(self, batch_
+00014410: 6170 7065 6e64 3a20 626f 6f6c 2920 2d3e  append: bool) ->
+00014420: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00014430: 2222 0a20 2020 2020 2020 2053 6574 2077  "".        Set w
+00014440: 6865 7468 6572 2062 6174 6368 2061 7070  hether batch app
+00014450: 656e 6420 6d73 6720 6174 2072 756e 7469  end msg at runti
+00014460: 6d65 2e0a 2020 2020 2020 2020 2222 220a  me..        """.
+00014470: 2020 2020 6465 6620 7365 745f 6d61 785f      def set_max_
+00014480: 636f 6d6d 6974 7465 645f 7369 7a65 5f70  committed_size_p
+00014490: 6572 5f72 6561 6479 2873 656c 662c 2073  er_ready(self, s
+000144a0: 697a 653a 2069 6e74 2920 2d3e 204e 6f6e  ize: int) -> Non
+000144b0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+000144c0: 2020 2020 2020 2053 6574 2060 6d61 785f         Set `max_
+000144d0: 636f 6d6d 6974 7465 645f 7369 7a65 5f70  committed_size_p
+000144e0: 6572 5f72 6561 6479 6020 746f 2060 7369  er_ready` to `si
+000144f0: 7a65 602e 0a20 2020 2020 2020 2022 2222  ze`..        """
+00014500: 0a0a 636c 6173 7320 496e 4d65 6d6f 7279  ..class InMemory
+00014510: 5261 6674 285f 5f41 5049 5f52 6166 7429  Raft(__API_Raft)
+00014520: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
+00014530: 7374 7275 6374 2074 6861 7420 7265 7072  struct that repr
+00014540: 6573 656e 7473 2074 6865 2072 6166 7420  esents the raft 
+00014550: 636f 6e73 656e 7375 7320 6974 7365 6c66  consensus itself
+00014560: 2e20 5374 6f72 6573 2064 6574 6169 6c73  . Stores details
+00014570: 2063 6f6e 6365 726e 696e 6720 7468 6520   concerning the 
+00014580: 6375 7272 656e 740a 2020 2020 616e 6420  current.    and 
+00014590: 706f 7373 6962 6c65 2073 7461 7465 2074  possible state t
+000145a0: 6865 2073 7973 7465 6d20 6361 6e20 7461  he system can ta
+000145b0: 6b65 2e0a 2020 2020 2222 220a 0a20 2020  ke..    """..   
+000145c0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000145d0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000145e0: 2020 2020 2063 6667 3a20 2243 6f6e 6669       cfg: "Confi
+000145f0: 6722 207c 2022 436f 6e66 6967 5265 6622  g" | "ConfigRef"
+00014600: 2c0a 2020 2020 2020 2020 7374 6f72 653a  ,.        store:
+00014610: 2022 4d65 6d53 746f 7261 6765 2220 7c20   "MemStorage" | 
+00014620: 224d 656d 5374 6f72 6167 6552 6566 222c  "MemStorageRef",
+00014630: 0a20 2020 2020 2020 206c 6f67 6765 723a  .        logger:
+00014640: 2022 4c6f 6767 6572 2220 7c20 224c 6f67   "Logger" | "Log
+00014650: 6765 7252 6566 222c 0a20 2020 2029 202d  gerRef",.    ) -
+00014660: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+00014670: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
+00014680: 6629 202d 3e20 2249 6e4d 656d 6f72 7952  f) -> "InMemoryR
+00014690: 6166 7452 6566 223a 202e 2e2e 0a20 2020  aftRef": ....   
+000146a0: 2064 6566 2067 6574 5f72 6166 745f 6c6f   def get_raft_lo
+000146b0: 6728 7365 6c66 2920 2d3e 2022 496e 4d65  g(self) -> "InMe
+000146c0: 6d6f 7279 5261 6674 4c6f 6752 6566 223a  moryRaftLogRef":
+000146d0: 0a20 2020 2020 2020 2022 2222 2022 2222  .        """ """
+000146e0: 0a0a 636c 6173 7320 496e 4d65 6d6f 7279  ..class InMemory
+000146f0: 5261 6674 5265 6628 5f5f 4150 495f 5261  RaftRef(__API_Ra
+00014700: 6674 293a 0a20 2020 2022 2222 0a20 2020  ft):.    """.   
+00014710: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+00014720: 6f66 203a 636c 6173 733a 6049 6e4d 656d  of :class:`InMem
+00014730: 6f72 7952 6166 7460 2e0a 2020 2020 2222  oryRaft`..    ""
+00014740: 220a 0a20 2020 2064 6566 2067 6574 5f72  "..    def get_r
+00014750: 6166 745f 6c6f 6728 7365 6c66 2920 2d3e  aft_log(self) ->
+00014760: 2022 496e 4d65 6d6f 7279 5261 6674 4c6f   "InMemoryRaftLo
+00014770: 6752 6566 223a 0a20 2020 2020 2020 2022  gRef":.        "
+00014780: 2222 2022 2222 0a0a 636c 6173 7320 5261  "" """..class Ra
+00014790: 6674 285f 5f41 5049 5f52 6166 7429 3a0a  ft(__API_Raft):.
+000147a0: 2020 2020 2222 220a 2020 2020 4120 7374      """.    A st
+000147b0: 7275 6374 2074 6861 7420 7265 7072 6573  ruct that repres
+000147c0: 656e 7473 2074 6865 2072 6166 7420 636f  ents the raft co
+000147d0: 6e73 656e 7375 7320 6974 7365 6c66 2e20  nsensus itself. 
+000147e0: 5374 6f72 6573 2064 6574 6169 6c73 2063  Stores details c
+000147f0: 6f6e 6365 726e 696e 6720 7468 6520 6375  oncerning the cu
+00014800: 7272 656e 740a 2020 2020 616e 6420 706f  rrent.    and po
+00014810: 7373 6962 6c65 2073 7461 7465 2074 6865  ssible state the
+00014820: 2073 7973 7465 6d20 6361 6e20 7461 6b65   system can take
+00014830: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+00014840: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00014850: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00014860: 2020 2063 6667 3a20 2243 6f6e 6669 6722     cfg: "Config"
+00014870: 207c 2022 436f 6e66 6967 5265 6622 2c0a   | "ConfigRef",.
+00014880: 2020 2020 2020 2020 7374 6f72 653a 2022          store: "
+00014890: 5374 6f72 6167 6522 207c 2022 5374 6f72  Storage" | "Stor
+000148a0: 6167 6552 6566 222c 0a20 2020 2020 2020  ageRef",.       
+000148b0: 206c 6f67 6765 723a 2022 4c6f 6767 6572   logger: "Logger
+000148c0: 2220 7c20 224c 6f67 6765 7252 6566 222c  " | "LoggerRef",
+000148d0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
+000148e0: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
+000148f0: 5f72 6566 2873 656c 6629 202d 3e20 2252  _ref(self) -> "R
+00014900: 6166 7452 6566 223a 202e 2e2e 0a20 2020  aftRef": ....   
+00014910: 2064 6566 2067 6574 5f72 6166 745f 6c6f   def get_raft_lo
+00014920: 6728 7365 6c66 2920 2d3e 2022 5261 6674  g(self) -> "Raft
+00014930: 4c6f 6752 6566 223a 0a20 2020 2020 2020  LogRef":.       
+00014940: 2022 2222 2022 2222 0a0a 636c 6173 7320   """ """..class 
+00014950: 5261 6674 5265 6628 5f5f 4150 495f 5261  RaftRef(__API_Ra
+00014960: 6674 293a 0a20 2020 2022 2222 0a20 2020  ft):.    """.   
+00014970: 2052 6566 6572 656e 6365 2074 7970 6520   Reference type 
+00014980: 6f66 203a 636c 6173 733a 6052 6166 7460  of :class:`Raft`
+00014990: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
+000149a0: 6566 2067 6574 5f72 6166 745f 6c6f 6728  ef get_raft_log(
+000149b0: 7365 6c66 2920 2d3e 2022 5261 6674 4c6f  self) -> "RaftLo
+000149c0: 6752 6566 223a 0a20 2020 2020 2020 2022  gRef":.        "
+000149d0: 2222 2022 2222 0a0a 636c 6173 7320 5072  "" """..class Pr
+000149e0: 6f67 7265 7373 4d61 7049 7465 6d3a 0a20  ogressMapItem:. 
+000149f0: 2020 2064 6566 2069 6428 7365 6c66 2920     def id(self) 
+00014a00: 2d3e 2069 6e74 3a20 2e2e 2e0a 2020 2020  -> int: ....    
+00014a10: 6465 6620 7072 6f67 7265 7373 2873 656c  def progress(sel
+00014a20: 6629 202d 3e20 2250 726f 6772 6573 7322  f) -> "Progress"
+00014a30: 3a20 2e2e 2e0a 0a63 6c61 7373 205f 5f41  : .....class __A
+00014a40: 5049 5f50 726f 6772 6573 7354 7261 636b  PI_ProgressTrack
+00014a50: 6572 285f 5f43 6c6f 6e65 6162 6c65 293a  er(__Cloneable):
+00014a60: 0a20 2020 2064 6566 2063 6c6f 6e65 2873  .    def clone(s
+00014a70: 656c 6629 202d 3e20 2250 726f 6772 6573  elf) -> "Progres
+00014a80: 7354 7261 636b 6572 223a 202e 2e2e 0a20  sTracker": .... 
+00014a90: 2020 2064 6566 2067 6574 2873 656c 662c     def get(self,
+00014aa0: 2069 643a 2069 6e74 2920 2d3e 204f 7074   id: int) -> Opt
+00014ab0: 696f 6e61 6c5b 2250 726f 6772 6573 7352  ional["ProgressR
+00014ac0: 6566 225d 3a0a 2020 2020 2020 2020 2222  ef"]:.        ""
+00014ad0: 2222 2222 0a20 2020 2064 6566 2067 726f  """".    def gro
+00014ae0: 7570 5f63 6f6d 6d69 7428 7365 6c66 2920  up_commit(self) 
+00014af0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00014b00: 2022 2222 0a20 2020 2020 2020 2057 6865   """.        Whe
+00014b10: 7468 6572 2065 6e61 626c 6520 6772 6f75  ther enable grou
+00014b20: 7020 636f 6d6d 6974 2e0a 2020 2020 2020  p commit..      
+00014b30: 2020 2222 220a 2020 2020 6465 6620 656e    """.    def en
+00014b40: 6162 6c65 5f67 726f 7570 5f63 6f6d 6d69  able_group_commi
+00014b50: 7428 7365 6c66 2c20 656e 6162 6c65 3a20  t(self, enable: 
+00014b60: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
+00014b70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014b80: 2020 2043 6f6e 6669 6775 7265 7320 6772     Configures gr
+00014b90: 6f75 7020 636f 6d6d 6974 2e0a 2020 2020  oup commit..    
+00014ba0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00014bb0: 6861 735f 7175 6f72 756d 2873 656c 662c  has_quorum(self,
+00014bc0: 2070 6f74 656e 7469 616c 5f71 756f 7275   potential_quoru
+00014bd0: 6d3a 2053 6574 5b69 6e74 5d29 202d 3e20  m: Set[int]) -> 
+00014be0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00014bf0: 220a 2020 2020 2020 2020 4465 7465 726d  ".        Determ
+00014c00: 696e 6520 6966 2061 2071 756f 7275 6d20  ine if a quorum 
+00014c10: 6973 2066 6f72 6d65 6420 6672 6f6d 2074  is formed from t
+00014c20: 6865 2067 6976 656e 2073 6574 206f 6620  he given set of 
+00014c30: 6e6f 6465 732e 0a0a 2020 2020 2020 2020  nodes...        
+00014c40: 5468 6973 2069 7320 7468 6520 6f6e 6c79  This is the only
+00014c50: 2063 6f72 7265 6374 2077 6179 2074 6f20   correct way to 
+00014c60: 7665 7269 6679 2079 6f75 2068 6176 6520  verify you have 
+00014c70: 7265 6163 6865 6420 6120 7175 6f72 756d  reached a quorum
+00014c80: 2066 6f72 2074 6865 2077 686f 6c65 2067   for the whole g
+00014c90: 726f 7570 2e0a 2020 2020 2020 2020 2222  roup..        ""
+00014ca0: 220a 2020 2020 6465 6620 6973 5f73 696e  ".    def is_sin
+00014cb0: 676c 6574 6f6e 2873 656c 6629 202d 3e20  gleton(self) -> 
+00014cc0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
+00014cd0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00014ce0: 7320 7472 7565 2069 6620 2861 6e64 206f  s true if (and o
+00014cf0: 6e6c 7920 6966 2920 7468 6572 6520 6973  nly if) there is
+00014d00: 206f 6e6c 7920 6f6e 6520 766f 7469 6e67   only one voting
+00014d10: 206d 656d 6265 720a 2020 2020 2020 2020   member.        
+00014d20: 2869 2e65 2e20 7468 6520 6c65 6164 6572  (i.e. the leader
+00014d30: 2920 696e 2074 6865 2063 7572 7265 6e74  ) in the current
+00014d40: 2063 6f6e 6669 6775 7261 7469 6f6e 2e0a   configuration..
+00014d50: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014d60: 6465 6620 7175 6f72 756d 5f72 6563 656e  def quorum_recen
+00014d70: 746c 795f 6163 7469 7665 2873 656c 662c  tly_active(self,
+00014d80: 2070 6572 7370 6563 7469 7665 5f6f 663a   perspective_of:
+00014d90: 2069 6e74 2920 2d3e 2062 6f6f 6c3a 0a20   int) -> bool:. 
+00014da0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014db0: 2020 2044 6574 6572 6d69 6e65 7320 6966     Determines if
+00014dc0: 2074 6865 2063 7572 7265 6e74 2071 756f   the current quo
+00014dd0: 7275 6d20 6973 2061 6374 6976 6520 6163  rum is active ac
+00014de0: 636f 7264 696e 6720 746f 2074 6865 2074  cording to the t
+00014df0: 6869 7320 7261 6674 206e 6f64 652e 0a20  his raft node.. 
+00014e00: 2020 2020 2020 2044 6f69 6e67 2074 6869         Doing thi
+00014e10: 7320 7769 6c6c 2073 6574 2074 6865 2060  s will set the `
+00014e20: 7265 6365 6e74 5f61 6374 6976 6560 206f  recent_active` o
+00014e30: 6620 6561 6368 2070 6565 7220 746f 2066  f each peer to f
+00014e40: 616c 7365 2e0a 0a20 2020 2020 2020 2054  alse...        T
+00014e50: 6869 7320 7368 6f75 6c64 206f 6e6c 7920  his should only 
+00014e60: 6265 2063 616c 6c65 6420 6279 2074 6865  be called by the
+00014e70: 206c 6561 6465 722e 0a20 2020 2020 2020   leader..       
+00014e80: 2022 2222 0a20 2020 2064 6566 206d 6178   """.    def max
+00014e90: 696d 616c 5f63 6f6d 6d69 7474 6564 5f69  imal_committed_i
+00014ea0: 6e64 6578 2873 656c 6629 202d 3e20 5475  ndex(self) -> Tu
+00014eb0: 706c 655b 696e 742c 2062 6f6f 6c5d 3a0a  ple[int, bool]:.
+00014ec0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014ed0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+00014ee0: 6d61 7869 6d61 6c20 636f 6d6d 6974 7465  maximal committe
+00014ef0: 6420 696e 6465 7820 666f 7220 7468 6520  d index for the 
+00014f00: 636c 7573 7465 722e 2054 6865 2062 6f6f  cluster. The boo
+00014f10: 6c20 666c 6167 2069 6e64 6963 6174 6573  l flag indicates
+00014f20: 2077 6865 7468 6572 0a20 2020 2020 2020   whether.       
+00014f30: 2074 6865 2069 6e64 6578 2069 7320 636f   the index is co
+00014f40: 6d70 7574 6564 2062 7920 6772 6f75 7020  mputed by group 
+00014f50: 636f 6d6d 6974 2061 6c67 6f72 6974 686d  commit algorithm
+00014f60: 2073 7563 6365 7373 6675 6c6c 790a 0a20   successfully.. 
+00014f70: 2020 2020 2020 2045 672e 2049 6620 7468         Eg. If th
+00014f80: 6520 6d61 7463 6865 6420 696e 6465 7865  e matched indexe
+00014f90: 7320 6172 6520 605b 322c 322c 322c 342c  s are `[2,2,2,4,
+00014fa0: 355d 602c 2069 7420 7769 6c6c 2072 6574  5]`, it will ret
+00014fb0: 7572 6e20 6032 602e 0a20 2020 2020 2020  urn `2`..       
+00014fc0: 2049 6620 7468 6520 6d61 7463 6865 6420   If the matched 
+00014fd0: 696e 6465 7865 7320 616e 6420 6772 6f75  indexes and grou
+00014fe0: 7073 2061 7265 2060 5b28 312c 2031 292c  ps are `[(1, 1),
+00014ff0: 2028 322c 2032 292c 2028 332c 2032 295d   (2, 2), (3, 2)]
+00015000: 602c 2069 7420 7769 6c6c 2072 6574 7572  `, it will retur
+00015010: 6e20 6031 602e 0a20 2020 2020 2020 2022  n `1`..        "
+00015020: 2222 0a20 2020 2064 6566 2072 6563 6f72  "".    def recor
+00015030: 645f 766f 7465 2873 656c 662c 2069 643a  d_vote(self, id:
+00015040: 2069 6e74 2c20 766f 7465 3a20 626f 6f6c   int, vote: bool
+00015050: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00015060: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00015070: 6563 6f72 6473 2074 6861 7420 7468 6520  ecords that the 
+00015080: 6e6f 6465 2077 6974 6820 7468 6520 6769  node with the gi
+00015090: 7665 6e20 6964 2076 6f74 6564 2066 6f72  ven id voted for
+000150a0: 2074 6869 7320 5261 6674 0a20 2020 2020   this Raft.     
+000150b0: 2020 2069 6e73 7461 6e63 6520 6966 2076     instance if v
+000150c0: 203d 3d20 7472 7565 2028 616e 6420 6465   == true (and de
+000150d0: 636c 696e 6564 2069 7420 6f74 6865 7277  clined it otherw
+000150e0: 6973 6529 2e0a 2020 2020 2020 2020 2222  ise)..        ""
+000150f0: 220a 2020 2020 6465 6620 7265 7365 745f  ".    def reset_
+00015100: 766f 7465 7328 7365 6c66 2920 2d3e 204e  votes(self) -> N
+00015110: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00015120: 0a20 2020 2020 2020 2050 7265 7061 7265  .        Prepare
+00015130: 7320 666f 7220 6120 6e65 7720 726f 756e  s for a new roun
+00015140: 6420 6f66 2076 6f74 6520 636f 756e 7469  d of vote counti
+00015150: 6e67 2076 6961 2072 6563 6f72 6456 6f74  ng via recordVot
+00015160: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00015170: 2020 2064 6566 2063 6f6e 665f 766f 7465     def conf_vote
+00015180: 7273 2873 656c 6629 202d 3e20 224a 6f69  rs(self) -> "Joi
+00015190: 6e74 436f 6e66 6967 5265 6622 3a0a 2020  ntConfigRef":.  
+000151a0: 2020 2020 2020 2222 2220 2222 220a 2020        """ """.  
+000151b0: 2020 6465 6620 636f 6e66 5f6c 6561 726e    def conf_learn
+000151c0: 6572 7328 7365 6c66 2920 2d3e 2053 6574  ers(self) -> Set
+000151d0: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
+000151e0: 2222 2022 2222 0a20 2020 2064 6566 2063  "" """.    def c
+000151f0: 6f6c 6c65 6374 2873 656c 6629 202d 3e20  ollect(self) -> 
+00015200: 4c69 7374 5b22 5072 6f67 7265 7373 4d61  List["ProgressMa
+00015210: 7049 7465 6d22 5d3a 0a20 2020 2020 2020  pItem"]:.       
+00015220: 2022 2222 2022 2222 0a0a 636c 6173 7320   """ """..class 
+00015230: 5072 6f67 7265 7373 5472 6163 6b65 7228  ProgressTracker(
+00015240: 5f5f 4150 495f 5072 6f67 7265 7373 5472  __API_ProgressTr
+00015250: 6163 6b65 7229 3a0a 2020 2020 2222 220a  acker):.    """.
+00015260: 2020 2020 6050 726f 6772 6573 7354 7261      `ProgressTra
+00015270: 636b 6572 6020 636f 6e74 6169 6e73 2073  cker` contains s
+00015280: 6576 6572 616c 2060 5072 6f67 7265 7373  everal `Progress
+00015290: 6065 732c 0a20 2020 2077 6869 6368 2063  `es,.    which c
+000152a0: 6f75 6c64 2062 6520 604c 6561 6465 7260  ould be `Leader`
+000152b0: 2c20 6046 6f6c 6c6f 7765 7260 2061 6e64  , `Follower` and
+000152c0: 2060 4c65 6172 6e65 7260 2e0a 2020 2020   `Learner`..    
+000152d0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+000152e0: 6e69 745f 5f28 7365 6c66 2c20 6d61 785f  nit__(self, max_
+000152f0: 696e 666c 6967 6874 3a20 696e 7429 202d  inflight: int) -
+00015300: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+00015310: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
+00015320: 6629 202d 3e20 2250 726f 6772 6573 7354  f) -> "ProgressT
+00015330: 7261 636b 6572 5265 6622 3a20 2e2e 2e0a  rackerRef": ....
+00015340: 0a63 6c61 7373 2050 726f 6772 6573 7354  .class ProgressT
+00015350: 7261 636b 6572 5265 6628 5f5f 4150 495f  rackerRef(__API_
+00015360: 5072 6f67 7265 7373 5472 6163 6b65 7229  ProgressTracker)
+00015370: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+00015380: 6665 7265 6e63 6520 7479 7065 206f 6620  ference type of 
+00015390: 3a63 6c61 7373 3a60 5072 6f67 7265 7373  :class:`Progress
+000153a0: 5472 6163 6b65 7260 2e0a 2020 2020 2222  Tracker`..    ""
+000153b0: 220a 0a63 6c61 7373 205f 5f41 5049 5f50  "..class __API_P
+000153c0: 726f 6772 6573 7328 5f5f 436c 6f6e 6561  rogress(__Clonea
+000153d0: 626c 6529 3a0a 2020 2020 6465 6620 636c  ble):.    def cl
+000153e0: 6f6e 6528 7365 6c66 2920 2d3e 2022 5072  one(self) -> "Pr
+000153f0: 6f67 7265 7373 223a 202e 2e2e 0a20 2020  ogress": ....   
+00015400: 2064 6566 2062 6563 6f6d 655f 7072 6f62   def become_prob
+00015410: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00015420: 0a20 2020 2020 2020 2022 2222 4368 616e  .        """Chan
+00015430: 6765 7320 7468 6520 7072 6f67 7265 7373  ges the progress
+00015440: 2074 6f20 6120 7072 6f62 652e 2222 220a   to a probe.""".
+00015450: 2020 2020 6465 6620 6265 636f 6d65 5f72      def become_r
+00015460: 6570 6c69 6361 7465 2873 656c 6629 202d  eplicate(self) -
+00015470: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00015480: 2222 2243 6861 6e67 6573 2074 6865 2070  """Changes the p
+00015490: 726f 6772 6573 7320 746f 2061 2052 6570  rogress to a Rep
+000154a0: 6c69 6361 7465 2e22 2222 0a20 2020 2064  licate.""".    d
+000154b0: 6566 2062 6563 6f6d 655f 736e 6170 7368  ef become_snapsh
+000154c0: 6f74 2873 656c 662c 2073 6e61 7073 686f  ot(self, snapsho
+000154d0: 745f 6964 783a 2069 6e74 2920 2d3e 204e  t_idx: int) -> N
+000154e0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000154f0: 4368 616e 6765 7320 7468 6520 7072 6f67  Changes the prog
+00015500: 7265 7373 2074 6f20 6120 736e 6170 7368  ress to a snapsh
+00015510: 6f74 2e22 2222 0a20 2020 2064 6566 206d  ot.""".    def m
+00015520: 6179 6265 5f75 7064 6174 6528 7365 6c66  aybe_update(self
+00015530: 2c20 6e3a 2069 6e74 2920 2d3e 2062 6f6f  , n: int) -> boo
+00015540: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00015550: 2020 2020 2020 2052 6574 7572 6e73 2066         Returns f
+00015560: 616c 7365 2069 6620 7468 6520 6769 7665  alse if the give
+00015570: 6e20 6e20 696e 6465 7820 636f 6d65 7320  n n index comes 
+00015580: 6672 6f6d 2061 6e20 6f75 7464 6174 6564  from an outdated
+00015590: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
+000155a0: 2020 4f74 6865 7277 6973 6520 6974 2075    Otherwise it u
+000155b0: 7064 6174 6573 2074 6865 2070 726f 6772  pdates the progr
+000155c0: 6573 7320 616e 6420 7265 7475 726e 7320  ess and returns 
+000155d0: 7472 7565 2e0a 2020 2020 2020 2020 2222  true..        ""
+000155e0: 220a 2020 2020 6465 6620 6d61 7962 655f  ".    def maybe_
+000155f0: 6465 6372 5f74 6f28 0a20 2020 2020 2020  decr_to(.       
+00015600: 2073 656c 662c 2072 656a 6563 7465 643a   self, rejected:
+00015610: 2069 6e74 2c20 6d61 7463 685f 6869 6e74   int, match_hint
+00015620: 3a20 696e 742c 2072 6571 7565 7374 5f73  : int, request_s
+00015630: 6e61 7073 686f 743a 2069 6e74 0a20 2020  napshot: int.   
+00015640: 2029 202d 3e20 626f 6f6c 3a0a 2020 2020   ) -> bool:.    
+00015650: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015660: 5265 7475 726e 7320 6661 6c73 6520 6966  Returns false if
+00015670: 2074 6865 2067 6976 656e 2069 6e64 6578   the given index
+00015680: 2063 6f6d 6573 2066 726f 6d20 616e 206f   comes from an o
+00015690: 7574 206f 6620 6f72 6465 7220 6d65 7373  ut of order mess
+000156a0: 6167 652e 0a20 2020 2020 2020 204f 7468  age..        Oth
+000156b0: 6572 7769 7365 2069 7420 6465 6372 6561  erwise it decrea
+000156c0: 7365 7320 7468 6520 7072 6f67 7265 7373  ses the progress
+000156d0: 206e 6578 7420 696e 6465 7820 746f 206d   next index to m
+000156e0: 696e 2872 656a 6563 7465 642c 206c 6173  in(rejected, las
+000156f0: 7429 0a20 2020 2020 2020 2061 6e64 2072  t).        and r
+00015700: 6574 7572 6e73 2074 7275 652e 0a20 2020  eturns true..   
+00015710: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00015720: 2073 6e61 7073 686f 745f 6661 696c 7572   snapshot_failur
+00015730: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+00015740: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015750: 2020 2020 2053 6574 7320 7468 6520 736e       Sets the sn
+00015760: 6170 7368 6f74 2074 6f20 6661 696c 7572  apshot to failur
+00015770: 652e 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
+00015780: 2020 2064 6566 2070 6175 7365 2873 656c     def pause(sel
+00015790: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+000157a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000157b0: 5061 7573 6520 7072 6f67 7265 7373 2e0a  Pause progress..
+000157c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000157d0: 6465 6620 6973 5f70 6175 7365 6428 7365  def is_paused(se
+000157e0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+000157f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00015800: 2044 6574 6572 6d69 6e65 2077 6865 7468   Determine wheth
+00015810: 6572 2070 726f 6772 6573 7320 6973 2070  er progress is p
+00015820: 6175 7365 642e 0a20 2020 2020 2020 2022  aused..        "
+00015830: 2222 0a20 2020 2064 6566 2069 735f 736e  "".    def is_sn
+00015840: 6170 7368 6f74 5f63 6175 6768 745f 7570  apshot_caught_up
+00015850: 2873 656c 6629 202d 3e20 626f 6f6c 3a0a  (self) -> bool:.
+00015860: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015870: 2020 2020 5265 7475 726e 7320 7472 7565      Returns true
+00015880: 2069 6620 4d61 7463 6820 6973 2065 7175   if Match is equ
+00015890: 616c 206f 7220 6869 6768 6572 2074 6861  al or higher tha
+000158a0: 6e20 7468 6520 7065 6e64 696e 6753 6e61  n the pendingSna
+000158b0: 7073 686f 742e 0a20 2020 2020 2020 2022  pshot..        "
+000158c0: 2222 0a20 2020 2064 6566 2072 6573 756d  "".    def resum
+000158d0: 6528 7365 6c66 2920 2d3e 204e 6f6e 653a  e(self) -> None:
+000158e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000158f0: 2020 2020 2052 6573 756d 6520 7072 6f67       Resume prog
+00015900: 7265 7373 0a20 2020 2020 2020 2022 2222  ress.        """
+00015910: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
+00015920: 7374 6174 6528 7365 6c66 2c20 6c61 7374  state(self, last
+00015930: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+00015940: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015950: 2020 2020 5570 6461 7465 2069 6e66 6c69      Update infli
+00015960: 6768 7420 6d73 6773 2061 6e64 206e 6578  ght msgs and nex
+00015970: 745f 6964 780a 2020 2020 2020 2020 2222  t_idx.        ""
+00015980: 220a 2020 2020 6465 6620 7570 6461 7465  ".    def update
+00015990: 5f63 6f6d 6d69 7474 6564 2873 656c 662c  _committed(self,
+000159a0: 2063 6f6d 6d69 7474 6564 5f69 6e64 6578   committed_index
+000159b0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a0a  : int) -> None:.
+000159c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000159d0: 2020 2020 5570 6461 7465 2063 6f6d 6d69      Update commi
+000159e0: 7474 6564 5f69 6e64 6578 2e0a 2020 2020  tted_index..    
+000159f0: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00015a00: 6f70 7469 6d69 7374 6963 5f75 7064 6174  optimistic_updat
+00015a10: 6528 7365 6c66 2c20 6e3a 2069 6e74 2920  e(self, n: int) 
+00015a20: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00015a30: 2022 2222 0a20 2020 2020 2020 204f 7074   """.        Opt
+00015a40: 696d 6973 7469 6361 6c6c 7920 6164 7661  imistically adva
+00015a50: 6e63 6520 7468 6520 696e 6465 780a 2020  nce the index.  
+00015a60: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00015a70: 6620 6765 745f 696e 7328 7365 6c66 2920  f get_ins(self) 
+00015a80: 2d3e 2022 496e 666c 6967 6874 7352 6566  -> "InflightsRef
+00015a90: 223a 0a20 2020 2020 2020 2022 2222 0a20  ":.        """. 
+00015aa0: 2020 2020 2020 2060 696e 7360 3a20 496e         `ins`: In
+00015ab0: 666c 6967 6874 7320 6973 2061 2073 6c69  flights is a sli
+00015ac0: 6469 6e67 2077 696e 646f 7720 666f 7220  ding window for 
+00015ad0: 7468 6520 696e 666c 6967 6874 206d 6573  the inflight mes
+00015ae0: 7361 6765 732e 0a20 2020 2020 2020 2057  sages..        W
+00015af0: 6865 6e20 696e 666c 6967 6874 7320 6973  hen inflights is
+00015b00: 2066 756c 6c2c 206e 6f20 6d6f 7265 206d   full, no more m
+00015b10: 6573 7361 6765 2073 686f 756c 6420 6265  essage should be
+00015b20: 2073 656e 742e 0a20 2020 2020 2020 2057   sent..        W
+00015b30: 6865 6e20 6120 6c65 6164 6572 2073 656e  hen a leader sen
+00015b40: 6473 206f 7574 2061 206d 6573 7361 6765  ds out a message
+00015b50: 2c20 7468 6520 696e 6465 7820 6f66 2074  , the index of t
+00015b60: 6865 206c 6173 740a 2020 2020 2020 2020  he last.        
+00015b70: 656e 7472 7920 7368 6f75 6c64 2062 6520  entry should be 
+00015b80: 6164 6465 6420 746f 2069 6e66 6c69 6768  added to infligh
+00015b90: 7473 2e20 5468 6520 696e 6465 7820 4d55  ts. The index MU
+00015ba0: 5354 2062 6520 6164 6465 640a 2020 2020  ST be added.    
+00015bb0: 2020 2020 696e 746f 2069 6e66 6c69 6768      into infligh
+00015bc0: 7473 2069 6e20 6f72 6465 722e 0a20 2020  ts in order..   
+00015bd0: 2020 2020 2057 6865 6e20 6120 6c65 6164       When a lead
+00015be0: 6572 2072 6563 6569 7665 7320 6120 7265  er receives a re
+00015bf0: 706c 792c 2074 6865 2070 7265 7669 6f75  ply, the previou
+00015c00: 7320 696e 666c 6967 6874 7320 7368 6f75  s inflights shou
+00015c10: 6c64 0a20 2020 2020 2020 2062 6520 6672  ld.        be fr
+00015c20: 6565 6420 6279 2063 616c 6c69 6e67 2069  eed by calling i
+00015c30: 6e66 6c69 6768 7473 2e66 7265 6554 6f2e  nflights.freeTo.
+00015c40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015c50: 2064 6566 2073 6574 5f69 6e73 2873 656c   def set_ins(sel
+00015c60: 662c 2069 6e66 6c69 6768 7473 3a20 2249  f, inflights: "I
+00015c70: 6e66 6c69 6768 7473 2220 7c20 2249 6e66  nflights" | "Inf
+00015c80: 6c69 6768 7473 5265 6622 2920 2d3e 204e  lightsRef") -> N
+00015c90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00015ca0: 0a20 2020 2020 2020 2060 696e 7360 3a20  .        `ins`: 
+00015cb0: 496e 666c 6967 6874 7320 6973 2061 2073  Inflights is a s
+00015cc0: 6c69 6469 6e67 2077 696e 646f 7720 666f  liding window fo
+00015cd0: 7220 7468 6520 696e 666c 6967 6874 206d  r the inflight m
+00015ce0: 6573 7361 6765 732e 0a20 2020 2020 2020  essages..       
+00015cf0: 2057 6865 6e20 696e 666c 6967 6874 7320   When inflights 
+00015d00: 6973 2066 756c 6c2c 206e 6f20 6d6f 7265  is full, no more
+00015d10: 206d 6573 7361 6765 2073 686f 756c 6420   message should 
+00015d20: 6265 2073 656e 742e 0a20 2020 2020 2020  be sent..       
+00015d30: 2057 6865 6e20 6120 6c65 6164 6572 2073   When a leader s
+00015d40: 656e 6473 206f 7574 2061 206d 6573 7361  ends out a messa
+00015d50: 6765 2c20 7468 6520 696e 6465 7820 6f66  ge, the index of
+00015d60: 2074 6865 206c 6173 740a 2020 2020 2020   the last.      
+00015d70: 2020 656e 7472 7920 7368 6f75 6c64 2062    entry should b
+00015d80: 6520 6164 6465 6420 746f 2069 6e66 6c69  e added to infli
+00015d90: 6768 7473 2e20 5468 6520 696e 6465 7820  ghts. The index 
+00015da0: 4d55 5354 2062 6520 6164 6465 640a 2020  MUST be added.  
+00015db0: 2020 2020 2020 696e 746f 2069 6e66 6c69        into infli
+00015dc0: 6768 7473 2069 6e20 6f72 6465 722e 0a20  ghts in order.. 
+00015dd0: 2020 2020 2020 2057 6865 6e20 6120 6c65         When a le
+00015de0: 6164 6572 2072 6563 6569 7665 7320 6120  ader receives a 
+00015df0: 7265 706c 792c 2074 6865 2070 7265 7669  reply, the previ
+00015e00: 6f75 7320 696e 666c 6967 6874 7320 7368  ous inflights sh
+00015e10: 6f75 6c64 0a20 2020 2020 2020 2062 6520  ould.        be 
+00015e20: 6672 6565 6420 6279 2063 616c 6c69 6e67  freed by calling
+00015e30: 2069 6e66 6c69 6768 7473 2e66 7265 6554   inflights.freeT
+00015e40: 6f2e 0a20 2020 2020 2020 2022 2222 0a20  o..        """. 
+00015e50: 2020 2064 6566 2067 6574 5f63 6f6d 6d69     def get_commi
+00015e60: 745f 6772 6f75 705f 6964 2873 656c 6629  t_group_id(self)
+00015e70: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00015e80: 2022 2222 0a20 2020 2020 2020 2060 636f   """.        `co
+00015e90: 6d6d 6974 5f67 726f 7570 5f69 6460 3a20  mmit_group_id`: 
+00015ea0: 4f6e 6c79 206c 6f67 7320 7265 706c 6963  Only logs replic
+00015eb0: 6174 6564 2074 6f20 6469 6666 6572 656e  ated to differen
+00015ec0: 7420 6772 6f75 7020 7769 6c6c 2062 6520  t group will be 
+00015ed0: 636f 6d6d 6974 7465 6420 6966 2061 6e79  committed if any
+00015ee0: 2067 726f 7570 2069 7320 636f 6e66 6967   group is config
+00015ef0: 7572 6564 2e0a 2020 2020 2020 2020 2222  ured..        ""
+00015f00: 220a 2020 2020 6465 6620 7365 745f 636f  ".    def set_co
+00015f10: 6d6d 6974 5f67 726f 7570 5f69 6428 7365  mmit_group_id(se
+00015f20: 6c66 2c20 636f 6d6d 6974 5f67 726f 7570  lf, commit_group
+00015f30: 5f69 643a 2069 6e74 2920 2d3e 204e 6f6e  _id: int) -> Non
+00015f40: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00015f50: 2020 2020 2020 2060 636f 6d6d 6974 5f67         `commit_g
+00015f60: 726f 7570 5f69 6460 3a20 4f6e 6c79 206c  roup_id`: Only l
+00015f70: 6f67 7320 7265 706c 6963 6174 6564 2074  ogs replicated t
+00015f80: 6f20 6469 6666 6572 656e 7420 6772 6f75  o different grou
+00015f90: 7020 7769 6c6c 2062 6520 636f 6d6d 6974  p will be commit
+00015fa0: 7465 6420 6966 2061 6e79 2067 726f 7570  ted if any group
+00015fb0: 2069 7320 636f 6e66 6967 7572 6564 2e0a   is configured..
+00015fc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015fd0: 6465 6620 6765 745f 636f 6d6d 6974 7465  def get_committe
+00015fe0: 645f 696e 6465 7828 7365 6c66 2920 2d3e  d_index(self) ->
+00015ff0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00016000: 220a 2020 2020 2020 2020 6063 6f6d 6d69  ".        `commi
+00016010: 7474 6564 5f69 6e64 6578 603a 2043 6f6d  tted_index`: Com
+00016020: 6d69 7474 6564 2069 6e64 6578 2069 6e20  mitted index in 
+00016030: 7261 6674 5f6c 6f67 0a20 2020 2020 2020  raft_log.       
+00016040: 2022 2222 0a20 2020 2064 6566 2073 6574   """.    def set
+00016050: 5f63 6f6d 6d69 7474 6564 5f69 6e64 6578  _committed_index
+00016060: 2873 656c 662c 2063 6f6d 6d69 7474 6564  (self, committed
+00016070: 5f69 6e64 6578 3a20 696e 7429 202d 3e20  _index: int) -> 
+00016080: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00016090: 220a 2020 2020 2020 2020 6063 6f6d 6d69  ".        `commi
+000160a0: 7474 6564 5f69 6e64 6578 603a 2043 6f6d  tted_index`: Com
+000160b0: 6d69 7474 6564 2069 6e64 6578 2069 6e20  mitted index in 
+000160c0: 7261 6674 5f6c 6f67 0a20 2020 2020 2020  raft_log.       
+000160d0: 2022 2222 0a20 2020 2064 6566 2067 6574   """.    def get
+000160e0: 5f6d 6174 6368 6564 2873 656c 6629 202d  _matched(self) -
+000160f0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00016100: 2222 0a20 2020 2020 2020 2060 6d61 7463  "".        `matc
+00016110: 6865 6460 3a20 486f 7720 6d75 6368 2073  hed`: How much s
+00016120: 7461 7465 2069 7320 6d61 7463 6865 642e  tate is matched.
+00016130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016140: 2064 6566 2073 6574 5f6d 6174 6368 6564   def set_matched
+00016150: 2873 656c 662c 206d 6174 6368 6564 3a20  (self, matched: 
+00016160: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00016170: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00016180: 2020 606d 6174 6368 6564 603a 2048 6f77    `matched`: How
+00016190: 206d 7563 6820 7374 6174 6520 6973 206d   much state is m
+000161a0: 6174 6368 6564 2e0a 2020 2020 2020 2020  atched..        
+000161b0: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+000161c0: 6e65 7874 5f69 6478 2873 656c 6629 202d  next_idx(self) -
+000161d0: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+000161e0: 2222 0a20 2020 2020 2020 2060 6e65 7874  "".        `next
+000161f0: 5f69 6478 603a 2054 6865 206e 6578 7420  _idx`: The next 
+00016200: 696e 6465 7820 746f 2061 7070 6c79 0a20  index to apply. 
+00016210: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00016220: 6566 2073 6574 5f6e 6578 745f 6964 7828  ef set_next_idx(
+00016230: 7365 6c66 2c20 6e65 7874 5f69 6478 3a20  self, next_idx: 
+00016240: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00016250: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00016260: 2020 606e 6578 745f 6964 7860 3a20 5468    `next_idx`: Th
+00016270: 6520 6e65 7874 2069 6e64 6578 2074 6f20  e next index to 
+00016280: 6170 706c 790a 2020 2020 2020 2020 2222  apply.        ""
+00016290: 220a 2020 2020 6465 6620 6765 745f 7065  ".    def get_pe
+000162a0: 6e64 696e 675f 736e 6170 7368 6f74 2873  nding_snapshot(s
+000162b0: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+000162c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000162d0: 2060 7065 6e64 696e 675f 736e 6170 7368   `pending_snapsh
+000162e0: 6f74 603a 2054 6869 7320 6669 656c 6420  ot`: This field 
+000162f0: 6973 2075 7365 6420 696e 2050 726f 6772  is used in Progr
+00016300: 6573 7353 7461 7465 536e 6170 7368 6f74  essStateSnapshot
+00016310: 2e0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
+00016320: 7265 2069 7320 6120 7065 6e64 696e 6720  re is a pending 
+00016330: 736e 6170 7368 6f74 2c20 7468 6520 7065  snapshot, the pe
+00016340: 6e64 696e 6753 6e61 7073 686f 7420 7769  ndingSnapshot wi
+00016350: 6c6c 2062 6520 7365 7420 746f 2074 6865  ll be set to the
+00016360: 0a20 2020 2020 2020 2069 6e64 6578 206f  .        index o
+00016370: 6620 7468 6520 736e 6170 7368 6f74 2e20  f the snapshot. 
+00016380: 4966 2070 656e 6469 6e67 536e 6170 7368  If pendingSnapsh
+00016390: 6f74 2069 7320 7365 742c 2074 6865 2072  ot is set, the r
+000163a0: 6570 6c69 6361 7469 6f6e 2070 726f 6365  eplication proce
+000163b0: 7373 206f 660a 2020 2020 2020 2020 7468  ss of.        th
+000163c0: 6973 2050 726f 6772 6573 7320 7769 6c6c  is Progress will
+000163d0: 2062 6520 7061 7573 6564 2e20 7261 6674   be paused. raft
+000163e0: 2077 696c 6c20 6e6f 7420 7265 7365 6e64   will not resend
+000163f0: 2073 6e61 7073 686f 7420 756e 7469 6c20   snapshot until 
+00016400: 7468 6520 7065 6e64 696e 6720 6f6e 650a  the pending one.
+00016410: 2020 2020 2020 2020 6973 2072 6570 6f72          is repor
+00016420: 7465 6420 746f 2062 6520 6661 696c 6564  ted to be failed
+00016430: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00016440: 2020 6465 6620 7365 745f 7065 6e64 696e    def set_pendin
+00016450: 675f 736e 6170 7368 6f74 2873 656c 662c  g_snapshot(self,
+00016460: 2070 656e 6469 6e67 5f73 6e61 7073 686f   pending_snapsho
+00016470: 743a 2069 6e74 2920 2d3e 204e 6f6e 653a  t: int) -> None:
+00016480: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016490: 2020 2020 2060 7065 6e64 696e 675f 736e       `pending_sn
+000164a0: 6170 7368 6f74 603a 2054 6869 7320 6669  apshot`: This fi
+000164b0: 656c 6420 6973 2075 7365 6420 696e 2050  eld is used in P
+000164c0: 726f 6772 6573 7353 7461 7465 536e 6170  rogressStateSnap
+000164d0: 7368 6f74 2e0a 2020 2020 2020 2020 4966  shot..        If
+000164e0: 2074 6865 7265 2069 7320 6120 7065 6e64   there is a pend
+000164f0: 696e 6720 736e 6170 7368 6f74 2c20 7468  ing snapshot, th
+00016500: 6520 7065 6e64 696e 6753 6e61 7073 686f  e pendingSnapsho
+00016510: 7420 7769 6c6c 2062 6520 7365 7420 746f  t will be set to
+00016520: 2074 6865 0a20 2020 2020 2020 2069 6e64   the.        ind
+00016530: 6578 206f 6620 7468 6520 736e 6170 7368  ex of the snapsh
+00016540: 6f74 2e20 4966 2070 656e 6469 6e67 536e  ot. If pendingSn
+00016550: 6170 7368 6f74 2069 7320 7365 742c 2074  apshot is set, t
+00016560: 6865 2072 6570 6c69 6361 7469 6f6e 2070  he replication p
+00016570: 726f 6365 7373 206f 660a 2020 2020 2020  rocess of.      
+00016580: 2020 7468 6973 2050 726f 6772 6573 7320    this Progress 
+00016590: 7769 6c6c 2062 6520 7061 7573 6564 2e20  will be paused. 
+000165a0: 7261 6674 2077 696c 6c20 6e6f 7420 7265  raft will not re
+000165b0: 7365 6e64 2073 6e61 7073 686f 7420 756e  send snapshot un
+000165c0: 7469 6c20 7468 6520 7065 6e64 696e 6720  til the pending 
+000165d0: 6f6e 650a 2020 2020 2020 2020 6973 2072  one.        is r
+000165e0: 6570 6f72 7465 6420 746f 2062 6520 6661  eported to be fa
+000165f0: 696c 6564 2e0a 2020 2020 2020 2020 2222  iled..        ""
+00016600: 220a 2020 2020 6465 6620 6765 745f 7065  ".    def get_pe
+00016610: 6e64 696e 675f 7265 7175 6573 745f 736e  nding_request_sn
+00016620: 6170 7368 6f74 2873 656c 6629 202d 3e20  apshot(self) -> 
+00016630: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
+00016640: 0a20 2020 2020 2020 2060 7065 6e64 696e  .        `pendin
+00016650: 675f 7265 7175 6573 745f 736e 6170 7368  g_request_snapsh
+00016660: 6f74 603a 2054 6869 7320 6669 656c 6420  ot`: This field 
+00016670: 6973 2075 7365 6420 696e 2072 6571 7565  is used in reque
+00016680: 7374 2073 6e61 7073 686f 742e 0a20 2020  st snapshot..   
+00016690: 2020 2020 2049 6620 7468 6572 6520 6973       If there is
+000166a0: 2061 2070 656e 6469 6e67 2072 6571 7565   a pending reque
+000166b0: 7374 2073 6e61 7073 686f 742c 2074 6869  st snapshot, thi
+000166c0: 7320 7769 6c6c 2062 6520 7365 7420 746f  s will be set to
+000166d0: 2074 6865 2072 6571 7565 7374 0a20 2020   the request.   
+000166e0: 2020 2020 2069 6e64 6578 206f 6620 7468       index of th
+000166f0: 6520 736e 6170 7368 6f74 2e0a 2020 2020  e snapshot..    
+00016700: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00016710: 7365 745f 7065 6e64 696e 675f 7265 7175  set_pending_requ
+00016720: 6573 745f 736e 6170 7368 6f74 2873 656c  est_snapshot(sel
+00016730: 662c 2070 656e 6469 6e67 5f72 6571 7565  f, pending_reque
+00016740: 7374 5f73 6e61 7073 686f 743a 2069 6e74  st_snapshot: int
+00016750: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00016760: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00016770: 7065 6e64 696e 675f 7265 7175 6573 745f  pending_request_
+00016780: 736e 6170 7368 6f74 603a 2054 6869 7320  snapshot`: This 
+00016790: 6669 656c 6420 6973 2075 7365 6420 696e  field is used in
+000167a0: 2072 6571 7565 7374 2073 6e61 7073 686f   request snapsho
+000167b0: 742e 0a20 2020 2020 2020 2049 6620 7468  t..        If th
+000167c0: 6572 6520 6973 2061 2070 656e 6469 6e67  ere is a pending
+000167d0: 2072 6571 7565 7374 2073 6e61 7073 686f   request snapsho
+000167e0: 742c 2074 6869 7320 7769 6c6c 2062 6520  t, this will be 
+000167f0: 7365 7420 746f 2074 6865 2072 6571 7565  set to the reque
+00016800: 7374 0a20 2020 2020 2020 2069 6e64 6578  st.        index
+00016810: 206f 6620 7468 6520 736e 6170 7368 6f74   of the snapshot
+00016820: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00016830: 2020 6465 6620 6765 745f 7265 6365 6e74    def get_recent
+00016840: 5f61 6374 6976 6528 7365 6c66 2920 2d3e  _active(self) ->
+00016850: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00016860: 2222 0a20 2020 2020 2020 2060 7265 6365  "".        `rece
+00016870: 6e74 5f61 6374 6976 6560 3a20 5468 6973  nt_active`: This
+00016880: 2069 7320 7472 7565 2069 6620 7468 6520   is true if the 
+00016890: 7072 6f67 7265 7373 2069 7320 7265 6365  progress is rece
+000168a0: 6e74 6c79 2061 6374 6976 652e 2052 6563  ntly active. Rec
+000168b0: 6569 7669 6e67 2061 6e79 206d 6573 7361  eiving any messa
+000168c0: 6765 730a 2020 2020 2020 2020 6672 6f6d  ges.        from
+000168d0: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+000168e0: 6e67 2066 6f6c 6c6f 7765 7220 696e 6469  ng follower indi
+000168f0: 6361 7465 7320 7468 6520 7072 6f67 7265  cates the progre
+00016900: 7373 2069 7320 6163 7469 7665 2e0a 2020  ss is active..  
+00016910: 2020 2020 2020 5265 6365 6e74 4163 7469        RecentActi
+00016920: 7665 2063 616e 2062 6520 7265 7365 7420  ve can be reset 
+00016930: 746f 2066 616c 7365 2061 6674 6572 2061  to false after a
+00016940: 6e20 656c 6563 7469 6f6e 2074 696d 656f  n election timeo
+00016950: 7574 2e0a 2020 2020 2020 2020 2222 220a  ut..        """.
+00016960: 2020 2020 6465 6620 7365 745f 7265 6365      def set_rece
+00016970: 6e74 5f61 6374 6976 6528 7365 6c66 2c20  nt_active(self, 
+00016980: 7265 6365 6e74 5f61 6374 6976 653a 2062  recent_active: b
+00016990: 6f6f 6c29 202d 3e20 4e6f 6e65 3a0a 2020  ool) -> None:.  
+000169a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000169b0: 2020 6072 6563 656e 745f 6163 7469 7665    `recent_active
+000169c0: 603a 2054 6869 7320 6973 2074 7275 6520  `: This is true 
+000169d0: 6966 2074 6865 2070 726f 6772 6573 7320  if the progress 
+000169e0: 6973 2072 6563 656e 746c 7920 6163 7469  is recently acti
+000169f0: 7665 2e20 5265 6365 6976 696e 6720 616e  ve. Receiving an
+00016a00: 7920 6d65 7373 6167 6573 0a20 2020 2020  y messages.     
+00016a10: 2020 2066 726f 6d20 7468 6520 636f 7272     from the corr
+00016a20: 6573 706f 6e64 696e 6720 666f 6c6c 6f77  esponding follow
+00016a30: 6572 2069 6e64 6963 6174 6573 2074 6865  er indicates the
+00016a40: 2070 726f 6772 6573 7320 6973 2061 6374   progress is act
+00016a50: 6976 652e 0a20 2020 2020 2020 2052 6563  ive..        Rec
+00016a60: 656e 7441 6374 6976 6520 6361 6e20 6265  entActive can be
+00016a70: 2072 6573 6574 2074 6f20 6661 6c73 6520   reset to false 
+00016a80: 6166 7465 7220 616e 2065 6c65 6374 696f  after an electio
+00016a90: 6e20 7469 6d65 6f75 742e 0a20 2020 2020  n timeout..     
+00016aa0: 2020 2022 2222 0a20 2020 2064 6566 2067     """.    def g
+00016ab0: 6574 5f70 6175 7365 6428 7365 6c66 2920  et_paused(self) 
+00016ac0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00016ad0: 2022 2222 0a20 2020 2020 2020 2060 7061   """.        `pa
+00016ae0: 7573 6564 603a 2050 6175 7365 6420 6973  used`: Paused is
+00016af0: 2075 7365 6420 696e 2050 726f 6772 6573   used in Progres
+00016b00: 7353 7461 7465 5072 6f62 652e 0a20 2020  sStateProbe..   
+00016b10: 2020 2020 2057 6865 6e20 5061 7573 6564       When Paused
+00016b20: 2069 7320 7472 7565 2c20 7261 6674 2073   is true, raft s
+00016b30: 686f 756c 6420 7061 7573 6520 7365 6e64  hould pause send
+00016b40: 696e 6720 7265 706c 6963 6174 696f 6e20  ing replication 
+00016b50: 6d65 7373 6167 6520 746f 2074 6869 7320  message to this 
+00016b60: 7065 6572 2e0a 2020 2020 2020 2020 2222  peer..        ""
+00016b70: 220a 2020 2020 6465 6620 7365 745f 7061  ".    def set_pa
+00016b80: 7573 6564 2873 656c 662c 2070 6175 7365  used(self, pause
+00016b90: 643a 2062 6f6f 6c29 202d 3e20 4e6f 6e65  d: bool) -> None
+00016ba0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00016bb0: 2020 2020 2020 6070 6175 7365 6460 3a20        `paused`: 
+00016bc0: 5061 7573 6564 2069 7320 7573 6564 2069  Paused is used i
+00016bd0: 6e20 5072 6f67 7265 7373 5374 6174 6550  n ProgressStateP
+00016be0: 726f 6265 2e0a 2020 2020 2020 2020 5768  robe..        Wh
+00016bf0: 656e 2050 6175 7365 6420 6973 2074 7275  en Paused is tru
+00016c00: 652c 2072 6166 7420 7368 6f75 6c64 2070  e, raft should p
+00016c10: 6175 7365 2073 656e 6469 6e67 2072 6570  ause sending rep
+00016c20: 6c69 6361 7469 6f6e 206d 6573 7361 6765  lication message
+00016c30: 2074 6f20 7468 6973 2070 6565 722e 0a20   to this peer.. 
+00016c40: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00016c50: 6566 2067 6574 5f73 7461 7465 2873 656c  ef get_state(sel
+00016c60: 6629 202d 3e20 2250 726f 6772 6573 7353  f) -> "ProgressS
+00016c70: 7461 7465 223a 0a20 2020 2020 2020 2022  tate":.        "
+00016c80: 2222 0a20 2020 2020 2020 2060 7374 6174  "".        `stat
+00016c90: 6560 3a20 5768 656e 2069 6e20 5072 6f67  e`: When in Prog
+00016ca0: 7265 7373 5374 6174 6550 726f 6265 2c20  ressStateProbe, 
+00016cb0: 6c65 6164 6572 2073 656e 6473 2061 7420  leader sends at 
+00016cc0: 6d6f 7374 206f 6e65 2072 6570 6c69 6361  most one replica
+00016cd0: 7469 6f6e 206d 6573 7361 6765 0a20 2020  tion message.   
+00016ce0: 2020 2020 2070 6572 2068 6561 7274 6265       per heartbe
+00016cf0: 6174 2069 6e74 6572 7661 6c2e 2049 7420  at interval. It 
+00016d00: 616c 736f 2070 726f 6265 7320 6163 7475  also probes actu
+00016d10: 616c 2070 726f 6772 6573 7320 6f66 2074  al progress of t
+00016d20: 6865 2066 6f6c 6c6f 7765 722e 0a0a 2020  he follower...  
+00016d30: 2020 2020 2020 5768 656e 2069 6e20 5072        When in Pr
+00016d40: 6f67 7265 7373 5374 6174 6552 6570 6c69  ogressStateRepli
+00016d50: 6361 7465 2c20 6c65 6164 6572 206f 7074  cate, leader opt
+00016d60: 696d 6973 7469 6361 6c6c 7920 696e 6372  imistically incr
+00016d70: 6561 7365 7320 6e65 7874 0a20 2020 2020  eases next.     
+00016d80: 2020 2074 6f20 7468 6520 6c61 7465 7374     to the latest
+00016d90: 2065 6e74 7279 2073 656e 7420 6166 7465   entry sent afte
+00016da0: 7220 7365 6e64 696e 6720 7265 706c 6963  r sending replic
+00016db0: 6174 696f 6e20 6d65 7373 6167 652e 2054  ation message. T
+00016dc0: 6869 7320 6973 0a20 2020 2020 2020 2061  his is.        a
+00016dd0: 6e20 6f70 7469 6d69 7a65 6420 7374 6174  n optimized stat
+00016de0: 6520 666f 7220 6661 7374 2072 6570 6c69  e for fast repli
+00016df0: 6361 7469 6e67 206c 6f67 2065 6e74 7269  cating log entri
+00016e00: 6573 2074 6f20 7468 6520 666f 6c6c 6f77  es to the follow
+00016e10: 6572 2e0a 0a20 2020 2020 2020 2057 6865  er...        Whe
+00016e20: 6e20 696e 2050 726f 6772 6573 7353 7461  n in ProgressSta
+00016e30: 7465 536e 6170 7368 6f74 2c20 6c65 6164  teSnapshot, lead
+00016e40: 6572 2073 686f 756c 6420 6861 7665 2073  er should have s
+00016e50: 656e 7420 6f75 7420 736e 6170 7368 6f74  ent out snapshot
+00016e60: 0a20 2020 2020 2020 2062 6566 6f72 6520  .        before 
+00016e70: 616e 6420 7374 6f70 2073 656e 6469 6e67  and stop sending
+00016e80: 2061 6e79 2072 6570 6c69 6361 7469 6f6e   any replication
+00016e90: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
+00016ea0: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00016eb0: 745f 7374 6174 6528 7365 6c66 2c20 7374  t_state(self, st
+00016ec0: 6174 653a 2022 5072 6f67 7265 7373 5374  ate: "ProgressSt
+00016ed0: 6174 6522 2920 2d3e 204e 6f6e 653a 0a20  ate") -> None:. 
+00016ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016ef0: 2020 2060 7374 6174 6560 3a20 5768 656e     `state`: When
+00016f00: 2069 6e20 5072 6f67 7265 7373 5374 6174   in ProgressStat
+00016f10: 6550 726f 6265 2c20 6c65 6164 6572 2073  eProbe, leader s
+00016f20: 656e 6473 2061 7420 6d6f 7374 206f 6e65  ends at most one
+00016f30: 2072 6570 6c69 6361 7469 6f6e 206d 6573   replication mes
+00016f40: 7361 6765 0a20 2020 2020 2020 2070 6572  sage.        per
+00016f50: 2068 6561 7274 6265 6174 2069 6e74 6572   heartbeat inter
+00016f60: 7661 6c2e 2049 7420 616c 736f 2070 726f  val. It also pro
+00016f70: 6265 7320 6163 7475 616c 2070 726f 6772  bes actual progr
+00016f80: 6573 7320 6f66 2074 6865 2066 6f6c 6c6f  ess of the follo
+00016f90: 7765 722e 0a0a 2020 2020 2020 2020 5768  wer...        Wh
+00016fa0: 656e 2069 6e20 5072 6f67 7265 7373 5374  en in ProgressSt
+00016fb0: 6174 6552 6570 6c69 6361 7465 2c20 6c65  ateReplicate, le
+00016fc0: 6164 6572 206f 7074 696d 6973 7469 6361  ader optimistica
+00016fd0: 6c6c 7920 696e 6372 6561 7365 7320 6e65  lly increases ne
+00016fe0: 7874 0a20 2020 2020 2020 2074 6f20 7468  xt.        to th
+00016ff0: 6520 6c61 7465 7374 2065 6e74 7279 2073  e latest entry s
+00017000: 656e 7420 6166 7465 7220 7365 6e64 696e  ent after sendin
+00017010: 6720 7265 706c 6963 6174 696f 6e20 6d65  g replication me
+00017020: 7373 6167 652e 2054 6869 7320 6973 0a20  ssage. This is. 
+00017030: 2020 2020 2020 2061 6e20 6f70 7469 6d69         an optimi
+00017040: 7a65 6420 7374 6174 6520 666f 7220 6661  zed state for fa
+00017050: 7374 2072 6570 6c69 6361 7469 6e67 206c  st replicating l
+00017060: 6f67 2065 6e74 7269 6573 2074 6f20 7468  og entries to th
+00017070: 6520 666f 6c6c 6f77 6572 2e0a 0a20 2020  e follower...   
+00017080: 2020 2020 2057 6865 6e20 696e 2050 726f       When in Pro
+00017090: 6772 6573 7353 7461 7465 536e 6170 7368  gressStateSnapsh
+000170a0: 6f74 2c20 6c65 6164 6572 2073 686f 756c  ot, leader shoul
+000170b0: 6420 6861 7665 2073 656e 7420 6f75 7420  d have sent out 
+000170c0: 736e 6170 7368 6f74 0a20 2020 2020 2020  snapshot.       
+000170d0: 2062 6566 6f72 6520 616e 6420 7374 6f70   before and stop
+000170e0: 2073 656e 6469 6e67 2061 6e79 2072 6570   sending any rep
+000170f0: 6c69 6361 7469 6f6e 206d 6573 7361 6765  lication message
+00017100: 2e0a 2020 2020 2020 2020 2222 220a 0a63  ..        """..c
+00017110: 6c61 7373 2050 726f 6772 6573 7328 5f5f  lass Progress(__
+00017120: 4150 495f 5072 6f67 7265 7373 293a 0a20  API_Progress):. 
+00017130: 2020 2022 2222 0a20 2020 2054 6865 2070     """.    The p
+00017140: 726f 6772 6573 7320 6f66 2063 6174 6368  rogress of catch
+00017150: 696e 6720 7570 2066 726f 6d20 6120 7265  ing up from a re
+00017160: 7374 6172 742e 0a20 2020 2022 2222 0a0a  start..    """..
+00017170: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00017180: 2873 656c 662c 206e 6578 745f 6964 783a  (self, next_idx:
+00017190: 2069 6e74 2c20 696e 735f 7369 7a65 3a20   int, ins_size: 
+000171a0: 696e 7429 202d 3e20 4e6f 6e65 3a20 2e2e  int) -> None: ..
+000171b0: 2e0a 2020 2020 6465 6620 6d61 6b65 5f72  ..    def make_r
+000171c0: 6566 2873 656c 6629 202d 3e20 2250 726f  ef(self) -> "Pro
+000171d0: 6772 6573 7352 6566 223a 202e 2e2e 0a0a  gressRef": .....
+000171e0: 636c 6173 7320 5072 6f67 7265 7373 5265  class ProgressRe
+000171f0: 6628 5f5f 4150 495f 5072 6f67 7265 7373  f(__API_Progress
+00017200: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
+00017210: 6566 6572 656e 6365 2074 7970 6520 6f66  eference type of
+00017220: 203a 636c 6173 733a 6050 726f 6772 6573   :class:`Progres
+00017230: 7360 2e0a 2020 2020 2222 220a 0a63 6c61  s`..    """..cla
+00017240: 7373 205f 5f41 5049 5f4a 6f69 6e74 436f  ss __API_JointCo
+00017250: 6e66 6967 285f 5f43 6c6f 6e65 6162 6c65  nfig(__Cloneable
+00017260: 293a 0a20 2020 2064 6566 2063 6c6f 6e65  ):.    def clone
+00017270: 2873 656c 6629 202d 3e20 224a 6f69 6e74  (self) -> "Joint
+00017280: 436f 6e66 6967 223a 202e 2e2e 0a20 2020  Config": ....   
+00017290: 2064 6566 2063 6c65 6172 2873 656c 6629   def clear(self)
+000172a0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000172b0: 2020 2222 2243 6c65 6172 7320 616c 6c20    """Clears all 
+000172c0: 4944 732e 2222 220a 2020 2020 6465 6620  IDs.""".    def 
+000172d0: 636f 6e74 6169 6e73 2873 656c 662c 2069  contains(self, i
+000172e0: 643a 2069 6e74 2920 2d3e 2062 6f6f 6c3a  d: int) -> bool:
+000172f0: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
+00017300: 6b20 6966 2061 6e20 6964 2069 7320 6120  k if an id is a 
+00017310: 766f 7465 722e 2222 220a 2020 2020 6465  voter.""".    de
+00017320: 6620 6964 7328 2920 2d3e 2053 6574 5b69  f ids() -> Set[i
+00017330: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
+00017340: 5265 7475 726e 7320 616e 2069 7465 7261  Returns an itera
+00017350: 746f 7220 6f76 6572 2074 776f 2068 6173  tor over two has
+00017360: 6820 7365 7420 7769 7468 6f75 7420 636c  h set without cl
+00017370: 6f6e 696e 672e 2222 220a 2020 2020 6465  oning.""".    de
+00017380: 6620 6973 5f73 696e 676c 6574 6f6e 2873  f is_singleton(s
+00017390: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+000173a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000173b0: 2020 5265 7475 726e 7320 7472 7565 2069    Returns true i
+000173c0: 6620 2861 6e64 206f 6e6c 7920 6966 2920  f (and only if) 
+000173d0: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
+000173e0: 6520 766f 7469 6e67 206d 656d 6265 720a  e voting member.
+000173f0: 2020 2020 2020 2020 2869 2e65 2e20 7468          (i.e. th
+00017400: 6520 6c65 6164 6572 2920 696e 2074 6865  e leader) in the
+00017410: 2063 7572 7265 6e74 2063 6f6e 6669 6775   current configu
+00017420: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+00017430: 2222 220a 0a63 6c61 7373 204a 6f69 6e74  """..class Joint
+00017440: 436f 6e66 6967 285f 5f41 5049 5f4a 6f69  Config(__API_Joi
+00017450: 6e74 436f 6e66 6967 293a 0a20 2020 2022  ntConfig):.    "
+00017460: 2222 0a20 2020 2041 2063 6f6e 6669 6775  "".    A configu
+00017470: 7261 7469 6f6e 206f 6620 7477 6f20 6772  ration of two gr
+00017480: 6f75 7073 206f 6620 2870 6f73 7369 626c  oups of (possibl
+00017490: 7920 6f76 6572 6c61 7070 696e 6729 206d  y overlapping) m
+000174a0: 616a 6f72 6974 7920 636f 6e66 6967 7572  ajority configur
+000174b0: 6174 696f 6e73 2e0a 2020 2020 4465 6369  ations..    Deci
+000174c0: 7369 6f6e 7320 7265 7175 6972 6520 7468  sions require th
+000174d0: 6520 7375 7070 6f72 7420 6f66 2062 6f74  e support of bot
+000174e0: 6820 6d61 6a6f 7269 7469 6573 2e0a 2020  h majorities..  
+000174f0: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+00017500: 5f69 6e69 745f 5f28 7365 6c66 2c20 766f  _init__(self, vo
+00017510: 7465 7273 3a20 5365 745b 696e 745d 2920  ters: Set[int]) 
+00017520: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+00017530: 2064 6566 206d 616b 655f 7265 6628 7365   def make_ref(se
+00017540: 6c66 2920 2d3e 2022 4a6f 696e 7443 6f6e  lf) -> "JointCon
+00017550: 6669 6752 6566 223a 202e 2e2e 0a0a 636c  figRef": .....cl
+00017560: 6173 7320 4a6f 696e 7443 6f6e 6669 6752  ass JointConfigR
+00017570: 6566 285f 5f41 5049 5f4a 6f69 6e74 436f  ef(__API_JointCo
+00017580: 6e66 6967 293a 0a20 2020 2022 2222 0a20  nfig):.    """. 
+00017590: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
+000175a0: 6520 6f66 203a 636c 6173 733a 604a 6f69  e of :class:`Joi
+000175b0: 6e74 436f 6e66 6967 602e 0a20 2020 2022  ntConfig`..    "
+000175c0: 2222 0a0a 636c 6173 7320 5f5f 4150 495f  ""..class __API_
+000175d0: 4d61 6a6f 7269 7479 436f 6e66 6967 285f  MajorityConfig(_
+000175e0: 5f43 6c6f 6e65 6162 6c65 293a 0a20 2020  _Cloneable):.   
+000175f0: 2064 6566 2063 6c6f 6e65 2873 656c 6629   def clone(self)
+00017600: 202d 3e20 224d 616a 6f72 6974 7943 6f6e   -> "MajorityCon
+00017610: 6669 6722 3a20 2e2e 2e0a 2020 2020 6465  fig": ....    de
+00017620: 6620 7261 775f 736c 6963 6528 7365 6c66  f raw_slice(self
+00017630: 2920 2d3e 204c 6973 745b 696e 745d 3a0a  ) -> List[int]:.
+00017640: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00017650: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+00017660: 4d61 6a6f 7269 7479 436f 6e66 6967 2061  MajorityConfig a
+00017670: 7320 6120 736c 6963 652e 0a20 2020 2020  s a slice..     
+00017680: 2020 2022 2222 0a20 2020 2064 6566 2063     """.    def c
+00017690: 6170 6163 6974 7928 7365 6c66 2920 2d3e  apacity(self) ->
+000176a0: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+000176b0: 2222 2222 0a20 2020 2064 6566 2065 7874  """".    def ext
+000176c0: 656e 6428 7365 6c66 2c20 6f74 6865 725f  end(self, other_
+000176d0: 7365 743a 2053 6574 5b69 6e74 5d29 202d  set: Set[int]) -
+000176e0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+000176f0: 2222 2222 2222 0a20 2020 2064 6566 2067  """""".    def g
+00017700: 6574 2873 656c 662c 2069 6e64 6578 3a20  et(self, index: 
+00017710: 696e 7429 202d 3e20 4f70 7469 6f6e 616c  int) -> Optional
+00017720: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
+00017730: 2222 2222 220a 2020 2020 6465 6620 696e  """"".    def in
+00017740: 7365 7274 2873 656c 662c 2076 616c 7565  sert(self, value
+00017750: 3a20 696e 7429 202d 3e20 626f 6f6c 3a0a  : int) -> bool:.
+00017760: 2020 2020 2020 2020 2222 2222 2222 0a20          """""". 
+00017770: 2020 2064 6566 2072 6570 6c61 6365 2873     def replace(s
+00017780: 656c 662c 2076 616c 7565 3a20 696e 7429  elf, value: int)
+00017790: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+000177a0: 2022 2222 2222 220a 2020 2020 6465 6620   """""".    def 
+000177b0: 6973 5f64 6973 6a6f 696e 7428 7365 6c66  is_disjoint(self
+000177c0: 2c20 6f74 6865 723a 2053 6574 5b69 6e74  , other: Set[int
+000177d0: 5d29 202d 3e20 626f 6f6c 3a0a 2020 2020  ]) -> bool:.    
+000177e0: 2020 2020 2222 2222 2222 0a20 2020 2064      """""".    d
+000177f0: 6566 2069 735f 7375 7065 7273 6574 2873  ef is_superset(s
+00017800: 656c 662c 206f 7468 6572 3a20 5365 745b  elf, other: Set[
+00017810: 696e 745d 2920 2d3e 2062 6f6f 6c3a 0a20  int]) -> bool:. 
+00017820: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
+00017830: 2020 6465 6620 6973 5f73 7562 7365 7428    def is_subset(
+00017840: 7365 6c66 2c20 6f74 6865 723a 2053 6574  self, other: Set
+00017850: 5b69 6e74 5d29 202d 3e20 626f 6f6c 3a0a  [int]) -> bool:.
+00017860: 2020 2020 2020 2020 2222 2222 2222 0a20          """""". 
+00017870: 2020 2064 6566 2072 6573 6572 7665 2873     def reserve(s
+00017880: 656c 662c 2061 6464 6974 696f 6e61 6c3a  elf, additional:
+00017890: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+000178a0: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
+000178b0: 2020 6465 6620 7265 6d6f 7665 2873 656c    def remove(sel
+000178c0: 662c 2076 616c 7565 3a20 696e 7429 202d  f, value: int) -
+000178d0: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+000178e0: 2222 2222 2222 0a20 2020 2064 6566 2073  """""".    def s
+000178f0: 6872 696e 6b5f 746f 2873 656c 662c 206d  hrink_to(self, m
+00017900: 696e 5f63 6170 6163 6974 793a 2069 6e74  in_capacity: int
+00017910: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00017920: 2020 2022 2222 2222 220a 2020 2020 6465     """""".    de
+00017930: 6620 7368 7269 6e6b 5f74 6f5f 6669 7428  f shrink_to_fit(
+00017940: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00017950: 2020 2020 2020 2022 2222 2222 220a 2020         """""".  
+00017960: 2020 6465 6620 7472 795f 7265 7365 7276    def try_reserv
+00017970: 6528 7365 6c66 2c20 6164 6469 7469 6f6e  e(self, addition
+00017980: 616c 3a20 696e 7429 202d 3e20 4e6f 6e65  al: int) -> None
+00017990: 3a0a 2020 2020 2020 2020 2222 2222 2222  :.        """"""
+000179a0: 0a0a 636c 6173 7320 4d61 6a6f 7269 7479  ..class Majority
+000179b0: 436f 6e66 6967 285f 5f41 5049 5f4d 616a  Config(__API_Maj
+000179c0: 6f72 6974 7943 6f6e 6669 6729 3a0a 2020  orityConfig):.  
+000179d0: 2020 2222 220a 2020 2020 4120 7365 7420    """.    A set 
+000179e0: 6f66 2049 4473 2074 6861 7420 7573 6573  of IDs that uses
+000179f0: 206d 616a 6f72 6974 7920 7175 6f72 756d   majority quorum
+00017a00: 7320 746f 206d 616b 6520 6465 6369 7369  s to make decisi
+00017a10: 6f6e 732e 0a20 2020 2022 2222 0a0a 2020  ons..    """..  
+00017a20: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00017a30: 656c 662c 2076 6f74 6572 733a 2053 6574  elf, voters: Set
+00017a40: 5b69 6e74 5d29 202d 3e20 4e6f 6e65 3a20  [int]) -> None: 
+00017a50: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
+00017a60: 5f72 6566 2873 656c 6629 202d 3e20 224d  _ref(self) -> "M
+00017a70: 616a 6f72 6974 7943 6f6e 6669 6752 6566  ajorityConfigRef
+00017a80: 223a 202e 2e2e 0a0a 636c 6173 7320 4d61  ": .....class Ma
+00017a90: 6a6f 7269 7479 436f 6e66 6967 5265 6628  jorityConfigRef(
+00017aa0: 5f5f 4150 495f 4d61 6a6f 7269 7479 436f  __API_MajorityCo
+00017ab0: 6e66 6967 293a 0a20 2020 2022 2222 0a20  nfig):.    """. 
+00017ac0: 2020 2052 6566 6572 656e 6365 2074 7970     Reference typ
+00017ad0: 6520 6f66 203a 636c 6173 733a 604d 616a  e of :class:`Maj
+00017ae0: 6f72 6974 7943 6f6e 6669 6760 2e0a 2020  orityConfig`..  
+00017af0: 2020 2222 220a 0a63 6c61 7373 205f 5f41    """..class __A
+00017b00: 5049 5f49 6e66 6c69 6768 7473 285f 5f43  PI_Inflights(__C
+00017b10: 6c6f 6e65 6162 6c65 293a 0a20 2020 2064  loneable):.    d
+00017b20: 6566 2063 6c6f 6e65 2873 656c 6629 202d  ef clone(self) -
+00017b30: 3e20 2249 6e66 6c69 6768 7473 223a 202e  > "Inflights": .
+00017b40: 2e2e 0a20 2020 2064 6566 2061 6464 2873  ...    def add(s
+00017b50: 656c 662c 2069 6e66 6c69 6768 743a 2069  elf, inflight: i
+00017b60: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00017b70: 2020 2020 2022 2222 4164 6473 2061 6e20       """Adds an 
+00017b80: 696e 666c 6967 6874 2069 6e74 6f20 696e  inflight into in
+00017b90: 666c 6967 6874 7322 2222 0a20 2020 2064  flights""".    d
+00017ba0: 6566 2066 756c 6c28 7365 6c66 2920 2d3e  ef full(self) ->
+00017bb0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00017bc0: 2222 5265 7475 726e 7320 7472 7565 2069  ""Returns true i
+00017bd0: 6620 7468 6520 696e 666c 6967 6874 7320  f the inflights 
+00017be0: 6973 2066 756c 6c2e 2222 220a 2020 2020  is full.""".    
+00017bf0: 6465 6620 7265 7365 7428 7365 6c66 2920  def reset(self) 
+00017c00: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00017c10: 2022 2222 4672 6565 7320 616c 6c20 696e   """Frees all in
+00017c20: 666c 6967 6874 732e 2222 220a 2020 2020  flights.""".    
+00017c30: 6465 6620 6672 6565 5f74 6f28 7365 6c66  def free_to(self
+00017c40: 2c20 746f 3a20 696e 7429 202d 3e20 4e6f  , to: int) -> No
+00017c50: 6e65 3a0a 2020 2020 2020 2020 2222 2246  ne:.        """F
+00017c60: 7265 6573 2074 6865 2069 6e66 6c69 6768  rees the infligh
+00017c70: 7473 2073 6d61 6c6c 6572 206f 7220 6571  ts smaller or eq
+00017c80: 7561 6c20 746f 2074 6865 2067 6976 656e  ual to the given
+00017c90: 2060 746f 6020 666c 6967 6874 2e22 2222   `to` flight."""
+00017ca0: 0a20 2020 2064 6566 2066 7265 655f 6669  .    def free_fi
+00017cb0: 7273 745f 6f6e 6528 7365 6c66 2920 2d3e  rst_one(self) ->
+00017cc0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00017cd0: 2222 4672 6565 7320 7468 6520 6669 7273  ""Frees the firs
+00017ce0: 7420 6275 6666 6572 2065 6e74 7279 2e22  t buffer entry."
+00017cf0: 2222 0a20 2020 2064 6566 206d 6179 6265  "".    def maybe
+00017d00: 5f66 7265 655f 6275 6666 6572 2873 656c  _free_buffer(sel
+00017d10: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00017d20: 2020 2020 2222 2246 7265 6520 756e 7573      """Free unus
+00017d30: 6564 206d 656d 6f72 7922 2222 0a20 2020  ed memory""".   
+00017d40: 2064 6566 2062 7566 6665 725f 6361 7061   def buffer_capa
+00017d50: 6369 7479 2873 656c 6629 202d 3e20 696e  city(self) -> in
+00017d60: 743a 0a20 2020 2020 2020 2022 2222 4361  t:.        """Ca
+00017d70: 7061 6369 7479 206f 6620 7468 6520 696e  pacity of the in
+00017d80: 7465 726e 616c 2062 7566 6665 722e 2222  ternal buffer.""
+00017d90: 220a 2020 2020 6465 6620 6275 6666 6572  ".    def buffer
+00017da0: 5f69 735f 616c 6c6f 6361 7465 6428 7365  _is_allocated(se
+00017db0: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00017dc0: 2020 2020 2022 2222 5768 6574 6865 7220       """Whether 
+00017dd0: 6275 6666 6572 2069 7320 616c 6c6f 6361  buffer is alloca
+00017de0: 7465 6420 6f72 206e 6f74 2e20 4974 2773  ted or not. It's
+00017df0: 2066 6f72 2074 6573 7473 2e22 2222 0a20   for tests.""". 
+00017e00: 2020 2064 6566 2063 6f75 6e74 2873 656c     def count(sel
+00017e10: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00017e20: 2020 2022 2222 4e75 6d62 6572 206f 6620     """Number of 
+00017e30: 696e 666c 6967 6874 206d 6573 7361 6765  inflight message
+00017e40: 732e 2049 7427 7320 666f 7220 7465 7374  s. It's for test
+00017e50: 732e 2222 220a 2020 2020 6465 6620 7365  s.""".    def se
+00017e60: 745f 6361 7028 7365 6c66 2c20 696e 636f  t_cap(self, inco
+00017e70: 6d69 6e67 5f63 6170 3a20 696e 7429 202d  ming_cap: int) -
+00017e80: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00017e90: 2222 220a 2020 2020 2020 2020 4164 6a75  """.        Adju
+00017ea0: 7374 2069 6e66 6c69 6768 7420 6275 6666  st inflight buff
+00017eb0: 6572 2063 6170 6163 6974 792e 2053 6574  er capacity. Set
+00017ec0: 2069 7420 746f 2060 3060 2077 696c 6c20   it to `0` will 
+00017ed0: 6469 7361 626c 6520 7468 6520 7072 6f67  disable the prog
+00017ee0: 7265 7373 2e0a 2020 2020 2020 2020 4361  ress..        Ca
+00017ef0: 6c6c 696e 6720 6974 2062 6574 7765 656e  lling it between
+00017f00: 2060 7365 6c66 2e66 756c 6c28 2960 2061   `self.full()` a
+00017f10: 6e64 2060 7365 6c66 2e61 6464 2829 6020  nd `self.add()` 
+00017f20: 6361 6e20 6361 7573 6520 6120 7061 6e69  can cause a pani
+00017f30: 632e 0a20 2020 2020 2020 2022 2222 0a0a  c..        """..
+00017f40: 636c 6173 7320 496e 666c 6967 6874 7328  class Inflights(
+00017f50: 5f5f 4150 495f 496e 666c 6967 6874 7329  __API_Inflights)
+00017f60: 3a0a 2020 2020 2222 220a 2020 2020 4120  :.    """.    A 
+00017f70: 6275 6666 6572 206f 6620 696e 666c 6967  buffer of inflig
+00017f80: 6874 206d 6573 7361 6765 732e 0a20 2020  ht messages..   
+00017f90: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+00017fa0: 696e 6974 5f5f 2873 656c 662c 2063 6170  init__(self, cap
+00017fb0: 3a20 696e 7429 202d 3e20 4e6f 6e65 3a20  : int) -> None: 
+00017fc0: 2e2e 2e0a 2020 2020 6465 6620 6d61 6b65  ....    def make
+00017fd0: 5f72 6566 2873 656c 6629 202d 3e20 2249  _ref(self) -> "I
+00017fe0: 6e66 6c69 6768 7473 5265 6622 3a20 2e2e  nflightsRef": ..
+00017ff0: 2e0a 0a63 6c61 7373 2049 6e66 6c69 6768  ...class Infligh
+00018000: 7473 5265 6628 5f5f 4150 495f 496e 666c  tsRef(__API_Infl
+00018010: 6967 6874 7329 3a0a 2020 2020 2222 220a  ights):.    """.
+00018020: 2020 2020 5265 6665 7265 6e63 6520 7479      Reference ty
+00018030: 7065 206f 6620 3a63 6c61 7373 3a60 496e  pe of :class:`In
+00018040: 666c 6967 6874 7352 6566 602e 0a20 2020  flightsRef`..   
+00018050: 2022 2222 0a0a 636c 6173 7320 5f5f 4150   """..class __AP
+00018060: 495f 436f 6e66 6967 285f 5f43 6c6f 6e65  I_Config(__Clone
+00018070: 6162 6c65 293a 0a20 2020 2064 6566 2063  able):.    def c
+00018080: 6c6f 6e65 2873 656c 6629 202d 3e20 2243  lone(self) -> "C
+00018090: 6f6e 6669 6722 3a20 2e2e 2e0a 2020 2020  onfig": ....    
+000180a0: 6465 6620 6d69 6e5f 656c 6563 7469 6f6e  def min_election
+000180b0: 5f74 6963 6b28 7365 6c66 2920 2d3e 2069  _tick(self) -> i
+000180c0: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+000180d0: 2020 2020 2020 2020 606d 696e 5f65 6c65          `min_ele
+000180e0: 6374 696f 6e5f 7469 636b 603a 2054 6865  ction_tick`: The
+000180f0: 206d 696e 696d 756d 206e 756d 6265 7220   minimum number 
+00018100: 6f66 2074 6963 6b73 2062 6566 6f72 6520  of ticks before 
+00018110: 616e 2065 6c65 6374 696f 6e2e 0a20 2020  an election..   
+00018120: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00018130: 2073 6574 5f6d 696e 5f65 6c65 6374 696f   set_min_electio
+00018140: 6e5f 7469 636b 2873 656c 662c 206d 696e  n_tick(self, min
+00018150: 5f65 6c65 6374 696f 6e5f 7469 636b 3a20  _election_tick: 
+00018160: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00018170: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00018180: 2020 606d 696e 5f65 6c65 6374 696f 6e5f    `min_election_
+00018190: 7469 636b 603a 2054 6865 206d 696e 696d  tick`: The minim
+000181a0: 756d 206e 756d 6265 7220 6f66 2074 6963  um number of tic
+000181b0: 6b73 2062 6566 6f72 6520 616e 2065 6c65  ks before an ele
+000181c0: 6374 696f 6e2e 0a20 2020 2020 2020 2022  ction..        "
+000181d0: 2222 0a20 2020 2064 6566 206d 6178 5f65  "".    def max_e
+000181e0: 6c65 6374 696f 6e5f 7469 636b 2873 656c  lection_tick(sel
+000181f0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00018200: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00018210: 6d61 785f 656c 6563 7469 6f6e 5f74 6963  max_election_tic
+00018220: 6b60 3a20 5468 6520 6d61 7869 6d75 6d20  k`: The maximum 
+00018230: 6e75 6d62 6572 206f 6620 7469 636b 7320  number of ticks 
+00018240: 6265 666f 7265 2061 6e20 656c 6563 7469  before an electi
+00018250: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
+00018260: 2020 2020 6465 6620 7365 745f 6d61 785f      def set_max_
+00018270: 656c 6563 7469 6f6e 5f74 6963 6b28 7365  election_tick(se
+00018280: 6c66 2c20 6d61 785f 656c 6563 7469 6f6e  lf, max_election
+00018290: 5f74 6963 6b3a 2069 6e74 2920 2d3e 204e  _tick: int) -> N
+000182a0: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+000182b0: 0a20 2020 2020 2020 2060 6d61 785f 656c  .        `max_el
+000182c0: 6563 7469 6f6e 5f74 6963 6b60 3a20 5468  ection_tick`: Th
+000182d0: 6520 6d61 7869 6d75 6d20 6e75 6d62 6572  e maximum number
+000182e0: 206f 6620 7469 636b 7320 6265 666f 7265   of ticks before
+000182f0: 2061 6e20 656c 6563 7469 6f6e 2e0a 2020   an election..  
+00018300: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00018310: 6620 6765 745f 7265 6164 5f6f 6e6c 795f  f get_read_only_
+00018320: 6f70 7469 6f6e 2873 656c 6629 202d 3e20  option(self) -> 
+00018330: 2252 6561 644f 6e6c 794f 7074 696f 6e22  "ReadOnlyOption"
+00018340: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00018350: 2020 2020 2020 6072 6561 645f 6f6e 6c79        `read_only
+00018360: 5f6f 7074 696f 6e60 3a20 4368 6f6f 7365  _option`: Choose
+00018370: 2074 6865 206c 696e 6561 7269 7a61 6269   the linearizabi
+00018380: 6c69 7479 206d 6f64 6520 6f72 2074 6865  lity mode or the
+00018390: 206c 6561 7365 206d 6f64 6520 746f 2072   lease mode to r
+000183a0: 6561 6420 6461 7461 2e20 4966 2079 6f75  ead data. If you
+000183b0: 2064 6f6e e280 9974 2063 6172 6520 6162   don...t care ab
+000183c0: 6f75 7420 7468 6520 7265 6164 2063 6f6e  out the read con
+000183d0: 7369 7374 656e 6379 2061 6e64 2077 616e  sistency and wan
+000183e0: 7420 6120 6869 6768 6572 2072 6561 6420  t a higher read 
+000183f0: 7065 7266 6f72 6d61 6e63 652c 2079 6f75  performance, you
+00018400: 2063 616e 2075 7365 2074 6865 206c 6561   can use the lea
+00018410: 7365 206d 6f64 652e 0a20 2020 2020 2020  se mode..       
+00018420: 2053 6574 7469 6e67 2074 6869 7320 746f   Setting this to
+00018430: 2060 4c65 6173 6542 6173 6564 6020 7265   `LeaseBased` re
+00018440: 7175 6972 6573 2060 6368 6563 6b5f 7175  quires `check_qu
+00018450: 6f72 756d 203d 2074 7275 6560 2e0a 2020  orum = true`..  
+00018460: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+00018470: 6620 7365 745f 7265 6164 5f6f 6e6c 795f  f set_read_only_
+00018480: 6f70 7469 6f6e 2873 656c 662c 2072 6561  option(self, rea
+00018490: 645f 6f6e 6c79 5f6f 7074 696f 6e3a 2022  d_only_option: "
+000184a0: 5265 6164 4f6e 6c79 4f70 7469 6f6e 2229  ReadOnlyOption")
+000184b0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000184c0: 2020 2222 220a 2020 2020 2020 2020 6072    """.        `r
+000184d0: 6561 645f 6f6e 6c79 5f6f 7074 696f 6e60  ead_only_option`
+000184e0: 3a20 4368 6f6f 7365 2074 6865 206c 696e  : Choose the lin
+000184f0: 6561 7269 7a61 6269 6c69 7479 206d 6f64  earizability mod
+00018500: 6520 6f72 2074 6865 206c 6561 7365 206d  e or the lease m
+00018510: 6f64 6520 746f 2072 6561 6420 6461 7461  ode to read data
+00018520: 2e20 4966 2079 6f75 2064 6f6e e280 9974  . If you don...t
+00018530: 2063 6172 6520 6162 6f75 7420 7468 6520   care about the 
+00018540: 7265 6164 2063 6f6e 7369 7374 656e 6379  read consistency
+00018550: 2061 6e64 2077 616e 7420 6120 6869 6768   and want a high
+00018560: 6572 2072 6561 6420 7065 7266 6f72 6d61  er read performa
+00018570: 6e63 652c 2079 6f75 2063 616e 2075 7365  nce, you can use
+00018580: 2074 6865 206c 6561 7365 206d 6f64 652e   the lease mode.
+00018590: 0a20 2020 2020 2020 2053 6574 7469 6e67  .        Setting
+000185a0: 2074 6869 7320 746f 2060 4c65 6173 6542   this to `LeaseB
+000185b0: 6173 6564 6020 7265 7175 6972 6573 2060  ased` requires `
+000185c0: 6368 6563 6b5f 7175 6f72 756d 203d 2074  check_quorum = t
+000185d0: 7275 6560 2e0a 2020 2020 2020 2020 2222  rue`..        ""
+000185e0: 220a 2020 2020 6465 6620 6765 745f 6964  ".    def get_id
+000185f0: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00018600: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00018610: 2020 2060 6964 603a 2054 6865 2069 6465     `id`: The ide
+00018620: 6e74 6974 7920 6f66 2074 6865 206c 6f63  ntity of the loc
+00018630: 616c 2072 6166 742e 2049 7420 6361 6e6e  al raft. It cann
+00018640: 6f74 2062 6520 302c 2061 6e64 206d 7573  ot be 0, and mus
+00018650: 7420 6265 2075 6e69 7175 6520 696e 2074  t be unique in t
+00018660: 6865 2067 726f 7570 2e0a 2020 2020 2020  he group..      
+00018670: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00018680: 745f 6964 2873 656c 662c 2069 643a 2069  t_id(self, id: i
+00018690: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+000186a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000186b0: 2060 6964 603a 2054 6865 2069 6465 6e74   `id`: The ident
+000186c0: 6974 7920 6f66 2074 6865 206c 6f63 616c  ity of the local
+000186d0: 2072 6166 742e 2049 7420 6361 6e6e 6f74   raft. It cannot
+000186e0: 2062 6520 302c 2061 6e64 206d 7573 7420   be 0, and must 
+000186f0: 6265 2075 6e69 7175 6520 696e 2074 6865  be unique in the
+00018700: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
+00018710: 2222 220a 2020 2020 6465 6620 6765 745f  """.    def get_
+00018720: 656c 6563 7469 6f6e 5f74 6963 6b28 7365  election_tick(se
+00018730: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
+00018740: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00018750: 6065 6c65 6374 696f 6e5f 7469 636b 603a  `election_tick`:
+00018760: 2054 6865 206e 756d 6265 7220 6f66 206e   The number of n
+00018770: 6f64 652e 7469 636b 2069 6e76 6f63 6174  ode.tick invocat
+00018780: 696f 6e73 2074 6861 7420 6d75 7374 2070  ions that must p
+00018790: 6173 7320 6265 7477 6565 6e0a 2020 2020  ass between.    
+000187a0: 2020 2020 656c 6563 7469 6f6e 732e 2054      elections. T
+000187b0: 6861 7420 6973 2c20 6966 2061 2066 6f6c  hat is, if a fol
+000187c0: 6c6f 7765 7220 646f 6573 206e 6f74 2072  lower does not r
+000187d0: 6563 6569 7665 2061 6e79 206d 6573 7361  eceive any messa
+000187e0: 6765 2066 726f 6d20 7468 650a 2020 2020  ge from the.    
+000187f0: 2020 2020 6c65 6164 6572 206f 6620 6375      leader of cu
+00018800: 7272 656e 7420 7465 726d 2062 6566 6f72  rrent term befor
+00018810: 6520 456c 6563 7469 6f6e 5469 636b 2068  e ElectionTick h
+00018820: 6173 2065 6c61 7073 6564 2c20 6974 2077  as elapsed, it w
+00018830: 696c 6c20 6265 636f 6d65 0a20 2020 2020  ill become.     
+00018840: 2020 2063 616e 6469 6461 7465 2061 6e64     candidate and
+00018850: 2073 7461 7274 2061 6e20 656c 6563 7469   start an electi
+00018860: 6f6e 2e20 656c 6563 7469 6f6e 5f74 6963  on. election_tic
+00018870: 6b20 6d75 7374 2062 6520 6772 6561 7465  k must be greate
+00018880: 7220 7468 616e 0a20 2020 2020 2020 2048  r than.        H
+00018890: 6561 7274 6265 6174 5469 636b 2e20 5765  eartbeatTick. We
+000188a0: 2073 7567 6765 7374 2065 6c65 6374 696f   suggest electio
+000188b0: 6e5f 7469 636b 203d 2031 3020 2a20 4865  n_tick = 10 * He
+000188c0: 6172 7462 6561 7454 6963 6b20 746f 2061  artbeatTick to a
+000188d0: 766f 6964 0a20 2020 2020 2020 2075 6e6e  void.        unn
+000188e0: 6563 6573 7361 7279 206c 6561 6465 7220  ecessary leader 
+000188f0: 7377 6974 6368 696e 670a 2020 2020 2020  switching.      
+00018900: 2020 2222 220a 2020 2020 6465 6620 7365    """.    def se
+00018910: 745f 656c 6563 7469 6f6e 5f74 6963 6b28  t_election_tick(
+00018920: 7365 6c66 2c20 656c 6563 7469 6f6e 5f74  self, election_t
+00018930: 6963 6b3a 2069 6e74 2920 2d3e 204e 6f6e  ick: int) -> Non
+00018940: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00018950: 2020 2020 2020 2060 656c 6563 7469 6f6e         `election
+00018960: 5f74 6963 6b60 3a20 5468 6520 6e75 6d62  _tick`: The numb
+00018970: 6572 206f 6620 6e6f 6465 2e74 6963 6b20  er of node.tick 
+00018980: 696e 766f 6361 7469 6f6e 7320 7468 6174  invocations that
+00018990: 206d 7573 7420 7061 7373 2062 6574 7765   must pass betwe
+000189a0: 656e 0a20 2020 2020 2020 2065 6c65 6374  en.        elect
+000189b0: 696f 6e73 2e20 5468 6174 2069 732c 2069  ions. That is, i
+000189c0: 6620 6120 666f 6c6c 6f77 6572 2064 6f65  f a follower doe
+000189d0: 7320 6e6f 7420 7265 6365 6976 6520 616e  s not receive an
+000189e0: 7920 6d65 7373 6167 6520 6672 6f6d 2074  y message from t
+000189f0: 6865 0a20 2020 2020 2020 206c 6561 6465  he.        leade
+00018a00: 7220 6f66 2063 7572 7265 6e74 2074 6572  r of current ter
+00018a10: 6d20 6265 666f 7265 2045 6c65 6374 696f  m before Electio
+00018a20: 6e54 6963 6b20 6861 7320 656c 6170 7365  nTick has elapse
+00018a30: 642c 2069 7420 7769 6c6c 2062 6563 6f6d  d, it will becom
+00018a40: 650a 2020 2020 2020 2020 6361 6e64 6964  e.        candid
+00018a50: 6174 6520 616e 6420 7374 6172 7420 616e  ate and start an
+00018a60: 2065 6c65 6374 696f 6e2e 2065 6c65 6374   election. elect
+00018a70: 696f 6e5f 7469 636b 206d 7573 7420 6265  ion_tick must be
+00018a80: 2067 7265 6174 6572 2074 6861 6e0a 2020   greater than.  
+00018a90: 2020 2020 2020 4865 6172 7462 6561 7454        HeartbeatT
+00018aa0: 6963 6b2e 2057 6520 7375 6767 6573 7420  ick. We suggest 
+00018ab0: 656c 6563 7469 6f6e 5f74 6963 6b20 3d20  election_tick = 
+00018ac0: 3130 202a 2048 6561 7274 6265 6174 5469  10 * HeartbeatTi
+00018ad0: 636b 2074 6f20 6176 6f69 640a 2020 2020  ck to avoid.    
+00018ae0: 2020 2020 756e 6e65 6365 7373 6172 7920      unnecessary 
+00018af0: 6c65 6164 6572 2073 7769 7463 6869 6e67  leader switching
+00018b00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00018b10: 2064 6566 2067 6574 5f68 6561 7274 6265   def get_heartbe
+00018b20: 6174 5f74 6963 6b28 7365 6c66 2920 2d3e  at_tick(self) ->
+00018b30: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00018b40: 220a 2020 2020 2020 2020 6068 6561 7274  ".        `heart
+00018b50: 6265 6174 5f74 6963 6b60 3a20 4865 6172  beat_tick`: Hear
+00018b60: 7462 6561 7454 6963 6b20 6973 2074 6865  tbeatTick is the
+00018b70: 206e 756d 6265 7220 6f66 206e 6f64 652e   number of node.
+00018b80: 7469 636b 2069 6e76 6f63 6174 696f 6e73  tick invocations
+00018b90: 2074 6861 7420 6d75 7374 2070 6173 7320   that must pass 
+00018ba0: 6265 7477 6565 6e0a 2020 2020 2020 2020  between.        
+00018bb0: 6865 6172 7462 6561 7473 2e20 5468 6174  heartbeats. That
+00018bc0: 2069 732c 2061 206c 6561 6465 7220 7365   is, a leader se
+00018bd0: 6e64 7320 6865 6172 7462 6561 7420 6d65  nds heartbeat me
+00018be0: 7373 6167 6573 2074 6f20 6d61 696e 7461  ssages to mainta
+00018bf0: 696e 2069 7473 0a20 2020 2020 2020 206c  in its.        l
+00018c00: 6561 6465 7273 6869 7020 6576 6572 7920  eadership every 
+00018c10: 6865 6172 7462 6561 7420 7469 636b 732e  heartbeat ticks.
+00018c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00018c30: 2064 6566 2073 6574 5f68 6561 7274 6265   def set_heartbe
+00018c40: 6174 5f74 6963 6b28 7365 6c66 2c20 6865  at_tick(self, he
+00018c50: 6172 7462 6561 745f 7469 636b 3a20 696e  artbeat_tick: in
+00018c60: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
+00018c70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00018c80: 6068 6561 7274 6265 6174 5f74 6963 6b60  `heartbeat_tick`
+00018c90: 3a20 4865 6172 7462 6561 7454 6963 6b20  : HeartbeatTick 
+00018ca0: 6973 2074 6865 206e 756d 6265 7220 6f66  is the number of
+00018cb0: 206e 6f64 652e 7469 636b 2069 6e76 6f63   node.tick invoc
+00018cc0: 6174 696f 6e73 2074 6861 7420 6d75 7374  ations that must
+00018cd0: 2070 6173 7320 6265 7477 6565 6e0a 2020   pass between.  
+00018ce0: 2020 2020 2020 6865 6172 7462 6561 7473        heartbeats
+00018cf0: 2e20 5468 6174 2069 732c 2061 206c 6561  . That is, a lea
+00018d00: 6465 7220 7365 6e64 7320 6865 6172 7462  der sends heartb
+00018d10: 6561 7420 6d65 7373 6167 6573 2074 6f20  eat messages to 
+00018d20: 6d61 696e 7461 696e 2069 7473 0a20 2020  maintain its.   
+00018d30: 2020 2020 206c 6561 6465 7273 6869 7020       leadership 
+00018d40: 6576 6572 7920 6865 6172 7462 6561 7420  every heartbeat 
+00018d50: 7469 636b 732e 0a20 2020 2020 2020 2022  ticks..        "
+00018d60: 2222 0a20 2020 2064 6566 2067 6574 5f6d  "".    def get_m
+00018d70: 6178 5f73 697a 655f 7065 725f 6d73 6728  ax_size_per_msg(
+00018d80: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
+00018d90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00018da0: 2020 606d 6178 5f73 697a 655f 7065 725f    `max_size_per_
+00018db0: 6d73 6760 3a20 4c69 6d69 7420 7468 6520  msg`: Limit the 
+00018dc0: 6d61 7820 7369 7a65 206f 6620 6561 6368  max size of each
+00018dd0: 2061 7070 656e 6420 6d65 7373 6167 652e   append message.
+00018de0: 2053 6d61 6c6c 6572 2076 616c 7565 206c   Smaller value l
+00018df0: 6f77 6572 730a 2020 2020 2020 2020 7468  owers.        th
+00018e00: 6520 7261 6674 2072 6563 6f76 6572 7920  e raft recovery 
+00018e10: 636f 7374 2869 6e69 7469 616c 2070 726f  cost(initial pro
+00018e20: 6269 6e67 2061 6e64 206d 6573 7361 6765  bing and message
+00018e30: 206c 6f73 7420 6475 7269 6e67 206e 6f72   lost during nor
+00018e40: 6d61 6c20 6f70 6572 6174 696f 6e29 2e0a  mal operation)..
+00018e50: 2020 2020 2020 2020 4f6e 2074 6865 206f          On the o
+00018e60: 7468 6572 2073 6964 652c 2069 7420 6d69  ther side, it mi
+00018e70: 6768 7420 6166 6665 6374 2074 6865 2074  ght affect the t
+00018e80: 6872 6f75 6768 7075 7420 6475 7269 6e67  hroughput during
+00018e90: 206e 6f72 6d61 6c20 7265 706c 6963 6174   normal replicat
+00018ea0: 696f 6e2e 0a20 2020 2020 2020 204e 6f74  ion..        Not
+00018eb0: 653a 206d 6174 682e 4d61 7855 7573 697a  e: math.MaxUusiz
+00018ec0: 6536 3420 666f 7220 756e 6c69 6d69 7465  e64 for unlimite
+00018ed0: 642c 2030 2066 6f72 2061 7420 6d6f 7374  d, 0 for at most
+00018ee0: 206f 6e65 2065 6e74 7279 2070 6572 206d   one entry per m
+00018ef0: 6573 7361 6765 2e0a 2020 2020 2020 2020  essage..        
+00018f00: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00018f10: 6d61 785f 7369 7a65 5f70 6572 5f6d 7367  max_size_per_msg
+00018f20: 2873 656c 662c 206d 6178 5f73 697a 655f  (self, max_size_
+00018f30: 7065 725f 6d73 673a 2069 6e74 2920 2d3e  per_msg: int) ->
+00018f40: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00018f50: 2222 0a20 2020 2020 2020 2060 6d61 785f  "".        `max_
+00018f60: 7369 7a65 5f70 6572 5f6d 7367 603a 204c  size_per_msg`: L
+00018f70: 696d 6974 2074 6865 206d 6178 2073 697a  imit the max siz
+00018f80: 6520 6f66 2065 6163 6820 6170 7065 6e64  e of each append
+00018f90: 206d 6573 7361 6765 2e20 536d 616c 6c65   message. Smalle
+00018fa0: 7220 7661 6c75 6520 6c6f 7765 7273 0a20  r value lowers. 
+00018fb0: 2020 2020 2020 2074 6865 2072 6166 7420         the raft 
+00018fc0: 7265 636f 7665 7279 2063 6f73 7428 696e  recovery cost(in
+00018fd0: 6974 6961 6c20 7072 6f62 696e 6720 616e  itial probing an
+00018fe0: 6420 6d65 7373 6167 6520 6c6f 7374 2064  d message lost d
+00018ff0: 7572 696e 6720 6e6f 726d 616c 206f 7065  uring normal ope
+00019000: 7261 7469 6f6e 292e 0a20 2020 2020 2020  ration)..       
+00019010: 204f 6e20 7468 6520 6f74 6865 7220 7369   On the other si
+00019020: 6465 2c20 6974 206d 6967 6874 2061 6666  de, it might aff
+00019030: 6563 7420 7468 6520 7468 726f 7567 6870  ect the throughp
+00019040: 7574 2064 7572 696e 6720 6e6f 726d 616c  ut during normal
+00019050: 2072 6570 6c69 6361 7469 6f6e 2e0a 2020   replication..  
+00019060: 2020 2020 2020 4e6f 7465 3a20 6d61 7468        Note: math
+00019070: 2e4d 6178 5575 7369 7a65 3634 2066 6f72  .MaxUusize64 for
+00019080: 2075 6e6c 696d 6974 6564 2c20 3020 666f   unlimited, 0 fo
+00019090: 7220 6174 206d 6f73 7420 6f6e 6520 656e  r at most one en
+000190a0: 7472 7920 7065 7220 6d65 7373 6167 652e  try per message.
+000190b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000190c0: 2064 6566 2067 6574 5f6d 6178 5f69 6e66   def get_max_inf
+000190d0: 6c69 6768 745f 6d73 6773 2873 656c 6629  light_msgs(self)
+000190e0: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+000190f0: 2022 2222 0a20 2020 2020 2020 2060 6d61   """.        `ma
+00019100: 785f 696e 666c 6967 6874 5f6d 7367 7360  x_inflight_msgs`
+00019110: 3a20 4c69 6d69 7420 7468 6520 6d61 7820  : Limit the max 
+00019120: 6e75 6d62 6572 206f 6620 696e 2d66 6c69  number of in-fli
+00019130: 6768 7420 6170 7065 6e64 206d 6573 7361  ght append messa
+00019140: 6765 7320 6475 7269 6e67 206f 7074 696d  ges during optim
+00019150: 6973 7469 630a 2020 2020 2020 2020 7265  istic.        re
+00019160: 706c 6963 6174 696f 6e20 7068 6173 652e  plication phase.
+00019170: 2054 6865 2061 7070 6c69 6361 7469 6f6e   The application
+00019180: 2074 7261 6e73 706f 7274 6174 696f 6e20   transportation 
+00019190: 6c61 7965 7220 7573 7561 6c6c 7920 6861  layer usually ha
+000191a0: 7320 6974 7320 6f77 6e20 7365 6e64 696e  s its own sendin
+000191b0: 670a 2020 2020 2020 2020 6275 6666 6572  g.        buffer
+000191c0: 206f 7665 7220 5443 502f 5544 502e 2053   over TCP/UDP. S
+000191d0: 6574 2074 6f20 6176 6f69 6420 6f76 6572  et to avoid over
+000191e0: 666c 6f77 696e 6720 7468 6174 2073 656e  flowing that sen
+000191f0: 6469 6e67 2062 7566 6665 722e 0a20 2020  ding buffer..   
+00019200: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00019210: 2073 6574 5f6d 6178 5f69 6e66 6c69 6768   set_max_infligh
+00019220: 745f 6d73 6773 2873 656c 662c 206d 6178  t_msgs(self, max
+00019230: 5f69 6e66 6c69 6768 745f 6d73 6773 3a20  _inflight_msgs: 
+00019240: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00019250: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00019260: 2020 606d 6178 5f69 6e66 6c69 6768 745f    `max_inflight_
+00019270: 6d73 6773 603a 204c 696d 6974 2074 6865  msgs`: Limit the
+00019280: 206d 6178 206e 756d 6265 7220 6f66 2069   max number of i
+00019290: 6e2d 666c 6967 6874 2061 7070 656e 6420  n-flight append 
+000192a0: 6d65 7373 6167 6573 2064 7572 696e 6720  messages during 
+000192b0: 6f70 7469 6d69 7374 6963 0a20 2020 2020  optimistic.     
+000192c0: 2020 2072 6570 6c69 6361 7469 6f6e 2070     replication p
+000192d0: 6861 7365 2e20 5468 6520 6170 706c 6963  hase. The applic
+000192e0: 6174 696f 6e20 7472 616e 7370 6f72 7461  ation transporta
+000192f0: 7469 6f6e 206c 6179 6572 2075 7375 616c  tion layer usual
+00019300: 6c79 2068 6173 2069 7473 206f 776e 2073  ly has its own s
+00019310: 656e 6469 6e67 0a20 2020 2020 2020 2062  ending.        b
+00019320: 7566 6665 7220 6f76 6572 2054 4350 2f55  uffer over TCP/U
+00019330: 4450 2e20 5365 7420 746f 2061 766f 6964  DP. Set to avoid
+00019340: 206f 7665 7266 6c6f 7769 6e67 2074 6861   overflowing tha
+00019350: 7420 7365 6e64 696e 6720 6275 6666 6572  t sending buffer
+00019360: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00019370: 2020 6465 6620 6765 745f 6170 706c 6965    def get_applie
+00019380: 6428 7365 6c66 2920 2d3e 2069 6e74 3a0a  d(self) -> int:.
+00019390: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000193a0: 2020 2020 6061 7070 6c69 6564 603a 2041      `applied`: A
+000193b0: 7070 6c69 6564 2069 7320 7468 6520 6c61  pplied is the la
+000193c0: 7374 2061 7070 6c69 6564 2069 6e64 6578  st applied index
+000193d0: 2e20 4974 2073 686f 756c 6420 6f6e 6c79  . It should only
+000193e0: 2062 6520 7365 7420 7768 656e 2072 6573   be set when res
+000193f0: 7461 7274 696e 670a 2020 2020 2020 2020  tarting.        
+00019400: 7261 6674 2e20 7261 6674 2077 696c 6c20  raft. raft will 
+00019410: 6e6f 7420 7265 7475 726e 2065 6e74 7269  not return entri
+00019420: 6573 2074 6f20 7468 6520 6170 706c 6963  es to the applic
+00019430: 6174 696f 6e20 736d 616c 6c65 7220 6f72  ation smaller or
+00019440: 2065 7175 616c 2074 6f20 4170 706c 6965   equal to Applie
+00019450: 642e 0a20 2020 2020 2020 2049 6620 4170  d..        If Ap
+00019460: 706c 6965 6420 6973 2075 6e73 6574 2077  plied is unset w
+00019470: 6865 6e20 7265 7374 6172 7469 6e67 2c20  hen restarting, 
+00019480: 7261 6674 206d 6967 6874 2072 6574 7572  raft might retur
+00019490: 6e20 7072 6576 696f 7573 2061 7070 6c69  n previous appli
+000194a0: 6564 2065 6e74 7269 6573 2e0a 2020 2020  ed entries..    
+000194b0: 2020 2020 5468 6973 2069 7320 6120 7665      This is a ve
+000194c0: 7279 2061 7070 6c69 6361 7469 6f6e 2064  ry application d
+000194d0: 6570 656e 6465 6e74 2063 6f6e 6669 6775  ependent configu
+000194e0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+000194f0: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+00019500: 6170 706c 6965 6428 7365 6c66 2c20 6170  applied(self, ap
+00019510: 706c 6965 643a 2069 6e74 2920 2d3e 204e  plied: int) -> N
+00019520: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00019530: 0a20 2020 2020 2020 2060 6170 706c 6965  .        `applie
+00019540: 6460 3a20 4170 706c 6965 6420 6973 2074  d`: Applied is t
+00019550: 6865 206c 6173 7420 6170 706c 6965 6420  he last applied 
+00019560: 696e 6465 782e 2049 7420 7368 6f75 6c64  index. It should
+00019570: 206f 6e6c 7920 6265 2073 6574 2077 6865   only be set whe
+00019580: 6e20 7265 7374 6172 7469 6e67 0a20 2020  n restarting.   
+00019590: 2020 2020 2072 6166 742e 2072 6166 7420       raft. raft 
+000195a0: 7769 6c6c 206e 6f74 2072 6574 7572 6e20  will not return 
+000195b0: 656e 7472 6965 7320 746f 2074 6865 2061  entries to the a
+000195c0: 7070 6c69 6361 7469 6f6e 2073 6d61 6c6c  pplication small
+000195d0: 6572 206f 7220 6571 7561 6c20 746f 2041  er or equal to A
+000195e0: 7070 6c69 6564 2e0a 2020 2020 2020 2020  pplied..        
+000195f0: 4966 2041 7070 6c69 6564 2069 7320 756e  If Applied is un
+00019600: 7365 7420 7768 656e 2072 6573 7461 7274  set when restart
+00019610: 696e 672c 2072 6166 7420 6d69 6768 7420  ing, raft might 
+00019620: 7265 7475 726e 2070 7265 7669 6f75 7320  return previous 
+00019630: 6170 706c 6965 6420 656e 7472 6965 732e  applied entries.
+00019640: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
+00019650: 2061 2076 6572 7920 6170 706c 6963 6174   a very applicat
+00019660: 696f 6e20 6465 7065 6e64 656e 7420 636f  ion dependent co
+00019670: 6e66 6967 7572 6174 696f 6e2e 0a20 2020  nfiguration..   
+00019680: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00019690: 2067 6574 5f63 6865 636b 5f71 756f 7275   get_check_quoru
+000196a0: 6d28 7365 6c66 2920 2d3e 2062 6f6f 6c3a  m(self) -> bool:
+000196b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000196c0: 2020 2020 2060 6368 6563 6b5f 7175 6f72       `check_quor
+000196d0: 756d 603a 2053 7065 6369 6679 2069 6620  um`: Specify if 
+000196e0: 7468 6520 6c65 6164 6572 2073 686f 756c  the leader shoul
+000196f0: 6420 6368 6563 6b20 7175 6f72 756d 2061  d check quorum a
+00019700: 6374 6976 6974 792e 204c 6561 6465 7220  ctivity. Leader 
+00019710: 7374 6570 7320 646f 776e 2077 6865 6e0a  steps down when.
+00019720: 2020 2020 2020 2020 7175 6f72 756d 2069          quorum i
+00019730: 7320 6e6f 7420 6163 7469 7665 2066 6f72  s not active for
+00019740: 2061 6e20 656c 6563 7469 6f6e 5469 6d65   an electionTime
+00019750: 6f75 742e 0a20 2020 2020 2020 2022 2222  out..        """
+00019760: 0a20 2020 2064 6566 2073 6574 5f63 6865  .    def set_che
+00019770: 636b 5f71 756f 7275 6d28 7365 6c66 2c20  ck_quorum(self, 
+00019780: 6368 6563 6b5f 7175 6f72 756d 3a20 626f  check_quorum: bo
+00019790: 6f6c 2920 2d3e 204e 6f6e 653a 0a20 2020  ol) -> None:.   
+000197a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000197b0: 2060 6368 6563 6b5f 7175 6f72 756d 603a   `check_quorum`:
+000197c0: 2053 7065 6369 6679 2069 6620 7468 6520   Specify if the 
+000197d0: 6c65 6164 6572 2073 686f 756c 6420 6368  leader should ch
+000197e0: 6563 6b20 7175 6f72 756d 2061 6374 6976  eck quorum activ
+000197f0: 6974 792e 204c 6561 6465 7220 7374 6570  ity. Leader step
+00019800: 7320 646f 776e 2077 6865 6e0a 2020 2020  s down when.    
+00019810: 2020 2020 7175 6f72 756d 2069 7320 6e6f      quorum is no
+00019820: 7420 6163 7469 7665 2066 6f72 2061 6e20  t active for an 
+00019830: 656c 6563 7469 6f6e 5469 6d65 6f75 742e  electionTimeout.
+00019840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00019850: 2064 6566 2067 6574 5f70 7265 5f76 6f74   def get_pre_vot
+00019860: 6528 7365 6c66 2920 2d3e 2062 6f6f 6c3a  e(self) -> bool:
+00019870: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00019880: 2020 2020 2060 7072 655f 766f 7465 603a       `pre_vote`:
+00019890: 2045 6e61 626c 6573 2074 6865 2050 7265   Enables the Pre
+000198a0: 2d56 6f74 6520 616c 676f 7269 7468 6d20  -Vote algorithm 
+000198b0: 6465 7363 7269 6265 6420 696e 2072 6166  described in raf
+000198c0: 7420 7468 6573 6973 2073 6563 7469 6f6e  t thesis section
+000198d0: 0a20 2020 2020 2020 2039 2e36 2e20 5468  .        9.6. Th
+000198e0: 6973 2070 7265 7665 6e74 7320 6469 7372  is prevents disr
+000198f0: 7570 7469 6f6e 2077 6865 6e20 6120 6e6f  uption when a no
+00019900: 6465 2074 6861 7420 6861 7320 6265 656e  de that has been
+00019910: 2070 6172 7469 7469 6f6e 6564 2061 7761   partitioned awa
+00019920: 790a 2020 2020 2020 2020 7265 6a6f 696e  y.        rejoin
+00019930: 7320 7468 6520 636c 7573 7465 722e 0a20  s the cluster.. 
+00019940: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00019950: 6566 2073 6574 5f70 7265 5f76 6f74 6528  ef set_pre_vote(
+00019960: 7365 6c66 2c20 7072 655f 766f 7465 3a20  self, pre_vote: 
+00019970: 626f 6f6c 2920 2d3e 204e 6f6e 653a 0a20  bool) -> None:. 
+00019980: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00019990: 2020 2060 7072 655f 766f 7465 603a 2045     `pre_vote`: E
+000199a0: 6e61 626c 6573 2074 6865 2050 7265 2d56  nables the Pre-V
+000199b0: 6f74 6520 616c 676f 7269 7468 6d20 6465  ote algorithm de
+000199c0: 7363 7269 6265 6420 696e 2072 6166 7420  scribed in raft 
+000199d0: 7468 6573 6973 2073 6563 7469 6f6e 0a20  thesis section. 
+000199e0: 2020 2020 2020 2039 2e36 2e20 5468 6973         9.6. This
+000199f0: 2070 7265 7665 6e74 7320 6469 7372 7570   prevents disrup
+00019a00: 7469 6f6e 2077 6865 6e20 6120 6e6f 6465  tion when a node
+00019a10: 2074 6861 7420 6861 7320 6265 656e 2070   that has been p
+00019a20: 6172 7469 7469 6f6e 6564 2061 7761 790a  artitioned away.
+00019a30: 2020 2020 2020 2020 7265 6a6f 696e 7320          rejoins 
+00019a40: 7468 6520 636c 7573 7465 722e 0a20 2020  the cluster..   
+00019a50: 2020 2020 2022 2222 0a20 2020 2064 6566       """.    def
+00019a60: 2067 6574 5f62 6174 6368 5f61 7070 656e   get_batch_appen
+00019a70: 6428 7365 6c66 2920 2d3e 2062 6f6f 6c3a  d(self) -> bool:
+00019a80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00019a90: 2020 2020 2060 6261 7463 685f 6170 7065       `batch_appe
+00019aa0: 6e64 603a 2042 6174 6368 6573 2065 7665  nd`: Batches eve
+00019ab0: 7279 2061 7070 656e 6420 6d73 6720 6966  ry append msg if
+00019ac0: 2061 6e79 2061 7070 656e 6420 6d73 6720   any append msg 
+00019ad0: 616c 7265 6164 7920 6578 6973 7473 0a20  already exists. 
+00019ae0: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00019af0: 6566 2073 6574 5f62 6174 6368 5f61 7070  ef set_batch_app
+00019b00: 656e 6428 7365 6c66 2c20 6261 7463 685f  end(self, batch_
+00019b10: 6170 7065 6e64 3a20 626f 6f6c 2920 2d3e  append: bool) ->
+00019b20: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00019b30: 2222 0a20 2020 2020 2020 2060 6261 7463  "".        `batc
+00019b40: 685f 6170 7065 6e64 603a 2042 6174 6368  h_append`: Batch
+00019b50: 6573 2065 7665 7279 2061 7070 656e 6420  es every append 
+00019b60: 6d73 6720 6966 2061 6e79 2061 7070 656e  msg if any appen
+00019b70: 6420 6d73 6720 616c 7265 6164 7920 6578  d msg already ex
+00019b80: 6973 7473 0a20 2020 2020 2020 2022 2222  ists.        """
+00019b90: 0a20 2020 2064 6566 2067 6574 5f73 6b69  .    def get_ski
+00019ba0: 705f 6263 6173 745f 636f 6d6d 6974 2873  p_bcast_commit(s
+00019bb0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+00019bc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00019bd0: 2020 6073 6b69 705f 6263 6173 745f 636f    `skip_bcast_co
+00019be0: 6d6d 6974 603a 2044 6f6e 2774 2062 726f  mmit`: Don't bro
+00019bf0: 6164 6361 7374 2061 6e20 656d 7074 7920  adcast an empty 
+00019c00: 7261 6674 2065 6e74 7279 2074 6f20 6e6f  raft entry to no
+00019c10: 7469 6679 2066 6f6c 6c6f 7765 7220 746f  tify follower to
+00019c20: 2063 6f6d 6d69 7420 616e 2065 6e74 7279   commit an entry
+00019c30: 2e0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
+00019c40: 6179 206d 616b 6520 666f 6c6c 6f77 6572  ay make follower
+00019c50: 2077 6169 7420 6120 6c6f 6e67 6572 2074   wait a longer t
+00019c60: 696d 6520 746f 2061 7070 6c79 2061 6e20  ime to apply an 
+00019c70: 656e 7472 792e 2054 6869 7320 636f 6e66  entry. This conf
+00019c80: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+00019c90: 2020 4d61 7920 6166 6665 6374 2070 726f    May affect pro
+00019ca0: 706f 7361 6c20 666f 7277 6172 6469 6e67  posal forwarding
+00019cb0: 2061 6e64 2066 6f6c 6c6f 7765 7220 7265   and follower re
+00019cc0: 6164 2e0a 2020 2020 2020 2020 2222 220a  ad..        """.
+00019cd0: 2020 2020 6465 6620 7365 745f 736b 6970      def set_skip
+00019ce0: 5f62 6361 7374 5f63 6f6d 6d69 7428 7365  _bcast_commit(se
+00019cf0: 6c66 2c20 736b 6970 5f62 6361 7374 5f63  lf, skip_bcast_c
+00019d00: 6f6d 6d69 743a 2062 6f6f 6c29 202d 3e20  ommit: bool) -> 
+00019d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00019d20: 220a 2020 2020 2020 2020 6073 6b69 705f  ".        `skip_
+00019d30: 6263 6173 745f 636f 6d6d 6974 603a 2044  bcast_commit`: D
+00019d40: 6f6e 2774 2062 726f 6164 6361 7374 2061  on't broadcast a
+00019d50: 6e20 656d 7074 7920 7261 6674 2065 6e74  n empty raft ent
+00019d60: 7279 2074 6f20 6e6f 7469 6679 2066 6f6c  ry to notify fol
+00019d70: 6c6f 7765 7220 746f 2063 6f6d 6d69 7420  lower to commit 
+00019d80: 616e 2065 6e74 7279 2e0a 2020 2020 2020  an entry..      
+00019d90: 2020 5468 6973 206d 6179 206d 616b 6520    This may make 
+00019da0: 666f 6c6c 6f77 6572 2077 6169 7420 6120  follower wait a 
+00019db0: 6c6f 6e67 6572 2074 696d 6520 746f 2061  longer time to a
+00019dc0: 7070 6c79 2061 6e20 656e 7472 792e 2054  pply an entry. T
+00019dd0: 6869 7320 636f 6e66 6967 7572 6174 696f  his configuratio
+00019de0: 6e0a 2020 2020 2020 2020 4d61 7920 6166  n.        May af
+00019df0: 6665 6374 2070 726f 706f 7361 6c20 666f  fect proposal fo
+00019e00: 7277 6172 6469 6e67 2061 6e64 2066 6f6c  rwarding and fol
+00019e10: 6c6f 7765 7220 7265 6164 2e0a 2020 2020  lower read..    
+00019e20: 2020 2020 2222 220a 2020 2020 6465 6620      """.    def 
+00019e30: 6765 745f 7072 696f 7269 7479 2873 656c  get_priority(sel
+00019e40: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
+00019e50: 2020 2022 2222 0a20 2020 2020 2020 2060     """.        `
+00019e60: 7072 696f 7269 7479 603a 2054 6865 2065  priority`: The e
+00019e70: 6c65 6374 696f 6e20 7072 696f 7269 7479  lection priority
+00019e80: 206f 6620 7468 6973 206e 6f64 652e 0a20   of this node.. 
+00019e90: 2020 2020 2020 2022 2222 0a20 2020 2064         """.    d
+00019ea0: 6566 2073 6574 5f70 7269 6f72 6974 7928  ef set_priority(
+00019eb0: 7365 6c66 2c20 7072 696f 7269 7479 3a20  self, priority: 
+00019ec0: 696e 7429 202d 3e20 4e6f 6e65 3a0a 2020  int) -> None:.  
+00019ed0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00019ee0: 2020 6070 7269 6f72 6974 7960 3a20 5468    `priority`: Th
+00019ef0: 6520 656c 6563 7469 6f6e 2070 7269 6f72  e election prior
+00019f00: 6974 7920 6f66 2074 6869 7320 6e6f 6465  ity of this node
+00019f10: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00019f20: 2020 6465 6620 6765 745f 6d61 785f 756e    def get_max_un
+00019f30: 636f 6d6d 6974 7465 645f 7369 7a65 2873  committed_size(s
+00019f40: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+00019f50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00019f60: 2060 6d61 785f 756e 636f 6d6d 6974 7465   `max_uncommitte
+00019f70: 645f 7369 7a65 603a 2053 7065 6369 6679  d_size`: Specify
+00019f80: 206d 6178 696d 756d 206f 6620 756e 636f   maximum of unco
+00019f90: 6d6d 6974 7465 6420 656e 7472 7920 7369  mmitted entry si
+00019fa0: 7a65 2e0a 2020 2020 2020 2020 5768 656e  ze..        When
+00019fb0: 2074 6869 7320 6c69 6d69 7420 6973 2072   this limit is r
+00019fc0: 6561 6368 6564 2c20 616c 6c20 7072 6f70  eached, all prop
+00019fd0: 6f73 616c 7320 746f 2061 7070 656e 6420  osals to append 
+00019fe0: 6e65 7720 6c6f 6720 7769 6c6c 2062 6520  new log will be 
+00019ff0: 6472 6f70 7065 640a 2020 2020 2020 2020  dropped.        
+0001a000: 2222 220a 2020 2020 6465 6620 7365 745f  """.    def set_
+0001a010: 6d61 785f 756e 636f 6d6d 6974 7465 645f  max_uncommitted_
+0001a020: 7369 7a65 2873 656c 662c 206d 6178 5f75  size(self, max_u
+0001a030: 6e63 6f6d 6d69 7474 6564 5f73 697a 653a  ncommitted_size:
+0001a040: 2069 6e74 2920 2d3e 204e 6f6e 653a 0a20   int) -> None:. 
+0001a050: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001a060: 2020 2060 6d61 785f 756e 636f 6d6d 6974     `max_uncommit
+0001a070: 7465 645f 7369 7a65 603a 2053 7065 6369  ted_size`: Speci
+0001a080: 6679 206d 6178 696d 756d 206f 6620 756e  fy maximum of un
+0001a090: 636f 6d6d 6974 7465 6420 656e 7472 7920  committed entry 
+0001a0a0: 7369 7a65 2e0a 2020 2020 2020 2020 5768  size..        Wh
+0001a0b0: 656e 2074 6869 7320 6c69 6d69 7420 6973  en this limit is
+0001a0c0: 2072 6561 6368 6564 2c20 616c 6c20 7072   reached, all pr
+0001a0d0: 6f70 6f73 616c 7320 746f 2061 7070 656e  oposals to appen
+0001a0e0: 6420 6e65 7720 6c6f 6720 7769 6c6c 2062  d new log will b
+0001a0f0: 6520 6472 6f70 7065 640a 2020 2020 2020  e dropped.      
+0001a100: 2020 2222 220a 2020 2020 6465 6620 6765    """.    def ge
+0001a110: 745f 6d61 785f 636f 6d6d 6974 7465 645f  t_max_committed_
+0001a120: 7369 7a65 5f70 6572 5f72 6561 6479 2873  size_per_ready(s
+0001a130: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+0001a140: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001a150: 2060 6d61 785f 636f 6d6d 6974 7465 645f   `max_committed_
+0001a160: 7369 7a65 5f70 6572 5f72 6561 6479 603a  size_per_ready`:
+0001a170: 204d 6178 2073 697a 6520 666f 7220 636f   Max size for co
+0001a180: 6d6d 6974 7465 6420 656e 7472 6965 7320  mmitted entries 
+0001a190: 696e 2061 2060 5265 6164 7960 2e0a 2020  in a `Ready`..  
+0001a1a0: 2020 2020 2020 2222 220a 2020 2020 6465        """.    de
+0001a1b0: 6620 7365 745f 6d61 785f 636f 6d6d 6974  f set_max_commit
+0001a1c0: 7465 645f 7369 7a65 5f70 6572 5f72 6561  ted_size_per_rea
+0001a1d0: 6479 280a 2020 2020 2020 2020 7365 6c66  dy(.        self
+0001a1e0: 2c20 6d61 785f 636f 6d6d 6974 7465 645f  , max_committed_
+0001a1f0: 7369 7a65 5f70 6572 5f72 6561 6479 3a20  size_per_ready: 
+0001a200: 696e 740a 2020 2020 2920 2d3e 204e 6f6e  int.    ) -> Non
+0001a210: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+0001a220: 2020 2020 2020 2060 6d61 785f 636f 6d6d         `max_comm
+0001a230: 6974 7465 645f 7369 7a65 5f70 6572 5f72  itted_size_per_r
+0001a240: 6561 6479 603a 204d 6178 2073 697a 6520  eady`: Max size 
+0001a250: 666f 7220 636f 6d6d 6974 7465 6420 656e  for committed en
+0001a260: 7472 6965 7320 696e 2061 2060 5265 6164  tries in a `Read
+0001a270: 7960 2e0a 2020 2020 2020 2020 2222 220a  y`..        """.
+0001a280: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0001a290: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+0001a2a0: 2020 2020 2020 2020 2222 2252 756e 7320          """Runs 
+0001a2b0: 7661 6c69 6461 7469 6f6e 7320 6167 6169  validations agai
+0001a2c0: 6e73 7420 7468 6520 636f 6e66 6967 2e22  nst the config."
+0001a2d0: 2222 0a0a 636c 6173 7320 436f 6e66 6967  ""..class Config
+0001a2e0: 285f 5f41 5049 5f43 6f6e 6669 6729 3a0a  (__API_Config):.
+0001a2f0: 2020 2020 2222 220a 2020 2020 436f 6e66      """.    Conf
+0001a300: 6967 2063 6f6e 7461 696e 7320 7468 6520  ig contains the 
+0001a310: 7061 7261 6d65 7465 7273 2074 6f20 7374  parameters to st
+0001a320: 6172 7420 6120 7261 6674 2e0a 2020 2020  art a raft..    
+0001a330: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+0001a340: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+0001a350: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
+0001a360: 2020 2020 2020 2020 6964 3a20 4f70 7469          id: Opti
+0001a370: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0001a380: 2c0a 2020 2020 2020 2020 656c 6563 7469  ,.        electi
+0001a390: 6f6e 5f74 6963 6b3a 204f 7074 696f 6e61  on_tick: Optiona
+0001a3a0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+0001a3b0: 2020 2020 2020 2068 6561 7274 6265 6174         heartbeat
+0001a3c0: 5f74 6963 6b3a 204f 7074 696f 6e61 6c5b  _tick: Optional[
+0001a3d0: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+0001a3e0: 2020 2020 2061 7070 6c69 6564 3a20 4f70       applied: Op
+0001a3f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0001a400: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
+0001a410: 7369 7a65 5f70 6572 5f6d 7367 3a20 4f70  size_per_msg: Op
+0001a420: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0001a430: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
+0001a440: 696e 666c 6967 6874 5f6d 7367 733a 204f  inflight_msgs: O
+0001a450: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0001a460: 6f6e 652c 0a20 2020 2020 2020 2063 6865  one,.        che
+0001a470: 636b 5f71 756f 7275 6d3a 204f 7074 696f  ck_quorum: Optio
+0001a480: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
+0001a490: 2c0a 2020 2020 2020 2020 7072 655f 766f  ,.        pre_vo
+0001a4a0: 7465 3a20 4f70 7469 6f6e 616c 5b62 6f6f  te: Optional[boo
+0001a4b0: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
+0001a4c0: 2020 206d 696e 5f65 6c65 6374 696f 6e5f     min_election_
+0001a4d0: 7469 636b 3a20 4f70 7469 6f6e 616c 5b69  tick: Optional[i
+0001a4e0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+0001a4f0: 2020 2020 6d61 785f 656c 6563 7469 6f6e      max_election
+0001a500: 5f74 6963 6b3a 204f 7074 696f 6e61 6c5b  _tick: Optional[
+0001a510: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+0001a520: 2020 2020 2072 6561 645f 6f6e 6c79 5f6f       read_only_o
+0001a530: 7074 696f 6e3a 204f 7074 696f 6e61 6c5b  ption: Optional[
+0001a540: 2252 6561 644f 6e6c 794f 7074 696f 6e22  "ReadOnlyOption"
+0001a550: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0001a560: 2020 736b 6970 5f62 6361 7374 5f63 6f6d    skip_bcast_com
+0001a570: 6d69 743a 204f 7074 696f 6e61 6c5b 626f  mit: Optional[bo
+0001a580: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
+0001a590: 2020 2020 6261 7463 685f 6170 7065 6e64      batch_append
+0001a5a0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+0001a5b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0001a5c0: 2070 7269 6f72 6974 793a 204f 7074 696f   priority: Optio
+0001a5d0: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+0001a5e0: 0a20 2020 2020 2020 206d 6178 5f75 6e63  .        max_unc
+0001a5f0: 6f6d 6d69 7474 6564 5f73 697a 653a 204f  ommitted_size: O
+0001a600: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+0001a610: 6f6e 652c 0a20 2020 2020 2020 206d 6178  one,.        max
+0001a620: 5f63 6f6d 6d69 7474 6564 5f73 697a 655f  _committed_size_
+0001a630: 7065 725f 7265 6164 793a 204f 7074 696f  per_ready: Optio
+0001a640: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+0001a650: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a0a  .    ) -> None:.
+0001a660: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001a670: 2020 2020 3a70 6172 616d 2069 643a 2054      :param id: T
+0001a680: 6865 2069 6465 6e74 6974 7920 6f66 2074  he identity of t
+0001a690: 6865 206c 6f63 616c 2072 6166 742e 2049  he local raft. I
+0001a6a0: 7420 6361 6e6e 6f74 2062 6520 302c 2061  t cannot be 0, a
+0001a6b0: 6e64 206d 7573 7420 6265 2075 6e69 7175  nd must be uniqu
+0001a6c0: 6520 696e 2074 6865 2067 726f 7570 2e0a  e in the group..
+0001a6d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0001a6e0: 656c 6563 7469 6f6e 5f74 6963 6b3a 2054  election_tick: T
+0001a6f0: 6865 206e 756d 6265 7220 6f66 206e 6f64  he number of nod
+0001a700: 652e 7469 636b 2069 6e76 6f63 6174 696f  e.tick invocatio
+0001a710: 6e73 2074 6861 7420 6d75 7374 2070 6173  ns that must pas
+0001a720: 7320 6265 7477 6565 6e0a 2020 2020 2020  s between.      
+0001a730: 2020 656c 6563 7469 6f6e 732e 2054 6861    elections. Tha
+0001a740: 7420 6973 2c20 6966 2061 2066 6f6c 6c6f  t is, if a follo
+0001a750: 7765 7220 646f 6573 206e 6f74 2072 6563  wer does not rec
+0001a760: 6569 7665 2061 6e79 206d 6573 7361 6765  eive any message
+0001a770: 2066 726f 6d20 7468 650a 2020 2020 2020   from the.      
+0001a780: 2020 6c65 6164 6572 206f 6620 6375 7272    leader of curr
+0001a790: 656e 7420 7465 726d 2062 6566 6f72 6520  ent term before 
+0001a7a0: 456c 6563 7469 6f6e 5469 636b 2068 6173  ElectionTick has
+0001a7b0: 2065 6c61 7073 6564 2c20 6974 2077 696c   elapsed, it wil
+0001a7c0: 6c20 6265 636f 6d65 0a20 2020 2020 2020  l become.       
+0001a7d0: 2063 616e 6469 6461 7465 2061 6e64 2073   candidate and s
+0001a7e0: 7461 7274 2061 6e20 656c 6563 7469 6f6e  tart an election
+0001a7f0: 2e20 656c 6563 7469 6f6e 5f74 6963 6b20  . election_tick 
+0001a800: 6d75 7374 2062 6520 6772 6561 7465 7220  must be greater 
+0001a810: 7468 616e 0a20 2020 2020 2020 2048 6561  than.        Hea
+0001a820: 7274 6265 6174 5469 636b 2e20 5765 2073  rtbeatTick. We s
+0001a830: 7567 6765 7374 2065 6c65 6374 696f 6e5f  uggest election_
+0001a840: 7469 636b 203d 2031 3020 2a20 4865 6172  tick = 10 * Hear
+0001a850: 7462 6561 7454 6963 6b20 746f 2061 766f  tbeatTick to avo
+0001a860: 6964 0a20 2020 2020 2020 2075 6e6e 6563  id.        unnec
+0001a870: 6573 7361 7279 206c 6561 6465 7220 7377  essary leader sw
+0001a880: 6974 6368 696e 670a 0a20 2020 2020 2020  itching..       
+0001a890: 203a 7061 7261 6d20 6865 6172 7462 6561   :param heartbea
+0001a8a0: 745f 7469 636b 3a20 4865 6172 7462 6561  t_tick: Heartbea
+0001a8b0: 7454 6963 6b20 6973 2074 6865 206e 756d  tTick is the num
+0001a8c0: 6265 7220 6f66 206e 6f64 652e 7469 636b  ber of node.tick
+0001a8d0: 2069 6e76 6f63 6174 696f 6e73 2074 6861   invocations tha
+0001a8e0: 7420 6d75 7374 2070 6173 7320 6265 7477  t must pass betw
+0001a8f0: 6565 6e0a 2020 2020 2020 2020 6865 6172  een.        hear
+0001a900: 7462 6561 7473 2e20 5468 6174 2069 732c  tbeats. That is,
+0001a910: 2061 206c 6561 6465 7220 7365 6e64 7320   a leader sends 
+0001a920: 6865 6172 7462 6561 7420 6d65 7373 6167  heartbeat messag
+0001a930: 6573 2074 6f20 6d61 696e 7461 696e 2069  es to maintain i
+0001a940: 7473 0a20 2020 2020 2020 206c 6561 6465  ts.        leade
+0001a950: 7273 6869 7020 6576 6572 7920 6865 6172  rship every hear
+0001a960: 7462 6561 7420 7469 636b 732e 0a0a 2020  tbeat ticks...  
+0001a970: 2020 2020 2020 3a70 6172 616d 2061 7070        :param app
+0001a980: 6c69 6564 3a20 4170 706c 6965 6420 6973  lied: Applied is
+0001a990: 2074 6865 206c 6173 7420 6170 706c 6965   the last applie
+0001a9a0: 6420 696e 6465 782e 2049 7420 7368 6f75  d index. It shou
+0001a9b0: 6c64 206f 6e6c 7920 6265 2073 6574 2077  ld only be set w
+0001a9c0: 6865 6e20 7265 7374 6172 7469 6e67 0a20  hen restarting. 
+0001a9d0: 2020 2020 2020 2072 6166 742e 2072 6166         raft. raf
+0001a9e0: 7420 7769 6c6c 206e 6f74 2072 6574 7572  t will not retur
+0001a9f0: 6e20 656e 7472 6965 7320 746f 2074 6865  n entries to the
+0001aa00: 2061 7070 6c69 6361 7469 6f6e 2073 6d61   application sma
+0001aa10: 6c6c 6572 206f 7220 6571 7561 6c20 746f  ller or equal to
+0001aa20: 2041 7070 6c69 6564 2e0a 2020 2020 2020   Applied..      
+0001aa30: 2020 4966 2041 7070 6c69 6564 2069 7320    If Applied is 
+0001aa40: 756e 7365 7420 7768 656e 2072 6573 7461  unset when resta
+0001aa50: 7274 696e 672c 2072 6166 7420 6d69 6768  rting, raft migh
+0001aa60: 7420 7265 7475 726e 2070 7265 7669 6f75  t return previou
+0001aa70: 7320 6170 706c 6965 6420 656e 7472 6965  s applied entrie
+0001aa80: 732e 0a20 2020 2020 2020 2054 6869 7320  s..        This 
+0001aa90: 6973 2061 2076 6572 7920 6170 706c 6963  is a very applic
+0001aaa0: 6174 696f 6e20 6465 7065 6e64 656e 7420  ation dependent 
+0001aab0: 636f 6e66 6967 7572 6174 696f 6e2e 0a0a  configuration...
+0001aac0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
+0001aad0: 6178 5f73 697a 655f 7065 725f 6d73 673a  ax_size_per_msg:
+0001aae0: 204c 696d 6974 2074 6865 206d 6178 2073   Limit the max s
+0001aaf0: 697a 6520 6f66 2065 6163 6820 6170 7065  ize of each appe
+0001ab00: 6e64 206d 6573 7361 6765 2e20 536d 616c  nd message. Smal
+0001ab10: 6c65 7220 7661 6c75 6520 6c6f 7765 7273  ler value lowers
+0001ab20: 0a20 2020 2020 2020 2074 6865 2072 6166  .        the raf
+0001ab30: 7420 7265 636f 7665 7279 2063 6f73 7428  t recovery cost(
+0001ab40: 696e 6974 6961 6c20 7072 6f62 696e 6720  initial probing 
+0001ab50: 616e 6420 6d65 7373 6167 6520 6c6f 7374  and message lost
+0001ab60: 2064 7572 696e 6720 6e6f 726d 616c 206f   during normal o
+0001ab70: 7065 7261 7469 6f6e 292e 0a20 2020 2020  peration)..     
+0001ab80: 2020 204f 6e20 7468 6520 6f74 6865 7220     On the other 
+0001ab90: 7369 6465 2c20 6974 206d 6967 6874 2061  side, it might a
+0001aba0: 6666 6563 7420 7468 6520 7468 726f 7567  ffect the throug
+0001abb0: 6870 7574 2064 7572 696e 6720 6e6f 726d  hput during norm
+0001abc0: 616c 2072 6570 6c69 6361 7469 6f6e 2e0a  al replication..
+0001abd0: 2020 2020 2020 2020 4e6f 7465 3a20 6d61          Note: ma
+0001abe0: 7468 2e4d 6178 5575 7369 7a65 3634 2066  th.MaxUusize64 f
+0001abf0: 6f72 2075 6e6c 696d 6974 6564 2c20 3020  or unlimited, 0 
+0001ac00: 666f 7220 6174 206d 6f73 7420 6f6e 6520  for at most one 
+0001ac10: 656e 7472 7920 7065 7220 6d65 7373 6167  entry per messag
+0001ac20: 652e 0a0a 2020 2020 2020 2020 3a70 6172  e...        :par
+0001ac30: 616d 206d 6178 5f69 6e66 6c69 6768 745f  am max_inflight_
+0001ac40: 6d73 6773 3a20 4c69 6d69 7420 7468 6520  msgs: Limit the 
+0001ac50: 6d61 7820 6e75 6d62 6572 206f 6620 696e  max number of in
+0001ac60: 2d66 6c69 6768 7420 6170 7065 6e64 206d  -flight append m
+0001ac70: 6573 7361 6765 7320 6475 7269 6e67 206f  essages during o
+0001ac80: 7074 696d 6973 7469 630a 2020 2020 2020  ptimistic.      
+0001ac90: 2020 7265 706c 6963 6174 696f 6e20 7068    replication ph
+0001aca0: 6173 652e 2054 6865 2061 7070 6c69 6361  ase. The applica
+0001acb0: 7469 6f6e 2074 7261 6e73 706f 7274 6174  tion transportat
+0001acc0: 696f 6e20 6c61 7965 7220 7573 7561 6c6c  ion layer usuall
+0001acd0: 7920 6861 7320 6974 7320 6f77 6e20 7365  y has its own se
+0001ace0: 6e64 696e 670a 2020 2020 2020 2020 6275  nding.        bu
+0001acf0: 6666 6572 206f 7665 7220 5443 502f 5544  ffer over TCP/UD
+0001ad00: 502e 2053 6574 2074 6f20 6176 6f69 6420  P. Set to avoid 
+0001ad10: 6f76 6572 666c 6f77 696e 6720 7468 6174  overflowing that
+0001ad20: 2073 656e 6469 6e67 2062 7566 6665 722e   sending buffer.
+0001ad30: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0001ad40: 2063 6865 636b 5f71 756f 7275 6d3a 2053   check_quorum: S
+0001ad50: 7065 6369 6679 2069 6620 7468 6520 6c65  pecify if the le
+0001ad60: 6164 6572 2073 686f 756c 6420 6368 6563  ader should chec
+0001ad70: 6b20 7175 6f72 756d 2061 6374 6976 6974  k quorum activit
+0001ad80: 792e 204c 6561 6465 7220 7374 6570 7320  y. Leader steps 
+0001ad90: 646f 776e 2077 6865 6e0a 2020 2020 2020  down when.      
+0001ada0: 2020 7175 6f72 756d 2069 7320 6e6f 7420    quorum is not 
+0001adb0: 6163 7469 7665 2066 6f72 2061 6e20 656c  active for an el
+0001adc0: 6563 7469 6f6e 5469 6d65 6f75 742e 0a0a  ectionTimeout...
+0001add0: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+0001ade0: 7265 5f76 6f74 653a 2045 6e61 626c 6573  re_vote: Enables
+0001adf0: 2074 6865 2050 7265 2d56 6f74 6520 616c   the Pre-Vote al
+0001ae00: 676f 7269 7468 6d20 6465 7363 7269 6265  gorithm describe
+0001ae10: 6420 696e 2072 6166 7420 7468 6573 6973  d in raft thesis
+0001ae20: 2073 6563 7469 6f6e 0a20 2020 2020 2020   section.       
+0001ae30: 2039 2e36 2e20 5468 6973 2070 7265 7665   9.6. This preve
+0001ae40: 6e74 7320 6469 7372 7570 7469 6f6e 2077  nts disruption w
+0001ae50: 6865 6e20 6120 6e6f 6465 2074 6861 7420  hen a node that 
+0001ae60: 6861 7320 6265 656e 2070 6172 7469 7469  has been partiti
+0001ae70: 6f6e 6564 2061 7761 790a 2020 2020 2020  oned away.      
+0001ae80: 2020 7265 6a6f 696e 7320 7468 6520 636c    rejoins the cl
+0001ae90: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
+0001aea0: 3a70 6172 616d 206d 696e 5f65 6c65 6374  :param min_elect
+0001aeb0: 696f 6e5f 7469 636b 3a20 5468 6520 7261  ion_tick: The ra
+0001aec0: 6e67 6520 6f66 2065 6c65 6374 696f 6e20  nge of election 
+0001aed0: 7469 6d65 6f75 742e 2049 6e20 736f 6d65  timeout. In some
+0001aee0: 2063 6173 6573 2c20 7765 2068 6f70 6520   cases, we hope 
+0001aef0: 736f 6d65 206e 6f64 6573 2068 6173 206c  some nodes has l
+0001af00: 6573 7320 706f 7373 6962 696c 6974 790a  ess possibility.
+0001af10: 2020 2020 2020 2020 746f 2062 6563 6f6d          to becom
+0001af20: 6520 6c65 6164 6572 2e20 5468 6973 2063  e leader. This c
+0001af30: 6f6e 6669 6775 7261 7469 6f6e 2065 6e73  onfiguration ens
+0001af40: 7572 6573 2074 6861 7420 7468 6520 7261  ures that the ra
+0001af50: 6e64 6f6d 697a 6564 2065 6c65 6374 696f  ndomized electio
+0001af60: 6e5f 7469 6d65 6f75 740a 2020 2020 2020  n_timeout.      
+0001af70: 2020 7769 6c6c 2061 6c77 6179 7320 6265    will always be
+0001af80: 2073 7569 7420 696e 205b 6d69 6e5f 656c   suit in [min_el
+0001af90: 6563 7469 6f6e 5f74 6963 6b2c 206d 6178  ection_tick, max
+0001afa0: 5f65 6c65 6374 696f 6e5f 7469 636b 292e  _election_tick).
+0001afb0: 0a20 2020 2020 2020 2049 6620 6974 2069  .        If it i
+0001afc0: 7320 302c 2074 6865 6e20 656c 6563 7469  s 0, then electi
+0001afd0: 6f6e 5f74 6963 6b20 7769 6c6c 2062 6520  on_tick will be 
+0001afe0: 6368 6f73 656e 2e0a 0a20 2020 2020 2020  chosen...       
+0001aff0: 203a 7061 7261 6d20 6d61 785f 656c 6563   :param max_elec
+0001b000: 7469 6f6e 5f74 6963 6b3a 2049 6620 6974  tion_tick: If it
+0001b010: 2069 7320 302c 2074 6865 6e20 3220 2a20   is 0, then 2 * 
+0001b020: 656c 6563 7469 6f6e 5f74 6963 6b20 7769  election_tick wi
+0001b030: 6c6c 2062 6520 6368 6f73 656e 2e0a 0a20  ll be chosen... 
+0001b040: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+0001b050: 6164 5f6f 6e6c 795f 6f70 7469 6f6e 3a20  ad_only_option: 
+0001b060: 4368 6f6f 7365 2074 6865 206c 696e 6561  Choose the linea
+0001b070: 7269 7a61 6269 6c69 7479 206d 6f64 6520  rizability mode 
+0001b080: 6f72 2074 6865 206c 6561 7365 206d 6f64  or the lease mod
+0001b090: 6520 746f 2072 6561 6420 6461 7461 2e20  e to read data. 
+0001b0a0: 4966 2079 6f75 2064 6f6e e280 9974 2063  If you don...t c
+0001b0b0: 6172 6520 6162 6f75 7420 7468 6520 7265  are about the re
+0001b0c0: 6164 2063 6f6e 7369 7374 656e 6379 2061  ad consistency a
+0001b0d0: 6e64 2077 616e 7420 6120 6869 6768 6572  nd want a higher
+0001b0e0: 2072 6561 6420 7065 7266 6f72 6d61 6e63   read performanc
+0001b0f0: 652c 2079 6f75 2063 616e 2075 7365 2074  e, you can use t
+0001b100: 6865 206c 6561 7365 206d 6f64 652e 0a20  he lease mode.. 
+0001b110: 2020 2020 2020 2053 6574 7469 6e67 2074         Setting t
+0001b120: 6869 7320 746f 2060 4c65 6173 6542 6173  his to `LeaseBas
+0001b130: 6564 6020 7265 7175 6972 6573 2060 6368  ed` requires `ch
+0001b140: 6563 6b5f 7175 6f72 756d 203d 2074 7275  eck_quorum = tru
+0001b150: 6560 2e0a 0a20 2020 2020 2020 203a 7061  e`...        :pa
+0001b160: 7261 6d20 736b 6970 5f62 6361 7374 5f63  ram skip_bcast_c
+0001b170: 6f6d 6d69 743a 2044 6f6e 2774 2062 726f  ommit: Don't bro
+0001b180: 6164 6361 7374 2061 6e20 656d 7074 7920  adcast an empty 
+0001b190: 7261 6674 2065 6e74 7279 2074 6f20 6e6f  raft entry to no
+0001b1a0: 7469 6679 2066 6f6c 6c6f 7765 7220 746f  tify follower to
+0001b1b0: 2063 6f6d 6d69 7420 616e 2065 6e74 7279   commit an entry
+0001b1c0: 2e0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
+0001b1d0: 6179 206d 616b 6520 666f 6c6c 6f77 6572  ay make follower
+0001b1e0: 2077 6169 7420 6120 6c6f 6e67 6572 2074   wait a longer t
+0001b1f0: 696d 6520 746f 2061 7070 6c79 2061 6e20  ime to apply an 
+0001b200: 656e 7472 792e 2054 6869 7320 636f 6e66  entry. This conf
+0001b210: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+0001b220: 2020 4d61 7920 6166 6665 6374 2070 726f    May affect pro
+0001b230: 706f 7361 6c20 666f 7277 6172 6469 6e67  posal forwarding
+0001b240: 2061 6e64 2066 6f6c 6c6f 7765 7220 7265   and follower re
+0001b250: 6164 2e0a 0a20 2020 2020 2020 203a 7061  ad...        :pa
+0001b260: 7261 6d20 6261 7463 685f 6170 7065 6e64  ram batch_append
+0001b270: 3a20 4261 7463 6865 7320 6576 6572 7920  : Batches every 
+0001b280: 6170 7065 6e64 206d 7367 2069 6620 616e  append msg if an
+0001b290: 7920 6170 7065 6e64 206d 7367 2061 6c72  y append msg alr
+0001b2a0: 6561 6479 2065 7869 7374 730a 0a20 2020  eady exists..   
+0001b2b0: 2020 2020 203a 7061 7261 6d20 7072 696f       :param prio
+0001b2c0: 7269 7479 3a20 5468 6520 656c 6563 7469  rity: The electi
+0001b2d0: 6f6e 2070 7269 6f72 6974 7920 6f66 2074  on priority of t
+0001b2e0: 6869 7320 6e6f 6465 2e0a 0a20 2020 2020  his node...     
+0001b2f0: 2020 203a 7061 7261 6d20 6d61 785f 756e     :param max_un
+0001b300: 636f 6d6d 6974 7465 645f 7369 7a65 3a20  committed_size: 
+0001b310: 5370 6563 6966 7920 6d61 7869 6d75 6d20  Specify maximum 
+0001b320: 6f66 2075 6e63 6f6d 6d69 7474 6564 2065  of uncommitted e
+0001b330: 6e74 7279 2073 697a 652e 0a20 2020 2020  ntry size..     
+0001b340: 2020 2057 6865 6e20 7468 6973 206c 696d     When this lim
+0001b350: 6974 2069 7320 7265 6163 6865 642c 2061  it is reached, a
+0001b360: 6c6c 2070 726f 706f 7361 6c73 2074 6f20  ll proposals to 
+0001b370: 6170 7065 6e64 206e 6577 206c 6f67 2077  append new log w
+0001b380: 696c 6c20 6265 2064 726f 7070 6564 0a0a  ill be dropped..
+0001b390: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
+0001b3a0: 6178 5f63 6f6d 6d69 7474 6564 5f73 697a  ax_committed_siz
+0001b3b0: 655f 7065 725f 7265 6164 793a 204d 6178  e_per_ready: Max
+0001b3c0: 2073 697a 6520 666f 7220 636f 6d6d 6974   size for commit
+0001b3d0: 7465 6420 656e 7472 6965 7320 696e 2061  ted entries in a
+0001b3e0: 2060 5265 6164 7960 2e0a 2020 2020 2020   `Ready`..      
+0001b3f0: 2020 2222 220a 2020 2020 6465 6620 6d61    """.    def ma
+0001b400: 6b65 5f72 6566 2873 656c 6629 202d 3e20  ke_ref(self) -> 
+0001b410: 2243 6f6e 6669 6752 6566 223a 202e 2e2e  "ConfigRef": ...
+0001b420: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+0001b430: 6f64 0a20 2020 2064 6566 2064 6566 6175  od.    def defau
+0001b440: 6c74 2829 202d 3e20 2243 6f6e 6669 6722  lt() -> "Config"
+0001b450: 3a20 2e2e 2e0a 0a63 6c61 7373 2043 6f6e  : .....class Con
+0001b460: 6669 6752 6566 285f 5f41 5049 5f43 6f6e  figRef(__API_Con
+0001b470: 6669 6729 3a0a 2020 2020 2222 220a 2020  fig):.    """.  
+0001b480: 2020 5265 6665 7265 6e63 6520 7479 7065    Reference type
+0001b490: 206f 6620 3a63 6c61 7373 3a60 496e 666c   of :class:`Infl
+0001b4a0: 6967 6874 7352 6566 602e 0a20 2020 2022  ightsRef`..    "
+0001b4b0: 2222 0a0a 2320 544f 444f 3a20 4164 6420  ""..# TODO: Add 
+0001b4c0: 6265 6c6f 7720 696d 706c 656d 656e 7461  below implementa
+0001b4d0: 7469 6f6e 2069 6620 6e65 6564 6564 2c20  tion if needed, 
+0001b4e0: 6f74 6865 7277 6973 6520 7265 6d6f 7665  otherwise remove
+0001b4f0: 2062 656c 6f77 2063 6f64 6573 2e0a 2320   below codes..# 
+0001b500: 636c 6173 7320 5f5f 4150 495f 5374 6174  class __API_Stat
+0001b510: 7573 3a0a 2320 2020 2020 6465 6620 6765  us:.#     def ge
+0001b520: 745f 6170 706c 6965 6428 7365 6c66 2920  t_applied(self) 
+0001b530: 2d3e 2069 6e74 3a0a 2320 2020 2020 2020  -> int:.#       
+0001b540: 2020 2222 2220 2222 220a 2320 2020 2020    """ """.#     
+0001b550: 6465 6620 7365 745f 6170 706c 6965 6428  def set_applied(
+0001b560: 7365 6c66 2c20 6170 706c 6965 643a 2069  self, applied: i
+0001b570: 6e74 2920 2d3e 204e 6f6e 653a 0a23 2020  nt) -> None:.#  
+0001b580: 2020 2020 2020 2022 2222 2022 2222 0a23         """ """.#
+0001b590: 2020 2020 2064 6566 2067 6574 5f69 6428       def get_id(
+0001b5a0: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2320  self) -> int:.# 
+0001b5b0: 2020 2020 2020 2020 2222 2220 2222 220a          """ """.
+0001b5c0: 2320 2020 2020 6465 6620 7365 745f 6964  #     def set_id
+0001b5d0: 2873 656c 662c 2069 643a 2069 6e74 2920  (self, id: int) 
+0001b5e0: 2d3e 204e 6f6e 653a 0a23 2020 2020 2020  -> None:.#      
+0001b5f0: 2020 2022 2222 2022 2222 0a23 2020 2020     """ """.#    
+0001b600: 2064 6566 2067 6574 5f68 7328 7365 6c66   def get_hs(self
+0001b610: 2920 2d3e 2048 6172 6453 7461 7465 5265  ) -> HardStateRe
+0001b620: 663a 0a23 2020 2020 2020 2020 2022 2222  f:.#         """
+0001b630: 2022 2222 0a23 2020 2020 2064 6566 2073   """.#     def s
+0001b640: 6574 5f68 7328 7365 6c66 2c20 6873 3a20  et_hs(self, hs: 
+0001b650: 4861 7264 5374 6174 6552 6566 2920 2d3e  HardStateRef) ->
+0001b660: 204e 6f6e 653a 0a23 2020 2020 2020 2020   None:.#        
+0001b670: 2022 2222 2022 2222 0a23 2020 2020 2064   """ """.#     d
+0001b680: 6566 2067 6574 5f73 7328 7365 6c66 2920  ef get_ss(self) 
+0001b690: 2d3e 2053 6f66 7453 7461 7465 5265 663a  -> SoftStateRef:
+0001b6a0: 0a23 2020 2020 2020 2020 2022 2222 2022  .#         """ "
+0001b6b0: 2222 0a23 2020 2020 2064 6566 2073 6574  "".#     def set
+0001b6c0: 5f73 7328 7365 6c66 2c20 7373 3a20 536f  _ss(self, ss: So
+0001b6d0: 6674 5374 6174 6552 6566 2920 2d3e 204e  ftStateRef) -> N
+0001b6e0: 6f6e 653a 0a23 2020 2020 2020 2020 2022  one:.#         "
+0001b6f0: 2222 2022 2222 0a23 2020 2020 2064 6566  "" """.#     def
+0001b700: 2067 6574 5f70 726f 6772 6573 7328 7365   get_progress(se
+0001b710: 6c66 2920 2d3e 204f 7074 696f 6e61 6c5b  lf) -> Optional[
+0001b720: 5072 6f67 7265 7373 5472 6163 6b65 7252  ProgressTrackerR
+0001b730: 6566 5d3a 0a23 2020 2020 2020 2020 2022  ef]:.#         "
+0001b740: 2222 2022 2222 0a23 2020 2020 2064 6566  "" """.#     def
+0001b750: 2073 6574 5f70 726f 6772 6573 7328 0a23   set_progress(.#
+0001b760: 2020 2020 2020 2020 2073 656c 662c 2074           self, t
+0001b770: 7261 636b 6572 3a20 4f70 7469 6f6e 616c  racker: Optional
+0001b780: 5b50 726f 6772 6573 7354 7261 636b 6572  [ProgressTracker
+0001b790: 5d20 7c20 4f70 7469 6f6e 616c 5b50 726f  ] | Optional[Pro
+0001b7a0: 6772 6573 7354 7261 636b 6572 5265 665d  gressTrackerRef]
+0001b7b0: 0a23 2020 2020 2029 202d 3e20 4e6f 6e65  .#     ) -> None
+0001b7c0: 3a0a 2320 2020 2020 2020 2020 2222 2220  :.#         """ 
+0001b7d0: 2222 220a 0a23 2063 6c61 7373 2049 6e4d  """..# class InM
+0001b7e0: 656d 6f72 7953 7461 7475 7328 5f5f 4150  emoryStatus(__AP
+0001b7f0: 495f 5374 6174 7573 293a 0a23 2020 2020  I_Status):.#    
+0001b800: 2022 2222 0a23 2020 2020 2052 6570 7265   """.#     Repre
+0001b810: 7365 6e74 7320 7468 6520 6375 7272 656e  sents the curren
+0001b820: 7420 7374 6174 7573 206f 6620 7468 6520  t status of the 
+0001b830: 7261 6674 0a23 2020 2020 2022 2222 0a0a  raft.#     """..
+0001b840: 2320 2020 2020 6465 6620 5f5f 696e 6974  #     def __init
+0001b850: 5f5f 2873 656c 662c 2072 6166 743a 2049  __(self, raft: I
+0001b860: 6e4d 656d 6f72 7952 6166 7429 202d 3e20  nMemoryRaft) -> 
+0001b870: 4e6f 6e65 3a20 2e2e 2e0a 2320 2020 2020  None: ....#     
+0001b880: 6465 6620 6d61 6b65 5f72 6566 2873 656c  def make_ref(sel
+0001b890: 6629 202d 3e20 5374 6174 7573 5f5f 4d65  f) -> Status__Me
+0001b8a0: 6d73 746f 7261 6765 5265 663a 202e 2e2e  mstorageRef: ...
+0001b8b0: 0a0a 2320 636c 6173 7320 496e 4d65 6d6f  ..# class InMemo
+0001b8c0: 7279 5374 6174 7573 5265 6628 5f5f 4150  ryStatusRef(__AP
+0001b8d0: 495f 5374 6174 7573 293a 0a23 2020 2020  I_Status):.#    
+0001b8e0: 2022 2222 0a23 2020 2020 2052 6566 6572   """.#     Refer
+0001b8f0: 656e 6365 2074 7970 6520 6f66 203a 636c  ence type of :cl
+0001b900: 6173 733a 6053 7461 7475 735f 5f4d 656d  ass:`Status__Mem
+0001b910: 7374 6f72 6167 6560 2e0a 2320 2020 2020  storage`..#     
+0001b920: 2222 220a 0a63 6c61 7373 2044 6573 7472  """..class Destr
+0001b930: 6f79 6564 5265 6655 7365 6445 7272 6f72  oyedRefUsedError
+0001b940: 2845 7863 6570 7469 6f6e 293a 0a20 2020  (Exception):.   
+0001b950: 2022 2222 2022 2222 0a0a 636c 6173 7320   """ """..class 
+0001b960: 5261 6674 4572 726f 7228 4578 6365 7074  RaftError(Except
+0001b970: 696f 6e29 3a0a 2020 2020 2222 2220 2222  ion):.    """ ""
+0001b980: 220a 0a63 6c61 7373 2045 7869 7374 7345  "..class ExistsE
+0001b990: 7272 6f72 2852 6166 7445 7272 6f72 293a  rror(RaftError):
+0001b9a0: 0a20 2020 2022 2222 0a20 2020 2054 6865  .    """.    The
+0001b9b0: 206e 6f64 6520 7b69 647d 2061 6c72 6561   node {id} alrea
+0001b9c0: 6479 2065 7869 7374 7320 696e 2074 6865  dy exists in the
+0001b9d0: 207b 7365 747d 2073 6574 2e0a 2020 2020   {set} set..    
+0001b9e0: 2222 220a 0a20 2020 2069 643a 2069 6e74  """..    id: int
+0001b9f0: 0a20 2020 2073 6574 3a20 7374 720a 0a63  .    set: str..c
+0001ba00: 6c61 7373 204e 6f74 4578 6973 7473 2852  lass NotExists(R
+0001ba10: 6166 7445 7272 6f72 293a 0a20 2020 2022  aftError):.    "
+0001ba20: 2222 0a20 2020 2054 6865 206e 6f64 6520  "".    The node 
+0001ba30: 7b69 647d 2069 7320 6e6f 7420 696e 2074  {id} is not in t
+0001ba40: 6865 207b 7365 747d 2073 6574 2e0a 2020  he {set} set..  
+0001ba50: 2020 2222 220a 0a20 2020 2069 643a 2069    """..    id: i
+0001ba60: 6e74 0a20 2020 2073 6574 3a20 7374 720a  nt.    set: str.
+0001ba70: 0a63 6c61 7373 2043 6f64 6563 4572 726f  .class CodecErro
+0001ba80: 7228 5261 6674 4572 726f 7229 3a0a 2020  r(RaftError):.  
+0001ba90: 2020 2222 220a 2020 2020 4120 7072 6f74    """.    A prot
+0001baa0: 6f62 7566 206d 6573 7361 6765 2063 6f64  obuf message cod
+0001bab0: 6563 2066 6169 6c65 6420 696e 2073 6f6d  ec failed in som
+0001bac0: 6520 6d61 6e6e 6572 2e0a 2020 2020 2222  e manner..    ""
+0001bad0: 220a 0a63 6c61 7373 2043 6f6e 6669 6749  "..class ConfigI
+0001bae0: 6e76 616c 6964 4572 726f 7228 5261 6674  nvalidError(Raft
+0001baf0: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
+0001bb00: 2020 2020 5468 6520 636f 6e66 6967 7572      The configur
+0001bb10: 6174 696f 6e20 6973 2069 6e76 616c 6964  ation is invalid
+0001bb20: 2e0a 2020 2020 2222 220a 0a63 6c61 7373  ..    """..class
+0001bb30: 2050 726f 706f 7361 6c44 726f 7070 6564   ProposalDropped
+0001bb40: 4572 726f 7228 5261 6674 4572 726f 7229  Error(RaftError)
+0001bb50: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+0001bb60: 6520 7072 6f70 6f73 616c 206f 6620 6368  e proposal of ch
+0001bb70: 616e 6765 7320 7761 7320 6472 6f70 7065  anges was droppe
+0001bb80: 642e 0a20 2020 2022 2222 0a0a 636c 6173  d..    """..clas
+0001bb90: 7320 5265 7175 6573 7453 6e61 7073 686f  s RequestSnapsho
+0001bba0: 7444 726f 7070 6564 4572 726f 7228 5261  tDroppedError(Ra
+0001bbb0: 6674 4572 726f 7229 3a0a 2020 2020 2222  ftError):.    ""
+0001bbc0: 220a 2020 2020 5468 6520 7265 7175 6573  ".    The reques
+0001bbd0: 7420 736e 6170 7368 6f74 2069 7320 6472  t snapshot is dr
+0001bbe0: 6f70 7065 642e 0a20 2020 2022 2222 0a0a  opped..    """..
+0001bbf0: 636c 6173 7320 436f 6e66 4368 616e 6765  class ConfChange
+0001bc00: 4572 726f 7228 5261 6674 4572 726f 7229  Error(RaftError)
+0001bc10: 3a0a 2020 2020 2222 220a 2020 2020 436f  :.    """.    Co
+0001bc20: 6e66 4368 616e 6765 2070 726f 706f 7361  nfChange proposa
+0001bc30: 6c20 6973 2069 6e76 616c 6964 2e0a 2020  l is invalid..  
+0001bc40: 2020 2222 220a 0a63 6c61 7373 2049 6f45    """..class IoE
+0001bc50: 7272 6f72 2852 6166 7445 7272 6f72 293a  rror(RaftError):
+0001bc60: 0a20 2020 2022 2222 0a20 2020 2041 6e20  .    """.    An 
+0001bc70: 494f 2065 7272 6f72 206f 6363 7572 7265  IO error occurre
+0001bc80: 642e 0a20 2020 2022 2222 0a0a 636c 6173  d..    """..clas
+0001bc90: 7320 5374 6f72 6545 7272 6f72 2852 6166  s StoreError(Raf
+0001bca0: 7445 7272 6f72 293a 0a20 2020 2022 2222  tError):.    """
+0001bcb0: 0a20 2020 2041 2073 746f 7261 6765 2065  .    A storage e
+0001bcc0: 7272 6f72 206f 6363 7572 7265 642e 0a20  rror occurred.. 
+0001bcd0: 2020 2022 2222 0a0a 636c 6173 7320 5374     """..class St
+0001bce0: 6570 4c6f 6361 6c4d 7367 2852 6166 7445  epLocalMsg(RaftE
+0001bcf0: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
+0001bd00: 2020 2052 6166 7420 6361 6e6e 6f74 2073     Raft cannot s
+0001bd10: 7465 7020 7468 6520 6c6f 6361 6c20 6d65  tep the local me
+0001bd20: 7373 6167 652e 0a20 2020 2022 2222 0a0a  ssage..    """..
+0001bd30: 636c 6173 7320 5374 6570 5065 6572 4e6f  class StepPeerNo
+0001bd40: 7446 6f75 6e64 2852 6166 7445 7272 6f72  tFound(RaftError
+0001bd50: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+0001bd60: 6865 2072 6166 7420 7065 6572 2069 7320  he raft peer is 
+0001bd70: 6e6f 7420 666f 756e 6420 616e 6420 7468  not found and th
+0001bd80: 7573 2063 616e 6e6f 7420 7374 6570 2e0a  us cannot step..
+0001bd90: 2020 2020 2222 220a 0a63 6c61 7373 2052      """..class R
+0001bda0: 6166 7453 746f 7261 6765 4572 726f 7228  aftStorageError(
+0001bdb0: 4578 6365 7074 696f 6e29 3a0a 2020 2020  Exception):.    
+0001bdc0: 2222 220a 2020 2020 416e 2065 7272 6f72  """.    An error
+0001bdd0: 2077 6974 6820 7468 6520 7374 6f72 6167   with the storag
+0001bde0: 652e 0a20 2020 2022 2222 0a0a 636c 6173  e..    """..clas
+0001bdf0: 7320 436f 6d70 6163 7465 6445 7272 6f72  s CompactedError
+0001be00: 2852 6166 7453 746f 7261 6765 4572 726f  (RaftStorageErro
+0001be10: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
+0001be20: 5468 6520 7374 6f72 6167 6520 7761 7320  The storage was 
+0001be30: 636f 6d70 6163 7465 6420 616e 6420 6e6f  compacted and no
+0001be40: 7420 6163 6365 7373 6962 6c65 0a20 2020  t accessible.   
+0001be50: 2022 2222 0a0a 636c 6173 7320 556e 6176   """..class Unav
+0001be60: 6169 6c61 626c 6545 7272 6f72 2852 6166  ailableError(Raf
+0001be70: 7453 746f 7261 6765 4572 726f 7229 3a0a  tStorageError):.
+0001be80: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
+0001be90: 6c6f 6720 6973 206e 6f74 2061 7661 696c  log is not avail
+0001bea0: 6162 6c65 2e0a 2020 2020 2222 220a 0a63  able..    """..c
+0001beb0: 6c61 7373 204c 6f67 5465 6d70 6f72 6172  lass LogTemporar
+0001bec0: 696c 7955 6e61 7661 696c 6162 6c65 4572  ilyUnavailableEr
+0001bed0: 726f 7228 5261 6674 5374 6f72 6167 6545  ror(RaftStorageE
+0001bee0: 7272 6f72 293a 0a20 2020 2022 2222 0a20  rror):.    """. 
+0001bef0: 2020 2054 6865 206c 6f67 2069 7320 6265     The log is be
+0001bf00: 696e 6720 6665 7463 6865 642e 0a20 2020  ing fetched..   
+0001bf10: 2022 2222 0a0a 636c 6173 7320 536e 6170   """..class Snap
+0001bf20: 7368 6f74 4f75 744f 6644 6174 6545 7272  shotOutOfDateErr
+0001bf30: 6f72 2852 6166 7453 746f 7261 6765 4572  or(RaftStorageEr
+0001bf40: 726f 7229 3a0a 2020 2020 2222 220a 2020  ror):.    """.  
+0001bf50: 2020 5468 6520 736e 6170 7368 6f74 2069    The snapshot i
+0001bf60: 7320 6f75 7420 6f66 2064 6174 652e 0a20  s out of date.. 
+0001bf70: 2020 2022 2222 0a0a 636c 6173 7320 536e     """..class Sn
+0001bf80: 6170 7368 6f74 5465 6d70 6f72 6172 696c  apshotTemporaril
+0001bf90: 7955 6e61 7661 696c 6162 6c65 2852 6166  yUnavailable(Raf
+0001bfa0: 7453 746f 7261 6765 4572 726f 7229 3a0a  tStorageError):.
+0001bfb0: 2020 2020 2222 220a 2020 2020 5468 6520      """.    The 
+0001bfc0: 736e 6170 7368 6f74 2069 7320 6265 696e  snapshot is bein
+0001bfd0: 6720 6372 6561 7465 642e 0a20 2020 2022  g created..    "
+0001bfe0: 2222 0a0a 636c 6173 7320 4f74 6865 7245  ""..class OtherE
+0001bff0: 7272 6f72 2852 6166 7453 746f 7261 6765  rror(RaftStorage
+0001c000: 4572 726f 7229 3a0a 2020 2020 2222 220a  Error):.    """.
+0001c010: 2020 2020 536f 6d65 206f 7468 6572 2065      Some other e
+0001c020: 7272 6f72 206f 6363 7572 7265 642e 0a20  rror occurred.. 
+0001c030: 2020 2022 2222 0a                           """.
```

### Comparing `rraft_py-0.1.1/src/bindings/config.rs` & `rraft_py-0.1.2/src/bindings/config.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/get_entries_context.rs` & `rraft_py-0.1.2/src/bindings/get_entries_context.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/global.rs` & `rraft_py-0.1.2/src/bindings/global.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/inflights.rs` & `rraft_py-0.1.2/src/bindings/inflights.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/joint_config.rs` & `rraft_py-0.1.2/src/bindings/joint_config.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/light_ready.rs` & `rraft_py-0.1.2/src/bindings/light_ready.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/majority_config.rs` & `rraft_py-0.1.2/src/bindings/majority_config.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/peer.rs` & `rraft_py-0.1.2/src/bindings/peer.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/progress.rs` & `rraft_py-0.1.2/src/bindings/progress.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/progress_state.rs` & `rraft_py-0.1.2/src/bindings/progress_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/progress_tracker.rs` & `rraft_py-0.1.2/src/bindings/progress_tracker.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/raft_state.rs` & `rraft_py-0.1.2/src/bindings/raft_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/read_state.rs` & `rraft_py-0.1.2/src/bindings/read_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/readonly_option.rs` & `rraft_py-0.1.2/src/bindings/readonly_option.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/ready.rs` & `rraft_py-0.1.2/src/bindings/ready.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/snapshot_status.rs` & `rraft_py-0.1.2/src/bindings/snapshot_status.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/soft_state.rs` & `rraft_py-0.1.2/src/bindings/soft_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/state_role.rs` & `rraft_py-0.1.2/src/bindings/state_role.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/bindings/unstable.rs` & `rraft_py-0.1.2/src/bindings/unstable.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/external_bindings/slog.rs` & `rraft_py-0.1.2/src/external_bindings/slog.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/lib.rs` & `rraft_py-0.1.2/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     m.add_class::<py_storage_bindings::raft::PyRaftRef>()?;
     m.add_class::<py_storage_bindings::raw_node::PyRawNode>()?;
     m.add_class::<py_storage_bindings::raw_node::PyRawNodeRef>()?;
 
     m.add_class::<external_bindings::slog::PyLogger>()?;
     m.add_class::<external_bindings::slog::PyLoggerRef>()?;
     m.add_class::<external_bindings::slog::PyOverflowStrategy>()?;
+    m.add_class::<external_bindings::thread_safe_slog::PyThreadSafeLogger>()?;
 
     m.add_class::<utils::errors::PyRaftError>()?;
     m.add_class::<utils::errors::PyStorageError>()?;
 
     m.add_function(wrap_pyfunction!(bindings::global::majority, m)?)?;
     m.add_function(wrap_pyfunction!(bindings::global::default_logger, m)?)?;
     m.add_function(wrap_pyfunction!(bindings::global::vote_resp_msg_type, m)?)?;
```

### Comparing `rraft_py-0.1.1/src/mem_storage_bindings/mem_storage.rs` & `rraft_py-0.1.2/src/mem_storage_bindings/mem_storage.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/mem_storage_bindings/mem_storage_core.rs` & `rraft_py-0.1.2/src/mem_storage_bindings/mem_storage_core.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/mem_storage_bindings/raft.rs` & `rraft_py-0.1.2/src/mem_storage_bindings/raft.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/mem_storage_bindings/raft_log.rs` & `rraft_py-0.1.2/src/mem_storage_bindings/raft_log.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/mem_storage_bindings/raw_node.rs` & `rraft_py-0.1.2/src/mem_storage_bindings/raw_node.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/py_storage_bindings/py_storage.rs` & `rraft_py-0.1.2/src/py_storage_bindings/py_storage.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/py_storage_bindings/raft.rs` & `rraft_py-0.1.2/src/py_storage_bindings/raft.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/py_storage_bindings/raft_log.rs` & `rraft_py-0.1.2/src/py_storage_bindings/raft_log.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/py_storage_bindings/raw_node.rs` & `rraft_py-0.1.2/src/py_storage_bindings/raw_node.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/conf_change.rs` & `rraft_py-0.1.2/src/raftpb_bindings/conf_change.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/conf_change_single.rs` & `rraft_py-0.1.2/src/raftpb_bindings/conf_change_single.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/conf_change_transition.rs` & `rraft_py-0.1.2/src/raftpb_bindings/conf_change_transition.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/conf_change_type.rs` & `rraft_py-0.1.2/src/raftpb_bindings/conf_change_type.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/conf_change_v2.rs` & `rraft_py-0.1.2/src/raftpb_bindings/conf_change_v2.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/conf_state.rs` & `rraft_py-0.1.2/src/raftpb_bindings/conf_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/entry.rs` & `rraft_py-0.1.2/src/raftpb_bindings/entry.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/entry_type.rs` & `rraft_py-0.1.2/src/raftpb_bindings/entry_type.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/hard_state.rs` & `rraft_py-0.1.2/src/raftpb_bindings/hard_state.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/message.rs` & `rraft_py-0.1.2/src/raftpb_bindings/message.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/message_type.rs` & `rraft_py-0.1.2/src/raftpb_bindings/message_type.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/snapshot.rs` & `rraft_py-0.1.2/src/raftpb_bindings/snapshot.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/raftpb_bindings/snapshot_metadata.rs` & `rraft_py-0.1.2/src/raftpb_bindings/snapshot_metadata.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/utils/errors.rs` & `rraft_py-0.1.2/src/utils/errors.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/src/utils/reference.rs` & `rraft_py-0.1.2/src/utils/reference.rs`

 * *Files identical despite different names*

### Comparing `rraft_py-0.1.1/Cargo.lock` & `rraft_py-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "rraft-py"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "bincode",
  "fxhash",
  "prost",
  "protobuf",
  "pyo3",
  "raft",
```

### Comparing `rraft_py-0.1.1/PKG-INFO` & `rraft_py-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: rraft-py
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE
 Summary: Unofficial Python Binding of the tikv/raft-rs
-
 Keywords: raft,distributed-systems,consensus-algorithm,replication,distributed-database
 Home-Page: https://github.com/lablup/rraft-py
 Author: Lablup Inc.
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/lablup/rraft-py
```


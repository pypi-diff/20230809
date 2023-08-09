# Comparing `tmp/halmos-0.1.1.tar.gz` & `tmp/halmos-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halmos-0.1.1.tar", last modified: Wed Jul 26 06:37:20 2023, max compression
+gzip compressed data, was "halmos-0.1.2.tar", last modified: Wed Aug  9 02:02:29 2023, max compression
```

## Comparing `halmos-0.1.1.tar` & `halmos-0.1.2.tar`

### file list

```diff
@@ -1,129 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.472396 halmos-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 06:37:05.000000 halmos-0.1.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.452396 halmos-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/test-external.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/test-long.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-26 06:37:05.000000 halmos-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-26 06:37:05.000000 halmos-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-26 06:37:05.000000 halmos-0.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-26 06:37:05.000000 halmos-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-26 06:37:05.000000 halmos-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-26 06:37:20.472396 halmos-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-26 06:37:05.000000 halmos-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/benchmarks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-26 06:37:05.000000 halmos-0.1.1/benchmarks/baolean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.452396 halmos-0.1.1/examples/tokens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/examples/tokens/ERC20/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.456396 halmos-0.1.1/examples/tokens/ERC20/src/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/src/SolmateERC20.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC20/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.sol
--rw-r--r--   0 runner    (1001) docker     (123)    27482 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/ERC20Test.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC20/test/SolmateERC20.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC721/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/foundry.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/remappings.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC721/src/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/src/SolmateERC721.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/tokens/ERC721/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/test/ERC721Test.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/tokens/ERC721/test/SolmateERC721.t.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/toy/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/toy/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/toy/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/toy/src/Example.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.460396 halmos-0.1.1/examples/toy/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-26 06:37:05.000000 halmos-0.1.1/examples/toy/test/Example.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-26 06:37:05.000000 halmos-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 06:37:05.000000 halmos-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:37:05.000000 halmos-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:37:20.472396 halmos-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.452396 halmos-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.464396 halmos-0.1.1/src/halmos/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35157 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/cheatcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/pools.py
--rw-r--r--   0 runner    (1001) docker     (123)    85996 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/sevm.py
--rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 06:37:05.000000 halmos-0.1.1/src/halmos/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.464396 halmos-0.1.1/src/halmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 06:37:20.000000 halmos-0.1.1/src/halmos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.464396 halmos-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.468396 halmos-0.1.1/tests/expected/
--rw-r--r--   0 runner    (1001) docker     (123)    34063 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/all.json
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/erc20.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/erc721.json
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/expected/toy.json
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/foundry.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.468396 halmos-0.1.1/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Const.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Counter.sol
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Create.sol
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/List.sol
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/SignExtend.sol
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/src/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:37:20.472396 halmos-0.1.1/tests/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Arith.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/AssertTest.sol
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Block.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Byte.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Console.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Const.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Counter.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Create.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Deal.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Foundry.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Getter.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/HalmosCheatCode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Invalid.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Library.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/LibraryLinking.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/List.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Math.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Natspec.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Opcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Prank.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Proxy.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Reset.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Revert.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Send.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Setup.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/SetupPlus.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/SetupSymbolic.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/SignExtend.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Solver.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Storage.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Store.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Struct.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/TestConstructor.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Token.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/UnsupportedOpcode.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test/Warp.t.sol
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_halmos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-26 06:37:05.000000 halmos-0.1.1/tests/test_sevm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.743347 halmos-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-09 02:02:20.000000 halmos-0.1.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.711348 halmos-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.719348 halmos-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.719348 halmos-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/workflows/test-external.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/workflows/test-long.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-09 02:02:20.000000 halmos-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-09 02:02:20.000000 halmos-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-09 02:02:20.000000 halmos-0.1.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-09 02:02:20.000000 halmos-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-09 02:02:20.000000 halmos-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-09 02:02:29.743347 halmos-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-08-09 02:02:20.000000 halmos-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.723348 halmos-0.1.2/benchmarks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-08-09 02:02:20.000000 halmos-0.1.2/benchmarks/baolean.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.723348 halmos-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-09 02:02:20.000000 halmos-0.1.2/docs/getting-started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.723348 halmos-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.715348 halmos-0.1.2/examples/tokens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.723348 halmos-0.1.2/examples/tokens/ERC20/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.723348 halmos-0.1.2/examples/tokens/ERC20/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/src/OpenZeppelinERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/src/SolmateERC20.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.723348 halmos-0.1.2/examples/tokens/ERC20/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/test/DEIStablecoin.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    27482 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/test/DEIStablecoin.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/test/ERC20Test.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC20/test/SolmateERC20.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.727347 halmos-0.1.2/examples/tokens/ERC721/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/foundry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/remappings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.727347 halmos-0.1.2/examples/tokens/ERC721/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/src/OpenZeppelinERC721.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/src/SolmateERC721.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.727347 halmos-0.1.2/examples/tokens/ERC721/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/test/ERC721Test.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/tokens/ERC721/test/SolmateERC721.t.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.727347 halmos-0.1.2/examples/toy/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/toy/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.727347 halmos-0.1.2/examples/toy/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/toy/src/Example.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.727347 halmos-0.1.2/examples/toy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-09 02:02:20.000000 halmos-0.1.2/examples/toy/test/Example.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-09 02:02:20.000000 halmos-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-09 02:02:20.000000 halmos-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-09 02:02:20.000000 halmos-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 02:02:29.743347 halmos-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.715348 halmos-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.731347 halmos-0.1.2/src/halmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/calldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/cheatcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89009 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/sevm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-09 02:02:20.000000 halmos-0.1.2/src/halmos/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.731347 halmos-0.1.2/src/halmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-09 02:02:29.000000 halmos-0.1.2/src/halmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-08-09 02:02:29.000000 halmos-0.1.2/src/halmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 02:02:29.000000 halmos-0.1.2/src/halmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-09 02:02:29.000000 halmos-0.1.2/src/halmos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-09 02:02:29.000000 halmos-0.1.2/src/halmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-09 02:02:29.000000 halmos-0.1.2/src/halmos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.735347 halmos-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.735347 halmos-0.1.2/tests/expected/
+-rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/expected/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/expected/erc20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/expected/erc721.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/expected/toy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/foundry.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.735347 halmos-0.1.2/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/src/Const.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/src/Counter.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/src/Create.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/src/List.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/src/SignExtend.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/src/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:02:29.743347 halmos-0.1.2/tests/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Arith.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/AssertTest.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Block.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Byte.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Call.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Console.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Const.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Constructor.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Counter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Create.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Create2.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Deal.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Foundry.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Getter.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/HalmosCheatCode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Invalid.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Library.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/LibraryLinking.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/List.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Math.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Natspec.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Opcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Prank.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Proxy.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Reset.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Revert.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Send.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Setup.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/SetupPlus.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/SetupSymbolic.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/SignExtend.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Solver.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Storage.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Store.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Struct.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/TestConstructor.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Token.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/UnsupportedOpcode.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test/Warp.t.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test_halmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-08-09 02:02:20.000000 halmos-0.1.2/tests/test_sevm.py
```

### Comparing `halmos-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `halmos-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/.github/workflows/codeql.yml` & `halmos-0.1.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/.github/workflows/test-external.yml` & `halmos-0.1.2/.github/workflows/test-external.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/.github/workflows/test-long.yml` & `halmos-0.1.2/.github/workflows/test-long.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/.github/workflows/test.yml` & `halmos-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/LICENSE` & `halmos-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/PKG-INFO` & `halmos-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.1.1
+Version: 0.1.2
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: a16z crypto
-Maintainer: Daejun Park
-Maintainer-email: karmacoma <karma@coma.lol>
+Maintainer: Daejun Park, karmacoma <karma@coma.lol>
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -83,15 +82,15 @@
 ```
 $ forge test
 [PASS] testTotalPriceBuggy(uint96,uint32) (runs: 256, μ: 462, ~: 466)
 ```
 
 Once it passes, you can also perform **symbolic testing** to verify the same properties for **all possible inputs** (up to a specified limit):
 ```
-$ halmos
+$ halmos --function test
 [FAIL] testTotalPriceBuggy(uint96,uint32) (paths: 6, time: 0.10s, bounds: [])
 Counterexample: [p_price_uint96 = 39614081294025656978550816768, p_quantity_uint32 = 1073741824]
 ```
 
 _(In this specific example, Halmos discovered an input that violated the assertion, which was missed by the fuzzer!)_
 
 ## Develop
```

### Comparing `halmos-0.1.1/README.md` & `halmos-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ```
 $ forge test
 [PASS] testTotalPriceBuggy(uint96,uint32) (runs: 256, μ: 462, ~: 466)
 ```
 
 Once it passes, you can also perform **symbolic testing** to verify the same properties for **all possible inputs** (up to a specified limit):
 ```
-$ halmos
+$ halmos --function test
 [FAIL] testTotalPriceBuggy(uint96,uint32) (paths: 6, time: 0.10s, bounds: [])
 Counterexample: [p_price_uint96 = 39614081294025656978550816768, p_quantity_uint32 = 1073741824]
 ```
 
 _(In this specific example, Halmos discovered an input that violated the assertion, which was missed by the fuzzer!)_
 
 ## Develop
```

### Comparing `halmos-0.1.1/benchmarks/baolean.sh` & `halmos-0.1.2/benchmarks/baolean.sh`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/README.md` & `halmos-0.1.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.sol` & `halmos-0.1.2/examples/tokens/ERC20/test/DEIStablecoin.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC20/test/DEIStablecoin.t.sol` & `halmos-0.1.2/examples/tokens/ERC20/test/DEIStablecoin.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC20/test/ERC20Test.sol` & `halmos-0.1.2/examples/tokens/ERC20/test/ERC20Test.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol` & `halmos-0.1.2/examples/tokens/ERC20/test/OpenZeppelinERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC20/test/SolmateERC20.t.sol` & `halmos-0.1.2/examples/tokens/ERC20/test/SolmateERC20.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC721/test/ERC721Test.sol` & `halmos-0.1.2/examples/tokens/ERC721/test/ERC721Test.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol` & `halmos-0.1.2/examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/tokens/ERC721/test/SolmateERC721.t.sol` & `halmos-0.1.2/examples/tokens/ERC721/test/SolmateERC721.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/toy/src/Example.sol` & `halmos-0.1.2/examples/toy/src/Example.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/examples/toy/test/Example.t.sol` & `halmos-0.1.2/examples/toy/test/Example.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/pyproject.toml` & `halmos-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 description = "Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode"
 readme = "README.md"
 authors = [
     { name="a16z crypto" },
 ]
 maintainers = [
     { name="Daejun Park" },
-    { name="karmacoma", email="karma@coma.lol" },
+    { name="karmacoma <karma@coma.lol>" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
```

### Comparing `halmos-0.1.1/src/halmos/__main__.py` & `halmos-0.1.2/src/halmos/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from importlib import metadata
 
 from .pools import thread_pool, process_pool
 from .sevm import *
 from .utils import color_good, color_warn, hexify
 from .warnings import *
 from .parser import mk_arg_parser
+from .calldata import Calldata
 
 arg_parser = mk_arg_parser()
 
 # Python version >=3.8.14, >=3.9.14, >=3.10.7, or >=3.11
 if hasattr(sys, "set_int_max_str_digits"):
     sys.set_int_max_str_digits(0)
 
@@ -38,16 +39,17 @@
 
 
 def str_abi(item: Dict) -> str:
     def str_tuple(args: List) -> str:
         ret = []
         for arg in args:
             typ = arg["type"]
-            if typ == "tuple":
-                ret.append(str_tuple(arg["components"]))
+            match = re.search(r"^tuple((\[[0-9]*\])*)$", typ)
+            if match:
+                ret.append(str_tuple(arg["components"]) + match.group(1))
             else:
                 ret.append(typ)
         return "(" + ",".join(ret) + ")"
 
     if item["type"] != "function":
         raise ValueError(item)
     return item["name"] + str_tuple(item["inputs"])
@@ -68,82 +70,27 @@
 def mk_calldata(
     abi: List,
     fun_info: FunctionInfo,
     cd: List,
     dyn_param_size: List[str],
     args: Namespace,
 ) -> None:
-    item = find_abi(abi, fun_info)
-    tba = []
-    offset = 0
-    for param in item["inputs"]:
-        param_name = param["name"]
-        param_type = param["type"]
-        if param_type == "tuple":
-            # TODO: support struct types
-            raise NotImplementedError(f"Not supported parameter type: {param_type}")
-        elif param_type == "bytes" or param_type == "string":
-            # wstore(cd, 4+offset, 32, BitVecVal(<?offset?>, 256))
-            tba.append((4 + offset, param))
-            offset += 32
-        elif param_type.endswith("[]"):
-            raise NotImplementedError(f"Not supported dynamic arrays: {param_type}")
-        else:
-            match = re.search(
-                r"(u?int[0-9]*|address|bool|bytes[0-9]+)(\[([0-9]+)\])?", param_type
-            )
-            if not match:
-                raise NotImplementedError(f"Unknown parameter type: {param_type}")
-            typ = match.group(1)
-            dim = match.group(3)
-            if dim:  # array
-                for idx in range(int(dim)):
-                    wstore(
-                        cd, 4 + offset, 32, BitVec(f"p_{param_name}[{idx}]_{typ}", 256)
-                    )
-                    offset += 32
-            else:  # primitive
-                wstore(cd, 4 + offset, 32, BitVec(f"p_{param_name}_{typ}", 256))
-                offset += 32
-
-    arrlen = mk_arrlen(args)
-    for loc_param in tba:
-        loc = loc_param[0]
-        param = loc_param[1]
-        param_name = param["name"]
-        param_type = param["type"]
-
-        if param_name not in arrlen:
-            size = args.loop
-            if args.debug:
-                print(
-                    f"Warning: no size provided for {param_name}; default value {size} will be used."
-                )
-        else:
-            size = arrlen[param_name]
+    # find function abi
+    fun_abi = find_abi(abi, fun_info)
 
-        dyn_param_size.append(f"|{param_name}|={size}")
+    # no parameters
+    if len(fun_abi["inputs"]) == 0:
+        return
+
+    # generate symbolic ABI calldata
+    calldata = Calldata(args, mk_arrlen(args), dyn_param_size)
+    result = calldata.create(fun_abi)
 
-        if param_type == "bytes" or param_type == "string":
-            # head
-            wstore(cd, loc, 32, BitVecVal(offset, 256))
-            # tail
-            size_pad_right = int((size + 31) / 32) * 32
-            wstore(cd, 4 + offset, 32, BitVecVal(size, 256))
-            offset += 32
-            if size_pad_right > 0:
-                wstore(
-                    cd,
-                    4 + offset,
-                    size_pad_right,
-                    BitVec(f"p_{param_name}_{param_type}", 8 * size_pad_right),
-                )
-                offset += size_pad_right
-        else:
-            raise ValueError(param_type)
+    # TODO: use Contract abstraction for calldata
+    wstore(cd, 4, result.size() // 8, result)
 
 
 def mk_callvalue() -> Word:
     return BitVec("msg_value", 256)
 
 
 def mk_balance() -> Word:
@@ -206,64 +153,116 @@
         storage={this: storage},
         balance=balance,
         block=block,
         calldata=[],
         callvalue=callvalue,
         caller=caller,
         this=this,
+        pgm=contract,
         symbolic=args.symbolic_storage,
         solver=solver,
     )
     (exs, _, _) = sevm.run(ex)
 
     for idx, ex in enumerate(exs):
         opcode = ex.current_opcode()
         if opcode in [EVM.STOP, EVM.RETURN, EVM.REVERT, EVM.INVALID]:
             model_with_context = gen_model(args, idx, ex)
             print(
                 f"Final opcode: {mnemonic(opcode)} | Return data: {ex.output} | Input example: {model_with_context.model}"
             )
         else:
-            print(color_warn(f"Not supported: {mnemonic(opcode)} {ex.error}"))
+            warn(INTERNAL_ERROR, f"{mnemonic(opcode)} failed: {ex.error}")
         if args.print_states:
             print(f"# {idx+1} / {len(exs)}")
             print(ex)
 
     return exs
 
 
-def setup(
-    hexcode: str,
-    abi: List,
-    setup_info: FunctionInfo,
+def deploy_test(
+    creation_hexcode: str,
+    deployed_hexcode: str,
+    sevm: SEVM,
     args: Namespace,
+    libs: Dict,
 ) -> Exec:
-    setup_start = timer()
-
-    contract = Contract.from_hexcode(hexcode)
-
-    solver = mk_solver(args)
     this = mk_this()
-    options = mk_options(args)
-
-    sevm = SEVM(options)
 
-    setup_ex = sevm.mk_exec(
-        code={this: contract},
+    ex = sevm.mk_exec(
+        code={this: Contract(b"")},
         storage={this: {}},
         balance=mk_balance(),
         block=mk_block(),
         calldata=[],
         callvalue=con(0),
         caller=mk_caller(args),
         this=this,
+        pgm=None,  # to be added
         symbolic=False,
-        solver=solver,
+        solver=mk_solver(args),
     )
 
+    # deploy libraries and resolve library placeholders in hexcode
+    (creation_hexcode, deployed_hexcode) = ex.resolve_libs(
+        creation_hexcode, deployed_hexcode, libs
+    )
+
+    # test contract creation bytecode
+    creation_bytecode = Contract.from_hexcode(creation_hexcode)
+    ex.pgm = creation_bytecode
+
+    # use the given deployed bytecode if --no-test-constructor is enabled
+    if args.no_test_constructor:
+        deployed_bytecode = Contract.from_hexcode(deployed_hexcode)
+        ex.code[this] = deployed_bytecode
+        ex.pgm = deployed_bytecode
+        return ex
+
+    # create test contract
+    (exs, _, _) = sevm.run(ex)
+
+    # sanity check
+    if len(exs) != 1:
+        raise ValueError(f"constructor: # of paths: {len(exs)}")
+    ex = exs[0]
+    if ex.failed:
+        raise ValueError(f"constructor: failed: {ex.error}")
+    if ex.current_opcode() not in [EVM.STOP, EVM.RETURN]:
+        raise ValueError(f"constructor: failed: {ex.current_opcode()}: {ex.error}")
+
+    # deployed bytecode
+    deployed_bytecode = Contract(ex.output)
+    ex.code[this] = deployed_bytecode
+    ex.pgm = deployed_bytecode
+
+    # reset vm state
+    ex.pc = 0
+    ex.st = State()
+    ex.jumpis = {}
+    ex.output = None
+    ex.prank = Prank()
+
+    return ex
+
+
+def setup(
+    creation_hexcode: str,
+    deployed_hexcode: str,
+    abi: List,
+    setup_info: FunctionInfo,
+    args: Namespace,
+    libs: Dict,
+) -> Exec:
+    setup_start = timer()
+
+    sevm = SEVM(mk_options(args))
+
+    setup_ex = deploy_test(creation_hexcode, deployed_hexcode, sevm, args, libs)
+
     setup_mid = timer()
 
     setup_sig, setup_name, setup_selector = (
         setup_info.sig,
         setup_info.name,
         setup_info.selector,
     )
@@ -400,30 +399,31 @@
             block=deepcopy(setup_ex.block),
             #
             calldata=cd,
             callvalue=callvalue,
             caller=setup_ex.caller,
             this=setup_ex.this,
             #
+            pgm=setup_ex.code[setup_ex.this],
             pc=0,
             st=State(),
             jumpis={},
             output=None,
             symbolic=args.symbolic_storage,
             prank=Prank(),  # prank is reset after setUp()
             #
             solver=solver,
-            path=deepcopy(setup_ex.path),
+            path=setup_ex.path.copy(),
             #
-            log=deepcopy(setup_ex.log),
+            log=setup_ex.log.copy(),
             cnts=deepcopy(setup_ex.cnts),
-            sha3s=deepcopy(setup_ex.sha3s),
-            storages=deepcopy(setup_ex.storages),
-            balances=deepcopy(setup_ex.balances),
-            calls=deepcopy(setup_ex.calls),
+            sha3s=setup_ex.sha3s.copy(),
+            storages=setup_ex.storages.copy(),
+            balances=setup_ex.balances.copy(),
+            calls=setup_ex.calls.copy(),
             failed=setup_ex.failed,
             error=setup_ex.error,
         )
     )
 
     mid = timer()
 
@@ -507,15 +507,15 @@
             warn(COUNTEREXAMPLE_UNKNOWN, f"Counterexample: {result}")
 
         if args.print_failed_states:
             print(f"# {idx+1} / {len(exs)}")
             print(ex)
 
     for opcode, idx, ex in stuck:
-        print(color_warn(f"Not supported: {mnemonic(opcode)}: {ex.error}"))
+        warn(INTERNAL_ERROR, f"{mnemonic(opcode)} failed: {ex.error}")
         if args.print_blocked_states:
             print(f"# {idx+1} / {len(exs)}")
             print(ex)
 
     if bounded_loops:
         warn(
             LOOP_BOUND,
@@ -549,30 +549,34 @@
         )
     else:
         return TestResult(funsig, exitcode, num_counterexamples)
 
 
 @dataclass(frozen=True)
 class SetupAndRunSingleArgs:
-    hexcode: str
+    creation_hexcode: str
+    deployed_hexcode: str
     abi: List
     setup_info: FunctionInfo
     fun_info: FunctionInfo
     setup_args: Namespace
     args: Namespace
+    libs: Dict
 
 
 def setup_and_run_single(fn_args: SetupAndRunSingleArgs) -> List[TestResult]:
     args = fn_args.args
     try:
         setup_ex = setup(
-            fn_args.hexcode,
+            fn_args.creation_hexcode,
+            fn_args.deployed_hexcode,
             fn_args.abi,
             fn_args.setup_info,
             fn_args.setup_args,
+            fn_args.libs,
         )
     except Exception as err:
         print(
             color_warn(
                 f"Error: {fn_args.setup_info.sig} failed: {type(err).__name__}: {err}"
             )
         )
@@ -616,45 +620,51 @@
 
 @dataclass(frozen=True)
 class RunArgs:
     # signatures of test functions to run
     funsigs: List[str]
 
     # code of the current contract
-    hexcode: str
+    creation_hexcode: str
+    deployed_hexcode: str
 
     abi: List
     methodIdentifiers: Dict[str, str]
 
     args: Namespace
     contract_json: Dict
+    libs: Dict
 
 
 def run_parallel(run_args: RunArgs) -> List[TestResult]:
     args = run_args.args
-    hexcode, abi, methodIdentifiers = (
-        run_args.hexcode,
+    creation_hexcode, deployed_hexcode, abi, methodIdentifiers, libs = (
+        run_args.creation_hexcode,
+        run_args.deployed_hexcode,
         run_args.abi,
         run_args.methodIdentifiers,
+        run_args.libs,
     )
 
     setup_info = extract_setup(methodIdentifiers)
 
     fun_infos = [
         FunctionInfo(funsig.split("(")[0], funsig, methodIdentifiers[funsig])
         for funsig in run_args.funsigs
     ]
     single_run_args = [
         SetupAndRunSingleArgs(
-            hexcode,
+            creation_hexcode,
+            deployed_hexcode,
             abi,
             setup_info,
             fun_info,
             extend_args(args, parse_devdoc(setup_info.sig, run_args.contract_json)),
             extend_args(args, parse_devdoc(fun_info.sig, run_args.contract_json)),
+            libs,
         )
         for fun_info in fun_infos
     ]
 
     # dispatch to the shared process pool
     test_results = list(process_pool.map(setup_and_run_single, single_run_args))
     test_results = sum(test_results, [])  # flatten lists
@@ -666,15 +676,22 @@
     args = run_args.args
     setup_info = extract_setup(run_args.methodIdentifiers)
 
     try:
         setup_args = extend_args(
             args, parse_devdoc(setup_info.sig, run_args.contract_json)
         )
-        setup_ex = setup(run_args.hexcode, run_args.abi, setup_info, setup_args)
+        setup_ex = setup(
+            run_args.creation_hexcode,
+            run_args.deployed_hexcode,
+            run_args.abi,
+            setup_info,
+            setup_args,
+            run_args.libs,
+        )
     except Exception as err:
         print(
             color_warn(f"Error: {setup_info.sig} failed: {type(err).__name__}: {err}")
         )
         if args.debug:
             traceback.print_exc()
         return []
@@ -982,14 +999,36 @@
         elif re.match(r"^@\S", item):
             isHalmosTag = False
         elif isHalmosTag:
             result += item
     return result.strip()
 
 
+def import_libs(build_out_map: Dict, hexcode: str, linkReferences: Dict) -> Dict:
+    libs = {}
+
+    for filepath in linkReferences:
+        file_name = filepath.split("/")[-1]
+
+        for lib_name in linkReferences[filepath]:
+            (lib_json, _, _) = build_out_map[file_name][lib_name]
+            lib_hexcode = lib_json["deployedBytecode"]["object"]
+
+            # in bytes, multiply indices by 2 and offset 0x
+            placeholder_index = linkReferences[filepath][lib_name][0]["start"] * 2 + 2
+            placeholder = hexcode[placeholder_index : placeholder_index + 40]
+
+            libs[f"{filepath}:{lib_name}"] = {
+                "placeholder": placeholder,
+                "hexcode": lib_hexcode,
+            }
+
+    return libs
+
+
 @dataclass(frozen=True)
 class MainResult:
     exitcode: int
     # contract path -> list of test results
     test_results: Dict[str, List[TestResult]] = None
 
 
@@ -1069,17 +1108,26 @@
 
                 (contract_json, contract_type, natspec) = build_out_map[filename][
                     contract_name
                 ]
                 if contract_type != "contract":
                     continue
 
-                hexcode = contract_json["deployedBytecode"]["object"]
+                creation_hexcode = contract_json["bytecode"]["object"]
+                deployed_hexcode = contract_json["deployedBytecode"]["object"]
+
                 abi = contract_json["abi"]
                 methodIdentifiers = contract_json["methodIdentifiers"]
+                linkReferences = contract_json["bytecode"]["linkReferences"]
+
+                libs = (
+                    import_libs(build_out_map, creation_hexcode, linkReferences)
+                    if linkReferences
+                    else {}
+                )
 
                 funsigs = [
                     funsig
                     for funsig in methodIdentifiers
                     if funsig.startswith(args.function)
                 ]
 
@@ -1093,20 +1141,23 @@
 
                     contract_args = (
                         extend_args(args, parse_natspec(natspec)) if natspec else args
                     )
 
                     run_args = RunArgs(
                         funsigs,
-                        hexcode,
+                        creation_hexcode,
+                        deployed_hexcode,
                         abi,
                         methodIdentifiers,
                         contract_args,
                         contract_json,
+                        libs,
                     )
+
                     enable_parallel = args.test_parallel and len(funsigs) > 1
                     test_results = (
                         run_parallel(run_args)
                         if enable_parallel
                         else run_sequential(run_args)
                     )
```

### Comparing `halmos-0.1.1/src/halmos/cheatcodes.py` & `halmos-0.1.2/src/halmos/cheatcodes.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/src/halmos/parser.py` & `halmos-0.1.2/src/halmos/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,19 @@
         "--symbolic-storage",
         action="store_true",
         help="set default storage values to symbolic",
     )
     parser.add_argument(
         "--symbolic-msg-sender", action="store_true", help="set msg.sender symbolic"
     )
+    parser.add_argument(
+        "--no-test-constructor",
+        action="store_true",
+        help="do not run the constructor of test contracts",
+    )
 
     parser.add_argument(
         "--version", action="store_true", help="print the version number"
     )
 
     # debugging options
     group_debug = parser.add_argument_group("Debugging options")
```

### Comparing `halmos-0.1.1/src/halmos/sevm.py` & `halmos-0.1.2/src/halmos/sevm.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     assert_address,
     assert_uint256,
     con_addr,
     bv_value_to_bytes,
     hexify,
 )
 from .cheatcodes import halmos_cheat_code, hevm_cheat_code, console, Prank
+from .warnings import warn, UNSUPPORTED_OPCODE, LIBRARY_PLACEHOLDER
 
 Word = Any  # z3 expression (including constants)
 Byte = Any  # z3 expression (including constants)
 Bytes = Any  # z3 expression (including constants)
 Address = BitVecRef  # 160-bitvector
 
 Steps = Dict[int, Dict[str, Any]]  # execution tree
@@ -66,14 +67,16 @@
 }
 f_sdiv = Function("evm_bvsdiv", BitVecSort(256), BitVecSort(256), BitVecSort(256))
 f_smod = Function("evm_bvsrem", BitVecSort(256), BitVecSort(256), BitVecSort(256))
 f_exp = Function("evm_exp", BitVecSort(256), BitVecSort(256), BitVecSort(256))
 
 magic_address: int = 0xAAAA0000
 
+create2_magic_address: int = 0xBBBB0000
+
 new_address_offset: int = 1
 
 
 def id_str(x: Any) -> str:
     return hexify(x).replace(" ", "")
 
 
@@ -373,16 +376,16 @@
 
     def __init__(self) -> None:
         self.stack: List[Word] = []
         self.memory: List[Byte] = []
 
     def __deepcopy__(self, memo):  # -> State:
         st = State()
-        st.stack = deepcopy(self.stack)
-        st.memory = deepcopy(self.memory)
+        st.stack = self.stack.copy()
+        st.memory = self.memory.copy()
         return st
 
     def __str__(self) -> str:
         return "".join(
             [
                 f"Stack: {str(self.stack)}\n",
                 # self.str_memory(),
@@ -496,15 +499,21 @@
 
         if len(hexcode) % 2 != 0:
             raise ValueError(hexcode)
 
         if hexcode.startswith("0x"):
             hexcode = hexcode[2:]
 
-        return Contract(bytes.fromhex(hexcode))
+        if "__" in hexcode:
+            warn(LIBRARY_PLACEHOLDER, f"contract hexcode contains library placeholder")
+
+        try:
+            return Contract(bytes.fromhex(hexcode))
+        except ValueError as e:
+            raise ValueError(f"{e} (hexcode={hexcode})")
 
     def decode_instruction(self, pc: int) -> Instruction:
         opcode = int_of(self[pc])
 
         if EVM.PUSH1 <= opcode <= EVM.PUSH32:
             operand = self[pc + 1 : pc + opcode - EVM.PUSH0 + 1]
             return Instruction(opcode, pc=pc, operand=operand)
@@ -602,27 +611,28 @@
     block: Block
     # tx
     calldata: List[Byte]  # msg.data
     callvalue: Word  # msg.value
     caller: Address  # msg.sender
     this: Address  # current account address
     # vm state
+    pgm: Contract
     pc: int
     st: State  # stack and memory
     jumpis: Dict[str, Dict[bool, int]]  # for loop detection
     output: Any  # returndata
     symbolic: bool  # symbolic or concrete storage
     prank: Prank
     # path
     solver: Solver
     path: List[Any]  # path conditions
     # logs
     log: List[Tuple[List[Word], Any]]  # event logs emitted
     cnts: Dict[str, Dict[int, int]]  # opcode -> frequency; counters
-    sha3s: List[Tuple[Word, Word]]  # sha3 hashes generated
+    sha3s: Dict[Word, int]  # sha3 hashes generated
     storages: Dict[Any, Any]  # storage updates
     balances: Dict[Any, Any]  # balance updates
     calls: List[Any]  # external calls
     failed: bool
     error: str
 
     def __init__(self, **kwargs) -> None:
@@ -633,14 +643,15 @@
         self.block = kwargs["block"]
         #
         self.calldata = kwargs["calldata"]
         self.callvalue = kwargs["callvalue"]
         self.caller = kwargs["caller"]
         self.this = kwargs["this"]
         #
+        self.pgm = kwargs["pgm"]
         self.pc = kwargs["pc"]
         self.st = kwargs["st"]
         self.jumpis = kwargs["jumpis"]
         self.output = kwargs["output"]
         self.symbolic = kwargs["symbolic"]
         self.prank = kwargs["prank"]
         #
@@ -656,18 +667,18 @@
         self.failed = kwargs["failed"]
         self.error = kwargs["error"]
 
         assert_address(self.caller)
         assert_address(self.this)
 
     def current_opcode(self) -> UnionType[int, BitVecRef]:
-        return unbox_int(self.code[self.this][self.pc])
+        return unbox_int(self.pgm[self.pc])
 
     def current_instruction(self) -> Instruction:
-        return self.code[self.this].decode_instruction(self.pc)
+        return self.pgm.decode_instruction(self.pc)
 
     def str_cnts(self) -> str:
         return "".join(
             [
                 f"{x[0]}: {x[1]}\n"
                 for x in sorted(self.cnts["opcode"].items(), key=lambda x: x[0])
             ]
@@ -715,24 +726,24 @@
                     "".join(
                         map(
                             lambda x: f"- {x}\n",
                             sorted(self.storages.items(), key=lambda x: str(x[0])),
                         )
                     ),
                     f"SHA3 hashes:\n",
-                    "".join(map(lambda x: f"- {x}\n", self.sha3s)),
+                    "".join(map(lambda x: f"- {self.sha3s[x]}: {x}\n", self.sha3s)),
                     f"External calls:\n",
                     "".join(map(lambda x: f"- {x}\n", self.calls)),
                     # f"Calldata: {self.calldata}\n",
                 ]
             )
         )
 
     def next_pc(self) -> None:
-        self.pc = self.code[self.this].next_pc(self.pc)
+        self.pc = self.pgm.next_pc(self.pc)
 
     def check(self, cond: Any) -> Any:
         self.solver.push()
         self.solver.add(simplify(cond))
         result = self.solver.check()
         self.solver.pop()
         return result
@@ -906,40 +917,58 @@
             return (loc,)
         else:
             raise ValueError(loc)
 
     def sha3(self) -> None:
         loc: int = self.st.mloc()
         size: int = int_of(self.st.pop(), "symbolic SHA3 data size")
-        self.sha3_data(wload(self.st.memory, loc, size), size)
+        self.st.push(self.sha3_data(wload(self.st.memory, loc, size), size))
 
-    def sha3_data(self, data: Bytes, size: int) -> None:
+    def sha3_data(self, data: Bytes, size: int) -> Word:
         f_sha3 = Function(
             "sha3_" + str(size * 8), BitVecSort(size * 8), BitVecSort(256)
         )
-        sha3 = f_sha3(data)
-        sha3_var = BitVec(f"sha3_var_{len(self.sha3s):>02}", 256)
-        self.solver.add(sha3_var == sha3)
+        sha3_expr = f_sha3(data)
+
         # assume hash values are sufficiently smaller than the uint max
-        self.solver.add(ULE(sha3_var, con(2**256 - 2**64)))
-        self.assume_sha3_distinct(sha3_var, sha3)
-        if size == 64 or size == 32:  # for storage hashed location
-            self.st.push(sha3)
+        self.solver.add(ULE(sha3_expr, con(2**256 - 2**64)))
+
+        # assume no hash collision
+        self.assume_sha3_distinct(sha3_expr)
+
+        # handle create2 hash
+        if size == 85 and eq(extract_bytes(data, 0, 1), con(0xFF, 8)):
+            return con(create2_magic_address + self.sha3s[sha3_expr])
         else:
-            self.st.push(sha3_var)
+            return sha3_expr
 
-    def assume_sha3_distinct(self, sha3_var, sha3) -> None:
-        for v, s in self.sha3s:
-            if s.decl().name() == sha3.decl().name():  # same size
-                # self.solver.add(Implies(sha3_var == v, sha3.arg(0) == s.arg(0)))
-                self.solver.add(Implies(sha3.arg(0) != s.arg(0), sha3_var != v))
+    def assume_sha3_distinct(self, sha3_expr) -> None:
+        # skip if already exist
+        if sha3_expr in self.sha3s:
+            return
+
+        # we expect sha3_expr to be `sha3_<input-bitsize>(input_expr)`
+        sha3_decl_name = sha3_expr.decl().name()
+
+        for prev_sha3_expr in self.sha3s:
+            if prev_sha3_expr.decl().name() == sha3_decl_name:
+                # inputs have the same size: assume different inputs
+                # lead to different outputs
+                self.solver.add(
+                    Implies(
+                        sha3_expr.arg(0) != prev_sha3_expr.arg(0),
+                        sha3_expr != prev_sha3_expr,
+                    )
+                )
             else:
-                self.solver.add(sha3_var != v)
-        self.solver.add(sha3_var != con(0))
-        self.sha3s.append((sha3_var, sha3))
+                # inputs have different sizes: assume the outputs are different
+                self.solver.add(sha3_expr != prev_sha3_expr)
+
+        self.solver.add(sha3_expr != con(0))
+        self.sha3s[sha3_expr] = len(self.sha3s)
 
     def new_gas_id(self) -> int:
         self.cnts["fresh"]["gas"] += 1
         return self.cnts["fresh"]["gas"]
 
     def new_address(self) -> Address:
         self.cnts["fresh"]["address"] += 1
@@ -958,22 +987,40 @@
         if not is_concrete(x):
             return False
 
         pc: int = int_of(x)
         if pc < 0:
             raise ValueError(pc)
 
-        opcode = unbox_int(self.code[self.this][pc])
+        opcode = unbox_int(self.pgm[pc])
         return opcode == EVM.JUMPDEST
 
     def jumpi_id(self) -> str:
         return f"{self.pc}:" + ",".join(
             map(lambda x: str(x) if self.is_jumpdest(x) else "", self.st.stack)
         )
 
+    # deploy libraries and resolve library placeholders in hexcode
+    def resolve_libs(self, creation_hexcode, deployed_hexcode, lib_references) -> str:
+        if lib_references:
+            for lib in lib_references:
+                address = self.new_address()
+
+                self.code[address] = Contract.from_hexcode(
+                    lib_references[lib]["hexcode"]
+                )
+
+                placeholder = lib_references[lib]["placeholder"]
+                hex_address = hex(address.as_long())[2:].zfill(40)
+
+                creation_hexcode = creation_hexcode.replace(placeholder, hex_address)
+                deployed_hexcode = deployed_hexcode.replace(placeholder, hex_address)
+
+        return (creation_hexcode, deployed_hexcode)
+
 
 #             x  == b   if sort(x) = bool
 # int_to_bool(x) == b   if sort(x) = int
 def test(x: Word, b: bool) -> Word:
     if is_bool(x):
         if b:
             return x
@@ -1239,15 +1286,15 @@
         out: List[Exec],
         bounded_loops: List[str],
     ) -> None:
         gas = ex.st.pop()
 
         to = uint160(ex.st.pop())
 
-        if op == EVM.STATICCALL:
+        if op == EVM.STATICCALL or op == EVM.DELEGATECALL:
             fund = con(0)
         else:
             fund = ex.st.pop()
         arg_loc: int = ex.st.mloc()
         # size (in bytes)
         arg_size: int = int_of(ex.st.pop(), "symbolic CALL input data size")
         ret_loc: int = ex.st.mloc()
@@ -1259,18 +1306,19 @@
         if not ret_size >= 0:
             raise ValueError(ret_size)
 
         caller = ex.prank.lookup(ex.this, to)
 
         orig_code = ex.code.copy()
         orig_storage = deepcopy(ex.storage)
-        orig_balance = deepcopy(ex.balance)
-        orig_log = deepcopy(ex.log)
+        orig_balance = ex.balance
+        orig_log = ex.log.copy()
 
-        if not (is_bv_value(fund) and fund.as_long() == 0):
+        if op == EVM.CALL and not (is_bv_value(fund) and fund.as_long() == 0):
+            # no balance update for CALLCODE which transfers to itself
             ex.balance_update(
                 caller, self.arith(ex, EVM.SUB, ex.balance_of(caller), fund)
             )
             ex.balance_update(to, self.arith(ex, EVM.ADD, ex.balance_of(to), fund))
 
         def call_known() -> None:
             calldata = [None] * arg_size
@@ -1285,18 +1333,19 @@
                     code=ex.code,
                     storage=ex.storage,
                     balance=ex.balance,
                     #
                     block=ex.block,
                     #
                     calldata=calldata,
-                    callvalue=fund,
-                    caller=caller,
-                    this=to,
+                    callvalue=fund if op != EVM.DELEGATECALL else ex.callvalue,
+                    caller=caller if op != EVM.DELEGATECALL else ex.caller,
+                    this=to if op in [EVM.CALL, EVM.STATICCALL] else ex.this,
                     #
+                    pgm=ex.code[to],
                     pc=0,
                     st=State(),
                     jumpis={},
                     output=None,
                     symbolic=ex.symbolic,
                     prank=Prank(),
                     #
@@ -1323,20 +1372,21 @@
                 # restore tx msg
                 new_ex.calldata = ex.calldata
                 new_ex.callvalue = ex.callvalue
                 new_ex.caller = ex.caller
                 new_ex.this = ex.this
 
                 # restore vm state
+                new_ex.pgm = ex.pgm
                 new_ex.pc = ex.pc
                 new_ex.st = deepcopy(ex.st)
                 new_ex.jumpis = deepcopy(ex.jumpis)
                 # new_ex.output is passed into the caller
                 new_ex.symbolic = ex.symbolic
-                new_ex.prank = ex.prank
+                new_ex.prank = deepcopy(ex.prank)
 
                 # set return data (in memory)
                 actual_ret_size = new_ex.returndatasize()
                 wstore_partial(
                     new_ex.st.memory,
                     ret_loc,
                     0,
@@ -1711,40 +1761,58 @@
             call_known()
         else:
             call_unknown()
 
     def create(
         self,
         ex: Exec,
+        op: int,
         stack: List[Tuple[Exec, int]],
         step_id: int,
         out: List[Exec],
         bounded_loops: List[str],
     ) -> None:
         value: Word = ex.st.pop()
         loc: int = int_of(ex.st.pop(), "symbolic CREATE offset")
         size: int = int_of(ex.st.pop(), "symbolic CREATE size")
 
+        if op == EVM.CREATE2:
+            salt = ex.st.pop()
+
+        # lookup prank
+        caller = ex.prank.lookup(ex.this, con_addr(0))
+
         # contract creation code
         create_hexcode = wload(ex.st.memory, loc, size, prefer_concrete=True)
         create_code = Contract(create_hexcode)
 
         # new account address
-        new_addr = ex.new_address()
+        if op == EVM.CREATE:
+            new_addr = ex.new_address()
+        else:  # EVM.CREATE2
+            if isinstance(create_hexcode, bytes):
+                create_hexcode = con(
+                    int.from_bytes(create_hexcode, "big"), len(create_hexcode) * 8
+                )
+            code_hash = ex.sha3_data(create_hexcode, create_hexcode.size() // 8)
+            hash_data = simplify(Concat(con(0xFF, 8), caller, salt, code_hash))
+            new_addr = uint160(ex.sha3_data(hash_data, 85))
+
+        if new_addr in ex.code:
+            ex.error = f"existing address: {hexify(new_addr)}"
+            out.append(ex)
+            return
 
         for addr in ex.code:
             ex.solver.add(new_addr != addr)  # ensure new address is fresh
 
         # setup new account
-        ex.code[new_addr] = create_code  # existing code must be empty
+        ex.code[new_addr] = Contract(b"")  # existing code must be empty
         ex.storage[new_addr] = {}  # existing storage may not be empty and reset here
 
-        # lookup prank
-        caller = ex.prank.lookup(ex.this, new_addr)
-
         # transfer value
         # assume balance is enough; otherwise ignore this path
         ex.solver.add(UGE(ex.balance_of(caller), value))
         if not (is_bv_value(value) and value.as_long() == 0):
             ex.balance_update(
                 caller, self.arith(ex, EVM.SUB, ex.balance_of(caller), value)
             )
@@ -1762,14 +1830,15 @@
                 block=ex.block,
                 #
                 calldata=[],
                 callvalue=value,
                 caller=caller,
                 this=new_addr,
                 #
+                pgm=create_code,
                 pc=0,
                 st=State(),
                 jumpis={},
                 output=None,
                 symbolic=False,
                 prank=Prank(),
                 #
@@ -1803,20 +1872,21 @@
                 # restore tx msg
                 new_ex.calldata = ex.calldata
                 new_ex.callvalue = ex.callvalue
                 new_ex.caller = ex.caller
                 new_ex.this = ex.this
 
                 # restore vm state
+                new_ex.pgm = ex.pgm
                 new_ex.pc = ex.pc
                 new_ex.st = deepcopy(ex.st)
                 new_ex.jumpis = deepcopy(ex.jumpis)
                 new_ex.output = None  # output is reset, not restored
                 new_ex.symbolic = ex.symbolic
-                new_ex.prank = ex.prank
+                new_ex.prank = deepcopy(ex.prank)
 
                 # push new address to stack
                 new_ex.st.push(uint256(new_addr))
 
                 # add to worklist
                 new_ex.next_pc()
                 stack.append((new_ex, step_id))
@@ -1901,59 +1971,60 @@
         # if dst is concrete, just jump
         if is_concrete(dst):
             ex.pc = int_of(dst)
             stack.append((ex, step_id))
 
         # otherwise, create a new execution for feasible targets
         elif self.options["sym_jump"]:
-            for target in ex.code[ex.this].valid_jump_destinations():
+            for target in ex.pgm.valid_jump_destinations():
                 target_reachable = simplify(dst == target)
                 if ex.check(target_reachable) != unsat:  # jump
                     if self.options.get("debug"):
                         print(f"We can jump to {target} with model {ex.solver.model()}")
                     new_ex = self.create_branch(ex, target_reachable, target)
                     stack.append((new_ex, step_id))
         else:
             raise NotConcreteError(f"symbolic JUMP target: {dst}")
 
     def create_branch(self, ex: Exec, cond: BitVecRef, target: int) -> Exec:
         new_solver = SolverFor("QF_AUFBV")
         new_solver.set(timeout=self.options["timeout"])
         new_solver.add(ex.solver.assertions())
         new_solver.add(cond)
-        new_path = deepcopy(ex.path)
+        new_path = ex.path.copy()
         new_path.append(str(cond))
         new_ex = Exec(
             code=ex.code.copy(),  # shallow copy for potential new contract creation; existing code doesn't change
             storage=deepcopy(ex.storage),
-            balance=deepcopy(ex.balance),
+            balance=ex.balance,
             #
             block=deepcopy(ex.block),
             #
             calldata=ex.calldata,
             callvalue=ex.callvalue,
             caller=ex.caller,
             this=ex.this,
             #
+            pgm=ex.pgm,
             pc=target,
             st=deepcopy(ex.st),
             jumpis=deepcopy(ex.jumpis),
-            output=deepcopy(ex.output),
+            output=ex.output,
             symbolic=ex.symbolic,
             prank=deepcopy(ex.prank),
             #
             solver=new_solver,
             path=new_path,
             #
-            log=deepcopy(ex.log),
+            log=ex.log.copy(),
             cnts=deepcopy(ex.cnts),
-            sha3s=deepcopy(ex.sha3s),
-            storages=deepcopy(ex.storages),
-            balances=deepcopy(ex.balances),
-            calls=deepcopy(ex.calls),
+            sha3s=ex.sha3s.copy(),
+            storages=ex.storages.copy(),
+            balances=ex.balances.copy(),
+            calls=ex.calls.copy(),
             failed=ex.failed,
             error=ex.error,
         )
         return new_ex
 
     def sym_byte_of(self, idx: BitVecRef, w: BitVecRef) -> BitVecRef:
         """generate symbolic BYTE opcode result using 32 nested ite"""
@@ -2152,15 +2223,15 @@
                             or address == halmos_cheat_code.address
                         ):
                             ex.solver.add(codesize > 0)
                     ex.st.push(codesize)
                 elif opcode == EVM.EXTCODEHASH:
                     ex.st.push(f_extcodehash(ex.st.pop()))
                 elif opcode == EVM.CODESIZE:
-                    ex.st.push(con(len(ex.code[ex.this])))
+                    ex.st.push(con(len(ex.pgm)))
                 elif opcode == EVM.GAS:
                     ex.st.push(f_gas(con(ex.new_gas_id())))
                 elif opcode == EVM.GASPRICE:
                     ex.st.push(f_gasprice())
 
                 elif opcode == EVM.BASEFEE:
                     ex.st.push(ex.block.basefee)
@@ -2184,23 +2255,28 @@
                     ex.st.push(f_blockhash(ex.st.pop()))
 
                 elif opcode == EVM.BALANCE:
                     ex.st.push(ex.balance_of(uint160(ex.st.pop())))
                 elif opcode == EVM.SELFBALANCE:
                     ex.st.push(ex.balance_of(ex.this))
 
-                elif opcode == EVM.CALL or opcode == EVM.STATICCALL:
+                elif opcode in [
+                    EVM.CALL,
+                    EVM.CALLCODE,
+                    EVM.DELEGATECALL,
+                    EVM.STATICCALL,
+                ]:
                     self.call(ex, opcode, stack, step_id, out, bounded_loops)
                     continue
 
                 elif opcode == EVM.SHA3:
                     ex.sha3()
 
-                elif opcode == EVM.CREATE:
-                    self.create(ex, stack, step_id, out, bounded_loops)
+                elif opcode in [EVM.CREATE, EVM.CREATE2]:
+                    self.create(ex, opcode, stack, step_id, out, bounded_loops)
                     continue
 
                 elif opcode == EVM.POP:
                     ex.st.pop()
                 elif opcode == EVM.MLOAD:
                     ex.st.mload()
                 elif opcode == EVM.MSTORE:
@@ -2266,15 +2342,15 @@
                 elif opcode == EVM.CODECOPY:
                     loc: int = ex.st.mloc()
                     offset: int = int_of(ex.st.pop(), "symbolic CODECOPY offset")
                     # size (in bytes)
                     size: int = int_of(ex.st.pop(), "symbolic CODECOPY size")
                     wextend(ex.st.memory, loc, size)
 
-                    codeslice = ex.code[ex.this][offset : offset + size]
+                    codeslice = ex.pgm[offset : offset + size]
                     ex.st.memory[loc : loc + size] = iter_bytes(codeslice)
 
                 elif opcode == EVM.BYTE:
                     idx = ex.st.pop()
                     w = ex.st.pop()
                     if is_bv_value(idx):
                         idx = idx.as_long()
@@ -2311,28 +2387,32 @@
                     ex.st.push(con(0))
 
                 elif EVM.PUSH1 <= opcode <= EVM.PUSH32:
                     if is_concrete(insn.operand):
                         val = int_of(insn.operand)
                         if opcode == EVM.PUSH32 and val in sha3_inv:
                             # restore precomputed hashes
-                            ex.sha3_data(con(sha3_inv[val]), 32)
+                            ex.st.push(ex.sha3_data(con(sha3_inv[val]), 32))
                         else:
                             ex.st.push(con(val))
                     else:
                         if opcode == EVM.PUSH32:
                             ex.st.push(insn.operand)
                         else:
                             ex.st.push(ZeroExt((EVM.PUSH32 - opcode) * 8, insn.operand))
                 elif EVM.DUP1 <= opcode <= EVM.DUP16:
                     ex.st.dup(opcode - EVM.DUP1 + 1)
                 elif EVM.SWAP1 <= opcode <= EVM.SWAP16:
                     ex.st.swap(opcode - EVM.SWAP1 + 1)
 
                 else:
+                    warn(
+                        UNSUPPORTED_OPCODE,
+                        f"Unsupported opcode {hex(opcode)} ({str_opcode.get(opcode, '?')})",
+                    )
                     out.append(ex)
                     continue
 
                 ex.next_pc()
                 stack.append((ex, step_id))
 
             except NotConcreteError as err:
@@ -2357,14 +2437,15 @@
         block,
         #
         calldata,
         callvalue,
         caller,
         this,
         #
+        pgm,
         # pc,
         # st,
         # jumpis,
         # output,
         symbolic,
         # prank,
         #
@@ -2388,26 +2469,27 @@
             block=block,
             #
             calldata=calldata,
             callvalue=callvalue,
             caller=caller,
             this=this,
             #
+            pgm=pgm,
             pc=0,
             st=State(),
             jumpis={},
             output=None,
             symbolic=symbolic,
             prank=Prank(),
             #
             solver=solver,
             path=[],
             #
             log=[],
             cnts=defaultdict(lambda: defaultdict(int)),
-            sha3s=[],
+            sha3s={},
             storages={},
             balances={},
             calls=[],
             failed=False,
             error="",
         )
```

### Comparing `halmos-0.1.1/src/halmos/utils.py` & `halmos-0.1.2/src/halmos/utils.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/src/halmos/warnings.py` & `halmos-0.1.2/src/halmos/warnings.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,13 +16,16 @@
 
     def url(self) -> str:
         return f"{WARNINGS_BASE_URL}#{self.code}"
 
 
 COUNTEREXAMPLE_INVALID = ErrorCode("counterexample-invalid")
 COUNTEREXAMPLE_UNKNOWN = ErrorCode("counterexample-unknown")
+INTERNAL_ERROR = ErrorCode("internal-error")
+UNSUPPORTED_OPCODE = ErrorCode("unsupported-opcode")
+LIBRARY_PLACEHOLDER = ErrorCode("library-placeholder")
 
 LOOP_BOUND = ErrorCode("loop-bound")
 
 
 def warn(error_code: ErrorCode, msg: str):
     logger.warning(f"{color_warn(msg)}\n(see {error_code.url()})")
```

### Comparing `halmos-0.1.1/src/halmos.egg-info/PKG-INFO` & `halmos-0.1.2/src/halmos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: halmos
-Version: 0.1.1
+Version: 0.1.2
 Summary: Halmos: Symbolic Bounded Model Checker for Ethereum Smart Contracts Bytecode
 Author: a16z crypto
-Maintainer: Daejun Park
-Maintainer-email: karmacoma <karma@coma.lol>
+Maintainer: Daejun Park, karmacoma <karma@coma.lol>
 Project-URL: Homepage, https://github.com/a16z/halmos
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -83,15 +82,15 @@
 ```
 $ forge test
 [PASS] testTotalPriceBuggy(uint96,uint32) (runs: 256, μ: 462, ~: 466)
 ```
 
 Once it passes, you can also perform **symbolic testing** to verify the same properties for **all possible inputs** (up to a specified limit):
 ```
-$ halmos
+$ halmos --function test
 [FAIL] testTotalPriceBuggy(uint96,uint32) (paths: 6, time: 0.10s, bounds: [])
 Counterexample: [p_price_uint96 = 39614081294025656978550816768, p_quantity_uint32 = 1073741824]
 ```
 
 _(In this specific example, Halmos discovered an input that violated the assertion, which was missed by the fuzzer!)_
 
 ## Develop
```

### Comparing `halmos-0.1.1/src/halmos.egg-info/SOURCES.txt` & `halmos-0.1.2/src/halmos.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .github/workflows/black.yml
 .github/workflows/codeql.yml
 .github/workflows/publish.yml
 .github/workflows/test-external.yml
 .github/workflows/test-long.yml
 .github/workflows/test.yml
 benchmarks/baolean.sh
+docs/getting-started.md
 examples/README.md
 examples/tokens/ERC20/foundry.toml
 examples/tokens/ERC20/remappings.txt
 examples/tokens/ERC20/src/OpenZeppelinERC20.sol
 examples/tokens/ERC20/src/SolmateERC20.sol
 examples/tokens/ERC20/test/DEIStablecoin.sol
 examples/tokens/ERC20/test/DEIStablecoin.t.sol
@@ -34,14 +35,15 @@
 examples/tokens/ERC721/test/OpenZeppelinERC721.t.sol
 examples/tokens/ERC721/test/SolmateERC721.t.sol
 examples/toy/foundry.toml
 examples/toy/src/Example.sol
 examples/toy/test/Example.t.sol
 src/halmos/__init__.py
 src/halmos/__main__.py
+src/halmos/calldata.py
 src/halmos/cheatcodes.py
 src/halmos/parser.py
 src/halmos/pools.py
 src/halmos/sevm.py
 src/halmos/utils.py
 src/halmos/warnings.py
 src/halmos.egg-info/PKG-INFO
@@ -66,18 +68,21 @@
 tests/src/List.sol
 tests/src/SignExtend.sol
 tests/src/Storage.sol
 tests/test/Arith.t.sol
 tests/test/AssertTest.sol
 tests/test/Block.t.sol
 tests/test/Byte.t.sol
+tests/test/Call.t.sol
 tests/test/Console.t.sol
 tests/test/Const.t.sol
+tests/test/Constructor.t.sol
 tests/test/Counter.t.sol
 tests/test/Create.t.sol
+tests/test/Create2.t.sol
 tests/test/Deal.t.sol
 tests/test/Foundry.t.sol
 tests/test/Getter.t.sol
 tests/test/HalmosCheatCode.t.sol
 tests/test/Invalid.t.sol
 tests/test/Library.t.sol
 tests/test/LibraryLinking.t.sol
```

### Comparing `halmos-0.1.1/tests/expected/all.json` & `halmos-0.1.2/tests/expected/all.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9762840670859538%*

 * *Differences: {"'test_results'": "{'test/LibraryLinking.t.sol:LibTest': [OrderedDict([('name', 'check_foo()'), "*

 * *                   "('exitcode', 0), ('num_models', 0), ('num_paths', None), ('time', None), "*

 * *                   "('num_bounded_loops', None)])], 'test/Proxy.t.sol:ProxyTest': {0: {'name': "*

 * *                   "'check_foo(uint256,uint256,address)', 'exitcode': 0}}, "*

 * *                   "'test/Struct.t.sol:StructTest': {0: {'exitcode': 1, 'num_models': 1}, insert: "*

 * *                   "[(1, OrderedDict([('name […]*

```diff
@@ -103,14 +103,48 @@
                 "name": "check_SymbolicByteIndex(uint8,uint8)",
                 "num_bounded_loops": null,
                 "num_models": 2,
                 "num_paths": null,
                 "time": null
             }
         ],
+        "test/Call.t.sol:CallTest": [
+            {
+                "exitcode": 0,
+                "name": "check_call(uint256,uint256)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_callcode(uint256,uint256)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_delegatecall(uint256,uint256)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_staticcall(uint256,uint256)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            }
+        ],
         "test/Console.t.sol:ConsoleTest": [
             {
                 "exitcode": 0,
                 "name": "check_log()",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
@@ -133,14 +167,32 @@
                 "name": "check_Const()",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
+        "test/Constructor.t.sol:ConstructorTest": [
+            {
+                "exitcode": 0,
+                "name": "check_constructor()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_setCodesize()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            }
+        ],
         "test/Counter.t.sol:CounterTest": [
             {
                 "exitcode": 0,
                 "name": "check_div_1(uint256,uint256)",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
@@ -289,14 +341,72 @@
                 "name": "check_set(uint256)",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
+        "test/Create2.t.sol:Create2Test": [
+            {
+                "exitcode": 0,
+                "name": "check_create2(uint256,uint256,bytes32)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_create2_caller(address,uint256,uint256,bytes32)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 1,
+                "name": "check_create2_collision(uint256,uint256,bytes32)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 1,
+                "name": "check_create2_collision_alias(uint256,uint256,bytes32)",
+                "num_bounded_loops": null,
+                "num_models": 1,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_create2_concrete()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_create2_no_collision_1(uint256,uint256,bytes32,bytes32)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 0,
+                "name": "check_create2_no_collision_2(uint256,uint256,bytes32)",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            }
+        ],
         "test/Deal.t.sol:DealTest": [
             {
                 "exitcode": 0,
                 "name": "check_deal_1(address,uint256)",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
@@ -453,15 +563,24 @@
                 "name": "check_add(uint256,uint256)",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
-        "test/LibraryLinking.t.sol:LibTest": [],
+        "test/LibraryLinking.t.sol:LibTest": [
+            {
+                "exitcode": 0,
+                "name": "check_foo()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            }
+        ],
         "test/LibraryLinking.t.sol:LibTest2": [
             {
                 "exitcode": 0,
                 "name": "check_bar()",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
@@ -768,16 +887,16 @@
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
         "test/Proxy.t.sol:ProxyTest": [
             {
-                "exitcode": 1,
-                "name": "check_foo(uint256)",
+                "exitcode": 0,
+                "name": "check_foo(uint256,uint256,address)",
                 "num_bounded_loops": null,
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
         "test/Reset.t.sol:ResetTest": [
@@ -977,32 +1096,58 @@
                 "num_models": 0,
                 "num_paths": null,
                 "time": null
             }
         ],
         "test/Struct.t.sol:StructTest": [
             {
-                "exitcode": 2,
+                "exitcode": 1,
                 "name": "check_Struct((uint256,uint256))",
                 "num_bounded_loops": null,
-                "num_models": null,
+                "num_models": 1,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 1,
+                "name": "check_StructArray((uint256,uint256)[],(uint256,uint256)[2])",
+                "num_bounded_loops": null,
+                "num_models": 1,
+                "num_paths": null,
+                "time": null
+            },
+            {
+                "exitcode": 1,
+                "name": "check_StructArrayArray((uint256,uint256)[][],(uint256,uint256)[2][],(uint256,uint256)[][2],(uint256,uint256)[2][2])",
+                "num_bounded_loops": null,
+                "num_models": 1,
                 "num_paths": null,
                 "time": null
             }
         ],
-        "test/TestConstructor.t.sol:TestConstructorTest": [
+        "test/Struct.t.sol:StructTest2": [
             {
                 "exitcode": 1,
-                "name": "check_value()",
+                "name": "check_S((uint256,uint256[],uint256),(uint256,(uint256,uint256[],uint256),uint256[],(uint256,uint256[],uint256)[],uint256[1],(uint256,uint256[],uint256)[][])[])",
                 "num_bounded_loops": null,
                 "num_models": 1,
                 "num_paths": null,
                 "time": null
             }
         ],
+        "test/TestConstructor.t.sol:TestConstructorTest": [
+            {
+                "exitcode": 0,
+                "name": "check_value()",
+                "num_bounded_loops": null,
+                "num_models": 0,
+                "num_paths": null,
+                "time": null
+            }
+        ],
         "test/Token.t.sol:TokenTest": [
             {
                 "exitcode": 1,
                 "name": "check_BalanceInvariant()",
                 "num_bounded_loops": null,
                 "num_models": 2,
                 "num_paths": null,
```

### Comparing `halmos-0.1.1/tests/expected/erc20.json` & `halmos-0.1.2/tests/expected/erc20.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/expected/erc721.json` & `halmos-0.1.2/tests/expected/erc721.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/expected/toy.json` & `halmos-0.1.2/tests/expected/toy.json`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/src/Counter.sol` & `halmos-0.1.2/tests/src/Counter.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/src/Storage.sol` & `halmos-0.1.2/tests/src/Storage.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Arith.t.sol` & `halmos-0.1.2/tests/test/Arith.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/AssertTest.sol` & `halmos-0.1.2/tests/test/AssertTest.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Block.t.sol` & `halmos-0.1.2/tests/test/Block.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Byte.t.sol` & `halmos-0.1.2/tests/test/Byte.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Counter.t.sol` & `halmos-0.1.2/tests/test/Counter.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Create.t.sol` & `halmos-0.1.2/tests/test/Create.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Deal.t.sol` & `halmos-0.1.2/tests/test/Deal.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Foundry.t.sol` & `halmos-0.1.2/tests/test/Foundry.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/HalmosCheatCode.t.sol` & `halmos-0.1.2/tests/test/HalmosCheatCode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Invalid.t.sol` & `halmos-0.1.2/tests/test/Invalid.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Library.t.sol` & `halmos-0.1.2/tests/test/Library.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/List.t.sol` & `halmos-0.1.2/tests/test/List.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Natspec.t.sol` & `halmos-0.1.2/tests/test/Natspec.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Opcode.t.sol` & `halmos-0.1.2/tests/test/Opcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Prank.t.sol` & `halmos-0.1.2/tests/test/Prank.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Reset.t.sol` & `halmos-0.1.2/tests/test/Reset.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Revert.t.sol` & `halmos-0.1.2/tests/test/Revert.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Send.t.sol` & `halmos-0.1.2/tests/test/Send.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Setup.t.sol` & `halmos-0.1.2/tests/test/Setup.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/SetupPlus.t.sol` & `halmos-0.1.2/tests/test/SetupPlus.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Storage.t.sol` & `halmos-0.1.2/tests/test/Storage.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Store.t.sol` & `halmos-0.1.2/tests/test/Store.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Token.t.sol` & `halmos-0.1.2/tests/test/Token.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/UnsupportedOpcode.t.sol` & `halmos-0.1.2/tests/test/UnsupportedOpcode.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test/Warp.t.sol` & `halmos-0.1.2/tests/test/Warp.t.sol`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test_cli.py` & `halmos-0.1.2/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,23 +115,14 @@
 
     hexcode = "34381856FDFDFDFDFDFD5B00"
     exs = run_bytecode(hexcode, args)
     assert len(exs) == 1
     assert exs[0].current_opcode() == EVM.STOP
 
 
-def test_setup(setup_abi, setup_name, setup_sig, setup_selector, args):
-    hexcode = "600100"
-    abi = setup_abi
-    setup_ex = halmos.__main__.setup(
-        hexcode, abi, FunctionInfo(setup_name, setup_sig, setup_selector), args
-    )
-    assert setup_ex.st.stack == [1]
-
-
 def test_instruction():
     assert str(Instruction(con(0))) == "STOP"
     assert str(Instruction(con(1))) == "ADD"
     assert str(Instruction(con(EVM.PUSH32), operand=con(1))) == "PUSH32 1"
     assert str(Instruction(con(EVM.BASEFEE))) == "BASEFEE"
 
     # symbolic opcode is not supported
```

### Comparing `halmos-0.1.1/tests/test_fixtures.py` & `halmos-0.1.2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `halmos-0.1.1/tests/test_halmos.py` & `halmos-0.1.2/tests/test_halmos.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,29 +44,25 @@
     assert_eq(expected["test_results"], actual["test_results"])
 
 
 @pytest.mark.parametrize(
     "cmd",
     [
         ["--root", "tests", "--contract", "SetupFailTest"],
-        ["--root", "tests", "--contract", "LibTest"],
     ],
-    ids=(
-        "SetupFailTest",
-        "LibTest",
-    ),
+    ids=("SetupFailTest",),
 )
 def test_main_fail(cmd, halmos_options):
     actual = asdict(_main(cmd + halmos_options.split()))
     assert actual["exitcode"] != 0
 
 
 def assert_eq(m1: Dict, m2: Dict) -> int:
     assert list(m1.keys()) == list(m2.keys())
     for c in m1:
         l1 = sorted(m1[c], key=lambda x: x["name"])
         l2 = sorted(m2[c], key=lambda x: x["name"])
-        assert len(l1) == len(l2)
+        assert len(l1) == len(l2), c
         for r1, r2 in zip(l1, l2):
             assert r1["name"] == r2["name"]
-            assert r1["exitcode"] == r2["exitcode"]
-            assert r1["num_models"] == r2["num_models"]
+            assert r1["exitcode"] == r2["exitcode"], f"{c} {r1['name']}"
+            assert r1["num_models"] == r2["num_models"], f"{c} {r1['name']}"
```

### Comparing `halmos-0.1.1/tests/test_sevm.py` & `halmos-0.1.2/tests/test_sevm.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,23 +47,25 @@
 
 @pytest.fixture
 def storage():
     return {}
 
 
 def mk_ex(hexcode, sevm, solver, storage, caller, this):
+    bytecode = Contract(hexcode)
     return sevm.mk_exec(
-        code={this: Contract(hexcode)},
+        code={this: bytecode},
         storage={this: storage},
         balance=balance,
         block=mk_block(),
         calldata=[],
         callvalue=callvalue,
         caller=caller,
         this=this,
+        pgm=bytecode,
         symbolic=True,
         solver=solver,
     )
 
 
 x = BitVec("x", 256)
 y = BitVec("y", 256)
```


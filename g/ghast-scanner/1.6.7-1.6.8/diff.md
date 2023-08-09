# Comparing `tmp/ghast_scanner-1.6.7.tar.gz` & `tmp/ghast_scanner-1.6.8.tar.gz`

## Comparing `ghast_scanner-1.6.7.tar` & `ghast_scanner-1.6.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/.pylintrc
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/EXAMPLES.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/__about__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/colors.py
--rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/requirements.txt
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/setup.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/.github/workflows/ghast-scan.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-create-or-approves-pr-using-curl.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-creates-or-approves-pr-using-gh-cli.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-creates-or-approves-pr-using-gh-script.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-using-upload-artifact-action.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-remote-script.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/__init__.py
--rw-r--r--   0        0        0    17447 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/analyzer.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/analyzer_test.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/analyzer/regex.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/LICENSE
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/README.md
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/pyproject.toml
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 ghast_scanner-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/.pylintrc
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/EXAMPLES.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/__about__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/colors.py
+-rw-r--r--   0        0        0     5139 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/requirements.txt
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/setup.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/.github/workflows/ghast-scan.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-create-or-approves-pr-using-curl.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-creates-or-approves-pr-using-gh-cli.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-creates-or-approves-pr-using-gh-script.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-using-upload-artifact-action.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-remote-script.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/analyzer/__init__.py
+-rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/analyzer/analyzer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/analyzer/regex.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/LICENSE
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/README.md
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/pyproject.toml
+-rw-r--r--   0        0        0     8725 2020-02-02 00:00:00.000000 ghast_scanner-1.6.8/PKG-INFO
```

### Comparing `ghast_scanner-1.6.7/action.yml` & `ghast_scanner-1.6.8/action.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/colors.py` & `ghast_scanner-1.6.8/colors.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/main.py` & `ghast_scanner-1.6.8/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     errored = False
     failed_actions = []
     try:
         if file_:
             file_ = Path(file_)
             if file_.exists():
-                print(f"FILE: {Colors.BOLD}{file_}{Colors.END}")
+                print(f"FILE => {Colors.BOLD}{file_}{Colors.END}")
                 with file_.open("r") as action_file:
                     action_dict = safe_load(action_file)
                     if not analyzer.run_checks(action=action_dict):
                         failed_actions.append(file_)
             else:
                 errored = True
                 print(f"[{Colors.RED}ERROR{Colors.END}]: the file '{str(file_)}' does not exist...")
```

### Comparing `ghast_scanner-1.6.7/setup.py` & `ghast_scanner-1.6.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ghast-scanner',
-    version='1.5.7',
+    version='1.6.8',
     packages=find_packages(),
     install_requires=[
         'iniconfig==2.0.0',
         'packaging==23.1',
         'pluggy==1.2.0',
         'pytest==7.4.0',
         'PyYAML==6.0',
     ],
     author='Alex Rodriguez',
     author_email='arodriguez99@protonmail.com',
     description='Analyze the security posture of your GitHub Action',
     url='https://github.com/bin3xish477/ghast',
-    classifiers = [
+    classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
-)
+)
```

### Comparing `ghast_scanner-1.6.7/.github/workflows/ghast-scan.yml` & `ghast_scanner-1.6.8/.github/workflows/ghast-scan.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/actions/action-create-or-approves-pr-using-curl.yml` & `ghast_scanner-1.6.8/actions/action-create-or-approves-pr-using-curl.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `ghast_scanner-1.6.8/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/analyzer/analyzer.py` & `ghast_scanner-1.6.8/analyzer/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
                 if "uses" in step:
                     uses = step["uses"]
                     if search(analyzer.regex.ACTION_WITH_VERSION, uses):
                         if self.verbose:
                             print(
                                 f"{Colors.LIGHT_GRAY}INFO{Colors.END} step using action('{uses}') with version number instead of a SHA hash"
                             )
-                        passed = False
-                        break
+                        if passed:
+                            passed = False
         return passed
 
     def _check_for_inline_script(self) -> bool:
         passed = True
         for job in self.jobs.keys():
             steps = self.jobs[job]["steps"]
             for step in steps:
@@ -332,19 +332,19 @@
                                 passed = False
         return passed
 
     # ==================================================================
     # ======================== Auxiliary Checks ========================
     # ==================================================================
 
-    def _check_for_codeowners_file(self) -> bool:
+    def _check_for_codeowners_file(self) -> None:
         if not Path(".github/workflows/CODEOWNERS").exists():
             print(
                 f"{Colors.LIGHT_BLUE}AUXI{Colors.END} missing CODEOWNERS file"
-                "which can provide additional protections for your workflow files"
+                " which can provide additional protections for your workflow files"
             )
         else:
             if self.verbose:
                 print(f"{Colors.LIGHT_BLUE}AUXI{Colors.END} found CODEOWNERS file")
 
     def _check_for_non_github_managed_actions(self) -> bool:
         passed = True
```

### Comparing `ghast_scanner-1.6.7/analyzer/analyzer_test.py` & `ghast_scanner-1.6.8/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/analyzer/regex.py` & `ghast_scanner-1.6.8/analyzer/regex.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/.gitignore` & `ghast_scanner-1.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/LICENSE` & `ghast_scanner-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/README.md` & `ghast_scanner-1.6.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,428 +1,476 @@
 00000000: 2320 6768 6173 740a 0a3c 7020 616c 6967  # ghast..<p alig
 00000010: 6e3d 2263 656e 7465 7222 3e3c 696d 6720  n="center"><img 
-00000020: 7769 6474 683d 2237 3030 2220 616c 743d  width="700" alt=
+00000020: 7769 6474 683d 2234 3030 2220 616c 743d  width="400" alt=
 00000030: 2269 6d61 6765 2220 7372 633d 2268 7474  "image" src="htt
 00000040: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000050: 6269 6e33 7869 7368 3437 372f 6768 6173  bin3xish477/ghas
 00000060: 742f 6173 7365 7473 2f34 3432 3831 3632  t/assets/4428162
 00000070: 302f 3039 3861 3464 3536 2d34 6564 632d  0/098a4d56-4edc-
 00000080: 3465 3230 2d62 3436 332d 3932 3363 3862  4e20-b463-923c8b
-00000090: 6166 3034 3138 223e 3c2f 703e 0a0a 4748  af0418"></p>..GH
-000000a0: 4153 5420 2847 6974 4875 6220 4163 7469  AST (GitHub Acti
+00000090: 6166 3034 3138 223e 3c2f 703e 0a0a 4768  af0418"></p>..Gh
+000000a0: 6173 7420 2847 6974 4875 6220 4163 7469  ast (GitHub Acti
 000000b0: 6f6e 7320 5374 6174 6963 2041 6e61 6c79  ons Static Analy
 000000c0: 7369 7320 546f 6f6c 2920 6973 2061 2074  sis Tool) is a t
 000000d0: 6f6f 6c20 746f 2061 6e61 6c79 7a65 2074  ool to analyze t
 000000e0: 6865 2073 6563 7572 6974 7920 706f 7374  he security post
 000000f0: 7572 6520 6f66 2079 6f75 7220 4769 7448  ure of your GitH
 00000100: 7562 2041 6374 696f 6e73 2061 6e64 2069  ub Actions and i
-00000110: 7473 2073 7572 726f 6e64 696e 6720 656e  ts surronding en
-00000120: 7669 726f 6e6d 656e 7420 666f 7220 636f  vironment for co
-00000130: 6d6d 6f6e 2073 6563 7572 6974 7920 7675  mmon security vu
-00000140: 6c6e 6572 6162 696c 6974 6965 7320 6f72  lnerabilities or
-00000150: 206d 6973 7369 6e67 2073 6563 7572 6974   missing securit
-00000160: 7920 636f 6e66 6967 7572 6174 696f 6e2e  y configuration.
-00000170: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-00000180: 6572 223e 3c69 6d67 2077 6964 7468 3d22  er"><img width="
-00000190: 3933 3622 2061 6c74 3d22 696d 6167 6522  936" alt="image"
-000001a0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-000001b0: 7468 7562 2e63 6f6d 2f62 696e 3378 6973  thub.com/bin3xis
-000001c0: 6834 3737 2f67 6861 7374 2f61 7373 6574  h477/ghast/asset
-000001d0: 732f 3434 3238 3136 3230 2f37 3231 3433  s/44281620/72143
-000001e0: 3263 612d 3739 3434 2d34 3062 342d 3830  2ca-7944-40b4-80
-000001f0: 3364 2d38 6333 6362 3836 3639 3936 6522  3d-8c3cb866996e"
-00000200: 3e3c 2f70 3e0a 0a0a 2323 2320 496e 7374  ></p>...### Inst
-00000210: 616c 6c61 7469 6f6e 0a0a 3e20 4d61 6b65  allation..> Make
-00000220: 2073 7572 6520 796f 7520 6861 7665 2060   sure you have `
-00000230: 2448 4f4d 452f 2e6c 6f63 616c 2f62 696e  $HOME/.local/bin
-00000240: 6020 696e 2079 6f75 7220 5041 5448 0a0a  ` in your PATH..
-00000250: 6060 600a 7079 7468 6f6e 3320 2d6d 2070  ```.python3 -m p
-00000260: 6970 2069 6e73 7461 6c6c 202e 0a60 6060  ip install ..```
-00000270: 0a0a 2323 2320 5573 6167 650a 0a60 6060  ..### Usage..```
-00000280: 0a67 6861 7374 202d 2d66 696c 6520 6163  .ghast --file ac
-00000290: 7469 6f6e 2e79 6d6c 0a67 6861 7374 202d  tion.yml.ghast -
-000002a0: 6420 6469 7265 6374 6f72 792d 7769 7468  d directory-with
-000002b0: 2d61 6374 696f 6e73 2f20 2d2d 7665 7262  -actions/ --verb
-000002c0: 6f73 650a 6768 6173 7420 2d2d 6669 6c65  ose.ghast --file
-000002d0: 2061 6374 696f 6e2e 796d 6c20 2d2d 6967   action.yml --ig
-000002e0: 6e6f 7265 2d77 6172 6e69 6e67 730a 6768  nore-warnings.gh
-000002f0: 6173 7420 2d2d 6c69 7374 2d63 6865 636b  ast --list-check
-00000300: 730a 6768 6173 7420 2d69 2063 6865 636b  s.ghast -i check
-00000310: 5f66 6f72 5f69 6e6c 696e 655f 7363 7269  _for_inline_scri
-00000320: 7074 202d 2d6e 6f2d 7375 6d6d 6172 790a  pt --no-summary.
-00000330: 6060 600a 0a23 2323 2055 7365 2060 6768  ```..### Use `gh
-00000340: 6173 7460 2069 6e20 596f 7572 2047 6974  ast` in Your Git
-00000350: 4875 6220 576f 726b 666c 6f77 730a 0a23  Hub Workflows..#
-00000360: 2323 2320 4465 6661 756c 7420 576f 726b  ### Default Work
-00000370: 666c 6f77 0a0a 6060 6079 616d 6c0a 6e61  flow..```yaml.na
-00000380: 6d65 3a20 2752 756e 4768 6173 7427 0a6f  me: 'RunGhast'.o
-00000390: 6e3a 0a20 2070 7573 683a 0a6a 6f62 733a  n:.  push:.jobs:
-000003a0: 0a20 2052 756e 4768 6173 743a 0a20 2020  .  RunGhast:.   
-000003b0: 2072 756e 732d 6f6e 3a20 7562 756e 7475   runs-on: ubuntu
-000003c0: 2d6c 6174 6573 740a 2020 2020 7374 6570  -latest.    step
-000003d0: 733a 0a20 2020 202d 206e 616d 653a 2022  s:.    - name: "
-000003e0: 4368 6563 6b6f 7574 2072 6570 6f22 0a20  Checkout repo". 
-000003f0: 2020 2020 2075 7365 733a 2061 6374 696f       uses: actio
-00000400: 6e73 2f63 6865 636b 6f75 7440 3936 6635  ns/checkout@96f5
-00000410: 3331 3030 6261 3261 3534 3439 6562 3731  3100ba2a5449eb71
-00000420: 6432 6536 3630 3462 6263 6439 3462 3934  d2e6604bbcd94b94
-00000430: 3439 6235 2023 2076 332e 352e 330a 2020  49b5 # v3.5.3.  
-00000440: 2020 2d20 6e61 6d65 3a20 2252 756e 2047    - name: "Run G
-00000450: 6861 7374 220a 2020 2020 2020 7573 6573  hast".      uses
-00000460: 3a20 2262 696e 3378 6973 6834 3737 2f67  : "bin3xish477/g
-00000470: 6861 7374 4034 3363 3437 3162 3865 3035  hast@43c471b8e05
-00000480: 3539 3964 3637 6636 3138 6563 6363 6663  599d67f618ecccfc
-00000490: 3864 3762 3932 3831 6266 6439 6222 0a60  8d7b9281bfd9b".`
-000004a0: 6060 0a0a 2323 2320 5365 6520 4164 6469  ``..### See Addi
-000004b0: 7469 6f6e 616c 2057 6f72 6b66 6c6f 7720  tional Workflow 
-000004c0: 4578 616d 706c 6573 0a5b 4164 6469 7469  Examples.[Additi
-000004d0: 6f6e 616c 2047 6861 7374 2057 6f72 6b66  onal Ghast Workf
-000004e0: 6c6f 7720 4578 616d 706c 6573 5d28 4558  low Examples](EX
-000004f0: 414d 504c 4553 2e6d 6429 0a0a 2323 2320  AMPLES.md)..### 
-00000500: 4368 6563 6b73 2050 6572 666f 726d 6564  Checks Performed
-00000510: 2062 7920 6067 6861 7374 600a 0a31 2e20   by `ghast`..1. 
-00000520: 4e61 6d65 3a20 6063 6865 636b 5f66 6f72  Name: `check_for
-00000530: 5f33 705f 6163 7469 6f6e 735f 7769 7468  _3p_actions_with
-00000540: 6f75 745f 6861 7368 602c 204c 6576 656c  out_hash`, Level
-00000550: 3a20 6046 4149 4c60 0a0a 2020 2020 2d20  : `FAIL`..    - 
-00000560: 5468 6973 2063 6865 636b 2069 6465 6e74  This check ident
-00000570: 6966 6965 7320 616e 7920 7468 6972 6420  ifies any third 
-00000580: 7061 7274 7920 4769 7448 7562 2041 6374  party GitHub Act
-00000590: 696f 6e73 2069 6e20 7573 6520 7468 6174  ions in use that
-000005a0: 2068 6176 6520 6265 656e 2072 6566 6572   have been refer
-000005b0: 656e 6365 6420 7669 6120 6120 7665 7273  enced via a vers
-000005c0: 696f 6e20 6e75 6d62 6572 2073 7563 6820  ion number such 
-000005d0: 6173 2060 7631 2e31 6020 696e 7374 6561  as `v1.1` instea
-000005e0: 6420 6f66 2063 6f6d 6d69 7420 5348 4120  d of commit SHA 
-000005f0: 6861 6168 2e20 5573 696e 6720 6120 6861  haah. Using a ha
-00000600: 7368 2063 616e 2068 656c 7020 6d69 7469  sh can help miti
-00000610: 6761 7465 2073 7570 706c 7920 6368 6169  gate supply chai
-00000620: 6e20 7468 7265 6174 7320 696e 2061 2073  n threats in a s
-00000630: 6365 6e61 7269 6f20 7768 6572 6520 6120  cenario where a 
-00000640: 7468 7265 6174 2061 6374 6f72 2068 6173  threat actor has
-00000650: 2063 6f6d 7072 6f6d 6973 6564 2074 6865   compromised the
-00000660: 2073 6f75 7263 6520 7265 706f 7369 746f   source reposito
-00000670: 7279 2077 6865 7265 2074 6865 2033 5020  ry where the 3P 
-00000680: 6163 7469 6f6e 206c 6976 6573 2e0a 0a32  action lives...2
-00000690: 2e20 4e61 6d65 3a20 6063 6865 636b 5f66  . Name: `check_f
-000006a0: 6f72 5f61 6c6c 6f77 5f75 6e73 6563 7572  or_allow_unsecur
-000006b0: 655f 636f 6d6d 616e 6473 602c 204c 6576  e_commands`, Lev
-000006c0: 656c 3a20 6046 4149 4c60 0a0a 2020 2020  el: `FAIL`..    
-000006d0: 2d20 5468 6973 2063 6865 636b 206c 6f6f  - This check loo
-000006e0: 6b73 2066 6f72 2074 6865 2075 7361 6765  ks for the usage
-000006f0: 206f 6620 656e 7669 726f 6e6d 656e 7420   of environment 
-00000700: 7661 7269 6162 6c65 2063 616c 6c65 6420  variable called 
-00000710: 6041 4354 494f 4e53 5f41 4c4c 4f57 5f55  `ACTIONS_ALLOW_U
-00000720: 4e53 4543 5552 455f 434f 4d4d 414e 4453  NSECURE_COMMANDS
-00000730: 6020 7768 6963 6820 616c 6c6f 7773 2066  ` which allows f
-00000740: 6f72 2061 6e20 4163 7469 6f6e 2074 6f20  or an Action to 
-00000750: 6765 7420 6163 6365 7373 2074 6f20 6461  get access to da
-00000760: 6e67 6572 6f75 7320 636f 6d6d 616e 6473  ngerous commands
-00000770: 2028 6067 6574 2d65 6e76 602c 2060 6164   (`get-env`, `ad
-00000780: 642d 7061 7468 6029 2077 6869 6368 2063  d-path`) which c
-00000790: 616e 206c 6561 6420 746f 2063 6f64 6520  an lead to code 
-000007a0: 696e 6a65 6374 696f 6e20 616e 6420 6372  injection and cr
-000007b0: 6564 656e 7469 616c 2074 6865 6674 7320  edential thefts 
-000007c0: 6f70 706f 7274 756e 6974 6965 732e 0a0a  opportunities...
-000007d0: 332e 204e 616d 653a 2060 6368 6563 6b5f  3. Name: `check_
-000007e0: 666f 725f 6361 6368 655f 6163 7469 6f6e  for_cache_action
-000007f0: 602c 204c 6576 656c 3a20 6057 4152 4e60  `, Level: `WARN`
-00000800: 0a0a 2020 2020 2d20 5468 6973 2063 6865  ..    - This che
-00000810: 636b 2066 696e 6473 2061 6e79 2075 7361  ck finds any usa
-00000820: 6765 206f 6620 4769 7448 7562 2773 2063  ge of GitHub's c
-00000830: 6163 6869 6e67 2041 6374 696f 6e20 2860  aching Action (`
-00000840: 6163 7469 6f6e 732f 6361 6368 6560 2920  actions/cache`) 
-00000850: 7768 6963 6820 6d61 7920 7265 7375 6c74  which may result
-00000860: 2069 6e20 7365 6e73 6974 6976 6520 696e   in sensitive in
-00000870: 666f 726d 6174 696f 6e20 6469 7363 6c6f  formation disclo
-00000880: 7375 7265 206f 7220 6361 6368 6520 706f  sure or cache po
-00000890: 6973 6f6e 696e 672e 0a0a 342e 204e 616d  isoning...4. Nam
-000008a0: 653a 2060 6368 6563 6b5f 666f 725f 6461  e: `check_for_da
-000008b0: 6e67 6572 6f75 735f 7772 6974 655f 7065  ngerous_write_pe
-000008c0: 726d 6973 7369 6f6e 7360 2c20 4c65 7665  rmissions`, Leve
-000008d0: 6c3a 2060 4641 494c 600a 0a20 2020 202d  l: `FAIL`..    -
-000008e0: 2054 6869 7320 6368 6563 6b20 6c6f 6f6b   This check look
-000008f0: 7320 666f 7220 7772 6974 6520 7065 726d  s for write perm
-00000900: 6973 7369 6f6e 7320 6772 616e 7465 6420  issions granted 
-00000910: 746f 2070 6f74 656e 7469 616c 6c79 2064  to potentially d
-00000920: 616e 6765 726f 7573 2073 636f 7065 7320  angerous scopes 
-00000930: 7375 6368 2061 7320 7468 6520 6063 6f6e  such as the `con
-00000940: 7465 6e74 7360 2073 636f 7065 2077 6869  tents` scope whi
-00000950: 6368 206d 6179 2061 6c6c 6f77 2061 6e20  ch may allow an 
-00000960: 6164 7665 7273 6172 7920 7772 6974 6520  adversary write 
-00000970: 636f 6465 2069 6e74 6f20 7468 6520 7461  code into the ta
-00000980: 7267 6574 2072 6570 6f73 6974 6f72 7920  rget repository 
-00000990: 6966 2074 6865 7927 7265 2061 626c 6520  if they're able 
-000009a0: 746f 2063 6f6d 7072 6f6d 6973 6520 7468  to compromise th
-000009b0: 6520 776f 726b 666c 6f77 2e20 4974 2773  e workflow. It's
-000009c0: 2061 6c73 6f20 6c6f 6f6b 7320 666f 7220   also looks for 
-000009d0: 7573 6167 6520 6f66 2074 6865 2060 7772  usage of the `wr
-000009e0: 6974 652d 616c 6c60 2077 6869 6368 2067  ite-all` which g
-000009f0: 6976 6573 2074 6865 2061 6374 696f 6e20  ives the action 
-00000a00: 636f 6d70 6c65 7465 2077 7269 7465 2061  complete write a
-00000a10: 6363 6573 7320 746f 2061 6c6c 2073 636f  ccess to all sco
-00000a20: 7065 732e 0a0a 352e 204e 616d 653a 2060  pes...5. Name: `
-00000a30: 6368 6563 6b5f 666f 725f 696e 6c69 6e65  check_for_inline
-00000a40: 5f73 6372 6970 7460 2c20 4c65 7665 6c3a  _script`, Level:
-00000a50: 2060 5741 524e 600a 0a20 2020 202d 2054   `WARN`..    - T
-00000a60: 6869 7320 6368 6563 6b20 7369 6d70 6c79  his check simply
-00000a70: 2077 6172 6e73 2074 6861 7420 796f 7527   warns that you'
-00000a80: 7265 2075 7369 6e67 2061 6e20 696e 6c69  re using an inli
-00000a90: 6e65 2073 6372 6970 7420 696e 7374 6561  ne script instea
-00000aa0: 6420 6f66 2047 6974 4875 6220 4163 7469  d of GitHub Acti
-00000ab0: 6f6e 2e20 496e 6c69 6e65 2073 6372 6970  on. Inline scrip
-00000ac0: 7473 2061 7265 2073 7573 6365 7074 6962  ts are susceptib
-00000ad0: 6c65 2074 6f20 7363 7269 7074 2069 6e6a  le to script inj
-00000ae0: 6563 7469 6f6e 2061 7474 6163 6b73 2028  ection attacks (
-00000af0: 616e 6f74 6865 7220 6368 6563 6b20 636f  another check co
-00000b00: 7665 7265 6420 6279 2060 6768 6173 7460  vered by `ghast`
-00000b10: 292e 2049 7420 6973 2072 6563 6f6d 6d65  ). It is recomme
-00000b20: 6e64 6564 2074 6f20 7772 6974 6520 616e  nded to write an
-00000b30: 2061 6374 696f 6e20 616e 6420 7061 7373   action and pass
-00000b40: 2061 6e79 2072 6571 7569 7265 6420 636f   any required co
-00000b50: 6e74 6578 7420 7661 6c75 6573 2061 7320  ntext values as 
-00000b60: 696e 7075 7473 2074 6f20 7468 6174 2061  inputs to that a
-00000b70: 6374 696f 6e20 7768 6963 6820 7265 6d6f  ction which remo
-00000b80: 7665 7320 7363 7269 7074 2069 6e6a 6563  ves script injec
-00000b90: 7469 6f6e 2076 6563 746f 7220 6265 6361  tion vector beca
-00000ba0: 7573 6520 6163 7469 6f6e 2069 6e70 7574  use action input
-00000bb0: 2061 7265 2070 726f 7065 726c 7920 7472   are properly tr
-00000bc0: 6561 7465 6420 6173 2061 7267 756d 656e  eated as argumen
-00000bd0: 7473 2061 6e64 2061 7265 206e 6f74 2065  ts and are not e
-00000be0: 7661 6c75 6174 6564 2061 7320 7061 7274  valuated as part
-00000bf0: 206f 6620 6120 7363 7269 7074 2e0a 0a36   of a script...6
-00000c00: 2e20 4e61 6d65 3a20 6063 6865 636b 5f66  . Name: `check_f
-00000c10: 6f72 5f70 756c 6c5f 7265 7175 6573 745f  or_pull_request_
-00000c20: 7461 7267 6574 602c 204c 6576 656c 3a20  target`, Level: 
-00000c30: 6046 4149 4c60 0a0a 2020 2020 2d20 5468  `FAIL`..    - Th
-00000c40: 6973 2063 6865 636b 206c 6f6f 6b73 2066  is check looks f
-00000c50: 6f72 2074 6865 2075 7361 6765 206f 6620  or the usage of 
-00000c60: 7468 6520 6461 6e67 6572 6f75 7320 6576  the dangerous ev
-00000c70: 656e 7420 7472 6967 6765 7220 6070 756c  ent trigger `pul
-00000c80: 6c5f 7265 7175 6573 745f 7461 7267 6574  l_request_target
-00000c90: 6020 7768 6963 6820 616c 6c6f 7773 2077  ` which allows w
-00000ca0: 6f72 6b66 6c6f 7720 6578 6563 7574 696f  orkflow executio
-00000cb0: 6e73 2074 6f20 7275 6e20 696e 2074 6865  ns to run in the
-00000cc0: 2063 6f6e 7465 7874 206f 6620 7468 6520   context of the 
-00000cd0: 7265 706f 7369 746f 7279 2074 6861 7420  repository that 
-00000ce0: 6465 6669 6e65 7320 7468 6520 776f 726b  defines the work
-00000cf0: 666c 6f77 2c20 6e6f 7420 7468 6520 7265  flow, not the re
-00000d00: 706f 7369 746f 7279 2074 6861 7420 7468  pository that th
-00000d10: 6520 7075 6c6c 2072 6571 7565 7374 206f  e pull request o
-00000d20: 7269 6769 6e61 7465 6420 6672 6f6d 2c20  riginated from, 
-00000d30: 706f 7465 6e74 6961 6c6c 7920 616c 6c6f  potentially allo
-00000d40: 7769 6e67 2061 2074 6872 6561 7420 6163  wing a threat ac
-00000d50: 746f 7220 746f 2067 6169 6e20 6163 6365  tor to gain acce
-00000d60: 7373 2074 6f20 6120 7265 706f 7369 746f  ss to a reposito
-00000d70: 7269 6573 2073 656e 7369 7469 7665 2073  ries sensitive s
-00000d80: 6563 7265 7473 210a 0a37 2e20 4e61 6d65  ecrets!..7. Name
-00000d90: 3a20 6063 6865 636b 5f66 6f72 5f73 6372  : `check_for_scr
-00000da0: 6970 745f 696e 6a65 6374 696f 6e60 2c20  ipt_injection`, 
-00000db0: 4c65 7665 6c3a 2060 4641 494c 600a 0a20  Level: `FAIL`.. 
-00000dc0: 2020 202d 2054 6869 7320 6368 6563 6b20     - This check 
-00000dd0: 6c6f 6f6b 7320 666f 7220 7468 6520 6d6f  looks for the mo
-00000de0: 7374 2063 6f6d 6d6f 6e6c 7920 6b6e 6f77  st commonly know
-00000df0: 6e20 7365 6375 7269 7479 2072 6973 6b20  n security risk 
-00000e00: 746f 2047 6974 4875 6220 4163 7469 6f6e  to GitHub Action
-00000e10: 202d 2073 6372 6970 7420 696e 6a65 6374   - script inject
-00000e20: 696f 6e2e 2053 6372 6970 7420 696e 6a65  ion. Script inje
-00000e30: 6374 696f 6e20 6f63 6375 7273 2077 6865  ction occurs whe
-00000e40: 6e20 616e 2061 6374 696f 6e20 6469 7265  n an action dire
-00000e50: 6374 6c79 2069 6e63 6c75 6465 7320 2875  ctly includes (u
-00000e60: 7369 6e67 2074 6865 2060 247b 7b20 2e2e  sing the `${{ ..
-00000e70: 2e20 7d7d 6020 7379 6e74 6178 2920 6120  . }}` syntax) a 
-00000e80: 4769 7448 7562 2043 6f6e 7465 7874 2076  GitHub Context v
-00000e90: 6172 6961 626c 6528 7329 2069 6e20 616e  ariable(s) in an
-00000ea0: 2069 6e6c 696e 6520 7363 7269 7074 2074   inline script t
-00000eb0: 6861 7420 6361 6e20 6265 2063 6f6e 7472  hat can be contr
-00000ec0: 6f6c 6c65 6420 6279 2061 6e20 756e 7472  olled by an untr
-00000ed0: 7573 7465 6420 6163 746f 722c 2072 6573  usted actor, res
-00000ee0: 756c 7469 6e67 2069 6e20 636f 6d6d 616e  ulting in comman
-00000ef0: 6420 6578 6563 7574 696f 6e20 696e 2074  d execution in t
-00000f00: 6865 2069 6e74 6572 7072 6574 6564 2073  he interpreted s
-00000f10: 6865 6c6c 2e20 5468 6573 6520 7573 6572  hell. These user
-00000f20: 2d63 6f6e 7472 6f6c 6c61 626c 6520 7061  -controllable pa
-00000f30: 7261 6d65 7465 7273 2073 686f 756c 6420  rameters should 
-00000f40: 6265 2070 6173 7365 6420 696e 746f 2061  be passed into a
-00000f50: 6e20 696e 6c69 6e65 2073 6372 6970 7420  n inline script 
-00000f60: 6173 2065 6e76 6972 6f6e 6d65 6e74 2076  as environment v
-00000f70: 6172 6961 626c 6573 2e0a 0a38 2e20 4e61  ariables...8. Na
-00000f80: 6d65 3a20 6063 6865 636b 5f66 6f72 5f73  me: `check_for_s
-00000f90: 656c 665f 686f 7374 6564 5f72 756e 6e65  elf_hosted_runne
-00000fa0: 7273 602c 204c 6576 656c 3a20 6057 4152  rs`, Level: `WAR
-00000fb0: 4e60 200a 0a20 2020 202d 2054 6869 7320  N` ..    - This 
-00000fc0: 6368 6563 6b73 2061 7474 656d 7074 7320  checks attempts 
-00000fd0: 746f 2069 6465 6e74 6966 7920 7468 6520  to identify the 
-00000fe0: 7573 6167 6520 6f66 2073 656c 662d 686f  usage of self-ho
-00000ff0: 7374 6564 2072 756e 6e65 7273 2e20 5365  sted runners. Se
-00001000: 6c66 2d68 6f73 7465 6420 7275 6e6e 6572  lf-hosted runner
-00001010: 7320 6172 6520 6461 6e67 6572 6f75 7320  s are dangerous 
-00001020: 6265 6361 7573 6520 6966 2074 6865 2041  because if the A
-00001030: 6374 696f 6e20 6973 2063 6f6d 7072 6f6d  ction is comprom
-00001040: 6973 6564 2069 7420 6d61 7920 616c 6c6f  ised it may allo
-00001050: 7720 6120 7468 7265 6174 2061 6374 6f72  w a threat actor
-00001060: 2074 6f20 6761 696e 2061 6363 6573 7320   to gain access 
-00001070: 746f 206f 6e20 7072 656d 6973 6520 656e  to on premise en
-00001080: 7669 726f 6e6d 656e 7420 6f72 2065 7374  vironment or est
-00001090: 6162 6c69 7368 2070 6572 7369 7374 656e  ablish persisten
-000010a0: 6365 206d 6563 6861 6e69 736d 7320 6f6e  ce mechanisms on
-000010b0: 2061 2073 6572 7665 7220 796f 7520 6f77   a server you ow
-000010c0: 6e2f 7265 6e74 2e0a 0a39 2e20 4e61 6d65  n/rent...9. Name
-000010d0: 3a20 6063 6865 636b 5f66 6f72 5f61 7773  : `check_for_aws
-000010e0: 5f63 6f6e 6669 6775 7265 5f63 7265 6465  _configure_crede
-000010f0: 6e74 6961 6c73 5f6e 6f6e 5f6f 6964 6360  ntials_non_oidc`
-00001100: 2c20 4c65 7665 6c3a 2060 5741 524e 600a  , Level: `WARN`.
-00001110: 0a20 2020 202d 2054 6869 7320 6368 6563  .    - This chec
-00001120: 6b73 206c 6f6f 6b73 2066 6f72 2074 6865  ks looks for the
-00001130: 2075 7361 6765 206f 6620 4157 5327 7320   usage of AWS's 
-00001140: 6061 7773 2d61 6374 696f 6e73 2f63 6f6e  `aws-actions/con
-00001150: 6669 6775 7265 2d61 7773 2d63 7265 6465  figure-aws-crede
-00001160: 6e74 6961 6c73 6020 6163 7469 6f6e 2061  ntials` action a
-00001170: 6e64 2061 7474 656d 7074 7320 746f 2069  nd attempts to i
-00001180: 6465 6e74 6966 7920 6e6f 6e2d 4f49 4443  dentify non-OIDC
-00001190: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
-000011a0: 7061 7261 6d65 7465 7273 2e20 4e6f 6e2d  parameters. Non-
-000011b0: 4f49 4443 2061 7574 6865 6e74 6963 6174  OIDC authenticat
-000011c0: 696f 6e20 7479 7065 7320 6172 6520 6c65  ion types are le
-000011d0: 7373 2073 6563 7572 6520 7468 616e 204f  ss secure than O
-000011e0: 4944 4320 6265 6361 7573 6520 7468 6579  IDC because they
-000011f0: 2072 6571 7569 7265 2074 6865 2063 7265   require the cre
-00001200: 6174 696f 6e20 6f66 206c 6f6e 672d 7465  ation of long-te
-00001210: 726d 2063 7265 6465 6e74 6961 6c73 2077  rm credentials w
-00001220: 6869 6368 2063 616e 2062 6520 636f 6d70  hich can be comp
-00001230: 726f 6d69 7365 642c 2068 6f77 6576 6572  romised, however
-00001240: 2c20 4f49 4443 2074 6f6b 656e 7320 6172  , OIDC tokens ar
-00001250: 6520 7368 6f72 742d 6c69 7665 6420 616e  e short-lived an
-00001260: 6420 6172 6520 7573 7561 6c6c 7920 7363  d are usually sc
-00001270: 6f70 6564 2074 6f20 6f6e 6c79 2074 6865  oped to only the
-00001280: 2070 6572 6d69 7373 696f 6e73 2074 6861   permissions tha
-00001290: 7420 6172 6520 6573 7365 6e74 6961 6c20  t are essential 
-000012a0: 746f 2061 2077 6f72 6b66 6c6f 7720 616e  to a workflow an
-000012b0: 6420 7468 7573 2068 656c 7020 7265 6475  d thus help redu
-000012c0: 6365 2074 6865 2061 7474 6163 6b20 7375  ce the attack su
-000012d0: 7266 6163 652e 0a0a 3130 2e20 4e61 6d65  rface...10. Name
-000012e0: 3a20 6063 6865 636b 5f66 6f72 5f63 7265  : `check_for_cre
-000012f0: 6174 655f 6f72 5f61 7070 726f 7665 5f70  ate_or_approve_p
-00001300: 756c 6c5f 7265 7175 6573 7460 2c20 4c65  ull_request`, Le
-00001310: 7665 6c3a 2060 5741 524e 600a 0a20 2020  vel: `WARN`..   
-00001320: 202d 2054 6869 7320 6368 6563 6b20 6c6f   - This check lo
-00001330: 6f6b 7320 666f 7220 4163 7469 6f6e 2074  oks for Action t
-00001340: 6861 7420 6861 7665 206c 6f67 6963 2072  hat have logic r
-00001350: 656c 6174 6564 2074 6f20 6372 6561 7469  elated to creati
-00001360: 6e67 206f 7220 696d 7072 6f76 696e 6720  ng or improving 
-00001370: 7075 6c6c 2072 6571 7565 7374 732e 2043  pull requests. C
-00001380: 7265 6174 696e 6720 6f72 2061 7070 726f  reating or appro
-00001390: 7669 6e67 2070 756c 6c20 7265 7175 6573  ving pull reques
-000013a0: 7473 2076 6961 2061 7574 6f6d 6174 696f  ts via automatio
-000013b0: 6e20 706f 7365 7320 6120 7365 6375 7269  n poses a securi
-000013c0: 7479 2072 6973 6b20 6966 2073 7566 6669  ty risk if suffi
-000013d0: 6369 656e 7420 636f 6e74 726f 6c73 2061  cient controls a
-000013e0: 7265 6e27 7420 696e 2070 6c61 6365 2074  ren't in place t
-000013f0: 6f20 7072 6f74 6563 7420 6167 6169 6e73  o protect agains
-00001400: 7420 6d61 6c69 6369 6f75 7320 636f 6465  t malicious code
-00001410: 2062 6569 6e67 206d 6572 6765 6420 696e   being merged in
-00001420: 746f 2061 2072 6570 6f73 6974 6f72 792e  to a repository.
-00001430: 0a0a 3131 2e20 4e61 6d65 3a20 6063 6865  ..11. Name: `che
-00001440: 636b 5f66 6f72 5f72 656d 6f74 655f 7363  ck_for_remote_sc
-00001450: 7269 7074 602c 204c 6576 656c 3a20 6057  ript`, Level: `W
-00001460: 4152 4e60 0a0a 2020 2020 2d20 5468 6973  ARN`..    - This
-00001470: 2063 6865 636b 206c 6f6f 6b73 2066 6f72   check looks for
-00001480: 2061 2055 524c 2069 6e20 616e 2069 6e6c   a URL in an inl
-00001490: 696e 6520 7363 7269 7074 206f 6620 6120  ine script of a 
-000014a0: 4769 7448 7562 2041 6374 696f 6e20 7768  GitHub Action wh
-000014b0: 6963 6820 7573 7561 6c6c 7920 7369 676e  ich usually sign
-000014c0: 616c 7320 7468 6520 696e 636c 7573 696f  als the inclusio
-000014d0: 6e20 6f66 2061 2072 656d 6f74 6520 7363  n of a remote sc
-000014e0: 7269 7074 2077 6869 6368 2063 616e 2062  ript which can b
-000014f0: 6520 6461 6e67 6572 6f75 732e 0a20 200a  e dangerous..  .
-00001500: 3132 2e20 4e61 6d65 3a20 6063 6865 636b  12. Name: `check
-00001510: 5f66 6f72 5f75 706c 6f61 645f 646f 776e  _for_upload_down
-00001520: 6c6f 6164 5f61 7274 6966 6163 745f 6163  load_artifact_ac
-00001530: 7469 6f6e 602c 204c 6576 656c 3a20 6057  tion`, Level: `W
-00001540: 4152 4e60 0a0a 2020 2020 2d20 5468 6973  ARN`..    - This
-00001550: 2063 6865 636b 2069 7320 6573 7365 6e74   check is essent
-00001560: 6961 6c20 666f 7220 6964 656e 7469 6679  ial for identify
-00001570: 696e 6720 616e 7920 7573 6167 6520 6f66  ing any usage of
-00001580: 2047 6974 4875 6227 7320 7570 6c6f 6164   GitHub's upload
-00001590: 2f64 6f77 6e6c 6f61 6420 6172 7469 6661  /download artifa
-000015a0: 6374 2041 6374 696f 6e2c 2061 7320 6974  ct Action, as it
-000015b0: 2063 616e 2070 6f74 656e 7469 616c 6c79   can potentially
-000015c0: 2065 7870 6f73 6520 796f 7572 2077 6f72   expose your wor
-000015d0: 6b66 6c6f 7720 746f 2063 6f6d 7072 6f6d  kflow to comprom
-000015e0: 6973 6564 2066 696c 6573 2e20 466f 7220  ised files. For 
-000015f0: 696e 7374 616e 6365 2c20 616e 2075 706c  instance, an upl
-00001600: 6f61 6465 6420 6172 7469 6661 6374 206d  oaded artifact m
-00001610: 6967 6874 2063 6f6e 7461 696e 2061 2063  ight contain a c
-00001620: 6f6d 7069 6c65 6420 6269 6e61 7279 2066  ompiled binary f
-00001630: 726f 6d20 6120 7072 6576 696f 7573 2077  rom a previous w
-00001640: 6f72 6b66 6c6f 772c 2062 7574 2074 6869  orkflow, but thi
-00001650: 7320 6269 6e61 7279 2063 6f75 6c64 2062  s binary could b
-00001660: 6520 636f 6d70 726f 6d69 7365 6420 6475  e compromised du
-00001670: 6520 746f 2074 6865 2069 6e74 726f 6475  e to the introdu
-00001680: 6374 696f 6e20 6f66 206d 616c 6963 696f  ction of malicio
-00001690: 7573 2064 6570 656e 6465 6e63 6965 7320  us dependencies 
-000016a0: 6475 7269 6e67 2074 6865 2063 6f6d 7069  during the compi
-000016b0: 6c61 7469 6f6e 2070 6861 7365 2e20 436f  lation phase. Co
-000016c0: 6e73 6571 7565 6e74 6c79 2c20 6966 2074  nsequently, if t
-000016d0: 6869 7320 7461 696e 7465 6420 6269 6e61  his tainted bina
-000016e0: 7279 2069 7320 6578 6563 7574 6564 2077  ry is executed w
-000016f0: 6974 6869 6e20 616e 6f74 6865 7220 776f  ithin another wo
-00001700: 726b 666c 6f77 2c20 6974 2063 6f75 6c64  rkflow, it could
-00001710: 206c 6561 6420 746f 2073 6967 6e69 6669   lead to signifi
-00001720: 6361 6e74 2073 6563 7572 6974 7920 7269  cant security ri
-00001730: 736b 732e 2054 6f20 6d69 7469 6761 7465  sks. To mitigate
-00001740: 2073 7563 6820 7269 736b 732c 2069 7420   such risks, it 
-00001750: 6973 2063 7275 6369 616c 2066 6f72 2075  is crucial for u
-00001760: 7365 7273 2074 6f20 636f 6e64 7563 7420  sers to conduct 
-00001770: 696e 7465 6772 6974 7920 6368 6563 6b73  integrity checks
-00001780: 206f 6e20 6172 7469 6661 6374 7320 6265   on artifacts be
-00001790: 666f 7265 2063 6f6e 7375 6d70 7469 6f6e  fore consumption
-000017a0: 2e20 5468 6973 2063 6865 636b 2073 6572  . This check ser
-000017b0: 7665 7320 6173 2061 2076 616c 7561 626c  ves as a valuabl
-000017c0: 6520 7265 6d69 6e64 6572 2074 6f20 7265  e reminder to re
-000017d0: 696e 666f 7263 6520 7468 6973 2073 6563  inforce this sec
-000017e0: 7572 6974 7920 7072 6163 7469 6365 2e0a  urity practice..
-000017f0: 0a31 332e 204e 616d 653a 2060 6368 6563  .13. Name: `chec
-00001800: 6b5f 666f 725f 6e6f 6e5f 6769 7468 7562  k_for_non_github
-00001810: 5f6d 616e 6167 6564 5f61 6374 696f 6e73  _managed_actions
-00001820: 602c 204c 6576 656c 3a20 6057 4152 4e60  `, Level: `WARN`
-00001830: 0a0a 2020 2020 2d20 5468 6973 2063 6865  ..    - This che
-00001840: 636b 206c 6f6f 6b73 2066 6f72 2069 6e63  ck looks for inc
-00001850: 6c75 7369 6f6e 206f 6620 6e6f 6e20 4769  lusion of non Gi
-00001860: 7448 7562 2d6d 616e 6167 6564 2061 6374  tHub-managed act
-00001870: 696f 6e73 2061 6e64 2073 6572 7665 7320  ions and serves 
-00001880: 6173 2061 2072 656d 696e 6465 7220 746f  as a reminder to
-00001890: 2072 6576 6965 7720 7468 6520 7365 6375   review the secu
-000018a0: 7269 7479 2070 6f73 7475 7265 206f 6620  rity posture of 
-000018b0: 616e 7920 7468 6972 6420 7061 7274 7920  any third party 
-000018c0: 6163 7469 6f6e 7320 796f 7520 696e 636c  actions you incl
-000018d0: 7564 6520 696e 2079 6f75 7220 776f 726b  ude in your work
-000018e0: 666c 6f77 2873 292c 2065 7370 6563 6961  flow(s), especia
-000018f0: 6c6c 7920 6966 2074 6865 7920 6172 6520  lly if they are 
-00001900: 6e6f 7420 6465 7665 6c6f 7065 6420 616e  not developed an
-00001910: 6420 6d61 696e 7461 696e 6564 2062 7920  d maintained by 
-00001920: 6372 6564 6962 6c65 2065 6e74 6974 6965  credible entitie
-00001930: 732e 0a0a 2323 2323 2041 7578 696c 6961  s...#### Auxilia
-00001940: 7279 2043 6865 636b 730a 0a31 2e20 4e61  ry Checks..1. Na
-00001950: 6d65 3a20 6063 6865 636b 5f66 6f72 5f63  me: `check_for_c
-00001960: 6f64 656f 776e 6572 735f 6669 6c65 6020  odeowners_file` 
-00001970: 2d20 6368 6563 6b73 2066 6f72 2065 7869  - checks for exi
-00001980: 7374 656e 6365 206f 6620 5b43 4f44 454f  stence of [CODEO
-00001990: 574e 4552 535d 2868 7474 7073 3a2f 2f64  WNERS](https://d
-000019a0: 6f63 732e 6769 7468 7562 2e63 6f6d 2f65  ocs.github.com/e
-000019b0: 6e2f 7265 706f 7369 746f 7269 6573 2f6d  n/repositories/m
-000019c0: 616e 6167 696e 672d 796f 7572 2d72 6570  anaging-your-rep
-000019d0: 6f73 6974 6f72 7973 2d73 6574 7469 6e67  ositorys-setting
-000019e0: 732d 616e 642d 6665 6174 7572 6573 2f63  s-and-features/c
-000019f0: 7573 746f 6d69 7a69 6e67 2d79 6f75 722d  ustomizing-your-
-00001a00: 7265 706f 7369 746f 7279 2f61 626f 7574  repository/about
-00001a10: 2d63 6f64 652d 6f77 6e65 7273 2920 6669  -code-owners) fi
-00001a20: 6c65 2e0a 0a23 2323 2052 6566 6572 656e  le...### Referen
-00001a30: 6365 730a 0a2d 205b 5365 6375 7269 7479  ces..- [Security
-00001a40: 2068 6172 6465 6e69 6e67 2066 6f72 2047   hardening for G
-00001a50: 6974 4875 6220 4163 7469 6f6e 735d 2868  itHub Actions](h
-00001a60: 7474 7073 3a2f 2f64 6f63 732e 6769 7468  ttps://docs.gith
-00001a70: 7562 2e63 6f6d 2f65 6e2f 6163 7469 6f6e  ub.com/en/action
-00001a80: 732f 7365 6375 7269 7479 2d67 7569 6465  s/security-guide
-00001a90: 732f 7365 6375 7269 7479 2d68 6172 6465  s/security-harde
-00001aa0: 6e69 6e67 2d66 6f72 2d67 6974 6875 622d  ning-for-github-
-00001ab0: 6163 7469 6f6e 7329 0a                   actions).
+00000110: 7473 2073 7572 726f 756e 6469 6e67 2065  ts surrounding e
+00000120: 6e76 6972 6f6e 6d65 6e74 2066 6f72 2063  nvironment for c
+00000130: 6f6d 6d6f 6e20 7365 6375 7269 7479 2076  ommon security v
+00000140: 756c 6e65 7261 6269 6c69 7469 6573 2061  ulnerabilities a
+00000150: 6e64 2f6f 7220 6d69 7373 696e 6720 7365  nd/or missing se
+00000160: 6375 7269 7479 2063 6f6e 6669 6775 7261  curity configura
+00000170: 7469 6f6e 2e20 2059 6f75 2063 616e 2075  tion.  You can u
+00000180: 7365 2047 6861 7374 2061 7320 6120 7374  se Ghast as a st
+00000190: 616e 642d 616c 6f6e 6520 616e 616c 7973  and-alone analys
+000001a0: 6973 2074 6f6f 6c20 7669 6120 7468 6520  is tool via the 
+000001b0: 4768 6173 7420 434c 4920 6f72 2062 7920  Ghast CLI or by 
+000001c0: 7275 6e6e 696e 6720 4768 6173 7420 6173  running Ghast as
+000001d0: 2061 206e 6174 6976 6520 4769 7448 7562   a native GitHub
+000001e0: 2041 6374 696f 6e2e 0a0a 5468 6520 6163   Action...The ac
+000001f0: 7469 6f6e 7320 6469 7265 6374 6f72 7920  tions directory 
+00000200: 6861 7320 736f 6d65 2065 7861 6d70 6c65  has some example
+00000210: 2047 6974 4875 6220 4163 7469 6f6e 7320   GitHub Actions 
+00000220: 7769 7468 2076 756c 6e65 7261 626c 6520  with vulnerable 
+00000230: 7374 6570 7320 7468 6174 2079 6f75 2063  steps that you c
+00000240: 616e 2075 7365 2074 6f20 7465 7374 2e0a  an use to test..
+00000250: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000260: 7222 3e3c 696d 6720 7769 6474 683d 2239  r"><img width="9
+00000270: 3336 2220 616c 743d 2269 6d61 6765 2220  36" alt="image" 
+00000280: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000290: 6875 622e 636f 6d2f 6269 6e33 7869 7368  hub.com/bin3xish
+000002a0: 3437 372f 6768 6173 742f 6173 7365 7473  477/ghast/assets
+000002b0: 2f34 3432 3831 3632 302f 3732 3134 3332  /44281620/721432
+000002c0: 6361 2d37 3934 342d 3430 6234 2d38 3033  ca-7944-40b4-803
+000002d0: 642d 3863 3363 6238 3636 3939 3665 223e  d-8c3cb866996e">
+000002e0: 3c2f 703e 0a0a 0a23 2323 2049 6e73 7461  </p>...### Insta
+000002f0: 6c6c 2074 6865 2047 6861 7374 2043 4c49  ll the Ghast CLI
+00000300: 0a0a 3e20 4d61 6b65 2073 7572 6520 796f  ..> Make sure yo
+00000310: 7520 6861 7665 2060 2448 4f4d 452f 2e6c  u have `$HOME/.l
+00000320: 6f63 616c 2f62 696e 6020 696e 2079 6f75  ocal/bin` in you
+00000330: 7220 5041 5448 0a0a 2323 2323 2055 7369  r PATH..#### Usi
+00000340: 6e67 2050 6970 0a0a 6060 600a 7069 7020  ng Pip..```.pip 
+00000350: 696e 7374 616c 6c20 6768 6173 742d 7363  install ghast-sc
+00000360: 616e 6e65 720a 6060 600a 0a23 2323 2320  anner.```..#### 
+00000370: 5769 7468 2047 6974 2f50 7974 686f 6e0a  With Git/Python.
+00000380: 0a60 6060 0a67 6974 2063 6c6f 6e65 2068  .```.git clone h
+00000390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003a0: 6d2f 6269 6e33 7869 7368 3437 372f 6768  m/bin3xish477/gh
+000003b0: 6173 742e 6769 740a 7079 7468 6f6e 3320  ast.git.python3 
+000003c0: 2d6d 2070 6970 2069 6e73 7461 6c6c 202e  -m pip install .
+000003d0: 0a60 6060 0a0a 2323 2320 486f 7720 746f  .```..### How to
+000003e0: 2075 7365 2074 6865 2047 6861 7374 2043   use the Ghast C
+000003f0: 4c49 0a0a 6060 600a 6768 6173 7420 2d68  LI..```.ghast -h
+00000400: 2009 0909 0909 2320 6765 7420 6865 6c70   .....# get help
+00000410: 200a 6768 6173 7420 2d2d 6669 6c65 2061   .ghast --file a
+00000420: 6374 696f 6e2e 796d 6c20 0909 0923 2073  ction.yml ...# s
+00000430: 6361 6e20 6120 7370 6563 6966 6963 2077  can a specific w
+00000440: 6f72 6b66 6c6f 7720 6669 6c65 0a67 6861  orkflow file.gha
+00000450: 7374 202d 6420 6469 7265 6374 6f72 792d  st -d directory-
+00000460: 7769 7468 2d61 6374 696f 6e73 2f20 2d2d  with-actions/ --
+00000470: 7665 7262 6f73 6509 2320 7363 616e 2061  verbose.# scan a
+00000480: 2064 6972 6563 746f 7279 2069 6e20 7665   directory in ve
+00000490: 7262 6f73 6520 6d6f 6465 0a67 6861 7374  rbose mode.ghast
+000004a0: 202d 2d66 696c 6520 6163 7469 6f6e 2e79   --file action.y
+000004b0: 6d6c 202d 2d69 676e 6f72 652d 7761 726e  ml --ignore-warn
+000004c0: 696e 6773 0923 2073 6361 6e20 6120 7370  ings.# scan a sp
+000004d0: 6563 6966 6963 2077 6f72 6b66 6c6f 7720  ecific workflow 
+000004e0: 6669 6c65 2061 6e64 2069 676e 6f72 6520  file and ignore 
+000004f0: 7761 726e 696e 6773 0a67 6861 7374 202d  warnings.ghast -
+00000500: 2d6c 6973 742d 6368 6563 6b73 0909 0909  -list-checks....
+00000510: 2320 6c69 7374 2061 6c6c 206b 6e6f 776e  # list all known
+00000520: 2063 6865 636b 730a 6768 6173 7420 2d69   checks.ghast -i
+00000530: 2063 6865 636b 5f66 6f72 5f69 6e6c 696e   check_for_inlin
+00000540: 655f 7363 7269 7074 202d 2d6e 6f2d 7375  e_script --no-su
+00000550: 6d6d 6172 7909 2320 6f6e 6c79 2072 756e  mmary.# only run
+00000560: 2061 2073 7065 6369 6669 6320 6368 6563   a specific chec
+00000570: 6b20 616e 6420 646f 6e27 7420 7368 6f77  k and don't show
+00000580: 2074 6f6f 6c20 7375 6d6d 6172 790a 6060   tool summary.``
+00000590: 600a 0a23 2323 2320 5365 6520 686f 7720  `..#### See how 
+000005a0: 7468 6520 4768 6173 7420 434c 4920 776f  the Ghast CLI wo
+000005b0: 726b 730a 3c61 2068 7265 663d 2268 7474  rks.<a href="htt
+000005c0: 7073 3a2f 2f61 7363 6969 6e65 6d61 2e6f  ps://asciinema.o
+000005d0: 7267 2f61 2f36 3030 3839 313f 6175 746f  rg/a/600891?auto
+000005e0: 706c 6179 3d31 2220 7769 6474 683d 2234  play=1" width="4
+000005f0: 3030 2220 7461 7267 6574 3d22 5f62 6c61  00" target="_bla
+00000600: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
+00000610: 7470 733a 2f2f 6173 6369 696e 656d 612e  tps://asciinema.
+00000620: 6f72 672f 612f 3630 3038 3931 2e73 7667  org/a/600891.svg
+00000630: 2220 2f3e 3c2f 613e 0a0a 2323 2320 5573  " /></a>..### Us
+00000640: 6520 6067 6861 7374 6020 696e 2059 6f75  e `ghast` in You
+00000650: 7220 4769 7448 7562 2057 6f72 6b66 6c6f  r GitHub Workflo
+00000660: 7773 0a0a 2323 2323 2044 6566 6175 6c74  ws..#### Default
+00000670: 2057 6f72 6b66 6c6f 770a 0a60 6060 7961   Workflow..```ya
+00000680: 6d6c 0a6e 616d 653a 2027 5275 6e47 6861  ml.name: 'RunGha
+00000690: 7374 270a 6f6e 3a0a 2020 7075 7368 3a0a  st'.on:.  push:.
+000006a0: 6a6f 6273 3a0a 2020 5275 6e47 6861 7374  jobs:.  RunGhast
+000006b0: 3a0a 2020 2020 7275 6e73 2d6f 6e3a 2075  :.    runs-on: u
+000006c0: 6275 6e74 752d 6c61 7465 7374 0a20 2020  buntu-latest.   
+000006d0: 2073 7465 7073 3a0a 2020 2020 2d20 6e61   steps:.    - na
+000006e0: 6d65 3a20 2243 6865 636b 6f75 7420 7265  me: "Checkout re
+000006f0: 706f 220a 2020 2020 2020 7573 6573 3a20  po".      uses: 
+00000700: 6163 7469 6f6e 732f 6368 6563 6b6f 7574  actions/checkout
+00000710: 4039 3666 3533 3130 3062 6132 6135 3434  @96f53100ba2a544
+00000720: 3965 6237 3164 3265 3636 3034 6262 6364  9eb71d2e6604bbcd
+00000730: 3934 6239 3434 3962 3520 2320 7633 2e35  94b9449b5 # v3.5
+00000740: 2e33 0a20 2020 202d 206e 616d 653a 2022  .3.    - name: "
+00000750: 5275 6e20 4768 6173 7422 0a20 2020 2020  Run Ghast".     
+00000760: 2075 7365 733a 2022 6269 6e33 7869 7368   uses: "bin3xish
+00000770: 3437 372f 6768 6173 7440 3433 6334 3731  477/ghast@43c471
+00000780: 6238 6530 3535 3939 6436 3766 3631 3865  b8e05599d67f618e
+00000790: 6363 6366 6338 6437 6239 3238 3162 6664  cccfc8d7b9281bfd
+000007a0: 3962 220a 6060 600a 0a23 2323 2053 6565  9b".```..### See
+000007b0: 2041 6464 6974 696f 6e61 6c20 576f 726b   Additional Work
+000007c0: 666c 6f77 2045 7861 6d70 6c65 730a 5b41  flow Examples.[A
+000007d0: 6464 6974 696f 6e61 6c20 4768 6173 7420  dditional Ghast 
+000007e0: 576f 726b 666c 6f77 2045 7861 6d70 6c65  Workflow Example
+000007f0: 735d 2845 5841 4d50 4c45 532e 6d64 290a  s](EXAMPLES.md).
+00000800: 0a23 2323 2043 6865 636b 7320 5065 7266  .### Checks Perf
+00000810: 6f72 6d65 6420 6279 2060 6768 6173 7460  ormed by `ghast`
+00000820: 0a0a 312e 204e 616d 653a 2060 6368 6563  ..1. Name: `chec
+00000830: 6b5f 666f 725f 3370 5f61 6374 696f 6e73  k_for_3p_actions
+00000840: 5f77 6974 686f 7574 5f68 6173 6860 2c20  _without_hash`, 
+00000850: 4c65 7665 6c3a 2060 4641 494c 600a 0a20  Level: `FAIL`.. 
+00000860: 2020 202d 2054 6869 7320 6368 6563 6b20     - This check 
+00000870: 6964 656e 7469 6669 6573 2061 6e79 2074  identifies any t
+00000880: 6869 7264 2070 6172 7479 2047 6974 4875  hird party GitHu
+00000890: 6220 4163 7469 6f6e 7320 696e 2075 7365  b Actions in use
+000008a0: 2074 6861 7420 6861 7665 2062 6565 6e20   that have been 
+000008b0: 7265 6665 7265 6e63 6564 2076 6961 2061  referenced via a
+000008c0: 2076 6572 7369 6f6e 206e 756d 6265 7220   version number 
+000008d0: 7375 6368 2061 7320 6076 312e 3160 2069  such as `v1.1` i
+000008e0: 6e73 7465 6164 206f 6620 636f 6d6d 6974  nstead of commit
+000008f0: 2053 4841 2068 6161 682e 2055 7369 6e67   SHA haah. Using
+00000900: 2061 2068 6173 6820 6361 6e20 6865 6c70   a hash can help
+00000910: 206d 6974 6967 6174 6520 7375 7070 6c79   mitigate supply
+00000920: 2063 6861 696e 2074 6872 6561 7473 2069   chain threats i
+00000930: 6e20 6120 7363 656e 6172 696f 2077 6865  n a scenario whe
+00000940: 7265 2061 2074 6872 6561 7420 6163 746f  re a threat acto
+00000950: 7220 6861 7320 636f 6d70 726f 6d69 7365  r has compromise
+00000960: 6420 7468 6520 736f 7572 6365 2072 6570  d the source rep
+00000970: 6f73 6974 6f72 7920 7768 6572 6520 7468  ository where th
+00000980: 6520 3350 2061 6374 696f 6e20 6c69 7665  e 3P action live
+00000990: 732e 0a0a 322e 204e 616d 653a 2060 6368  s...2. Name: `ch
+000009a0: 6563 6b5f 666f 725f 616c 6c6f 775f 756e  eck_for_allow_un
+000009b0: 7365 6375 7265 5f63 6f6d 6d61 6e64 7360  secure_commands`
+000009c0: 2c20 4c65 7665 6c3a 2060 4641 494c 600a  , Level: `FAIL`.
+000009d0: 0a20 2020 202d 2054 6869 7320 6368 6563  .    - This chec
+000009e0: 6b20 6c6f 6f6b 7320 666f 7220 7468 6520  k looks for the 
+000009f0: 7573 6167 6520 6f66 2065 6e76 6972 6f6e  usage of environ
+00000a00: 6d65 6e74 2076 6172 6961 626c 6520 6361  ment variable ca
+00000a10: 6c6c 6564 2060 4143 5449 4f4e 535f 414c  lled `ACTIONS_AL
+00000a20: 4c4f 575f 554e 5345 4355 5245 5f43 4f4d  LOW_UNSECURE_COM
+00000a30: 4d41 4e44 5360 2077 6869 6368 2061 6c6c  MANDS` which all
+00000a40: 6f77 7320 666f 7220 616e 2041 6374 696f  ows for an Actio
+00000a50: 6e20 746f 2067 6574 2061 6363 6573 7320  n to get access 
+00000a60: 746f 2064 616e 6765 726f 7573 2063 6f6d  to dangerous com
+00000a70: 6d61 6e64 7320 2860 6765 742d 656e 7660  mands (`get-env`
+00000a80: 2c20 6061 6464 2d70 6174 6860 2920 7768  , `add-path`) wh
+00000a90: 6963 6820 6361 6e20 6c65 6164 2074 6f20  ich can lead to 
+00000aa0: 636f 6465 2069 6e6a 6563 7469 6f6e 2061  code injection a
+00000ab0: 6e64 2063 7265 6465 6e74 6961 6c20 7468  nd credential th
+00000ac0: 6566 7473 206f 7070 6f72 7475 6e69 7469  efts opportuniti
+00000ad0: 6573 2e0a 0a33 2e20 4e61 6d65 3a20 6063  es...3. Name: `c
+00000ae0: 6865 636b 5f66 6f72 5f63 6163 6865 5f61  heck_for_cache_a
+00000af0: 6374 696f 6e60 2c20 4c65 7665 6c3a 2060  ction`, Level: `
+00000b00: 5741 524e 600a 0a20 2020 202d 2054 6869  WARN`..    - Thi
+00000b10: 7320 6368 6563 6b20 6669 6e64 7320 616e  s check finds an
+00000b20: 7920 7573 6167 6520 6f66 2047 6974 4875  y usage of GitHu
+00000b30: 6227 7320 6361 6368 696e 6720 4163 7469  b's caching Acti
+00000b40: 6f6e 2028 6061 6374 696f 6e73 2f63 6163  on (`actions/cac
+00000b50: 6865 6029 2077 6869 6368 206d 6179 2072  he`) which may r
+00000b60: 6573 756c 7420 696e 2073 656e 7369 7469  esult in sensiti
+00000b70: 7665 2069 6e66 6f72 6d61 7469 6f6e 2064  ve information d
+00000b80: 6973 636c 6f73 7572 6520 6f72 2063 6163  isclosure or cac
+00000b90: 6865 2070 6f69 736f 6e69 6e67 2e0a 0a34  he poisoning...4
+00000ba0: 2e20 4e61 6d65 3a20 6063 6865 636b 5f66  . Name: `check_f
+00000bb0: 6f72 5f64 616e 6765 726f 7573 5f77 7269  or_dangerous_wri
+00000bc0: 7465 5f70 6572 6d69 7373 696f 6e73 602c  te_permissions`,
+00000bd0: 204c 6576 656c 3a20 6046 4149 4c60 0a0a   Level: `FAIL`..
+00000be0: 2020 2020 2d20 5468 6973 2063 6865 636b      - This check
+00000bf0: 206c 6f6f 6b73 2066 6f72 2077 7269 7465   looks for write
+00000c00: 2070 6572 6d69 7373 696f 6e73 2067 7261   permissions gra
+00000c10: 6e74 6564 2074 6f20 706f 7465 6e74 6961  nted to potentia
+00000c20: 6c6c 7920 6461 6e67 6572 6f75 7320 7363  lly dangerous sc
+00000c30: 6f70 6573 2073 7563 6820 6173 2074 6865  opes such as the
+00000c40: 2060 636f 6e74 656e 7473 6020 7363 6f70   `contents` scop
+00000c50: 6520 7768 6963 6820 6d61 7920 616c 6c6f  e which may allo
+00000c60: 7720 616e 2061 6476 6572 7361 7279 2077  w an adversary w
+00000c70: 7269 7465 2063 6f64 6520 696e 746f 2074  rite code into t
+00000c80: 6865 2074 6172 6765 7420 7265 706f 7369  he target reposi
+00000c90: 746f 7279 2069 6620 7468 6579 2772 6520  tory if they're 
+00000ca0: 6162 6c65 2074 6f20 636f 6d70 726f 6d69  able to compromi
+00000cb0: 7365 2074 6865 2077 6f72 6b66 6c6f 772e  se the workflow.
+00000cc0: 2049 7427 7320 616c 736f 206c 6f6f 6b73   It's also looks
+00000cd0: 2066 6f72 2075 7361 6765 206f 6620 7468   for usage of th
+00000ce0: 6520 6077 7269 7465 2d61 6c6c 6020 7768  e `write-all` wh
+00000cf0: 6963 6820 6769 7665 7320 7468 6520 6163  ich gives the ac
+00000d00: 7469 6f6e 2063 6f6d 706c 6574 6520 7772  tion complete wr
+00000d10: 6974 6520 6163 6365 7373 2074 6f20 616c  ite access to al
+00000d20: 6c20 7363 6f70 6573 2e0a 0a35 2e20 4e61  l scopes...5. Na
+00000d30: 6d65 3a20 6063 6865 636b 5f66 6f72 5f69  me: `check_for_i
+00000d40: 6e6c 696e 655f 7363 7269 7074 602c 204c  nline_script`, L
+00000d50: 6576 656c 3a20 6057 4152 4e60 0a0a 2020  evel: `WARN`..  
+00000d60: 2020 2d20 5468 6973 2063 6865 636b 2073    - This check s
+00000d70: 696d 706c 7920 7761 726e 7320 7468 6174  imply warns that
+00000d80: 2079 6f75 2772 6520 7573 696e 6720 616e   you're using an
+00000d90: 2069 6e6c 696e 6520 7363 7269 7074 2069   inline script i
+00000da0: 6e73 7465 6164 206f 6620 4769 7448 7562  nstead of GitHub
+00000db0: 2041 6374 696f 6e2e 2049 6e6c 696e 6520   Action. Inline 
+00000dc0: 7363 7269 7074 7320 6172 6520 7375 7363  scripts are susc
+00000dd0: 6570 7469 626c 6520 746f 2073 6372 6970  eptible to scrip
+00000de0: 7420 696e 6a65 6374 696f 6e20 6174 7461  t injection atta
+00000df0: 636b 7320 2861 6e6f 7468 6572 2063 6865  cks (another che
+00000e00: 636b 2063 6f76 6572 6564 2062 7920 6067  ck covered by `g
+00000e10: 6861 7374 6029 2e20 4974 2069 7320 7265  hast`). It is re
+00000e20: 636f 6d6d 656e 6465 6420 746f 2077 7269  commended to wri
+00000e30: 7465 2061 6e20 6163 7469 6f6e 2061 6e64  te an action and
+00000e40: 2070 6173 7320 616e 7920 7265 7175 6972   pass any requir
+00000e50: 6564 2063 6f6e 7465 7874 2076 616c 7565  ed context value
+00000e60: 7320 6173 2069 6e70 7574 7320 746f 2074  s as inputs to t
+00000e70: 6861 7420 6163 7469 6f6e 2077 6869 6368  hat action which
+00000e80: 2072 656d 6f76 6573 2073 6372 6970 7420   removes script 
+00000e90: 696e 6a65 6374 696f 6e20 7665 6374 6f72  injection vector
+00000ea0: 2062 6563 6175 7365 2061 6374 696f 6e20   because action 
+00000eb0: 696e 7075 7420 6172 6520 7072 6f70 6572  input are proper
+00000ec0: 6c79 2074 7265 6174 6564 2061 7320 6172  ly treated as ar
+00000ed0: 6775 6d65 6e74 7320 616e 6420 6172 6520  guments and are 
+00000ee0: 6e6f 7420 6576 616c 7561 7465 6420 6173  not evaluated as
+00000ef0: 2070 6172 7420 6f66 2061 2073 6372 6970   part of a scrip
+00000f00: 742e 0a0a 362e 204e 616d 653a 2060 6368  t...6. Name: `ch
+00000f10: 6563 6b5f 666f 725f 7075 6c6c 5f72 6571  eck_for_pull_req
+00000f20: 7565 7374 5f74 6172 6765 7460 2c20 4c65  uest_target`, Le
+00000f30: 7665 6c3a 2060 4641 494c 600a 0a20 2020  vel: `FAIL`..   
+00000f40: 202d 2054 6869 7320 6368 6563 6b20 6c6f   - This check lo
+00000f50: 6f6b 7320 666f 7220 7468 6520 7573 6167  oks for the usag
+00000f60: 6520 6f66 2074 6865 2064 616e 6765 726f  e of the dangero
+00000f70: 7573 2065 7665 6e74 2074 7269 6767 6572  us event trigger
+00000f80: 2060 7075 6c6c 5f72 6571 7565 7374 5f74   `pull_request_t
+00000f90: 6172 6765 7460 2077 6869 6368 2061 6c6c  arget` which all
+00000fa0: 6f77 7320 776f 726b 666c 6f77 2065 7865  ows workflow exe
+00000fb0: 6375 7469 6f6e 7320 746f 2072 756e 2069  cutions to run i
+00000fc0: 6e20 7468 6520 636f 6e74 6578 7420 6f66  n the context of
+00000fd0: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
+00000fe0: 7468 6174 2064 6566 696e 6573 2074 6865  that defines the
+00000ff0: 2077 6f72 6b66 6c6f 772c 206e 6f74 2074   workflow, not t
+00001000: 6865 2072 6570 6f73 6974 6f72 7920 7468  he repository th
+00001010: 6174 2074 6865 2070 756c 6c20 7265 7175  at the pull requ
+00001020: 6573 7420 6f72 6967 696e 6174 6564 2066  est originated f
+00001030: 726f 6d2c 2070 6f74 656e 7469 616c 6c79  rom, potentially
+00001040: 2061 6c6c 6f77 696e 6720 6120 7468 7265   allowing a thre
+00001050: 6174 2061 6374 6f72 2074 6f20 6761 696e  at actor to gain
+00001060: 2061 6363 6573 7320 746f 2061 2072 6570   access to a rep
+00001070: 6f73 6974 6f72 6965 7320 7365 6e73 6974  ositories sensit
+00001080: 6976 6520 7365 6372 6574 7321 0a0a 372e  ive secrets!..7.
+00001090: 204e 616d 653a 2060 6368 6563 6b5f 666f   Name: `check_fo
+000010a0: 725f 7363 7269 7074 5f69 6e6a 6563 7469  r_script_injecti
+000010b0: 6f6e 602c 204c 6576 656c 3a20 6046 4149  on`, Level: `FAI
+000010c0: 4c60 0a0a 2020 2020 2d20 5468 6973 2063  L`..    - This c
+000010d0: 6865 636b 206c 6f6f 6b73 2066 6f72 2074  heck looks for t
+000010e0: 6865 206d 6f73 7420 636f 6d6d 6f6e 6c79  he most commonly
+000010f0: 206b 6e6f 776e 2073 6563 7572 6974 7920   known security 
+00001100: 7269 736b 2074 6f20 4769 7448 7562 2041  risk to GitHub A
+00001110: 6374 696f 6e20 2d20 7363 7269 7074 2069  ction - script i
+00001120: 6e6a 6563 7469 6f6e 2e20 5363 7269 7074  njection. Script
+00001130: 2069 6e6a 6563 7469 6f6e 206f 6363 7572   injection occur
+00001140: 7320 7768 656e 2061 6e20 6163 7469 6f6e  s when an action
+00001150: 2064 6972 6563 746c 7920 696e 636c 7564   directly includ
+00001160: 6573 2028 7573 696e 6720 7468 6520 6024  es (using the `$
+00001170: 7b7b 202e 2e2e 207d 7d60 2073 796e 7461  {{ ... }}` synta
+00001180: 7829 2061 2047 6974 4875 6220 436f 6e74  x) a GitHub Cont
+00001190: 6578 7420 7661 7269 6162 6c65 2873 2920  ext variable(s) 
+000011a0: 696e 2061 6e20 696e 6c69 6e65 2073 6372  in an inline scr
+000011b0: 6970 7420 7468 6174 2063 616e 2062 6520  ipt that can be 
+000011c0: 636f 6e74 726f 6c6c 6564 2062 7920 616e  controlled by an
+000011d0: 2075 6e74 7275 7374 6564 2061 6374 6f72   untrusted actor
+000011e0: 2c20 7265 7375 6c74 696e 6720 696e 2063  , resulting in c
+000011f0: 6f6d 6d61 6e64 2065 7865 6375 7469 6f6e  ommand execution
+00001200: 2069 6e20 7468 6520 696e 7465 7270 7265   in the interpre
+00001210: 7465 6420 7368 656c 6c2e 2054 6865 7365  ted shell. These
+00001220: 2075 7365 722d 636f 6e74 726f 6c6c 6162   user-controllab
+00001230: 6c65 2070 6172 616d 6574 6572 7320 7368  le parameters sh
+00001240: 6f75 6c64 2062 6520 7061 7373 6564 2069  ould be passed i
+00001250: 6e74 6f20 616e 2069 6e6c 696e 6520 7363  nto an inline sc
+00001260: 7269 7074 2061 7320 656e 7669 726f 6e6d  ript as environm
+00001270: 656e 7420 7661 7269 6162 6c65 732e 0a0a  ent variables...
+00001280: 382e 204e 616d 653a 2060 6368 6563 6b5f  8. Name: `check_
+00001290: 666f 725f 7365 6c66 5f68 6f73 7465 645f  for_self_hosted_
+000012a0: 7275 6e6e 6572 7360 2c20 4c65 7665 6c3a  runners`, Level:
+000012b0: 2060 5741 524e 6020 0a0a 2020 2020 2d20   `WARN` ..    - 
+000012c0: 5468 6973 2063 6865 636b 7320 6174 7465  This checks atte
+000012d0: 6d70 7473 2074 6f20 6964 656e 7469 6679  mpts to identify
+000012e0: 2074 6865 2075 7361 6765 206f 6620 7365   the usage of se
+000012f0: 6c66 2d68 6f73 7465 6420 7275 6e6e 6572  lf-hosted runner
+00001300: 732e 2053 656c 662d 686f 7374 6564 2072  s. Self-hosted r
+00001310: 756e 6e65 7273 2061 7265 2064 616e 6765  unners are dange
+00001320: 726f 7573 2062 6563 6175 7365 2069 6620  rous because if 
+00001330: 7468 6520 4163 7469 6f6e 2069 7320 636f  the Action is co
+00001340: 6d70 726f 6d69 7365 6420 6974 206d 6179  mpromised it may
+00001350: 2061 6c6c 6f77 2061 2074 6872 6561 7420   allow a threat 
+00001360: 6163 746f 7220 746f 2067 6169 6e20 6163  actor to gain ac
+00001370: 6365 7373 2074 6f20 6f6e 2070 7265 6d69  cess to on premi
+00001380: 7365 2065 6e76 6972 6f6e 6d65 6e74 206f  se environment o
+00001390: 7220 6573 7461 626c 6973 6820 7065 7273  r establish pers
+000013a0: 6973 7465 6e63 6520 6d65 6368 616e 6973  istence mechanis
+000013b0: 6d73 206f 6e20 6120 7365 7276 6572 2079  ms on a server y
+000013c0: 6f75 206f 776e 2f72 656e 742e 0a0a 392e  ou own/rent...9.
+000013d0: 204e 616d 653a 2060 6368 6563 6b5f 666f   Name: `check_fo
+000013e0: 725f 6177 735f 636f 6e66 6967 7572 655f  r_aws_configure_
+000013f0: 6372 6564 656e 7469 616c 735f 6e6f 6e5f  credentials_non_
+00001400: 6f69 6463 602c 204c 6576 656c 3a20 6057  oidc`, Level: `W
+00001410: 4152 4e60 0a0a 2020 2020 2d20 5468 6973  ARN`..    - This
+00001420: 2063 6865 636b 7320 6c6f 6f6b 7320 666f   checks looks fo
+00001430: 7220 7468 6520 7573 6167 6520 6f66 2041  r the usage of A
+00001440: 5753 2773 2060 6177 732d 6163 7469 6f6e  WS's `aws-action
+00001450: 732f 636f 6e66 6967 7572 652d 6177 732d  s/configure-aws-
+00001460: 6372 6564 656e 7469 616c 7360 2061 6374  credentials` act
+00001470: 696f 6e20 616e 6420 6174 7465 6d70 7473  ion and attempts
+00001480: 2074 6f20 6964 656e 7469 6679 206e 6f6e   to identify non
+00001490: 2d4f 4944 4320 6175 7468 656e 7469 6361  -OIDC authentica
+000014a0: 7469 6f6e 2070 6172 616d 6574 6572 732e  tion parameters.
+000014b0: 204e 6f6e 2d4f 4944 4320 6175 7468 656e   Non-OIDC authen
+000014c0: 7469 6361 7469 6f6e 2074 7970 6573 2061  tication types a
+000014d0: 7265 206c 6573 7320 7365 6375 7265 2074  re less secure t
+000014e0: 6861 6e20 4f49 4443 2062 6563 6175 7365  han OIDC because
+000014f0: 2074 6865 7920 7265 7175 6972 6520 7468   they require th
+00001500: 6520 6372 6561 7469 6f6e 206f 6620 6c6f  e creation of lo
+00001510: 6e67 2d74 6572 6d20 6372 6564 656e 7469  ng-term credenti
+00001520: 616c 7320 7768 6963 6820 6361 6e20 6265  als which can be
+00001530: 2063 6f6d 7072 6f6d 6973 6564 2c20 686f   compromised, ho
+00001540: 7765 7665 722c 204f 4944 4320 746f 6b65  wever, OIDC toke
+00001550: 6e73 2061 7265 2073 686f 7274 2d6c 6976  ns are short-liv
+00001560: 6564 2061 6e64 2061 7265 2075 7375 616c  ed and are usual
+00001570: 6c79 2073 636f 7065 6420 746f 206f 6e6c  ly scoped to onl
+00001580: 7920 7468 6520 7065 726d 6973 7369 6f6e  y the permission
+00001590: 7320 7468 6174 2061 7265 2065 7373 656e  s that are essen
+000015a0: 7469 616c 2074 6f20 6120 776f 726b 666c  tial to a workfl
+000015b0: 6f77 2061 6e64 2074 6875 7320 6865 6c70  ow and thus help
+000015c0: 2072 6564 7563 6520 7468 6520 6174 7461   reduce the atta
+000015d0: 636b 2073 7572 6661 6365 2e0a 0a31 302e  ck surface...10.
+000015e0: 204e 616d 653a 2060 6368 6563 6b5f 666f   Name: `check_fo
+000015f0: 725f 6372 6561 7465 5f6f 725f 6170 7072  r_create_or_appr
+00001600: 6f76 655f 7075 6c6c 5f72 6571 7565 7374  ove_pull_request
+00001610: 602c 204c 6576 656c 3a20 6057 4152 4e60  `, Level: `WARN`
+00001620: 0a0a 2020 2020 2d20 5468 6973 2063 6865  ..    - This che
+00001630: 636b 206c 6f6f 6b73 2066 6f72 2041 6374  ck looks for Act
+00001640: 696f 6e20 7468 6174 2068 6176 6520 6c6f  ion that have lo
+00001650: 6769 6320 7265 6c61 7465 6420 746f 2063  gic related to c
+00001660: 7265 6174 696e 6720 6f72 2069 6d70 726f  reating or impro
+00001670: 7669 6e67 2070 756c 6c20 7265 7175 6573  ving pull reques
+00001680: 7473 2e20 4372 6561 7469 6e67 206f 7220  ts. Creating or 
+00001690: 6170 7072 6f76 696e 6720 7075 6c6c 2072  approving pull r
+000016a0: 6571 7565 7374 7320 7669 6120 6175 746f  equests via auto
+000016b0: 6d61 7469 6f6e 2070 6f73 6573 2061 2073  mation poses a s
+000016c0: 6563 7572 6974 7920 7269 736b 2069 6620  ecurity risk if 
+000016d0: 7375 6666 6963 6965 6e74 2063 6f6e 7472  sufficient contr
+000016e0: 6f6c 7320 6172 656e 2774 2069 6e20 706c  ols aren't in pl
+000016f0: 6163 6520 746f 2070 726f 7465 6374 2061  ace to protect a
+00001700: 6761 696e 7374 206d 616c 6963 696f 7573  gainst malicious
+00001710: 2063 6f64 6520 6265 696e 6720 6d65 7267   code being merg
+00001720: 6564 2069 6e74 6f20 6120 7265 706f 7369  ed into a reposi
+00001730: 746f 7279 2e0a 0a31 312e 204e 616d 653a  tory...11. Name:
+00001740: 2060 6368 6563 6b5f 666f 725f 7265 6d6f   `check_for_remo
+00001750: 7465 5f73 6372 6970 7460 2c20 4c65 7665  te_script`, Leve
+00001760: 6c3a 2060 5741 524e 600a 0a20 2020 202d  l: `WARN`..    -
+00001770: 2054 6869 7320 6368 6563 6b20 6c6f 6f6b   This check look
+00001780: 7320 666f 7220 6120 5552 4c20 696e 2061  s for a URL in a
+00001790: 6e20 696e 6c69 6e65 2073 6372 6970 7420  n inline script 
+000017a0: 6f66 2061 2047 6974 4875 6220 4163 7469  of a GitHub Acti
+000017b0: 6f6e 2077 6869 6368 2075 7375 616c 6c79  on which usually
+000017c0: 2073 6967 6e61 6c73 2074 6865 2069 6e63   signals the inc
+000017d0: 6c75 7369 6f6e 206f 6620 6120 7265 6d6f  lusion of a remo
+000017e0: 7465 2073 6372 6970 7420 7768 6963 6820  te script which 
+000017f0: 6361 6e20 6265 2064 616e 6765 726f 7573  can be dangerous
+00001800: 2e0a 2020 0a31 322e 204e 616d 653a 2060  ..  .12. Name: `
+00001810: 6368 6563 6b5f 666f 725f 7570 6c6f 6164  check_for_upload
+00001820: 5f64 6f77 6e6c 6f61 645f 6172 7469 6661  _download_artifa
+00001830: 6374 5f61 6374 696f 6e60 2c20 4c65 7665  ct_action`, Leve
+00001840: 6c3a 2060 5741 524e 600a 0a20 2020 202d  l: `WARN`..    -
+00001850: 2054 6869 7320 6368 6563 6b20 6973 2065   This check is e
+00001860: 7373 656e 7469 616c 2066 6f72 2069 6465  ssential for ide
+00001870: 6e74 6966 7969 6e67 2061 6e79 2075 7361  ntifying any usa
+00001880: 6765 206f 6620 4769 7448 7562 2773 2075  ge of GitHub's u
+00001890: 706c 6f61 642f 646f 776e 6c6f 6164 2061  pload/download a
+000018a0: 7274 6966 6163 7420 4163 7469 6f6e 2c20  rtifact Action, 
+000018b0: 6173 2069 7420 6361 6e20 706f 7465 6e74  as it can potent
+000018c0: 6961 6c6c 7920 6578 706f 7365 2079 6f75  ially expose you
+000018d0: 7220 776f 726b 666c 6f77 2074 6f20 636f  r workflow to co
+000018e0: 6d70 726f 6d69 7365 6420 6669 6c65 732e  mpromised files.
+000018f0: 2046 6f72 2069 6e73 7461 6e63 652c 2061   For instance, a
+00001900: 6e20 7570 6c6f 6164 6564 2061 7274 6966  n uploaded artif
+00001910: 6163 7420 6d69 6768 7420 636f 6e74 6169  act might contai
+00001920: 6e20 6120 636f 6d70 696c 6564 2062 696e  n a compiled bin
+00001930: 6172 7920 6672 6f6d 2061 2070 7265 7669  ary from a previ
+00001940: 6f75 7320 776f 726b 666c 6f77 2c20 6275  ous workflow, bu
+00001950: 7420 7468 6973 2062 696e 6172 7920 636f  t this binary co
+00001960: 756c 6420 6265 2063 6f6d 7072 6f6d 6973  uld be compromis
+00001970: 6564 2064 7565 2074 6f20 7468 6520 696e  ed due to the in
+00001980: 7472 6f64 7563 7469 6f6e 206f 6620 6d61  troduction of ma
+00001990: 6c69 6369 6f75 7320 6465 7065 6e64 656e  licious dependen
+000019a0: 6369 6573 2064 7572 696e 6720 7468 6520  cies during the 
+000019b0: 636f 6d70 696c 6174 696f 6e20 7068 6173  compilation phas
+000019c0: 652e 2043 6f6e 7365 7175 656e 746c 792c  e. Consequently,
+000019d0: 2069 6620 7468 6973 2074 6169 6e74 6564   if this tainted
+000019e0: 2062 696e 6172 7920 6973 2065 7865 6375   binary is execu
+000019f0: 7465 6420 7769 7468 696e 2061 6e6f 7468  ted within anoth
+00001a00: 6572 2077 6f72 6b66 6c6f 772c 2069 7420  er workflow, it 
+00001a10: 636f 756c 6420 6c65 6164 2074 6f20 7369  could lead to si
+00001a20: 676e 6966 6963 616e 7420 7365 6375 7269  gnificant securi
+00001a30: 7479 2072 6973 6b73 2e20 546f 206d 6974  ty risks. To mit
+00001a40: 6967 6174 6520 7375 6368 2072 6973 6b73  igate such risks
+00001a50: 2c20 6974 2069 7320 6372 7563 6961 6c20  , it is crucial 
+00001a60: 666f 7220 7573 6572 7320 746f 2063 6f6e  for users to con
+00001a70: 6475 6374 2069 6e74 6567 7269 7479 2063  duct integrity c
+00001a80: 6865 636b 7320 6f6e 2061 7274 6966 6163  hecks on artifac
+00001a90: 7473 2062 6566 6f72 6520 636f 6e73 756d  ts before consum
+00001aa0: 7074 696f 6e2e 2054 6869 7320 6368 6563  ption. This chec
+00001ab0: 6b20 7365 7276 6573 2061 7320 6120 7661  k serves as a va
+00001ac0: 6c75 6162 6c65 2072 656d 696e 6465 7220  luable reminder 
+00001ad0: 746f 2072 6569 6e66 6f72 6365 2074 6869  to reinforce thi
+00001ae0: 7320 7365 6375 7269 7479 2070 7261 6374  s security pract
+00001af0: 6963 652e 0a0a 3133 2e20 4e61 6d65 3a20  ice...13. Name: 
+00001b00: 6063 6865 636b 5f66 6f72 5f6e 6f6e 5f67  `check_for_non_g
+00001b10: 6974 6875 625f 6d61 6e61 6765 645f 6163  ithub_managed_ac
+00001b20: 7469 6f6e 7360 2c20 4c65 7665 6c3a 2060  tions`, Level: `
+00001b30: 5741 524e 600a 0a20 2020 202d 2054 6869  WARN`..    - Thi
+00001b40: 7320 6368 6563 6b20 6c6f 6f6b 7320 666f  s check looks fo
+00001b50: 7220 696e 636c 7573 696f 6e20 6f66 206e  r inclusion of n
+00001b60: 6f6e 2047 6974 4875 622d 6d61 6e61 6765  on GitHub-manage
+00001b70: 6420 6163 7469 6f6e 7320 616e 6420 7365  d actions and se
+00001b80: 7276 6573 2061 7320 6120 7265 6d69 6e64  rves as a remind
+00001b90: 6572 2074 6f20 7265 7669 6577 2074 6865  er to review the
+00001ba0: 2073 6563 7572 6974 7920 706f 7374 7572   security postur
+00001bb0: 6520 6f66 2061 6e79 2074 6869 7264 2070  e of any third p
+00001bc0: 6172 7479 2061 6374 696f 6e73 2079 6f75  arty actions you
+00001bd0: 2069 6e63 6c75 6465 2069 6e20 796f 7572   include in your
+00001be0: 2077 6f72 6b66 6c6f 7728 7329 2c20 6573   workflow(s), es
+00001bf0: 7065 6369 616c 6c79 2069 6620 7468 6579  pecially if they
+00001c00: 2061 7265 206e 6f74 2064 6576 656c 6f70   are not develop
+00001c10: 6564 2061 6e64 206d 6169 6e74 6169 6e65  ed and maintaine
+00001c20: 6420 6279 2063 7265 6469 626c 6520 656e  d by credible en
+00001c30: 7469 7469 6573 2e0a 0a23 2323 2320 4175  tities...#### Au
+00001c40: 7869 6c69 6172 7920 4368 6563 6b73 0a0a  xiliary Checks..
+00001c50: 312e 204e 616d 653a 2060 6368 6563 6b5f  1. Name: `check_
+00001c60: 666f 725f 636f 6465 6f77 6e65 7273 5f66  for_codeowners_f
+00001c70: 696c 6560 202d 2063 6865 636b 7320 666f  ile` - checks fo
+00001c80: 7220 6578 6973 7465 6e63 6520 6f66 205b  r existence of [
+00001c90: 434f 4445 4f57 4e45 5253 5d28 6874 7470  CODEOWNERS](http
+00001ca0: 733a 2f2f 646f 6373 2e67 6974 6875 622e  s://docs.github.
+00001cb0: 636f 6d2f 656e 2f72 6570 6f73 6974 6f72  com/en/repositor
+00001cc0: 6965 732f 6d61 6e61 6769 6e67 2d79 6f75  ies/managing-you
+00001cd0: 722d 7265 706f 7369 746f 7279 732d 7365  r-repositorys-se
+00001ce0: 7474 696e 6773 2d61 6e64 2d66 6561 7475  ttings-and-featu
+00001cf0: 7265 732f 6375 7374 6f6d 697a 696e 672d  res/customizing-
+00001d00: 796f 7572 2d72 6570 6f73 6974 6f72 792f  your-repository/
+00001d10: 6162 6f75 742d 636f 6465 2d6f 776e 6572  about-code-owner
+00001d20: 7329 2066 696c 652e 0a0a 2323 2320 5265  s) file...### Re
+00001d30: 6665 7265 6e63 6573 0a0a 2d20 5b53 6563  ferences..- [Sec
+00001d40: 7572 6974 7920 6861 7264 656e 696e 6720  urity hardening 
+00001d50: 666f 7220 4769 7448 7562 2041 6374 696f  for GitHub Actio
+00001d60: 6e73 5d28 6874 7470 733a 2f2f 646f 6373  ns](https://docs
+00001d70: 2e67 6974 6875 622e 636f 6d2f 656e 2f61  .github.com/en/a
+00001d80: 6374 696f 6e73 2f73 6563 7572 6974 792d  ctions/security-
+00001d90: 6775 6964 6573 2f73 6563 7572 6974 792d  guides/security-
+00001da0: 6861 7264 656e 696e 672d 666f 722d 6769  hardening-for-gi
+00001db0: 7468 7562 2d61 6374 696f 6e73 290a       thub-actions).
```

### Comparing `ghast_scanner-1.6.7/pyproject.toml` & `ghast_scanner-1.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.6.7/PKG-INFO` & `ghast_scanner-1.6.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6768 6173  : 2.1.Name: ghas
 00000020: 742d 7363 616e 6e65 720a 5665 7273 696f  t-scanner.Versio
-00000030: 6e3a 2031 2e36 2e37 0a53 756d 6d61 7279  n: 1.6.7.Summary
+00000030: 6e3a 2031 2e36 2e38 0a53 756d 6d61 7279  n: 1.6.8.Summary
 00000040: 3a20 416e 616c 797a 6520 7468 6520 7365  : Analyze the se
 00000050: 6375 7269 7479 2070 6f73 7475 7265 206f  curity posture o
 00000060: 6620 796f 7572 2047 6974 4875 6220 4163  f your GitHub Ac
 00000070: 7469 6f6e 730a 5072 6f6a 6563 742d 5552  tions.Project-UR
 00000080: 4c3a 2044 6f63 756d 656e 7461 7469 6f6e  L: Documentation
 00000090: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
 000000a0: 2e63 6f6d 2f62 696e 3378 6973 6834 3737  .com/bin3xish477
@@ -65,433 +65,482 @@
 00000400: 6973 743a 2070 7974 6573 743d 3d37 2e34  ist: pytest==7.4
 00000410: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
 00000420: 3a20 7079 7961 6d6c 3d3d 362e 300a 4465  : pyyaml==6.0.De
 00000430: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
 00000440: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
 00000450: 6b64 6f77 6e0a 0a23 2067 6861 7374 0a0a  kdown..# ghast..
 00000460: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000470: 223e 3c69 6d67 2077 6964 7468 3d22 3730  "><img width="70
+00000470: 223e 3c69 6d67 2077 6964 7468 3d22 3430  "><img width="40
 00000480: 3022 2061 6c74 3d22 696d 6167 6522 2073  0" alt="image" s
 00000490: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
 000004a0: 7562 2e63 6f6d 2f62 696e 3378 6973 6834  ub.com/bin3xish4
 000004b0: 3737 2f67 6861 7374 2f61 7373 6574 732f  77/ghast/assets/
 000004c0: 3434 3238 3136 3230 2f30 3938 6134 6435  44281620/098a4d5
 000004d0: 362d 3465 6463 2d34 6532 302d 6234 3633  6-4edc-4e20-b463
 000004e0: 2d39 3233 6338 6261 6630 3431 3822 3e3c  -923c8baf0418"><
-000004f0: 2f70 3e0a 0a47 4841 5354 2028 4769 7448  /p>..GHAST (GitH
+000004f0: 2f70 3e0a 0a47 6861 7374 2028 4769 7448  /p>..Ghast (GitH
 00000500: 7562 2041 6374 696f 6e73 2053 7461 7469  ub Actions Stati
 00000510: 6320 416e 616c 7973 6973 2054 6f6f 6c29  c Analysis Tool)
 00000520: 2069 7320 6120 746f 6f6c 2074 6f20 616e   is a tool to an
 00000530: 616c 797a 6520 7468 6520 7365 6375 7269  alyze the securi
 00000540: 7479 2070 6f73 7475 7265 206f 6620 796f  ty posture of yo
 00000550: 7572 2047 6974 4875 6220 4163 7469 6f6e  ur GitHub Action
-00000560: 7320 616e 6420 6974 7320 7375 7272 6f6e  s and its surron
-00000570: 6469 6e67 2065 6e76 6972 6f6e 6d65 6e74  ding environment
-00000580: 2066 6f72 2063 6f6d 6d6f 6e20 7365 6375   for common secu
-00000590: 7269 7479 2076 756c 6e65 7261 6269 6c69  rity vulnerabili
-000005a0: 7469 6573 206f 7220 6d69 7373 696e 6720  ties or missing 
-000005b0: 7365 6375 7269 7479 2063 6f6e 6669 6775  security configu
-000005c0: 7261 7469 6f6e 2e0a 0a3c 7020 616c 6967  ration...<p alig
-000005d0: 6e3d 2263 656e 7465 7222 3e3c 696d 6720  n="center"><img 
-000005e0: 7769 6474 683d 2239 3336 2220 616c 743d  width="936" alt=
-000005f0: 2269 6d61 6765 2220 7372 633d 2268 7474  "image" src="htt
-00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000610: 6269 6e33 7869 7368 3437 372f 6768 6173  bin3xish477/ghas
-00000620: 742f 6173 7365 7473 2f34 3432 3831 3632  t/assets/4428162
-00000630: 302f 3732 3134 3332 6361 2d37 3934 342d  0/721432ca-7944-
-00000640: 3430 6234 2d38 3033 642d 3863 3363 6238  40b4-803d-8c3cb8
-00000650: 3636 3939 3665 223e 3c2f 703e 0a0a 0a23  66996e"></p>...#
-00000660: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00000670: 0a3e 204d 616b 6520 7375 7265 2079 6f75  .> Make sure you
-00000680: 2068 6176 6520 6024 484f 4d45 2f2e 6c6f   have `$HOME/.lo
-00000690: 6361 6c2f 6269 6e60 2069 6e20 796f 7572  cal/bin` in your
-000006a0: 2050 4154 480a 0a60 6060 0a70 7974 686f   PATH..```.pytho
-000006b0: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-000006c0: 6c20 2e0a 6060 600a 0a23 2323 2055 7361  l ..```..### Usa
-000006d0: 6765 0a0a 6060 600a 6768 6173 7420 2d2d  ge..```.ghast --
-000006e0: 6669 6c65 2061 6374 696f 6e2e 796d 6c0a  file action.yml.
-000006f0: 6768 6173 7420 2d64 2064 6972 6563 746f  ghast -d directo
-00000700: 7279 2d77 6974 682d 6163 7469 6f6e 732f  ry-with-actions/
-00000710: 202d 2d76 6572 626f 7365 0a67 6861 7374   --verbose.ghast
-00000720: 202d 2d66 696c 6520 6163 7469 6f6e 2e79   --file action.y
-00000730: 6d6c 202d 2d69 676e 6f72 652d 7761 726e  ml --ignore-warn
-00000740: 696e 6773 0a67 6861 7374 202d 2d6c 6973  ings.ghast --lis
-00000750: 742d 6368 6563 6b73 0a67 6861 7374 202d  t-checks.ghast -
-00000760: 6920 6368 6563 6b5f 666f 725f 696e 6c69  i check_for_inli
-00000770: 6e65 5f73 6372 6970 7420 2d2d 6e6f 2d73  ne_script --no-s
-00000780: 756d 6d61 7279 0a60 6060 0a0a 2323 2320  ummary.```..### 
-00000790: 5573 6520 6067 6861 7374 6020 696e 2059  Use `ghast` in Y
-000007a0: 6f75 7220 4769 7448 7562 2057 6f72 6b66  our GitHub Workf
-000007b0: 6c6f 7773 0a0a 2323 2323 2044 6566 6175  lows..#### Defau
-000007c0: 6c74 2057 6f72 6b66 6c6f 770a 0a60 6060  lt Workflow..```
-000007d0: 7961 6d6c 0a6e 616d 653a 2027 5275 6e47  yaml.name: 'RunG
-000007e0: 6861 7374 270a 6f6e 3a0a 2020 7075 7368  hast'.on:.  push
-000007f0: 3a0a 6a6f 6273 3a0a 2020 5275 6e47 6861  :.jobs:.  RunGha
-00000800: 7374 3a0a 2020 2020 7275 6e73 2d6f 6e3a  st:.    runs-on:
-00000810: 2075 6275 6e74 752d 6c61 7465 7374 0a20   ubuntu-latest. 
-00000820: 2020 2073 7465 7073 3a0a 2020 2020 2d20     steps:.    - 
-00000830: 6e61 6d65 3a20 2243 6865 636b 6f75 7420  name: "Checkout 
-00000840: 7265 706f 220a 2020 2020 2020 7573 6573  repo".      uses
-00000850: 3a20 6163 7469 6f6e 732f 6368 6563 6b6f  : actions/checko
-00000860: 7574 4039 3666 3533 3130 3062 6132 6135  ut@96f53100ba2a5
-00000870: 3434 3965 6237 3164 3265 3636 3034 6262  449eb71d2e6604bb
-00000880: 6364 3934 6239 3434 3962 3520 2320 7633  cd94b9449b5 # v3
-00000890: 2e35 2e33 0a20 2020 202d 206e 616d 653a  .5.3.    - name:
-000008a0: 2022 5275 6e20 4768 6173 7422 0a20 2020   "Run Ghast".   
-000008b0: 2020 2075 7365 733a 2022 6269 6e33 7869     uses: "bin3xi
-000008c0: 7368 3437 372f 6768 6173 7440 3433 6334  sh477/ghast@43c4
-000008d0: 3731 6238 6530 3535 3939 6436 3766 3631  71b8e05599d67f61
-000008e0: 3865 6363 6366 6338 6437 6239 3238 3162  8ecccfc8d7b9281b
-000008f0: 6664 3962 220a 6060 600a 0a23 2323 2053  fd9b".```..### S
-00000900: 6565 2041 6464 6974 696f 6e61 6c20 576f  ee Additional Wo
-00000910: 726b 666c 6f77 2045 7861 6d70 6c65 730a  rkflow Examples.
-00000920: 5b41 6464 6974 696f 6e61 6c20 4768 6173  [Additional Ghas
-00000930: 7420 576f 726b 666c 6f77 2045 7861 6d70  t Workflow Examp
-00000940: 6c65 735d 2845 5841 4d50 4c45 532e 6d64  les](EXAMPLES.md
-00000950: 290a 0a23 2323 2043 6865 636b 7320 5065  )..### Checks Pe
-00000960: 7266 6f72 6d65 6420 6279 2060 6768 6173  rformed by `ghas
-00000970: 7460 0a0a 312e 204e 616d 653a 2060 6368  t`..1. Name: `ch
-00000980: 6563 6b5f 666f 725f 3370 5f61 6374 696f  eck_for_3p_actio
-00000990: 6e73 5f77 6974 686f 7574 5f68 6173 6860  ns_without_hash`
-000009a0: 2c20 4c65 7665 6c3a 2060 4641 494c 600a  , Level: `FAIL`.
-000009b0: 0a20 2020 202d 2054 6869 7320 6368 6563  .    - This chec
-000009c0: 6b20 6964 656e 7469 6669 6573 2061 6e79  k identifies any
-000009d0: 2074 6869 7264 2070 6172 7479 2047 6974   third party Git
-000009e0: 4875 6220 4163 7469 6f6e 7320 696e 2075  Hub Actions in u
-000009f0: 7365 2074 6861 7420 6861 7665 2062 6565  se that have bee
-00000a00: 6e20 7265 6665 7265 6e63 6564 2076 6961  n referenced via
-00000a10: 2061 2076 6572 7369 6f6e 206e 756d 6265   a version numbe
-00000a20: 7220 7375 6368 2061 7320 6076 312e 3160  r such as `v1.1`
-00000a30: 2069 6e73 7465 6164 206f 6620 636f 6d6d   instead of comm
-00000a40: 6974 2053 4841 2068 6161 682e 2055 7369  it SHA haah. Usi
-00000a50: 6e67 2061 2068 6173 6820 6361 6e20 6865  ng a hash can he
-00000a60: 6c70 206d 6974 6967 6174 6520 7375 7070  lp mitigate supp
-00000a70: 6c79 2063 6861 696e 2074 6872 6561 7473  ly chain threats
-00000a80: 2069 6e20 6120 7363 656e 6172 696f 2077   in a scenario w
-00000a90: 6865 7265 2061 2074 6872 6561 7420 6163  here a threat ac
-00000aa0: 746f 7220 6861 7320 636f 6d70 726f 6d69  tor has compromi
-00000ab0: 7365 6420 7468 6520 736f 7572 6365 2072  sed the source r
-00000ac0: 6570 6f73 6974 6f72 7920 7768 6572 6520  epository where 
-00000ad0: 7468 6520 3350 2061 6374 696f 6e20 6c69  the 3P action li
-00000ae0: 7665 732e 0a0a 322e 204e 616d 653a 2060  ves...2. Name: `
-00000af0: 6368 6563 6b5f 666f 725f 616c 6c6f 775f  check_for_allow_
-00000b00: 756e 7365 6375 7265 5f63 6f6d 6d61 6e64  unsecure_command
-00000b10: 7360 2c20 4c65 7665 6c3a 2060 4641 494c  s`, Level: `FAIL
-00000b20: 600a 0a20 2020 202d 2054 6869 7320 6368  `..    - This ch
-00000b30: 6563 6b20 6c6f 6f6b 7320 666f 7220 7468  eck looks for th
-00000b40: 6520 7573 6167 6520 6f66 2065 6e76 6972  e usage of envir
-00000b50: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
-00000b60: 6361 6c6c 6564 2060 4143 5449 4f4e 535f  called `ACTIONS_
-00000b70: 414c 4c4f 575f 554e 5345 4355 5245 5f43  ALLOW_UNSECURE_C
-00000b80: 4f4d 4d41 4e44 5360 2077 6869 6368 2061  OMMANDS` which a
-00000b90: 6c6c 6f77 7320 666f 7220 616e 2041 6374  llows for an Act
-00000ba0: 696f 6e20 746f 2067 6574 2061 6363 6573  ion to get acces
-00000bb0: 7320 746f 2064 616e 6765 726f 7573 2063  s to dangerous c
-00000bc0: 6f6d 6d61 6e64 7320 2860 6765 742d 656e  ommands (`get-en
-00000bd0: 7660 2c20 6061 6464 2d70 6174 6860 2920  v`, `add-path`) 
-00000be0: 7768 6963 6820 6361 6e20 6c65 6164 2074  which can lead t
-00000bf0: 6f20 636f 6465 2069 6e6a 6563 7469 6f6e  o code injection
-00000c00: 2061 6e64 2063 7265 6465 6e74 6961 6c20   and credential 
-00000c10: 7468 6566 7473 206f 7070 6f72 7475 6e69  thefts opportuni
-00000c20: 7469 6573 2e0a 0a33 2e20 4e61 6d65 3a20  ties...3. Name: 
-00000c30: 6063 6865 636b 5f66 6f72 5f63 6163 6865  `check_for_cache
-00000c40: 5f61 6374 696f 6e60 2c20 4c65 7665 6c3a  _action`, Level:
-00000c50: 2060 5741 524e 600a 0a20 2020 202d 2054   `WARN`..    - T
-00000c60: 6869 7320 6368 6563 6b20 6669 6e64 7320  his check finds 
-00000c70: 616e 7920 7573 6167 6520 6f66 2047 6974  any usage of Git
-00000c80: 4875 6227 7320 6361 6368 696e 6720 4163  Hub's caching Ac
-00000c90: 7469 6f6e 2028 6061 6374 696f 6e73 2f63  tion (`actions/c
-00000ca0: 6163 6865 6029 2077 6869 6368 206d 6179  ache`) which may
-00000cb0: 2072 6573 756c 7420 696e 2073 656e 7369   result in sensi
-00000cc0: 7469 7665 2069 6e66 6f72 6d61 7469 6f6e  tive information
-00000cd0: 2064 6973 636c 6f73 7572 6520 6f72 2063   disclosure or c
-00000ce0: 6163 6865 2070 6f69 736f 6e69 6e67 2e0a  ache poisoning..
-00000cf0: 0a34 2e20 4e61 6d65 3a20 6063 6865 636b  .4. Name: `check
-00000d00: 5f66 6f72 5f64 616e 6765 726f 7573 5f77  _for_dangerous_w
-00000d10: 7269 7465 5f70 6572 6d69 7373 696f 6e73  rite_permissions
-00000d20: 602c 204c 6576 656c 3a20 6046 4149 4c60  `, Level: `FAIL`
-00000d30: 0a0a 2020 2020 2d20 5468 6973 2063 6865  ..    - This che
-00000d40: 636b 206c 6f6f 6b73 2066 6f72 2077 7269  ck looks for wri
-00000d50: 7465 2070 6572 6d69 7373 696f 6e73 2067  te permissions g
-00000d60: 7261 6e74 6564 2074 6f20 706f 7465 6e74  ranted to potent
-00000d70: 6961 6c6c 7920 6461 6e67 6572 6f75 7320  ially dangerous 
-00000d80: 7363 6f70 6573 2073 7563 6820 6173 2074  scopes such as t
-00000d90: 6865 2060 636f 6e74 656e 7473 6020 7363  he `contents` sc
-00000da0: 6f70 6520 7768 6963 6820 6d61 7920 616c  ope which may al
-00000db0: 6c6f 7720 616e 2061 6476 6572 7361 7279  low an adversary
-00000dc0: 2077 7269 7465 2063 6f64 6520 696e 746f   write code into
-00000dd0: 2074 6865 2074 6172 6765 7420 7265 706f   the target repo
-00000de0: 7369 746f 7279 2069 6620 7468 6579 2772  sitory if they'r
-00000df0: 6520 6162 6c65 2074 6f20 636f 6d70 726f  e able to compro
-00000e00: 6d69 7365 2074 6865 2077 6f72 6b66 6c6f  mise the workflo
-00000e10: 772e 2049 7427 7320 616c 736f 206c 6f6f  w. It's also loo
-00000e20: 6b73 2066 6f72 2075 7361 6765 206f 6620  ks for usage of 
-00000e30: 7468 6520 6077 7269 7465 2d61 6c6c 6020  the `write-all` 
-00000e40: 7768 6963 6820 6769 7665 7320 7468 6520  which gives the 
-00000e50: 6163 7469 6f6e 2063 6f6d 706c 6574 6520  action complete 
-00000e60: 7772 6974 6520 6163 6365 7373 2074 6f20  write access to 
-00000e70: 616c 6c20 7363 6f70 6573 2e0a 0a35 2e20  all scopes...5. 
-00000e80: 4e61 6d65 3a20 6063 6865 636b 5f66 6f72  Name: `check_for
-00000e90: 5f69 6e6c 696e 655f 7363 7269 7074 602c  _inline_script`,
-00000ea0: 204c 6576 656c 3a20 6057 4152 4e60 0a0a   Level: `WARN`..
-00000eb0: 2020 2020 2d20 5468 6973 2063 6865 636b      - This check
-00000ec0: 2073 696d 706c 7920 7761 726e 7320 7468   simply warns th
-00000ed0: 6174 2079 6f75 2772 6520 7573 696e 6720  at you're using 
-00000ee0: 616e 2069 6e6c 696e 6520 7363 7269 7074  an inline script
-00000ef0: 2069 6e73 7465 6164 206f 6620 4769 7448   instead of GitH
-00000f00: 7562 2041 6374 696f 6e2e 2049 6e6c 696e  ub Action. Inlin
-00000f10: 6520 7363 7269 7074 7320 6172 6520 7375  e scripts are su
-00000f20: 7363 6570 7469 626c 6520 746f 2073 6372  sceptible to scr
-00000f30: 6970 7420 696e 6a65 6374 696f 6e20 6174  ipt injection at
-00000f40: 7461 636b 7320 2861 6e6f 7468 6572 2063  tacks (another c
-00000f50: 6865 636b 2063 6f76 6572 6564 2062 7920  heck covered by 
-00000f60: 6067 6861 7374 6029 2e20 4974 2069 7320  `ghast`). It is 
-00000f70: 7265 636f 6d6d 656e 6465 6420 746f 2077  recommended to w
-00000f80: 7269 7465 2061 6e20 6163 7469 6f6e 2061  rite an action a
-00000f90: 6e64 2070 6173 7320 616e 7920 7265 7175  nd pass any requ
-00000fa0: 6972 6564 2063 6f6e 7465 7874 2076 616c  ired context val
-00000fb0: 7565 7320 6173 2069 6e70 7574 7320 746f  ues as inputs to
-00000fc0: 2074 6861 7420 6163 7469 6f6e 2077 6869   that action whi
-00000fd0: 6368 2072 656d 6f76 6573 2073 6372 6970  ch removes scrip
-00000fe0: 7420 696e 6a65 6374 696f 6e20 7665 6374  t injection vect
-00000ff0: 6f72 2062 6563 6175 7365 2061 6374 696f  or because actio
-00001000: 6e20 696e 7075 7420 6172 6520 7072 6f70  n input are prop
-00001010: 6572 6c79 2074 7265 6174 6564 2061 7320  erly treated as 
-00001020: 6172 6775 6d65 6e74 7320 616e 6420 6172  arguments and ar
-00001030: 6520 6e6f 7420 6576 616c 7561 7465 6420  e not evaluated 
-00001040: 6173 2070 6172 7420 6f66 2061 2073 6372  as part of a scr
-00001050: 6970 742e 0a0a 362e 204e 616d 653a 2060  ipt...6. Name: `
-00001060: 6368 6563 6b5f 666f 725f 7075 6c6c 5f72  check_for_pull_r
-00001070: 6571 7565 7374 5f74 6172 6765 7460 2c20  equest_target`, 
-00001080: 4c65 7665 6c3a 2060 4641 494c 600a 0a20  Level: `FAIL`.. 
-00001090: 2020 202d 2054 6869 7320 6368 6563 6b20     - This check 
-000010a0: 6c6f 6f6b 7320 666f 7220 7468 6520 7573  looks for the us
-000010b0: 6167 6520 6f66 2074 6865 2064 616e 6765  age of the dange
-000010c0: 726f 7573 2065 7665 6e74 2074 7269 6767  rous event trigg
-000010d0: 6572 2060 7075 6c6c 5f72 6571 7565 7374  er `pull_request
-000010e0: 5f74 6172 6765 7460 2077 6869 6368 2061  _target` which a
-000010f0: 6c6c 6f77 7320 776f 726b 666c 6f77 2065  llows workflow e
-00001100: 7865 6375 7469 6f6e 7320 746f 2072 756e  xecutions to run
-00001110: 2069 6e20 7468 6520 636f 6e74 6578 7420   in the context 
-00001120: 6f66 2074 6865 2072 6570 6f73 6974 6f72  of the repositor
-00001130: 7920 7468 6174 2064 6566 696e 6573 2074  y that defines t
-00001140: 6865 2077 6f72 6b66 6c6f 772c 206e 6f74  he workflow, not
-00001150: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-00001160: 7468 6174 2074 6865 2070 756c 6c20 7265  that the pull re
-00001170: 7175 6573 7420 6f72 6967 696e 6174 6564  quest originated
-00001180: 2066 726f 6d2c 2070 6f74 656e 7469 616c   from, potential
-00001190: 6c79 2061 6c6c 6f77 696e 6720 6120 7468  ly allowing a th
-000011a0: 7265 6174 2061 6374 6f72 2074 6f20 6761  reat actor to ga
-000011b0: 696e 2061 6363 6573 7320 746f 2061 2072  in access to a r
-000011c0: 6570 6f73 6974 6f72 6965 7320 7365 6e73  epositories sens
-000011d0: 6974 6976 6520 7365 6372 6574 7321 0a0a  itive secrets!..
-000011e0: 372e 204e 616d 653a 2060 6368 6563 6b5f  7. Name: `check_
-000011f0: 666f 725f 7363 7269 7074 5f69 6e6a 6563  for_script_injec
-00001200: 7469 6f6e 602c 204c 6576 656c 3a20 6046  tion`, Level: `F
-00001210: 4149 4c60 0a0a 2020 2020 2d20 5468 6973  AIL`..    - This
-00001220: 2063 6865 636b 206c 6f6f 6b73 2066 6f72   check looks for
-00001230: 2074 6865 206d 6f73 7420 636f 6d6d 6f6e   the most common
-00001240: 6c79 206b 6e6f 776e 2073 6563 7572 6974  ly known securit
-00001250: 7920 7269 736b 2074 6f20 4769 7448 7562  y risk to GitHub
-00001260: 2041 6374 696f 6e20 2d20 7363 7269 7074   Action - script
-00001270: 2069 6e6a 6563 7469 6f6e 2e20 5363 7269   injection. Scri
-00001280: 7074 2069 6e6a 6563 7469 6f6e 206f 6363  pt injection occ
-00001290: 7572 7320 7768 656e 2061 6e20 6163 7469  urs when an acti
-000012a0: 6f6e 2064 6972 6563 746c 7920 696e 636c  on directly incl
-000012b0: 7564 6573 2028 7573 696e 6720 7468 6520  udes (using the 
-000012c0: 6024 7b7b 202e 2e2e 207d 7d60 2073 796e  `${{ ... }}` syn
-000012d0: 7461 7829 2061 2047 6974 4875 6220 436f  tax) a GitHub Co
-000012e0: 6e74 6578 7420 7661 7269 6162 6c65 2873  ntext variable(s
-000012f0: 2920 696e 2061 6e20 696e 6c69 6e65 2073  ) in an inline s
-00001300: 6372 6970 7420 7468 6174 2063 616e 2062  cript that can b
-00001310: 6520 636f 6e74 726f 6c6c 6564 2062 7920  e controlled by 
-00001320: 616e 2075 6e74 7275 7374 6564 2061 6374  an untrusted act
-00001330: 6f72 2c20 7265 7375 6c74 696e 6720 696e  or, resulting in
-00001340: 2063 6f6d 6d61 6e64 2065 7865 6375 7469   command executi
-00001350: 6f6e 2069 6e20 7468 6520 696e 7465 7270  on in the interp
-00001360: 7265 7465 6420 7368 656c 6c2e 2054 6865  reted shell. The
-00001370: 7365 2075 7365 722d 636f 6e74 726f 6c6c  se user-controll
-00001380: 6162 6c65 2070 6172 616d 6574 6572 7320  able parameters 
-00001390: 7368 6f75 6c64 2062 6520 7061 7373 6564  should be passed
-000013a0: 2069 6e74 6f20 616e 2069 6e6c 696e 6520   into an inline 
-000013b0: 7363 7269 7074 2061 7320 656e 7669 726f  script as enviro
-000013c0: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
-000013d0: 0a0a 382e 204e 616d 653a 2060 6368 6563  ..8. Name: `chec
-000013e0: 6b5f 666f 725f 7365 6c66 5f68 6f73 7465  k_for_self_hoste
-000013f0: 645f 7275 6e6e 6572 7360 2c20 4c65 7665  d_runners`, Leve
-00001400: 6c3a 2060 5741 524e 6020 0a0a 2020 2020  l: `WARN` ..    
-00001410: 2d20 5468 6973 2063 6865 636b 7320 6174  - This checks at
-00001420: 7465 6d70 7473 2074 6f20 6964 656e 7469  tempts to identi
-00001430: 6679 2074 6865 2075 7361 6765 206f 6620  fy the usage of 
-00001440: 7365 6c66 2d68 6f73 7465 6420 7275 6e6e  self-hosted runn
-00001450: 6572 732e 2053 656c 662d 686f 7374 6564  ers. Self-hosted
-00001460: 2072 756e 6e65 7273 2061 7265 2064 616e   runners are dan
-00001470: 6765 726f 7573 2062 6563 6175 7365 2069  gerous because i
-00001480: 6620 7468 6520 4163 7469 6f6e 2069 7320  f the Action is 
-00001490: 636f 6d70 726f 6d69 7365 6420 6974 206d  compromised it m
-000014a0: 6179 2061 6c6c 6f77 2061 2074 6872 6561  ay allow a threa
-000014b0: 7420 6163 746f 7220 746f 2067 6169 6e20  t actor to gain 
-000014c0: 6163 6365 7373 2074 6f20 6f6e 2070 7265  access to on pre
-000014d0: 6d69 7365 2065 6e76 6972 6f6e 6d65 6e74  mise environment
-000014e0: 206f 7220 6573 7461 626c 6973 6820 7065   or establish pe
-000014f0: 7273 6973 7465 6e63 6520 6d65 6368 616e  rsistence mechan
-00001500: 6973 6d73 206f 6e20 6120 7365 7276 6572  isms on a server
-00001510: 2079 6f75 206f 776e 2f72 656e 742e 0a0a   you own/rent...
-00001520: 392e 204e 616d 653a 2060 6368 6563 6b5f  9. Name: `check_
-00001530: 666f 725f 6177 735f 636f 6e66 6967 7572  for_aws_configur
-00001540: 655f 6372 6564 656e 7469 616c 735f 6e6f  e_credentials_no
-00001550: 6e5f 6f69 6463 602c 204c 6576 656c 3a20  n_oidc`, Level: 
-00001560: 6057 4152 4e60 0a0a 2020 2020 2d20 5468  `WARN`..    - Th
-00001570: 6973 2063 6865 636b 7320 6c6f 6f6b 7320  is checks looks 
-00001580: 666f 7220 7468 6520 7573 6167 6520 6f66  for the usage of
-00001590: 2041 5753 2773 2060 6177 732d 6163 7469   AWS's `aws-acti
-000015a0: 6f6e 732f 636f 6e66 6967 7572 652d 6177  ons/configure-aw
-000015b0: 732d 6372 6564 656e 7469 616c 7360 2061  s-credentials` a
-000015c0: 6374 696f 6e20 616e 6420 6174 7465 6d70  ction and attemp
-000015d0: 7473 2074 6f20 6964 656e 7469 6679 206e  ts to identify n
-000015e0: 6f6e 2d4f 4944 4320 6175 7468 656e 7469  on-OIDC authenti
-000015f0: 6361 7469 6f6e 2070 6172 616d 6574 6572  cation parameter
-00001600: 732e 204e 6f6e 2d4f 4944 4320 6175 7468  s. Non-OIDC auth
-00001610: 656e 7469 6361 7469 6f6e 2074 7970 6573  entication types
-00001620: 2061 7265 206c 6573 7320 7365 6375 7265   are less secure
-00001630: 2074 6861 6e20 4f49 4443 2062 6563 6175   than OIDC becau
-00001640: 7365 2074 6865 7920 7265 7175 6972 6520  se they require 
-00001650: 7468 6520 6372 6561 7469 6f6e 206f 6620  the creation of 
-00001660: 6c6f 6e67 2d74 6572 6d20 6372 6564 656e  long-term creden
-00001670: 7469 616c 7320 7768 6963 6820 6361 6e20  tials which can 
-00001680: 6265 2063 6f6d 7072 6f6d 6973 6564 2c20  be compromised, 
-00001690: 686f 7765 7665 722c 204f 4944 4320 746f  however, OIDC to
-000016a0: 6b65 6e73 2061 7265 2073 686f 7274 2d6c  kens are short-l
-000016b0: 6976 6564 2061 6e64 2061 7265 2075 7375  ived and are usu
-000016c0: 616c 6c79 2073 636f 7065 6420 746f 206f  ally scoped to o
-000016d0: 6e6c 7920 7468 6520 7065 726d 6973 7369  nly the permissi
-000016e0: 6f6e 7320 7468 6174 2061 7265 2065 7373  ons that are ess
-000016f0: 656e 7469 616c 2074 6f20 6120 776f 726b  ential to a work
-00001700: 666c 6f77 2061 6e64 2074 6875 7320 6865  flow and thus he
-00001710: 6c70 2072 6564 7563 6520 7468 6520 6174  lp reduce the at
-00001720: 7461 636b 2073 7572 6661 6365 2e0a 0a31  tack surface...1
-00001730: 302e 204e 616d 653a 2060 6368 6563 6b5f  0. Name: `check_
-00001740: 666f 725f 6372 6561 7465 5f6f 725f 6170  for_create_or_ap
-00001750: 7072 6f76 655f 7075 6c6c 5f72 6571 7565  prove_pull_reque
-00001760: 7374 602c 204c 6576 656c 3a20 6057 4152  st`, Level: `WAR
-00001770: 4e60 0a0a 2020 2020 2d20 5468 6973 2063  N`..    - This c
-00001780: 6865 636b 206c 6f6f 6b73 2066 6f72 2041  heck looks for A
-00001790: 6374 696f 6e20 7468 6174 2068 6176 6520  ction that have 
-000017a0: 6c6f 6769 6320 7265 6c61 7465 6420 746f  logic related to
-000017b0: 2063 7265 6174 696e 6720 6f72 2069 6d70   creating or imp
-000017c0: 726f 7669 6e67 2070 756c 6c20 7265 7175  roving pull requ
-000017d0: 6573 7473 2e20 4372 6561 7469 6e67 206f  ests. Creating o
-000017e0: 7220 6170 7072 6f76 696e 6720 7075 6c6c  r approving pull
-000017f0: 2072 6571 7565 7374 7320 7669 6120 6175   requests via au
-00001800: 746f 6d61 7469 6f6e 2070 6f73 6573 2061  tomation poses a
-00001810: 2073 6563 7572 6974 7920 7269 736b 2069   security risk i
-00001820: 6620 7375 6666 6963 6965 6e74 2063 6f6e  f sufficient con
-00001830: 7472 6f6c 7320 6172 656e 2774 2069 6e20  trols aren't in 
-00001840: 706c 6163 6520 746f 2070 726f 7465 6374  place to protect
-00001850: 2061 6761 696e 7374 206d 616c 6963 696f   against malicio
-00001860: 7573 2063 6f64 6520 6265 696e 6720 6d65  us code being me
-00001870: 7267 6564 2069 6e74 6f20 6120 7265 706f  rged into a repo
-00001880: 7369 746f 7279 2e0a 0a31 312e 204e 616d  sitory...11. Nam
-00001890: 653a 2060 6368 6563 6b5f 666f 725f 7265  e: `check_for_re
-000018a0: 6d6f 7465 5f73 6372 6970 7460 2c20 4c65  mote_script`, Le
-000018b0: 7665 6c3a 2060 5741 524e 600a 0a20 2020  vel: `WARN`..   
-000018c0: 202d 2054 6869 7320 6368 6563 6b20 6c6f   - This check lo
-000018d0: 6f6b 7320 666f 7220 6120 5552 4c20 696e  oks for a URL in
-000018e0: 2061 6e20 696e 6c69 6e65 2073 6372 6970   an inline scrip
-000018f0: 7420 6f66 2061 2047 6974 4875 6220 4163  t of a GitHub Ac
-00001900: 7469 6f6e 2077 6869 6368 2075 7375 616c  tion which usual
-00001910: 6c79 2073 6967 6e61 6c73 2074 6865 2069  ly signals the i
-00001920: 6e63 6c75 7369 6f6e 206f 6620 6120 7265  nclusion of a re
-00001930: 6d6f 7465 2073 6372 6970 7420 7768 6963  mote script whic
-00001940: 6820 6361 6e20 6265 2064 616e 6765 726f  h can be dangero
-00001950: 7573 2e0a 2020 0a31 322e 204e 616d 653a  us..  .12. Name:
-00001960: 2060 6368 6563 6b5f 666f 725f 7570 6c6f   `check_for_uplo
-00001970: 6164 5f64 6f77 6e6c 6f61 645f 6172 7469  ad_download_arti
-00001980: 6661 6374 5f61 6374 696f 6e60 2c20 4c65  fact_action`, Le
-00001990: 7665 6c3a 2060 5741 524e 600a 0a20 2020  vel: `WARN`..   
-000019a0: 202d 2054 6869 7320 6368 6563 6b20 6973   - This check is
-000019b0: 2065 7373 656e 7469 616c 2066 6f72 2069   essential for i
-000019c0: 6465 6e74 6966 7969 6e67 2061 6e79 2075  dentifying any u
-000019d0: 7361 6765 206f 6620 4769 7448 7562 2773  sage of GitHub's
-000019e0: 2075 706c 6f61 642f 646f 776e 6c6f 6164   upload/download
-000019f0: 2061 7274 6966 6163 7420 4163 7469 6f6e   artifact Action
-00001a00: 2c20 6173 2069 7420 6361 6e20 706f 7465  , as it can pote
-00001a10: 6e74 6961 6c6c 7920 6578 706f 7365 2079  ntially expose y
-00001a20: 6f75 7220 776f 726b 666c 6f77 2074 6f20  our workflow to 
-00001a30: 636f 6d70 726f 6d69 7365 6420 6669 6c65  compromised file
-00001a40: 732e 2046 6f72 2069 6e73 7461 6e63 652c  s. For instance,
-00001a50: 2061 6e20 7570 6c6f 6164 6564 2061 7274   an uploaded art
-00001a60: 6966 6163 7420 6d69 6768 7420 636f 6e74  ifact might cont
-00001a70: 6169 6e20 6120 636f 6d70 696c 6564 2062  ain a compiled b
-00001a80: 696e 6172 7920 6672 6f6d 2061 2070 7265  inary from a pre
-00001a90: 7669 6f75 7320 776f 726b 666c 6f77 2c20  vious workflow, 
-00001aa0: 6275 7420 7468 6973 2062 696e 6172 7920  but this binary 
-00001ab0: 636f 756c 6420 6265 2063 6f6d 7072 6f6d  could be comprom
-00001ac0: 6973 6564 2064 7565 2074 6f20 7468 6520  ised due to the 
-00001ad0: 696e 7472 6f64 7563 7469 6f6e 206f 6620  introduction of 
-00001ae0: 6d61 6c69 6369 6f75 7320 6465 7065 6e64  malicious depend
-00001af0: 656e 6369 6573 2064 7572 696e 6720 7468  encies during th
-00001b00: 6520 636f 6d70 696c 6174 696f 6e20 7068  e compilation ph
-00001b10: 6173 652e 2043 6f6e 7365 7175 656e 746c  ase. Consequentl
-00001b20: 792c 2069 6620 7468 6973 2074 6169 6e74  y, if this taint
-00001b30: 6564 2062 696e 6172 7920 6973 2065 7865  ed binary is exe
-00001b40: 6375 7465 6420 7769 7468 696e 2061 6e6f  cuted within ano
-00001b50: 7468 6572 2077 6f72 6b66 6c6f 772c 2069  ther workflow, i
-00001b60: 7420 636f 756c 6420 6c65 6164 2074 6f20  t could lead to 
-00001b70: 7369 676e 6966 6963 616e 7420 7365 6375  significant secu
-00001b80: 7269 7479 2072 6973 6b73 2e20 546f 206d  rity risks. To m
-00001b90: 6974 6967 6174 6520 7375 6368 2072 6973  itigate such ris
-00001ba0: 6b73 2c20 6974 2069 7320 6372 7563 6961  ks, it is crucia
-00001bb0: 6c20 666f 7220 7573 6572 7320 746f 2063  l for users to c
-00001bc0: 6f6e 6475 6374 2069 6e74 6567 7269 7479  onduct integrity
-00001bd0: 2063 6865 636b 7320 6f6e 2061 7274 6966   checks on artif
-00001be0: 6163 7473 2062 6566 6f72 6520 636f 6e73  acts before cons
-00001bf0: 756d 7074 696f 6e2e 2054 6869 7320 6368  umption. This ch
-00001c00: 6563 6b20 7365 7276 6573 2061 7320 6120  eck serves as a 
-00001c10: 7661 6c75 6162 6c65 2072 656d 696e 6465  valuable reminde
-00001c20: 7220 746f 2072 6569 6e66 6f72 6365 2074  r to reinforce t
-00001c30: 6869 7320 7365 6375 7269 7479 2070 7261  his security pra
-00001c40: 6374 6963 652e 0a0a 3133 2e20 4e61 6d65  ctice...13. Name
-00001c50: 3a20 6063 6865 636b 5f66 6f72 5f6e 6f6e  : `check_for_non
-00001c60: 5f67 6974 6875 625f 6d61 6e61 6765 645f  _github_managed_
-00001c70: 6163 7469 6f6e 7360 2c20 4c65 7665 6c3a  actions`, Level:
-00001c80: 2060 5741 524e 600a 0a20 2020 202d 2054   `WARN`..    - T
-00001c90: 6869 7320 6368 6563 6b20 6c6f 6f6b 7320  his check looks 
-00001ca0: 666f 7220 696e 636c 7573 696f 6e20 6f66  for inclusion of
-00001cb0: 206e 6f6e 2047 6974 4875 622d 6d61 6e61   non GitHub-mana
-00001cc0: 6765 6420 6163 7469 6f6e 7320 616e 6420  ged actions and 
-00001cd0: 7365 7276 6573 2061 7320 6120 7265 6d69  serves as a remi
-00001ce0: 6e64 6572 2074 6f20 7265 7669 6577 2074  nder to review t
-00001cf0: 6865 2073 6563 7572 6974 7920 706f 7374  he security post
-00001d00: 7572 6520 6f66 2061 6e79 2074 6869 7264  ure of any third
-00001d10: 2070 6172 7479 2061 6374 696f 6e73 2079   party actions y
-00001d20: 6f75 2069 6e63 6c75 6465 2069 6e20 796f  ou include in yo
-00001d30: 7572 2077 6f72 6b66 6c6f 7728 7329 2c20  ur workflow(s), 
-00001d40: 6573 7065 6369 616c 6c79 2069 6620 7468  especially if th
-00001d50: 6579 2061 7265 206e 6f74 2064 6576 656c  ey are not devel
-00001d60: 6f70 6564 2061 6e64 206d 6169 6e74 6169  oped and maintai
-00001d70: 6e65 6420 6279 2063 7265 6469 626c 6520  ned by credible 
-00001d80: 656e 7469 7469 6573 2e0a 0a23 2323 2320  entities...#### 
-00001d90: 4175 7869 6c69 6172 7920 4368 6563 6b73  Auxiliary Checks
-00001da0: 0a0a 312e 204e 616d 653a 2060 6368 6563  ..1. Name: `chec
-00001db0: 6b5f 666f 725f 636f 6465 6f77 6e65 7273  k_for_codeowners
-00001dc0: 5f66 696c 6560 202d 2063 6865 636b 7320  _file` - checks 
-00001dd0: 666f 7220 6578 6973 7465 6e63 6520 6f66  for existence of
-00001de0: 205b 434f 4445 4f57 4e45 5253 5d28 6874   [CODEOWNERS](ht
-00001df0: 7470 733a 2f2f 646f 6373 2e67 6974 6875  tps://docs.githu
-00001e00: 622e 636f 6d2f 656e 2f72 6570 6f73 6974  b.com/en/reposit
-00001e10: 6f72 6965 732f 6d61 6e61 6769 6e67 2d79  ories/managing-y
-00001e20: 6f75 722d 7265 706f 7369 746f 7279 732d  our-repositorys-
-00001e30: 7365 7474 696e 6773 2d61 6e64 2d66 6561  settings-and-fea
-00001e40: 7475 7265 732f 6375 7374 6f6d 697a 696e  tures/customizin
-00001e50: 672d 796f 7572 2d72 6570 6f73 6974 6f72  g-your-repositor
-00001e60: 792f 6162 6f75 742d 636f 6465 2d6f 776e  y/about-code-own
-00001e70: 6572 7329 2066 696c 652e 0a0a 2323 2320  ers) file...### 
-00001e80: 5265 6665 7265 6e63 6573 0a0a 2d20 5b53  References..- [S
-00001e90: 6563 7572 6974 7920 6861 7264 656e 696e  ecurity hardenin
-00001ea0: 6720 666f 7220 4769 7448 7562 2041 6374  g for GitHub Act
-00001eb0: 696f 6e73 5d28 6874 7470 733a 2f2f 646f  ions](https://do
-00001ec0: 6373 2e67 6974 6875 622e 636f 6d2f 656e  cs.github.com/en
-00001ed0: 2f61 6374 696f 6e73 2f73 6563 7572 6974  /actions/securit
-00001ee0: 792d 6775 6964 6573 2f73 6563 7572 6974  y-guides/securit
-00001ef0: 792d 6861 7264 656e 696e 672d 666f 722d  y-hardening-for-
-00001f00: 6769 7468 7562 2d61 6374 696f 6e73 290a  github-actions).
+00000560: 7320 616e 6420 6974 7320 7375 7272 6f75  s and its surrou
+00000570: 6e64 696e 6720 656e 7669 726f 6e6d 656e  nding environmen
+00000580: 7420 666f 7220 636f 6d6d 6f6e 2073 6563  t for common sec
+00000590: 7572 6974 7920 7675 6c6e 6572 6162 696c  urity vulnerabil
+000005a0: 6974 6965 7320 616e 642f 6f72 206d 6973  ities and/or mis
+000005b0: 7369 6e67 2073 6563 7572 6974 7920 636f  sing security co
+000005c0: 6e66 6967 7572 6174 696f 6e2e 2020 596f  nfiguration.  Yo
+000005d0: 7520 6361 6e20 7573 6520 4768 6173 7420  u can use Ghast 
+000005e0: 6173 2061 2073 7461 6e64 2d61 6c6f 6e65  as a stand-alone
+000005f0: 2061 6e61 6c79 7369 7320 746f 6f6c 2076   analysis tool v
+00000600: 6961 2074 6865 2047 6861 7374 2043 4c49  ia the Ghast CLI
+00000610: 206f 7220 6279 2072 756e 6e69 6e67 2047   or by running G
+00000620: 6861 7374 2061 7320 6120 6e61 7469 7665  hast as a native
+00000630: 2047 6974 4875 6220 4163 7469 6f6e 2e0a   GitHub Action..
+00000640: 0a54 6865 2061 6374 696f 6e73 2064 6972  .The actions dir
+00000650: 6563 746f 7279 2068 6173 2073 6f6d 6520  ectory has some 
+00000660: 6578 616d 706c 6520 4769 7448 7562 2041  example GitHub A
+00000670: 6374 696f 6e73 2077 6974 6820 7675 6c6e  ctions with vuln
+00000680: 6572 6162 6c65 2073 7465 7073 2074 6861  erable steps tha
+00000690: 7420 796f 7520 6361 6e20 7573 6520 746f  t you can use to
+000006a0: 2074 6573 742e 0a0a 3c70 2061 6c69 676e   test...<p align
+000006b0: 3d22 6365 6e74 6572 223e 3c69 6d67 2077  ="center"><img w
+000006c0: 6964 7468 3d22 3933 3622 2061 6c74 3d22  idth="936" alt="
+000006d0: 696d 6167 6522 2073 7263 3d22 6874 7470  image" src="http
+000006e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+000006f0: 696e 3378 6973 6834 3737 2f67 6861 7374  in3xish477/ghast
+00000700: 2f61 7373 6574 732f 3434 3238 3136 3230  /assets/44281620
+00000710: 2f37 3231 3433 3263 612d 3739 3434 2d34  /721432ca-7944-4
+00000720: 3062 342d 3830 3364 2d38 6333 6362 3836  0b4-803d-8c3cb86
+00000730: 3639 3936 6522 3e3c 2f70 3e0a 0a0a 2323  6996e"></p>...##
+00000740: 2320 496e 7374 616c 6c20 7468 6520 4768  # Install the Gh
+00000750: 6173 7420 434c 490a 0a3e 204d 616b 6520  ast CLI..> Make 
+00000760: 7375 7265 2079 6f75 2068 6176 6520 6024  sure you have `$
+00000770: 484f 4d45 2f2e 6c6f 6361 6c2f 6269 6e60  HOME/.local/bin`
+00000780: 2069 6e20 796f 7572 2050 4154 480a 0a23   in your PATH..#
+00000790: 2323 2320 5573 696e 6720 5069 700a 0a60  ### Using Pip..`
+000007a0: 6060 0a70 6970 2069 6e73 7461 6c6c 2067  ``.pip install g
+000007b0: 6861 7374 2d73 6361 6e6e 6572 0a60 6060  hast-scanner.```
+000007c0: 0a0a 2323 2323 2057 6974 6820 4769 742f  ..#### With Git/
+000007d0: 5079 7468 6f6e 0a0a 6060 600a 6769 7420  Python..```.git 
+000007e0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
+000007f0: 7468 7562 2e63 6f6d 2f62 696e 3378 6973  thub.com/bin3xis
+00000800: 6834 3737 2f67 6861 7374 2e67 6974 0a70  h477/ghast.git.p
+00000810: 7974 686f 6e33 202d 6d20 7069 7020 696e  ython3 -m pip in
+00000820: 7374 616c 6c20 2e0a 6060 600a 0a23 2323  stall ..```..###
+00000830: 2048 6f77 2074 6f20 7573 6520 7468 6520   How to use the 
+00000840: 4768 6173 7420 434c 490a 0a60 6060 0a67  Ghast CLI..```.g
+00000850: 6861 7374 202d 6820 0909 0909 0923 2067  hast -h .....# g
+00000860: 6574 2068 656c 7020 0a67 6861 7374 202d  et help .ghast -
+00000870: 2d66 696c 6520 6163 7469 6f6e 2e79 6d6c  -file action.yml
+00000880: 2009 0909 2320 7363 616e 2061 2073 7065   ...# scan a spe
+00000890: 6369 6669 6320 776f 726b 666c 6f77 2066  cific workflow f
+000008a0: 696c 650a 6768 6173 7420 2d64 2064 6972  ile.ghast -d dir
+000008b0: 6563 746f 7279 2d77 6974 682d 6163 7469  ectory-with-acti
+000008c0: 6f6e 732f 202d 2d76 6572 626f 7365 0923  ons/ --verbose.#
+000008d0: 2073 6361 6e20 6120 6469 7265 6374 6f72   scan a director
+000008e0: 7920 696e 2076 6572 626f 7365 206d 6f64  y in verbose mod
+000008f0: 650a 6768 6173 7420 2d2d 6669 6c65 2061  e.ghast --file a
+00000900: 6374 696f 6e2e 796d 6c20 2d2d 6967 6e6f  ction.yml --igno
+00000910: 7265 2d77 6172 6e69 6e67 7309 2320 7363  re-warnings.# sc
+00000920: 616e 2061 2073 7065 6369 6669 6320 776f  an a specific wo
+00000930: 726b 666c 6f77 2066 696c 6520 616e 6420  rkflow file and 
+00000940: 6967 6e6f 7265 2077 6172 6e69 6e67 730a  ignore warnings.
+00000950: 6768 6173 7420 2d2d 6c69 7374 2d63 6865  ghast --list-che
+00000960: 636b 7309 0909 0923 206c 6973 7420 616c  cks....# list al
+00000970: 6c20 6b6e 6f77 6e20 6368 6563 6b73 0a67  l known checks.g
+00000980: 6861 7374 202d 6920 6368 6563 6b5f 666f  hast -i check_fo
+00000990: 725f 696e 6c69 6e65 5f73 6372 6970 7420  r_inline_script 
+000009a0: 2d2d 6e6f 2d73 756d 6d61 7279 0923 206f  --no-summary.# o
+000009b0: 6e6c 7920 7275 6e20 6120 7370 6563 6966  nly run a specif
+000009c0: 6963 2063 6865 636b 2061 6e64 2064 6f6e  ic check and don
+000009d0: 2774 2073 686f 7720 746f 6f6c 2073 756d  't show tool sum
+000009e0: 6d61 7279 0a60 6060 0a0a 2323 2323 2053  mary.```..#### S
+000009f0: 6565 2068 6f77 2074 6865 2047 6861 7374  ee how the Ghast
+00000a00: 2043 4c49 2077 6f72 6b73 0a3c 6120 6872   CLI works.<a hr
+00000a10: 6566 3d22 6874 7470 733a 2f2f 6173 6369  ef="https://asci
+00000a20: 696e 656d 612e 6f72 672f 612f 3630 3038  inema.org/a/6008
+00000a30: 3931 3f61 7574 6f70 6c61 793d 3122 2077  91?autoplay=1" w
+00000a40: 6964 7468 3d22 3430 3022 2074 6172 6765  idth="400" targe
+00000a50: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00000a60: 7372 633d 2268 7474 7073 3a2f 2f61 7363  src="https://asc
+00000a70: 6969 6e65 6d61 2e6f 7267 2f61 2f36 3030  iinema.org/a/600
+00000a80: 3839 312e 7376 6722 202f 3e3c 2f61 3e0a  891.svg" /></a>.
+00000a90: 0a23 2323 2055 7365 2060 6768 6173 7460  .### Use `ghast`
+00000aa0: 2069 6e20 596f 7572 2047 6974 4875 6220   in Your GitHub 
+00000ab0: 576f 726b 666c 6f77 730a 0a23 2323 2320  Workflows..#### 
+00000ac0: 4465 6661 756c 7420 576f 726b 666c 6f77  Default Workflow
+00000ad0: 0a0a 6060 6079 616d 6c0a 6e61 6d65 3a20  ..```yaml.name: 
+00000ae0: 2752 756e 4768 6173 7427 0a6f 6e3a 0a20  'RunGhast'.on:. 
+00000af0: 2070 7573 683a 0a6a 6f62 733a 0a20 2052   push:.jobs:.  R
+00000b00: 756e 4768 6173 743a 0a20 2020 2072 756e  unGhast:.    run
+00000b10: 732d 6f6e 3a20 7562 756e 7475 2d6c 6174  s-on: ubuntu-lat
+00000b20: 6573 740a 2020 2020 7374 6570 733a 0a20  est.    steps:. 
+00000b30: 2020 202d 206e 616d 653a 2022 4368 6563     - name: "Chec
+00000b40: 6b6f 7574 2072 6570 6f22 0a20 2020 2020  kout repo".     
+00000b50: 2075 7365 733a 2061 6374 696f 6e73 2f63   uses: actions/c
+00000b60: 6865 636b 6f75 7440 3936 6635 3331 3030  heckout@96f53100
+00000b70: 6261 3261 3534 3439 6562 3731 6432 6536  ba2a5449eb71d2e6
+00000b80: 3630 3462 6263 6439 3462 3934 3439 6235  604bbcd94b9449b5
+00000b90: 2023 2076 332e 352e 330a 2020 2020 2d20   # v3.5.3.    - 
+00000ba0: 6e61 6d65 3a20 2252 756e 2047 6861 7374  name: "Run Ghast
+00000bb0: 220a 2020 2020 2020 7573 6573 3a20 2262  ".      uses: "b
+00000bc0: 696e 3378 6973 6834 3737 2f67 6861 7374  in3xish477/ghast
+00000bd0: 4034 3363 3437 3162 3865 3035 3539 3964  @43c471b8e05599d
+00000be0: 3637 6636 3138 6563 6363 6663 3864 3762  67f618ecccfc8d7b
+00000bf0: 3932 3831 6266 6439 6222 0a60 6060 0a0a  9281bfd9b".```..
+00000c00: 2323 2320 5365 6520 4164 6469 7469 6f6e  ### See Addition
+00000c10: 616c 2057 6f72 6b66 6c6f 7720 4578 616d  al Workflow Exam
+00000c20: 706c 6573 0a5b 4164 6469 7469 6f6e 616c  ples.[Additional
+00000c30: 2047 6861 7374 2057 6f72 6b66 6c6f 7720   Ghast Workflow 
+00000c40: 4578 616d 706c 6573 5d28 4558 414d 504c  Examples](EXAMPL
+00000c50: 4553 2e6d 6429 0a0a 2323 2320 4368 6563  ES.md)..### Chec
+00000c60: 6b73 2050 6572 666f 726d 6564 2062 7920  ks Performed by 
+00000c70: 6067 6861 7374 600a 0a31 2e20 4e61 6d65  `ghast`..1. Name
+00000c80: 3a20 6063 6865 636b 5f66 6f72 5f33 705f  : `check_for_3p_
+00000c90: 6163 7469 6f6e 735f 7769 7468 6f75 745f  actions_without_
+00000ca0: 6861 7368 602c 204c 6576 656c 3a20 6046  hash`, Level: `F
+00000cb0: 4149 4c60 0a0a 2020 2020 2d20 5468 6973  AIL`..    - This
+00000cc0: 2063 6865 636b 2069 6465 6e74 6966 6965   check identifie
+00000cd0: 7320 616e 7920 7468 6972 6420 7061 7274  s any third part
+00000ce0: 7920 4769 7448 7562 2041 6374 696f 6e73  y GitHub Actions
+00000cf0: 2069 6e20 7573 6520 7468 6174 2068 6176   in use that hav
+00000d00: 6520 6265 656e 2072 6566 6572 656e 6365  e been reference
+00000d10: 6420 7669 6120 6120 7665 7273 696f 6e20  d via a version 
+00000d20: 6e75 6d62 6572 2073 7563 6820 6173 2060  number such as `
+00000d30: 7631 2e31 6020 696e 7374 6561 6420 6f66  v1.1` instead of
+00000d40: 2063 6f6d 6d69 7420 5348 4120 6861 6168   commit SHA haah
+00000d50: 2e20 5573 696e 6720 6120 6861 7368 2063  . Using a hash c
+00000d60: 616e 2068 656c 7020 6d69 7469 6761 7465  an help mitigate
+00000d70: 2073 7570 706c 7920 6368 6169 6e20 7468   supply chain th
+00000d80: 7265 6174 7320 696e 2061 2073 6365 6e61  reats in a scena
+00000d90: 7269 6f20 7768 6572 6520 6120 7468 7265  rio where a thre
+00000da0: 6174 2061 6374 6f72 2068 6173 2063 6f6d  at actor has com
+00000db0: 7072 6f6d 6973 6564 2074 6865 2073 6f75  promised the sou
+00000dc0: 7263 6520 7265 706f 7369 746f 7279 2077  rce repository w
+00000dd0: 6865 7265 2074 6865 2033 5020 6163 7469  here the 3P acti
+00000de0: 6f6e 206c 6976 6573 2e0a 0a32 2e20 4e61  on lives...2. Na
+00000df0: 6d65 3a20 6063 6865 636b 5f66 6f72 5f61  me: `check_for_a
+00000e00: 6c6c 6f77 5f75 6e73 6563 7572 655f 636f  llow_unsecure_co
+00000e10: 6d6d 616e 6473 602c 204c 6576 656c 3a20  mmands`, Level: 
+00000e20: 6046 4149 4c60 0a0a 2020 2020 2d20 5468  `FAIL`..    - Th
+00000e30: 6973 2063 6865 636b 206c 6f6f 6b73 2066  is check looks f
+00000e40: 6f72 2074 6865 2075 7361 6765 206f 6620  or the usage of 
+00000e50: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000e60: 6162 6c65 2063 616c 6c65 6420 6041 4354  able called `ACT
+00000e70: 494f 4e53 5f41 4c4c 4f57 5f55 4e53 4543  IONS_ALLOW_UNSEC
+00000e80: 5552 455f 434f 4d4d 414e 4453 6020 7768  URE_COMMANDS` wh
+00000e90: 6963 6820 616c 6c6f 7773 2066 6f72 2061  ich allows for a
+00000ea0: 6e20 4163 7469 6f6e 2074 6f20 6765 7420  n Action to get 
+00000eb0: 6163 6365 7373 2074 6f20 6461 6e67 6572  access to danger
+00000ec0: 6f75 7320 636f 6d6d 616e 6473 2028 6067  ous commands (`g
+00000ed0: 6574 2d65 6e76 602c 2060 6164 642d 7061  et-env`, `add-pa
+00000ee0: 7468 6029 2077 6869 6368 2063 616e 206c  th`) which can l
+00000ef0: 6561 6420 746f 2063 6f64 6520 696e 6a65  ead to code inje
+00000f00: 6374 696f 6e20 616e 6420 6372 6564 656e  ction and creden
+00000f10: 7469 616c 2074 6865 6674 7320 6f70 706f  tial thefts oppo
+00000f20: 7274 756e 6974 6965 732e 0a0a 332e 204e  rtunities...3. N
+00000f30: 616d 653a 2060 6368 6563 6b5f 666f 725f  ame: `check_for_
+00000f40: 6361 6368 655f 6163 7469 6f6e 602c 204c  cache_action`, L
+00000f50: 6576 656c 3a20 6057 4152 4e60 0a0a 2020  evel: `WARN`..  
+00000f60: 2020 2d20 5468 6973 2063 6865 636b 2066    - This check f
+00000f70: 696e 6473 2061 6e79 2075 7361 6765 206f  inds any usage o
+00000f80: 6620 4769 7448 7562 2773 2063 6163 6869  f GitHub's cachi
+00000f90: 6e67 2041 6374 696f 6e20 2860 6163 7469  ng Action (`acti
+00000fa0: 6f6e 732f 6361 6368 6560 2920 7768 6963  ons/cache`) whic
+00000fb0: 6820 6d61 7920 7265 7375 6c74 2069 6e20  h may result in 
+00000fc0: 7365 6e73 6974 6976 6520 696e 666f 726d  sensitive inform
+00000fd0: 6174 696f 6e20 6469 7363 6c6f 7375 7265  ation disclosure
+00000fe0: 206f 7220 6361 6368 6520 706f 6973 6f6e   or cache poison
+00000ff0: 696e 672e 0a0a 342e 204e 616d 653a 2060  ing...4. Name: `
+00001000: 6368 6563 6b5f 666f 725f 6461 6e67 6572  check_for_danger
+00001010: 6f75 735f 7772 6974 655f 7065 726d 6973  ous_write_permis
+00001020: 7369 6f6e 7360 2c20 4c65 7665 6c3a 2060  sions`, Level: `
+00001030: 4641 494c 600a 0a20 2020 202d 2054 6869  FAIL`..    - Thi
+00001040: 7320 6368 6563 6b20 6c6f 6f6b 7320 666f  s check looks fo
+00001050: 7220 7772 6974 6520 7065 726d 6973 7369  r write permissi
+00001060: 6f6e 7320 6772 616e 7465 6420 746f 2070  ons granted to p
+00001070: 6f74 656e 7469 616c 6c79 2064 616e 6765  otentially dange
+00001080: 726f 7573 2073 636f 7065 7320 7375 6368  rous scopes such
+00001090: 2061 7320 7468 6520 6063 6f6e 7465 6e74   as the `content
+000010a0: 7360 2073 636f 7065 2077 6869 6368 206d  s` scope which m
+000010b0: 6179 2061 6c6c 6f77 2061 6e20 6164 7665  ay allow an adve
+000010c0: 7273 6172 7920 7772 6974 6520 636f 6465  rsary write code
+000010d0: 2069 6e74 6f20 7468 6520 7461 7267 6574   into the target
+000010e0: 2072 6570 6f73 6974 6f72 7920 6966 2074   repository if t
+000010f0: 6865 7927 7265 2061 626c 6520 746f 2063  hey're able to c
+00001100: 6f6d 7072 6f6d 6973 6520 7468 6520 776f  ompromise the wo
+00001110: 726b 666c 6f77 2e20 4974 2773 2061 6c73  rkflow. It's als
+00001120: 6f20 6c6f 6f6b 7320 666f 7220 7573 6167  o looks for usag
+00001130: 6520 6f66 2074 6865 2060 7772 6974 652d  e of the `write-
+00001140: 616c 6c60 2077 6869 6368 2067 6976 6573  all` which gives
+00001150: 2074 6865 2061 6374 696f 6e20 636f 6d70   the action comp
+00001160: 6c65 7465 2077 7269 7465 2061 6363 6573  lete write acces
+00001170: 7320 746f 2061 6c6c 2073 636f 7065 732e  s to all scopes.
+00001180: 0a0a 352e 204e 616d 653a 2060 6368 6563  ..5. Name: `chec
+00001190: 6b5f 666f 725f 696e 6c69 6e65 5f73 6372  k_for_inline_scr
+000011a0: 6970 7460 2c20 4c65 7665 6c3a 2060 5741  ipt`, Level: `WA
+000011b0: 524e 600a 0a20 2020 202d 2054 6869 7320  RN`..    - This 
+000011c0: 6368 6563 6b20 7369 6d70 6c79 2077 6172  check simply war
+000011d0: 6e73 2074 6861 7420 796f 7527 7265 2075  ns that you're u
+000011e0: 7369 6e67 2061 6e20 696e 6c69 6e65 2073  sing an inline s
+000011f0: 6372 6970 7420 696e 7374 6561 6420 6f66  cript instead of
+00001200: 2047 6974 4875 6220 4163 7469 6f6e 2e20   GitHub Action. 
+00001210: 496e 6c69 6e65 2073 6372 6970 7473 2061  Inline scripts a
+00001220: 7265 2073 7573 6365 7074 6962 6c65 2074  re susceptible t
+00001230: 6f20 7363 7269 7074 2069 6e6a 6563 7469  o script injecti
+00001240: 6f6e 2061 7474 6163 6b73 2028 616e 6f74  on attacks (anot
+00001250: 6865 7220 6368 6563 6b20 636f 7665 7265  her check covere
+00001260: 6420 6279 2060 6768 6173 7460 292e 2049  d by `ghast`). I
+00001270: 7420 6973 2072 6563 6f6d 6d65 6e64 6564  t is recommended
+00001280: 2074 6f20 7772 6974 6520 616e 2061 6374   to write an act
+00001290: 696f 6e20 616e 6420 7061 7373 2061 6e79  ion and pass any
+000012a0: 2072 6571 7569 7265 6420 636f 6e74 6578   required contex
+000012b0: 7420 7661 6c75 6573 2061 7320 696e 7075  t values as inpu
+000012c0: 7473 2074 6f20 7468 6174 2061 6374 696f  ts to that actio
+000012d0: 6e20 7768 6963 6820 7265 6d6f 7665 7320  n which removes 
+000012e0: 7363 7269 7074 2069 6e6a 6563 7469 6f6e  script injection
+000012f0: 2076 6563 746f 7220 6265 6361 7573 6520   vector because 
+00001300: 6163 7469 6f6e 2069 6e70 7574 2061 7265  action input are
+00001310: 2070 726f 7065 726c 7920 7472 6561 7465   properly treate
+00001320: 6420 6173 2061 7267 756d 656e 7473 2061  d as arguments a
+00001330: 6e64 2061 7265 206e 6f74 2065 7661 6c75  nd are not evalu
+00001340: 6174 6564 2061 7320 7061 7274 206f 6620  ated as part of 
+00001350: 6120 7363 7269 7074 2e0a 0a36 2e20 4e61  a script...6. Na
+00001360: 6d65 3a20 6063 6865 636b 5f66 6f72 5f70  me: `check_for_p
+00001370: 756c 6c5f 7265 7175 6573 745f 7461 7267  ull_request_targ
+00001380: 6574 602c 204c 6576 656c 3a20 6046 4149  et`, Level: `FAI
+00001390: 4c60 0a0a 2020 2020 2d20 5468 6973 2063  L`..    - This c
+000013a0: 6865 636b 206c 6f6f 6b73 2066 6f72 2074  heck looks for t
+000013b0: 6865 2075 7361 6765 206f 6620 7468 6520  he usage of the 
+000013c0: 6461 6e67 6572 6f75 7320 6576 656e 7420  dangerous event 
+000013d0: 7472 6967 6765 7220 6070 756c 6c5f 7265  trigger `pull_re
+000013e0: 7175 6573 745f 7461 7267 6574 6020 7768  quest_target` wh
+000013f0: 6963 6820 616c 6c6f 7773 2077 6f72 6b66  ich allows workf
+00001400: 6c6f 7720 6578 6563 7574 696f 6e73 2074  low executions t
+00001410: 6f20 7275 6e20 696e 2074 6865 2063 6f6e  o run in the con
+00001420: 7465 7874 206f 6620 7468 6520 7265 706f  text of the repo
+00001430: 7369 746f 7279 2074 6861 7420 6465 6669  sitory that defi
+00001440: 6e65 7320 7468 6520 776f 726b 666c 6f77  nes the workflow
+00001450: 2c20 6e6f 7420 7468 6520 7265 706f 7369  , not the reposi
+00001460: 746f 7279 2074 6861 7420 7468 6520 7075  tory that the pu
+00001470: 6c6c 2072 6571 7565 7374 206f 7269 6769  ll request origi
+00001480: 6e61 7465 6420 6672 6f6d 2c20 706f 7465  nated from, pote
+00001490: 6e74 6961 6c6c 7920 616c 6c6f 7769 6e67  ntially allowing
+000014a0: 2061 2074 6872 6561 7420 6163 746f 7220   a threat actor 
+000014b0: 746f 2067 6169 6e20 6163 6365 7373 2074  to gain access t
+000014c0: 6f20 6120 7265 706f 7369 746f 7269 6573  o a repositories
+000014d0: 2073 656e 7369 7469 7665 2073 6563 7265   sensitive secre
+000014e0: 7473 210a 0a37 2e20 4e61 6d65 3a20 6063  ts!..7. Name: `c
+000014f0: 6865 636b 5f66 6f72 5f73 6372 6970 745f  heck_for_script_
+00001500: 696e 6a65 6374 696f 6e60 2c20 4c65 7665  injection`, Leve
+00001510: 6c3a 2060 4641 494c 600a 0a20 2020 202d  l: `FAIL`..    -
+00001520: 2054 6869 7320 6368 6563 6b20 6c6f 6f6b   This check look
+00001530: 7320 666f 7220 7468 6520 6d6f 7374 2063  s for the most c
+00001540: 6f6d 6d6f 6e6c 7920 6b6e 6f77 6e20 7365  ommonly known se
+00001550: 6375 7269 7479 2072 6973 6b20 746f 2047  curity risk to G
+00001560: 6974 4875 6220 4163 7469 6f6e 202d 2073  itHub Action - s
+00001570: 6372 6970 7420 696e 6a65 6374 696f 6e2e  cript injection.
+00001580: 2053 6372 6970 7420 696e 6a65 6374 696f   Script injectio
+00001590: 6e20 6f63 6375 7273 2077 6865 6e20 616e  n occurs when an
+000015a0: 2061 6374 696f 6e20 6469 7265 6374 6c79   action directly
+000015b0: 2069 6e63 6c75 6465 7320 2875 7369 6e67   includes (using
+000015c0: 2074 6865 2060 247b 7b20 2e2e 2e20 7d7d   the `${{ ... }}
+000015d0: 6020 7379 6e74 6178 2920 6120 4769 7448  ` syntax) a GitH
+000015e0: 7562 2043 6f6e 7465 7874 2076 6172 6961  ub Context varia
+000015f0: 626c 6528 7329 2069 6e20 616e 2069 6e6c  ble(s) in an inl
+00001600: 696e 6520 7363 7269 7074 2074 6861 7420  ine script that 
+00001610: 6361 6e20 6265 2063 6f6e 7472 6f6c 6c65  can be controlle
+00001620: 6420 6279 2061 6e20 756e 7472 7573 7465  d by an untruste
+00001630: 6420 6163 746f 722c 2072 6573 756c 7469  d actor, resulti
+00001640: 6e67 2069 6e20 636f 6d6d 616e 6420 6578  ng in command ex
+00001650: 6563 7574 696f 6e20 696e 2074 6865 2069  ecution in the i
+00001660: 6e74 6572 7072 6574 6564 2073 6865 6c6c  nterpreted shell
+00001670: 2e20 5468 6573 6520 7573 6572 2d63 6f6e  . These user-con
+00001680: 7472 6f6c 6c61 626c 6520 7061 7261 6d65  trollable parame
+00001690: 7465 7273 2073 686f 756c 6420 6265 2070  ters should be p
+000016a0: 6173 7365 6420 696e 746f 2061 6e20 696e  assed into an in
+000016b0: 6c69 6e65 2073 6372 6970 7420 6173 2065  line script as e
+000016c0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+000016d0: 626c 6573 2e0a 0a38 2e20 4e61 6d65 3a20  bles...8. Name: 
+000016e0: 6063 6865 636b 5f66 6f72 5f73 656c 665f  `check_for_self_
+000016f0: 686f 7374 6564 5f72 756e 6e65 7273 602c  hosted_runners`,
+00001700: 204c 6576 656c 3a20 6057 4152 4e60 200a   Level: `WARN` .
+00001710: 0a20 2020 202d 2054 6869 7320 6368 6563  .    - This chec
+00001720: 6b73 2061 7474 656d 7074 7320 746f 2069  ks attempts to i
+00001730: 6465 6e74 6966 7920 7468 6520 7573 6167  dentify the usag
+00001740: 6520 6f66 2073 656c 662d 686f 7374 6564  e of self-hosted
+00001750: 2072 756e 6e65 7273 2e20 5365 6c66 2d68   runners. Self-h
+00001760: 6f73 7465 6420 7275 6e6e 6572 7320 6172  osted runners ar
+00001770: 6520 6461 6e67 6572 6f75 7320 6265 6361  e dangerous beca
+00001780: 7573 6520 6966 2074 6865 2041 6374 696f  use if the Actio
+00001790: 6e20 6973 2063 6f6d 7072 6f6d 6973 6564  n is compromised
+000017a0: 2069 7420 6d61 7920 616c 6c6f 7720 6120   it may allow a 
+000017b0: 7468 7265 6174 2061 6374 6f72 2074 6f20  threat actor to 
+000017c0: 6761 696e 2061 6363 6573 7320 746f 206f  gain access to o
+000017d0: 6e20 7072 656d 6973 6520 656e 7669 726f  n premise enviro
+000017e0: 6e6d 656e 7420 6f72 2065 7374 6162 6c69  nment or establi
+000017f0: 7368 2070 6572 7369 7374 656e 6365 206d  sh persistence m
+00001800: 6563 6861 6e69 736d 7320 6f6e 2061 2073  echanisms on a s
+00001810: 6572 7665 7220 796f 7520 6f77 6e2f 7265  erver you own/re
+00001820: 6e74 2e0a 0a39 2e20 4e61 6d65 3a20 6063  nt...9. Name: `c
+00001830: 6865 636b 5f66 6f72 5f61 7773 5f63 6f6e  heck_for_aws_con
+00001840: 6669 6775 7265 5f63 7265 6465 6e74 6961  figure_credentia
+00001850: 6c73 5f6e 6f6e 5f6f 6964 6360 2c20 4c65  ls_non_oidc`, Le
+00001860: 7665 6c3a 2060 5741 524e 600a 0a20 2020  vel: `WARN`..   
+00001870: 202d 2054 6869 7320 6368 6563 6b73 206c   - This checks l
+00001880: 6f6f 6b73 2066 6f72 2074 6865 2075 7361  ooks for the usa
+00001890: 6765 206f 6620 4157 5327 7320 6061 7773  ge of AWS's `aws
+000018a0: 2d61 6374 696f 6e73 2f63 6f6e 6669 6775  -actions/configu
+000018b0: 7265 2d61 7773 2d63 7265 6465 6e74 6961  re-aws-credentia
+000018c0: 6c73 6020 6163 7469 6f6e 2061 6e64 2061  ls` action and a
+000018d0: 7474 656d 7074 7320 746f 2069 6465 6e74  ttempts to ident
+000018e0: 6966 7920 6e6f 6e2d 4f49 4443 2061 7574  ify non-OIDC aut
+000018f0: 6865 6e74 6963 6174 696f 6e20 7061 7261  hentication para
+00001900: 6d65 7465 7273 2e20 4e6f 6e2d 4f49 4443  meters. Non-OIDC
+00001910: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
+00001920: 7479 7065 7320 6172 6520 6c65 7373 2073  types are less s
+00001930: 6563 7572 6520 7468 616e 204f 4944 4320  ecure than OIDC 
+00001940: 6265 6361 7573 6520 7468 6579 2072 6571  because they req
+00001950: 7569 7265 2074 6865 2063 7265 6174 696f  uire the creatio
+00001960: 6e20 6f66 206c 6f6e 672d 7465 726d 2063  n of long-term c
+00001970: 7265 6465 6e74 6961 6c73 2077 6869 6368  redentials which
+00001980: 2063 616e 2062 6520 636f 6d70 726f 6d69   can be compromi
+00001990: 7365 642c 2068 6f77 6576 6572 2c20 4f49  sed, however, OI
+000019a0: 4443 2074 6f6b 656e 7320 6172 6520 7368  DC tokens are sh
+000019b0: 6f72 742d 6c69 7665 6420 616e 6420 6172  ort-lived and ar
+000019c0: 6520 7573 7561 6c6c 7920 7363 6f70 6564  e usually scoped
+000019d0: 2074 6f20 6f6e 6c79 2074 6865 2070 6572   to only the per
+000019e0: 6d69 7373 696f 6e73 2074 6861 7420 6172  missions that ar
+000019f0: 6520 6573 7365 6e74 6961 6c20 746f 2061  e essential to a
+00001a00: 2077 6f72 6b66 6c6f 7720 616e 6420 7468   workflow and th
+00001a10: 7573 2068 656c 7020 7265 6475 6365 2074  us help reduce t
+00001a20: 6865 2061 7474 6163 6b20 7375 7266 6163  he attack surfac
+00001a30: 652e 0a0a 3130 2e20 4e61 6d65 3a20 6063  e...10. Name: `c
+00001a40: 6865 636b 5f66 6f72 5f63 7265 6174 655f  heck_for_create_
+00001a50: 6f72 5f61 7070 726f 7665 5f70 756c 6c5f  or_approve_pull_
+00001a60: 7265 7175 6573 7460 2c20 4c65 7665 6c3a  request`, Level:
+00001a70: 2060 5741 524e 600a 0a20 2020 202d 2054   `WARN`..    - T
+00001a80: 6869 7320 6368 6563 6b20 6c6f 6f6b 7320  his check looks 
+00001a90: 666f 7220 4163 7469 6f6e 2074 6861 7420  for Action that 
+00001aa0: 6861 7665 206c 6f67 6963 2072 656c 6174  have logic relat
+00001ab0: 6564 2074 6f20 6372 6561 7469 6e67 206f  ed to creating o
+00001ac0: 7220 696d 7072 6f76 696e 6720 7075 6c6c  r improving pull
+00001ad0: 2072 6571 7565 7374 732e 2043 7265 6174   requests. Creat
+00001ae0: 696e 6720 6f72 2061 7070 726f 7669 6e67  ing or approving
+00001af0: 2070 756c 6c20 7265 7175 6573 7473 2076   pull requests v
+00001b00: 6961 2061 7574 6f6d 6174 696f 6e20 706f  ia automation po
+00001b10: 7365 7320 6120 7365 6375 7269 7479 2072  ses a security r
+00001b20: 6973 6b20 6966 2073 7566 6669 6369 656e  isk if sufficien
+00001b30: 7420 636f 6e74 726f 6c73 2061 7265 6e27  t controls aren'
+00001b40: 7420 696e 2070 6c61 6365 2074 6f20 7072  t in place to pr
+00001b50: 6f74 6563 7420 6167 6169 6e73 7420 6d61  otect against ma
+00001b60: 6c69 6369 6f75 7320 636f 6465 2062 6569  licious code bei
+00001b70: 6e67 206d 6572 6765 6420 696e 746f 2061  ng merged into a
+00001b80: 2072 6570 6f73 6974 6f72 792e 0a0a 3131   repository...11
+00001b90: 2e20 4e61 6d65 3a20 6063 6865 636b 5f66  . Name: `check_f
+00001ba0: 6f72 5f72 656d 6f74 655f 7363 7269 7074  or_remote_script
+00001bb0: 602c 204c 6576 656c 3a20 6057 4152 4e60  `, Level: `WARN`
+00001bc0: 0a0a 2020 2020 2d20 5468 6973 2063 6865  ..    - This che
+00001bd0: 636b 206c 6f6f 6b73 2066 6f72 2061 2055  ck looks for a U
+00001be0: 524c 2069 6e20 616e 2069 6e6c 696e 6520  RL in an inline 
+00001bf0: 7363 7269 7074 206f 6620 6120 4769 7448  script of a GitH
+00001c00: 7562 2041 6374 696f 6e20 7768 6963 6820  ub Action which 
+00001c10: 7573 7561 6c6c 7920 7369 676e 616c 7320  usually signals 
+00001c20: 7468 6520 696e 636c 7573 696f 6e20 6f66  the inclusion of
+00001c30: 2061 2072 656d 6f74 6520 7363 7269 7074   a remote script
+00001c40: 2077 6869 6368 2063 616e 2062 6520 6461   which can be da
+00001c50: 6e67 6572 6f75 732e 0a20 200a 3132 2e20  ngerous..  .12. 
+00001c60: 4e61 6d65 3a20 6063 6865 636b 5f66 6f72  Name: `check_for
+00001c70: 5f75 706c 6f61 645f 646f 776e 6c6f 6164  _upload_download
+00001c80: 5f61 7274 6966 6163 745f 6163 7469 6f6e  _artifact_action
+00001c90: 602c 204c 6576 656c 3a20 6057 4152 4e60  `, Level: `WARN`
+00001ca0: 0a0a 2020 2020 2d20 5468 6973 2063 6865  ..    - This che
+00001cb0: 636b 2069 7320 6573 7365 6e74 6961 6c20  ck is essential 
+00001cc0: 666f 7220 6964 656e 7469 6679 696e 6720  for identifying 
+00001cd0: 616e 7920 7573 6167 6520 6f66 2047 6974  any usage of Git
+00001ce0: 4875 6227 7320 7570 6c6f 6164 2f64 6f77  Hub's upload/dow
+00001cf0: 6e6c 6f61 6420 6172 7469 6661 6374 2041  nload artifact A
+00001d00: 6374 696f 6e2c 2061 7320 6974 2063 616e  ction, as it can
+00001d10: 2070 6f74 656e 7469 616c 6c79 2065 7870   potentially exp
+00001d20: 6f73 6520 796f 7572 2077 6f72 6b66 6c6f  ose your workflo
+00001d30: 7720 746f 2063 6f6d 7072 6f6d 6973 6564  w to compromised
+00001d40: 2066 696c 6573 2e20 466f 7220 696e 7374   files. For inst
+00001d50: 616e 6365 2c20 616e 2075 706c 6f61 6465  ance, an uploade
+00001d60: 6420 6172 7469 6661 6374 206d 6967 6874  d artifact might
+00001d70: 2063 6f6e 7461 696e 2061 2063 6f6d 7069   contain a compi
+00001d80: 6c65 6420 6269 6e61 7279 2066 726f 6d20  led binary from 
+00001d90: 6120 7072 6576 696f 7573 2077 6f72 6b66  a previous workf
+00001da0: 6c6f 772c 2062 7574 2074 6869 7320 6269  low, but this bi
+00001db0: 6e61 7279 2063 6f75 6c64 2062 6520 636f  nary could be co
+00001dc0: 6d70 726f 6d69 7365 6420 6475 6520 746f  mpromised due to
+00001dd0: 2074 6865 2069 6e74 726f 6475 6374 696f   the introductio
+00001de0: 6e20 6f66 206d 616c 6963 696f 7573 2064  n of malicious d
+00001df0: 6570 656e 6465 6e63 6965 7320 6475 7269  ependencies duri
+00001e00: 6e67 2074 6865 2063 6f6d 7069 6c61 7469  ng the compilati
+00001e10: 6f6e 2070 6861 7365 2e20 436f 6e73 6571  on phase. Conseq
+00001e20: 7565 6e74 6c79 2c20 6966 2074 6869 7320  uently, if this 
+00001e30: 7461 696e 7465 6420 6269 6e61 7279 2069  tainted binary i
+00001e40: 7320 6578 6563 7574 6564 2077 6974 6869  s executed withi
+00001e50: 6e20 616e 6f74 6865 7220 776f 726b 666c  n another workfl
+00001e60: 6f77 2c20 6974 2063 6f75 6c64 206c 6561  ow, it could lea
+00001e70: 6420 746f 2073 6967 6e69 6669 6361 6e74  d to significant
+00001e80: 2073 6563 7572 6974 7920 7269 736b 732e   security risks.
+00001e90: 2054 6f20 6d69 7469 6761 7465 2073 7563   To mitigate suc
+00001ea0: 6820 7269 736b 732c 2069 7420 6973 2063  h risks, it is c
+00001eb0: 7275 6369 616c 2066 6f72 2075 7365 7273  rucial for users
+00001ec0: 2074 6f20 636f 6e64 7563 7420 696e 7465   to conduct inte
+00001ed0: 6772 6974 7920 6368 6563 6b73 206f 6e20  grity checks on 
+00001ee0: 6172 7469 6661 6374 7320 6265 666f 7265  artifacts before
+00001ef0: 2063 6f6e 7375 6d70 7469 6f6e 2e20 5468   consumption. Th
+00001f00: 6973 2063 6865 636b 2073 6572 7665 7320  is check serves 
+00001f10: 6173 2061 2076 616c 7561 626c 6520 7265  as a valuable re
+00001f20: 6d69 6e64 6572 2074 6f20 7265 696e 666f  minder to reinfo
+00001f30: 7263 6520 7468 6973 2073 6563 7572 6974  rce this securit
+00001f40: 7920 7072 6163 7469 6365 2e0a 0a31 332e  y practice...13.
+00001f50: 204e 616d 653a 2060 6368 6563 6b5f 666f   Name: `check_fo
+00001f60: 725f 6e6f 6e5f 6769 7468 7562 5f6d 616e  r_non_github_man
+00001f70: 6167 6564 5f61 6374 696f 6e73 602c 204c  aged_actions`, L
+00001f80: 6576 656c 3a20 6057 4152 4e60 0a0a 2020  evel: `WARN`..  
+00001f90: 2020 2d20 5468 6973 2063 6865 636b 206c    - This check l
+00001fa0: 6f6f 6b73 2066 6f72 2069 6e63 6c75 7369  ooks for inclusi
+00001fb0: 6f6e 206f 6620 6e6f 6e20 4769 7448 7562  on of non GitHub
+00001fc0: 2d6d 616e 6167 6564 2061 6374 696f 6e73  -managed actions
+00001fd0: 2061 6e64 2073 6572 7665 7320 6173 2061   and serves as a
+00001fe0: 2072 656d 696e 6465 7220 746f 2072 6576   reminder to rev
+00001ff0: 6965 7720 7468 6520 7365 6375 7269 7479  iew the security
+00002000: 2070 6f73 7475 7265 206f 6620 616e 7920   posture of any 
+00002010: 7468 6972 6420 7061 7274 7920 6163 7469  third party acti
+00002020: 6f6e 7320 796f 7520 696e 636c 7564 6520  ons you include 
+00002030: 696e 2079 6f75 7220 776f 726b 666c 6f77  in your workflow
+00002040: 2873 292c 2065 7370 6563 6961 6c6c 7920  (s), especially 
+00002050: 6966 2074 6865 7920 6172 6520 6e6f 7420  if they are not 
+00002060: 6465 7665 6c6f 7065 6420 616e 6420 6d61  developed and ma
+00002070: 696e 7461 696e 6564 2062 7920 6372 6564  intained by cred
+00002080: 6962 6c65 2065 6e74 6974 6965 732e 0a0a  ible entities...
+00002090: 2323 2323 2041 7578 696c 6961 7279 2043  #### Auxiliary C
+000020a0: 6865 636b 730a 0a31 2e20 4e61 6d65 3a20  hecks..1. Name: 
+000020b0: 6063 6865 636b 5f66 6f72 5f63 6f64 656f  `check_for_codeo
+000020c0: 776e 6572 735f 6669 6c65 6020 2d20 6368  wners_file` - ch
+000020d0: 6563 6b73 2066 6f72 2065 7869 7374 656e  ecks for existen
+000020e0: 6365 206f 6620 5b43 4f44 454f 574e 4552  ce of [CODEOWNER
+000020f0: 535d 2868 7474 7073 3a2f 2f64 6f63 732e  S](https://docs.
+00002100: 6769 7468 7562 2e63 6f6d 2f65 6e2f 7265  github.com/en/re
+00002110: 706f 7369 746f 7269 6573 2f6d 616e 6167  positories/manag
+00002120: 696e 672d 796f 7572 2d72 6570 6f73 6974  ing-your-reposit
+00002130: 6f72 7973 2d73 6574 7469 6e67 732d 616e  orys-settings-an
+00002140: 642d 6665 6174 7572 6573 2f63 7573 746f  d-features/custo
+00002150: 6d69 7a69 6e67 2d79 6f75 722d 7265 706f  mizing-your-repo
+00002160: 7369 746f 7279 2f61 626f 7574 2d63 6f64  sitory/about-cod
+00002170: 652d 6f77 6e65 7273 2920 6669 6c65 2e0a  e-owners) file..
+00002180: 0a23 2323 2052 6566 6572 656e 6365 730a  .### References.
+00002190: 0a2d 205b 5365 6375 7269 7479 2068 6172  .- [Security har
+000021a0: 6465 6e69 6e67 2066 6f72 2047 6974 4875  dening for GitHu
+000021b0: 6220 4163 7469 6f6e 735d 2868 7474 7073  b Actions](https
+000021c0: 3a2f 2f64 6f63 732e 6769 7468 7562 2e63  ://docs.github.c
+000021d0: 6f6d 2f65 6e2f 6163 7469 6f6e 732f 7365  om/en/actions/se
+000021e0: 6375 7269 7479 2d67 7569 6465 732f 7365  curity-guides/se
+000021f0: 6375 7269 7479 2d68 6172 6465 6e69 6e67  curity-hardening
+00002200: 2d66 6f72 2d67 6974 6875 622d 6163 7469  -for-github-acti
+00002210: 6f6e 7329 0a                             ons).
```


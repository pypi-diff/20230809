# Comparing `tmp/localeet-0.1.6.tar.gz` & `tmp/localeet-0.1.7.tar.gz`

## Comparing `localeet-0.1.6.tar` & `localeet-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 localeet-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 localeet-0.1.6/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.6/.github/workflows/pr.yml
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 localeet-0.1.6/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/__main__.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/get_leetcode_problem.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/get_version.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.6/src/localeet/language_maps.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/get_leetcode_problem_test.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/version_number_test.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum.go
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum.rs
--rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum_details.json
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.6/tests/data/two_sum_essentials.json
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 localeet-0.1.6/LICENSE
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 localeet-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 localeet-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 localeet-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 localeet-0.1.7/.github/workflows/pr.yml
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 localeet-0.1.7/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 localeet-0.1.7/src/localeet/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 localeet-0.1.7/src/localeet/__main__.py
+-rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 localeet-0.1.7/src/localeet/get_leetcode_problem.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 localeet-0.1.7/src/localeet/get_version.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 localeet-0.1.7/src/localeet/language_maps.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/get_leetcode_problem_test.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/version_number_test.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/data/two_sum.go
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/data/two_sum.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/data/two_sum.rs
+-rw-r--r--   0        0        0    20293 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/data/two_sum_details.json
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 localeet-0.1.7/tests/data/two_sum_essentials.json
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 localeet-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 localeet-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 localeet-0.1.7/README.md
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 localeet-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 localeet-0.1.7/PKG-INFO
```

### Comparing `localeet-0.1.6/.pre-commit-config.yaml` & `localeet-0.1.7/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,10 +27,10 @@
         name: Pytest
         always_run: true
         entry: pytest tests -s -vvl
         language: system
         types: [python]
       - id: ruff
         name: Ruff
-        entry: ruff src tests --fix
+        entry: ruff src tests
         language: system
         types: [python]
```

### Comparing `localeet-0.1.6/README.md` & `localeet-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 file opened in it.
 
 Examples of output files:
 * [Python](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.py)
 * [Rust](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.rs)
 * [Go](https://github.com/dannybrown37/localeet/blob/main/tests/data/two_sum.go)
 
-## CLI Args
+## cli args
 
 See the installed version of localeet with:
 
 ```
 localeet --version
 localeet -v
 ```
```

### Comparing `localeet-0.1.6/.github/workflows/pr.yml` & `localeet-0.1.7/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/.github/workflows/pypi.yaml` & `localeet-0.1.7/.github/workflows/pypi.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     - name: pip install localeet
       run: pip install localeet
     - name: Compare Repo and Pip Versions
       run: |
         repo_version=$(grep "__version__" src/localeet/__init__.py | cut -d "'" -f 2)
         echo "Version from __init__.py: $repo_version"
         pip_version=$(localeet --version)
-        echo "Local version: $pip_version"
+        echo "Pip version: $pip_version"
         if [[ $repo_version = $pip_version ]]; then
           echo "Latest version successfully deployed and pip installed"
         else
           echo "Versions do not match! There was an issue with deployment"
           exit 1
         fi
```

### Comparing `localeet-0.1.6/src/localeet/__main__.py` & `localeet-0.1.7/src/localeet/__main__.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/src/localeet/get_leetcode_problem.py` & `localeet-0.1.7/src/localeet/get_leetcode_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,14 +157,17 @@
     output_path.mkdir(parents=True, exist_ok=True)
     regex = r'[-\s]+'  # replace spaces and hyphens with underscores
     file_name = f'{re.sub(regex, "_", title.lower())}.{extension}'
     output_path = output_path / file_name
     header = f'{oc}\n{qid} - {difficulty} - {title}\n\n{question}\n{cc}\n\n'
     content = header + snippet + f'\n{lc} Example test case:\n'
     content += '\n'.join([f'{lc} {d}' for d in test_case.split('\n')])
+    content += f'\n\n{lc} Suggestion to get started:'
+    content += f'\n{lc} 1. write 5-10+ good test cases, including edge cases'
+    content += f'\n{lc} 2. write code to take test cases and call the function'
     content = [c.rstrip() for c in content.split('\n')]
     wrapped_content = []
     for s in content:
         if not s.strip():
             wrapped_content.append('')
             continue
         wrapped_lines = textwrap.wrap(s, width=79)
```

### Comparing `localeet-0.1.6/src/localeet/language_maps.py` & `localeet-0.1.7/src/localeet/language_maps.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/tests/conftest.py` & `localeet-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/tests/get_leetcode_problem_test.py` & `localeet-0.1.7/tests/get_leetcode_problem_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/tests/version_number_test.py` & `localeet-0.1.7/tests/version_number_test.py`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/tests/data/two_sum.go` & `localeet-0.1.7/tests/data/two_sum.go`

 * *Files 13% similar despite different names*

```diff
@@ -28,17 +28,21 @@
 
 `2 <= nums.length <= 104`
 `-109 <= nums[i] <= 109`
 `-109 <= target <= 109`
 Only one valid answer exists.
 
 
-Follow-up: Can you come up with an algorithm that is less than `O(n2) `time
+Follow-up: Can you come up with an algorithm that is less than `O(n2)` time
 complexity?
 */
 
 func twoSum(nums []int, target int) []int {
 
 }
 // Example test case:
 // [2,7,11,15]
 // 9
+
+// Suggestion to get started:
+// 1. write 5-10+ good test cases, including edge cases
+// 2. write code to take test cases and call the function
```

### Comparing `localeet-0.1.6/tests/data/two_sum.py` & `localeet-0.1.7/tests/data/two_sum.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,22 +28,26 @@
 
 `2 <= nums.length <= 104`
 `-109 <= nums[i] <= 109`
 `-109 <= target <= 109`
 Only one valid answer exists.
 
 
-Follow-up: Can you come up with an algorithm that is less than `O(n2) `time
+Follow-up: Can you come up with an algorithm that is less than `O(n2)` time
 complexity?
 """
 
 class Solution(object):
     def twoSum(self, nums, target):
         """
         :type nums: List[int]
         :type target: int
         :rtype: List[int]
         """
 
 # Example test case:
 # [2,7,11,15]
 # 9
+
+# Suggestion to get started:
+# 1. write 5-10+ good test cases, including edge cases
+# 2. write code to take test cases and call the function
```

### Comparing `localeet-0.1.6/tests/data/two_sum.rs` & `localeet-0.1.7/tests/data/two_sum.rs`

 * *Files 12% similar despite different names*

```diff
@@ -28,19 +28,23 @@
 
 `2 <= nums.length <= 104`
 `-109 <= nums[i] <= 109`
 `-109 <= target <= 109`
 Only one valid answer exists.
 
 
-Follow-up: Can you come up with an algorithm that is less than `O(n2) `time
+Follow-up: Can you come up with an algorithm that is less than `O(n2)` time
 complexity?
 */
 
 impl Solution {
     pub fn two_sum(nums: Vec<i32>, target: i32) -> Vec<i32> {
 
     }
 }
 // Example test case:
 // [2,7,11,15]
 // 9
+
+// Suggestion to get started:
+// 1. write 5-10+ good test cases, including edge cases
+// 2. write code to take test cases and call the function
```

### Comparing `localeet-0.1.6/tests/data/two_sum_details.json` & `localeet-0.1.7/tests/data/two_sum_details.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734848484848485%*

 * *Differences: {"'data'": "{'question': {'content': '<p>Given an array of integers <code>nums</code>&nbsp;and an "*

 * *           'integer <code>target</code>, return <em>indices of the two numbers such that they add '*

 * *           'up to <code>target</code></em>.</p>\\n\\n<p>You may assume that each input would have '*

 * *           '<strong><em>exactly</em> one solution</strong>, and you may not use the <em>same</em> '*

 * *           'element twice.</p>\\n\\n<p>You can return the answer in any '*

 * *           'order.</p>\\n\\n<p>&nbsp;< […]*

```diff
@@ -116,45 +116,45 @@
                     "__typename": "CodeSnippetNode",
                     "code": "class Solution {\n  List<int> twoSum(List<int> nums, int target) {\n\n  }\n}",
                     "lang": "Dart",
                     "langSlug": "dart"
                 }
             ],
             "companyTagStats": null,
-            "content": "<p>Given an array of integers <code>nums</code>&nbsp;and an integer <code>target</code>, return <em>indices of the two numbers such that they add up to <code>target</code></em>.</p>\n\n<p>You may assume that each input would have <strong><em>exactly</em> one solution</strong>, and you may not use the <em>same</em> element twice.</p>\n\n<p>You can return the answer in any order.</p>\n\n<p>&nbsp;</p>\n<p><strong class=\"example\">Example 1:</strong></p>\n\n<pre>\n<strong>Input:</strong> nums = [2,7,11,15], target = 9\n<strong>Output:</strong> [0,1]\n<strong>Explanation:</strong> Because nums[0] + nums[1] == 9, we return [0, 1].\n</pre>\n\n<p><strong class=\"example\">Example 2:</strong></p>\n\n<pre>\n<strong>Input:</strong> nums = [3,2,4], target = 6\n<strong>Output:</strong> [1,2]\n</pre>\n\n<p><strong class=\"example\">Example 3:</strong></p>\n\n<pre>\n<strong>Input:</strong> nums = [3,3], target = 6\n<strong>Output:</strong> [0,1]\n</pre>\n\n<p>&nbsp;</p>\n<p><strong>Constraints:</strong></p>\n\n<ul>\n\t<li><code>2 &lt;= nums.length &lt;= 10<sup>4</sup></code></li>\n\t<li><code>-10<sup>9</sup> &lt;= nums[i] &lt;= 10<sup>9</sup></code></li>\n\t<li><code>-10<sup>9</sup> &lt;= target &lt;= 10<sup>9</sup></code></li>\n\t<li><strong>Only one valid answer exists.</strong></li>\n</ul>\n\n<p>&nbsp;</p>\n<strong>Follow-up:&nbsp;</strong>Can you come up with an algorithm that is less than&nbsp;<code>O(n<sup>2</sup>)&nbsp;</code>time complexity?",
+            "content": "<p>Given an array of integers <code>nums</code>&nbsp;and an integer <code>target</code>, return <em>indices of the two numbers such that they add up to <code>target</code></em>.</p>\n\n<p>You may assume that each input would have <strong><em>exactly</em> one solution</strong>, and you may not use the <em>same</em> element twice.</p>\n\n<p>You can return the answer in any order.</p>\n\n<p>&nbsp;</p>\n<p><strong class=\"example\">Example 1:</strong></p>\n\n<pre>\n<strong>Input:</strong> nums = [2,7,11,15], target = 9\n<strong>Output:</strong> [0,1]\n<strong>Explanation:</strong> Because nums[0] + nums[1] == 9, we return [0, 1].\n</pre>\n\n<p><strong class=\"example\">Example 2:</strong></p>\n\n<pre>\n<strong>Input:</strong> nums = [3,2,4], target = 6\n<strong>Output:</strong> [1,2]\n</pre>\n\n<p><strong class=\"example\">Example 3:</strong></p>\n\n<pre>\n<strong>Input:</strong> nums = [3,3], target = 6\n<strong>Output:</strong> [0,1]\n</pre>\n\n<p>&nbsp;</p>\n<p><strong>Constraints:</strong></p>\n\n<ul>\n\t<li><code>2 &lt;= nums.length &lt;= 10<sup>4</sup></code></li>\n\t<li><code>-10<sup>9</sup> &lt;= nums[i] &lt;= 10<sup>9</sup></code></li>\n\t<li><code>-10<sup>9</sup> &lt;= target &lt;= 10<sup>9</sup></code></li>\n\t<li><strong>Only one valid answer exists.</strong></li>\n</ul>\n\n<p>&nbsp;</p>\n<strong>Follow-up:&nbsp;</strong>Can you come up with an algorithm that is less than <code>O(n<sup>2</sup>)</code><font face=\"monospace\">&nbsp;</font>time complexity?",
             "contributors": [],
             "difficulty": "Easy",
-            "dislikes": 1598,
+            "dislikes": 1610,
             "enableRunCode": true,
             "enableTestMode": false,
-            "envInfo": "{\"cpp\": [\"C++\", \"<p>Compiled with <code> clang 11 </code> using the latest C++ 17 standard.</p>\\r\\n\\r\\n<p>Your code is compiled with level two optimization (<code>-O2</code>). <a href=\\\"https://github.com/google/sanitizers/wiki/AddressSanitizer\\\" target=\\\"_blank\\\">AddressSanitizer</a> is also enabled to help detect out-of-bounds and use-after-free bugs.</p>\\r\\n\\r\\n<p>Most standard library headers are already included automatically for your convenience.</p>\"], \"java\": [\"Java\", \"<p><code>OpenJDK 17</code>. Java 8 features such as lambda expressions and stream API can be used. </p>\\r\\n\\r\\n<p>Most standard library headers are already included automatically for your convenience.</p>\\r\\n<p>Includes <code>Pair</code> class from https://docs.oracle.com/javase/8/javafx/api/javafx/util/Pair.html.</p>\"], \"python\": [\"Python\", \"<p><code>Python 2.7.12</code>.</p>\\r\\n\\r\\n<p>Most libraries are already imported automatically for your convenience, such as <a href=\\\"https://docs.python.org/2/library/array.html\\\" target=\\\"_blank\\\">array</a>, <a href=\\\"https://docs.python.org/2/library/bisect.html\\\" target=\\\"_blank\\\">bisect</a>, <a href=\\\"https://docs.python.org/2/library/collections.html\\\" target=\\\"_blank\\\">collections</a>. If you need more libraries, you can import it yourself.</p>\\r\\n\\r\\n<p>For Map/TreeMap data structure, you may use <a href=\\\"http://www.grantjenks.com/docs/sortedcontainers/\\\" target=\\\"_blank\\\">sortedcontainers</a> library.</p>\\r\\n\\r\\n<p>Note that Python 2.7 <a href=\\\"https://www.python.org/dev/peps/pep-0373/\\\" target=\\\"_blank\\\">will not be maintained past 2020</a>. For the latest Python, please choose Python3 instead.</p>\"], \"c\": [\"C\", \"<p>Compiled with <code>gcc 8.2</code> using the gnu11 standard.</p>\\r\\n\\r\\n<p>Your code is compiled with level one optimization (<code>-O1</code>). <a href=\\\"https://github.com/google/sanitizers/wiki/AddressSanitizer\\\" target=\\\"_blank\\\">AddressSanitizer</a> is also enabled to help detect out-of-bounds and use-after-free bugs.</p>\\r\\n\\r\\n<p>Most standard library headers are already included automatically for your convenience.</p>\\r\\n\\r\\n<p>For hash table operations, you may use <a href=\\\"https://troydhanson.github.io/uthash/\\\" target=\\\"_blank\\\">uthash</a>. \\\"uthash.h\\\" is included by default. Below are some examples:</p>\\r\\n\\r\\n<p><b>1. Adding an item to a hash.</b>\\r\\n<pre>\\r\\nstruct hash_entry {\\r\\n    int id;            /* we'll use this field as the key */\\r\\n    char name[10];\\r\\n    UT_hash_handle hh; /* makes this structure hashable */\\r\\n};\\r\\n\\r\\nstruct hash_entry *users = NULL;\\r\\n\\r\\nvoid add_user(struct hash_entry *s) {\\r\\n    HASH_ADD_INT(users, id, s);\\r\\n}\\r\\n</pre>\\r\\n</p>\\r\\n\\r\\n<p><b>2. Looking up an item in a hash:</b>\\r\\n<pre>\\r\\nstruct hash_entry *find_user(int user_id) {\\r\\n    struct hash_entry *s;\\r\\n    HASH_FIND_INT(users, &user_id, s);\\r\\n    return s;\\r\\n}\\r\\n</pre>\\r\\n</p>\\r\\n\\r\\n<p><b>3. Deleting an item in a hash:</b>\\r\\n<pre>\\r\\nvoid delete_user(struct hash_entry *user) {\\r\\n    HASH_DEL(users, user);  \\r\\n}\\r\\n</pre>\\r\\n</p>\"], \"csharp\": [\"C#\", \"<p><a href=\\\"https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-10\\\" target=\\\"_blank\\\">C# 10 with .NET 6 runtime</a></p>\"], \"javascript\": [\"JavaScript\", \"<p><code>Node.js 16.13.2</code>.</p>\\r\\n\\r\\n<p>Your code is run with <code>--harmony</code> flag, enabling <a href=\\\"http://node.green/\\\" target=\\\"_blank\\\">new ES6 features</a>.</p>\\r\\n\\r\\n<p><a href=\\\"https://lodash.com\\\" target=\\\"_blank\\\">lodash.js</a> library is included by default.</p>\\r\\n\\r\\n<p>For Priority Queue / Queue data structures, you may use 5.3.0 version of <a href=\\\"https://github.com/datastructures-js/priority-queue/tree/fb4fdb984834421279aeb081df7af624d17c2a03\\\" target=\\\"_blank\\\">datastructures-js/priority-queue</a> and 4.2.1 version of <a href=\\\"https://github.com/datastructures-js/queue/tree/e63563025a5a805aa16928cb53bcd517bfea9230\\\" target=\\\"_blank\\\">datastructures-js/queue</a>.</p>\"], \"ruby\": [\"Ruby\", \"<p><code>Ruby 3.1</code></p>\\r\\n\\r\\n<p>Some common data structure implementations are provided in the Algorithms module: https://www.rubydoc.info/github/kanwei/algorithms/Algorithms</p>\"], \"swift\": [\"Swift\", \"<p><code>Swift 5.5.2</code>.</p>\"], \"golang\": [\"Go\", \"<p><code>Go 1.18</code></p>\\r\\n<p>Support <a href=\\\"https://github.com/emirpasic/gods/tree/v1.18.1\\\" target=\\\"_blank\\\">https://godoc.org/github.com/emirpasic/gods@v1.18.1</a> library.</p>\"], \"python3\": [\"Python3\", \"<p><code>Python 3.10</code>.</p>\\r\\n\\r\\n<p>Most libraries are already imported automatically for your convenience, such as <a href=\\\"https://docs.python.org/3/library/array.html\\\" target=\\\"_blank\\\">array</a>, <a href=\\\"https://docs.python.org/3/library/bisect.html\\\" target=\\\"_blank\\\">bisect</a>, <a href=\\\"https://docs.python.org/3/library/collections.html\\\" target=\\\"_blank\\\">collections</a>. If you need more libraries, you can import it yourself.</p>\\r\\n\\r\\n<p>For Map/TreeMap data structure, you may use <a href=\\\"http://www.grantjenks.com/docs/sortedcontainers/\\\" target=\\\"_blank\\\">sortedcontainers</a> library.</p>\"], \"scala\": [\"Scala\", \"<p><code>Scala 2.13.7</code>.</p>\"], \"kotlin\": [\"Kotlin\", \"<p><code>Kotlin 1.3.10</code>.</p>\"], \"rust\": [\"Rust\", \"<p><code>Rust 1.58.1</code></p>\\r\\n\\r\\n<p>Supports <a href=\\\"https://crates.io/crates/rand\\\" target=\\\"_blank\\\">rand </a> v0.6\\u00a0from crates.io</p>\"], \"php\": [\"PHP\", \"<p><code>PHP 8.1</code>.</p>\\r\\n<p>With bcmath module</p>\"], \"typescript\": [\"Typescript\", \"<p><code>TypeScript 5.1.6, Node.js 16.13.2</code>.</p>\\r\\n\\r\\n<p>Your code is run with <code>--harmony</code> flag, enabling <a href=\\\"http://node.green/\\\" target=\\\"_blank\\\">new ES2022 features</a>.</p>\\r\\n\\r\\n<p><a href=\\\"https://lodash.com\\\" target=\\\"_blank\\\">lodash.js</a> library is included by default.</p>\"], \"racket\": [\"Racket\", \"<p>Run with <code>Racket 8.3</code>.</p>\"], \"erlang\": [\"Erlang\", \"Erlang/OTP 25.0\"], \"elixir\": [\"Elixir\", \"Elixir 1.13.4 with Erlang/OTP 25.0\"], \"dart\": [\"Dart\", \"<p>Dart 2.17.3</p>\\r\\n\\r\\n<p>Your code will be run directly without compiling</p>\"]}",
+            "envInfo": "{\"cpp\": [\"C++\", \"<p>Compiled with <code> clang 11 </code> using the latest C++ 20 standard.</p>\\r\\n\\r\\n<p>Your code is compiled with level two optimization (<code>-O2</code>). <a href=\\\"https://github.com/google/sanitizers/wiki/AddressSanitizer\\\" target=\\\"_blank\\\">AddressSanitizer</a> is also enabled to help detect out-of-bounds and use-after-free bugs.</p>\\r\\n\\r\\n<p>Most standard library headers are already included automatically for your convenience.</p>\"], \"java\": [\"Java\", \"<p><code>OpenJDK 17</code>. Java 8 features such as lambda expressions and stream API can be used. </p>\\r\\n\\r\\n<p>Most standard library headers are already included automatically for your convenience.</p>\\r\\n<p>Includes <code>Pair</code> class from https://docs.oracle.com/javase/8/javafx/api/javafx/util/Pair.html.</p>\"], \"python\": [\"Python\", \"<p><code>Python 2.7.12</code>.</p>\\r\\n\\r\\n<p>Most libraries are already imported automatically for your convenience, such as <a href=\\\"https://docs.python.org/2/library/array.html\\\" target=\\\"_blank\\\">array</a>, <a href=\\\"https://docs.python.org/2/library/bisect.html\\\" target=\\\"_blank\\\">bisect</a>, <a href=\\\"https://docs.python.org/2/library/collections.html\\\" target=\\\"_blank\\\">collections</a>. If you need more libraries, you can import it yourself.</p>\\r\\n\\r\\n<p>For Map/TreeMap data structure, you may use <a href=\\\"http://www.grantjenks.com/docs/sortedcontainers/\\\" target=\\\"_blank\\\">sortedcontainers</a> library.</p>\\r\\n\\r\\n<p>Note that Python 2.7 <a href=\\\"https://www.python.org/dev/peps/pep-0373/\\\" target=\\\"_blank\\\">will not be maintained past 2020</a>. For the latest Python, please choose Python3 instead.</p>\"], \"c\": [\"C\", \"<p>Compiled with <code>gcc 8.2</code> using the gnu11 standard.</p>\\r\\n\\r\\n<p>Your code is compiled with level one optimization (<code>-O1</code>). <a href=\\\"https://github.com/google/sanitizers/wiki/AddressSanitizer\\\" target=\\\"_blank\\\">AddressSanitizer</a> is also enabled to help detect out-of-bounds and use-after-free bugs.</p>\\r\\n\\r\\n<p>Most standard library headers are already included automatically for your convenience.</p>\\r\\n\\r\\n<p>For hash table operations, you may use <a href=\\\"https://troydhanson.github.io/uthash/\\\" target=\\\"_blank\\\">uthash</a>. \\\"uthash.h\\\" is included by default. Below are some examples:</p>\\r\\n\\r\\n<p><b>1. Adding an item to a hash.</b>\\r\\n<pre>\\r\\nstruct hash_entry {\\r\\n    int id;            /* we'll use this field as the key */\\r\\n    char name[10];\\r\\n    UT_hash_handle hh; /* makes this structure hashable */\\r\\n};\\r\\n\\r\\nstruct hash_entry *users = NULL;\\r\\n\\r\\nvoid add_user(struct hash_entry *s) {\\r\\n    HASH_ADD_INT(users, id, s);\\r\\n}\\r\\n</pre>\\r\\n</p>\\r\\n\\r\\n<p><b>2. Looking up an item in a hash:</b>\\r\\n<pre>\\r\\nstruct hash_entry *find_user(int user_id) {\\r\\n    struct hash_entry *s;\\r\\n    HASH_FIND_INT(users, &user_id, s);\\r\\n    return s;\\r\\n}\\r\\n</pre>\\r\\n</p>\\r\\n\\r\\n<p><b>3. Deleting an item in a hash:</b>\\r\\n<pre>\\r\\nvoid delete_user(struct hash_entry *user) {\\r\\n    HASH_DEL(users, user);  \\r\\n}\\r\\n</pre>\\r\\n</p>\"], \"csharp\": [\"C#\", \"<p><a href=\\\"https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-10\\\" target=\\\"_blank\\\">C# 10 with .NET 6 runtime</a></p>\"], \"javascript\": [\"JavaScript\", \"<p><code>Node.js 16.13.2</code>.</p>\\r\\n\\r\\n<p>Your code is run with <code>--harmony</code> flag, enabling <a href=\\\"http://node.green/\\\" target=\\\"_blank\\\">new ES6 features</a>.</p>\\r\\n\\r\\n<p><a href=\\\"https://lodash.com\\\" target=\\\"_blank\\\">lodash.js</a> library is included by default.</p>\\r\\n\\r\\n<p>For Priority Queue / Queue data structures, you may use 5.3.0 version of <a href=\\\"https://github.com/datastructures-js/priority-queue/tree/fb4fdb984834421279aeb081df7af624d17c2a03\\\" target=\\\"_blank\\\">datastructures-js/priority-queue</a> and 4.2.1 version of <a href=\\\"https://github.com/datastructures-js/queue/tree/e63563025a5a805aa16928cb53bcd517bfea9230\\\" target=\\\"_blank\\\">datastructures-js/queue</a>.</p>\"], \"ruby\": [\"Ruby\", \"<p><code>Ruby 3.1</code></p>\\r\\n\\r\\n<p>Some common data structure implementations are provided in the Algorithms module: https://www.rubydoc.info/github/kanwei/algorithms/Algorithms</p>\"], \"swift\": [\"Swift\", \"<p><code>Swift 5.5.2</code>.</p>\"], \"golang\": [\"Go\", \"<p><code>Go 1.18</code></p>\\r\\n<p>Support <a href=\\\"https://github.com/emirpasic/gods/tree/v1.18.1\\\" target=\\\"_blank\\\">https://godoc.org/github.com/emirpasic/gods@v1.18.1</a> library.</p>\"], \"python3\": [\"Python3\", \"<p><code>Python 3.10</code>.</p>\\r\\n\\r\\n<p>Most libraries are already imported automatically for your convenience, such as <a href=\\\"https://docs.python.org/3/library/array.html\\\" target=\\\"_blank\\\">array</a>, <a href=\\\"https://docs.python.org/3/library/bisect.html\\\" target=\\\"_blank\\\">bisect</a>, <a href=\\\"https://docs.python.org/3/library/collections.html\\\" target=\\\"_blank\\\">collections</a>. If you need more libraries, you can import it yourself.</p>\\r\\n\\r\\n<p>For Map/TreeMap data structure, you may use <a href=\\\"http://www.grantjenks.com/docs/sortedcontainers/\\\" target=\\\"_blank\\\">sortedcontainers</a> library.</p>\"], \"scala\": [\"Scala\", \"<p><code>Scala 2.13.7</code>.</p>\"], \"kotlin\": [\"Kotlin\", \"<p><code>Kotlin 1.3.10</code>.</p>\"], \"rust\": [\"Rust\", \"<p><code>Rust 1.58.1</code></p>\\r\\n\\r\\n<p>Supports <a href=\\\"https://crates.io/crates/rand\\\" target=\\\"_blank\\\">rand </a> v0.6\\u00a0from crates.io</p>\"], \"php\": [\"PHP\", \"<p><code>PHP 8.1</code>.</p>\\r\\n<p>With bcmath module</p>\"], \"typescript\": [\"Typescript\", \"<p><code>TypeScript 5.1.6, Node.js 16.13.2</code>.</p>\\r\\n\\r\\n<p>Your code is run with <code>--harmony</code> flag, enabling <a href=\\\"http://node.green/\\\" target=\\\"_blank\\\">new ES2022 features</a>.</p>\\r\\n\\r\\n<p><a href=\\\"https://lodash.com\\\" target=\\\"_blank\\\">lodash.js</a> library is included by default.</p>\"], \"racket\": [\"Racket\", \"<p>Run with <code>Racket 8.3</code>.</p>\"], \"erlang\": [\"Erlang\", \"Erlang/OTP 25.0\"], \"elixir\": [\"Elixir\", \"Elixir 1.13.4 with Erlang/OTP 25.0\"], \"dart\": [\"Dart\", \"<p>Dart 2.17.3</p>\\r\\n\\r\\n<p>Your code will be run directly without compiling</p>\"]}",
             "hints": [
                 "A really brute force way would be to search for all possible pairs of numbers but that would be too slow. Again, it's best to try out brute force solutions for just for completeness. It is from these brute force solutions that you can come up with optimizations.",
                 "So, if we fix one of the numbers, say <code>x</code>, we have to scan the entire array to find the next number <code>y</code> which is <code>value - x</code> where value is the input parameter. Can we change our array somehow so that this search becomes faster?",
                 "The second train of thought is, without changing the array, can we use additional space somehow? Like maybe a hash map to speed up the search?"
             ],
             "isLiked": null,
             "isPaidOnly": false,
-            "judgeType": "small",
+            "judgeType": "large",
             "judgerAvailable": true,
-            "langToValidPlayground": "{\"cpp\": true, \"java\": true, \"python\": true, \"python3\": true, \"mysql\": false, \"mssql\": false, \"oraclesql\": false, \"c\": false, \"csharp\": false, \"javascript\": false, \"ruby\": false, \"bash\": false, \"swift\": false, \"golang\": false, \"scala\": false, \"html\": false, \"pythonml\": false, \"kotlin\": false, \"rust\": false, \"php\": false, \"typescript\": false, \"racket\": false, \"erlang\": false, \"elixir\": false, \"dart\": false, \"pythondata\": false, \"react\": false}",
+            "langToValidPlayground": "{\"cpp\": true, \"java\": true, \"python\": true, \"python3\": true, \"mysql\": false, \"mssql\": false, \"oraclesql\": false, \"c\": false, \"csharp\": false, \"javascript\": false, \"ruby\": false, \"bash\": false, \"swift\": false, \"golang\": false, \"scala\": false, \"html\": false, \"pythonml\": false, \"kotlin\": false, \"rust\": false, \"php\": false, \"typescript\": false, \"racket\": false, \"erlang\": false, \"elixir\": false, \"dart\": false, \"pythondata\": false, \"react\": false, \"vanillajs\": false}",
             "libraryUrl": null,
-            "likes": 49028,
+            "likes": 49764,
             "metaData": "{\n  \"name\": \"twoSum\",\n  \"params\": [\n    {\n      \"name\": \"nums\",\n      \"type\": \"integer[]\"\n    },\n    {\n      \"name\": \"target\",\n      \"type\": \"integer\"\n    }\n  ],\n  \"return\": {\n    \"type\": \"integer[]\",\n    \"size\": 2\n  },\n  \"manual\": false\n}",
             "mysqlSchemas": [],
             "questionFrontendId": "1",
             "questionId": "1",
             "sampleTestCase": "[2,7,11,15]\n9",
             "similarQuestions": "[{\"title\": \"3Sum\", \"titleSlug\": \"3sum\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"4Sum\", \"titleSlug\": \"4sum\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Two Sum II - Input Array Is Sorted\", \"titleSlug\": \"two-sum-ii-input-array-is-sorted\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Two Sum III - Data structure design\", \"titleSlug\": \"two-sum-iii-data-structure-design\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Subarray Sum Equals K\", \"titleSlug\": \"subarray-sum-equals-k\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Two Sum IV - Input is a BST\", \"titleSlug\": \"two-sum-iv-input-is-a-bst\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Two Sum Less Than K\", \"titleSlug\": \"two-sum-less-than-k\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Max Number of K-Sum Pairs\", \"titleSlug\": \"max-number-of-k-sum-pairs\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Count Good Meals\", \"titleSlug\": \"count-good-meals\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Count Number of Pairs With Absolute Difference K\", \"titleSlug\": \"count-number-of-pairs-with-absolute-difference-k\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Number of Pairs of Strings With Concatenation Equal to Target\", \"titleSlug\": \"number-of-pairs-of-strings-with-concatenation-equal-to-target\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Find All K-Distant Indices in an Array\", \"titleSlug\": \"find-all-k-distant-indices-in-an-array\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"First Letter to Appear Twice\", \"titleSlug\": \"first-letter-to-appear-twice\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Number of Excellent Pairs\", \"titleSlug\": \"number-of-excellent-pairs\", \"difficulty\": \"Hard\", \"translatedTitle\": null}, {\"title\": \"Number of Arithmetic Triplets\", \"titleSlug\": \"number-of-arithmetic-triplets\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Node With Highest Edge Score\", \"titleSlug\": \"node-with-highest-edge-score\", \"difficulty\": \"Medium\", \"translatedTitle\": null}, {\"title\": \"Check Distances Between Same Letters\", \"titleSlug\": \"check-distances-between-same-letters\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Find Subarrays With Equal Sum\", \"titleSlug\": \"find-subarrays-with-equal-sum\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Largest Positive Integer That Exists With Its Negative\", \"titleSlug\": \"largest-positive-integer-that-exists-with-its-negative\", \"difficulty\": \"Easy\", \"translatedTitle\": null}, {\"title\": \"Number of Distinct Averages\", \"titleSlug\": \"number-of-distinct-averages\", \"difficulty\": \"Easy\", \"translatedTitle\": null}]",
             "solution": {
                 "__typename": "ArticleNode",
                 "canSeeDetail": true,
                 "id": "7"
             },
-            "stats": "{\"totalAccepted\": \"10.2M\", \"totalSubmission\": \"20.3M\", \"totalAcceptedRaw\": 10223832, \"totalSubmissionRaw\": 20341518, \"acRate\": \"50.3%\"}",
+            "stats": "{\"totalAccepted\": \"10.4M\", \"totalSubmission\": \"20.6M\", \"totalAcceptedRaw\": 10386184, \"totalSubmissionRaw\": 20618382, \"acRate\": \"50.4%\"}",
             "status": null,
             "title": "Two Sum",
             "titleSlug": "two-sum",
             "topicTags": [
                 {
                     "__typename": "TopicTagNode",
                     "name": "Array",
```

### Comparing `localeet-0.1.6/tests/data/two_sum_essentials.json` & `localeet-0.1.7/tests/data/two_sum_essentials.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'question'": "'Given an array of integers `nums` and an integer `target`, return indices of the "*

 * *               'two numbers such that they add up to `target`.\\nYou may assume that each input '*

 * *               'would have exactly one solution, and you may not use the same element twice.\\nYou '*

 * *               'can return the answer in any order.\\n \\nExample 1:\\n\\nInput: nums = '*

 * *               '[2,7,11,15], target = 9\\nOutput: [0,1]\\nExplanation: Because nums[0] + nums[1] '*

 * *               '== 9, we […]*

```diff
@@ -112,12 +112,12 @@
             "__typename": "CodeSnippetNode",
             "code": "class Solution {\n  List<int> twoSum(List<int> nums, int target) {\n\n  }\n}",
             "lang": "Dart",
             "langSlug": "dart"
         }
     ],
     "difficulty": "Easy",
-    "question": "Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.\nYou may assume that each input would have exactly one solution, and you may not use the same element twice.\nYou can return the answer in any order.\n \nExample 1:\n\nInput: nums = [2,7,11,15], target = 9\nOutput: [0,1]\nExplanation: Because nums[0] + nums[1] == 9, we return [0, 1].\n\nExample 2:\n\nInput: nums = [3,2,4], target = 6\nOutput: [1,2]\n\nExample 3:\n\nInput: nums = [3,3], target = 6\nOutput: [0,1]\n\n \nConstraints:\n\n`2 <= nums.length <= 104`\n`-109 <= nums[i] <= 109`\n`-109 <= target <= 109`\nOnly one valid answer exists.\n\n \nFollow-up: Can you come up with an algorithm that is less than `O(n2) `time complexity?",
+    "question": "Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.\nYou may assume that each input would have exactly one solution, and you may not use the same element twice.\nYou can return the answer in any order.\n \nExample 1:\n\nInput: nums = [2,7,11,15], target = 9\nOutput: [0,1]\nExplanation: Because nums[0] + nums[1] == 9, we return [0, 1].\n\nExample 2:\n\nInput: nums = [3,2,4], target = 6\nOutput: [1,2]\n\nExample 3:\n\nInput: nums = [3,3], target = 6\nOutput: [0,1]\n\n \nConstraints:\n\n`2 <= nums.length <= 104`\n`-109 <= nums[i] <= 109`\n`-109 <= target <= 109`\nOnly one valid answer exists.\n\n \nFollow-up: Can you come up with an algorithm that is less than `O(n2)` time complexity?",
     "question_id": "1",
     "test_case": "[2,7,11,15]\n9",
     "title": "Two Sum"
 }
```

### Comparing `localeet-0.1.6/.gitignore` & `localeet-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `localeet-0.1.6/LICENSE` & `localeet-0.1.7/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012-2023 Scott Chacon and others
+Copyright (c) 2023 Danny Brown
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `localeet-0.1.6/pyproject.toml` & `localeet-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 [project]
 name = "localeet"
 dynamic = [
     "version",
 ]
-description = "A CLI tool to do LeetCode and LeetCode-like exercises"
+description = "A CLI tool to do LeetCode and LeetCode-like exercises locally"
+readme = "README.md"
 authors = [
     { name = "Danny Brown", email = "dannybrown37@gmail.com" }
 ]
 dependencies = [
     "requests",
     "bs4",
     "lxml",
     "click",
 ]
 
+[project.urls]
+homepage = 'https://pypi.org/project/localeet/'
+documentation = 'https://github.com/dannybrown37/localeet#localeet'
+repository = 'https://github.com/dannybrown37/localeet'
+
 [project.scripts]
 localeet = "localeet:main"
 
 [project.optional-dependencies]
 dev = [
   "ruff==0.0.263",
   "pre-commit",
```


# Comparing `tmp/pyflowchart-0.2.3.tar.gz` & `tmp/pyflowchart-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyflowchart/pyflowchart/dist/tmphak1yxlt/pyflowchart-0.2.3.tar", last modified: Mon Feb 14 03:52:37 2022, max compression
+gzip compressed data, was "/home/runner/work/pyflowchart/pyflowchart/dist/.tmp-bhe251x7/pyflowchart-0.3.0.tar", last modified: Wed Aug  9 00:32:07 2023, max compression
```

## Comparing `pyflowchart-0.2.3.tar` & `pyflowchart-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9593 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9015 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/pyflowchart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/pyflowchart/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21008 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/pyflowchart/ast_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     4629 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/pyflowchart/flowchart.py
--rw-r--r--   0 runner    (1001) docker     (121)    13111 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/pyflowchart/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/pyflowchart/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9593 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/pyflowchart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-14 03:52:37.000000 pyflowchart-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-02-14 03:52:25.000000 pyflowchart-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21008 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/ast_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/flowchart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/output_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/pyflowchart/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/pyflowchart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:32:07.000000 pyflowchart-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-09 00:31:58.000000 pyflowchart-0.3.0/setup.py
```

### Comparing `pyflowchart-0.2.3/LICENSE` & `pyflowchart-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowchart-0.2.3/PKG-INFO` & `pyflowchart-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-Metadata-Version: 2.1
-Name: pyflowchart
-Version: 0.2.3
-Summary: Python codes to Flowcharts.
-Home-page: https://github.com/cdfmlr/pyflowchart
-Author: CDFMLR
-Author-email: cdfmlr@outlook.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyFlowchart
 
-PyFlowchart is a package to:
+English | [机翻中文](README_zh-CN.md)
+
+PyFlowchart is a Python package that lets you:
 
-- write flowcharts in the Python language,
-- translate Python source codes into flowcharts.
+- Write flowcharts in Python.
+- Translate Python source code into flowcharts.
 
-PyFlowchart produces flowcharts in [flowchart.js](https://github.com/adrai/flowchart.js) flowchart DSL, a widely used flow chart textual representation. It's easy to convert these flowcharts text into a picture via [flowchart.js.org](http://flowchart.js.org), [francoislaberge/diagrams](https://github.com/francoislaberge/diagrams/#flowchart), or some markdown editors. 
+PyFlowchart produces flowcharts in the [flowchart.js](https://github.com/adrai/flowchart.js)  flowchart DSL, a widely used textual representation of flowcharts. You can convert these flowcharts to images using [flowchart.js.org](http://flowchart.js.org), [francoislaberge/diagrams](https://github.com/francoislaberge/diagrams/#flowchart), or some markdown editors. Alternatively, we  also support an option to output the generated flowchart into a interactive HTML page.
 
 ## Get PyFlowchart
 
 ```sh
-$ pip3 install pyflowchart
+$ pip install pyflowchart
 ```
 
 ## Quick Start
 
-To flowchartlize your python codes in `example.py`，run:
+Want to **flowchart your Python code in `example.py`?** Run this:
 
 ```sh
-$ python3 -m pyflowchart example.py
+$ python -m pyflowchart example.py
 ```
 
-PyFlowchart will output the generated flowchart.js DSL. Go to http://flowchart.js.org or use editors like [Typora](https://support.typora.io/Draw-Diagrams-With-Markdown/#flowcharts) to turn the output code into a rendered diagram.
+> ⚠️ PyFlowchart works with **Python 3.7+**. To check your Python version, run [`python --version`](https://docs.python.org/3/using/cmdline.html#cmdoption-version).
+>
+> If you have both Python 2 and Python 3 installed, you may need to use `python3` instead of `python`. This is becoming less common as [Python 2 is sunsetting](https://www.python.org/doc/sunset-python-2/).
 
-To specify a function (or a method in a class) to flowchartlize:
+PyFlowchart will output the generated flowchart.js DSL. You can convert the output code to a rendered diagram by going to http://flowchart.js.org or using editors like Typora.
+
+**To output a HTML file** containing the generated flowchart:
 
 ```sh
-$ python3 -m pyflowchart example.py -f function_name
+$ python -m pyflowchart example.py -o example.html
+$ # open example.html
+```
+
+Open `example.html` in your browser to see the output in graphical representation.
+
+**To specify a function (or a method in a class) to flowchartlize:**
+
+- Use the `-f` flag to specify the function or method name.
+
+```sh
+$ python -m pyflowchart example.py -f function_name
 # or
-$ python3 -m pyflowchart example.py -f ClassName.method_name
+$ python -m pyflowchart example.py -f ClassName.method_name
 ```
 
-🎉 Now you are ready to enjoy the flowchartlization.
+For example, to flowchartlize the `add()` function in the `MyClass` class, you would use the following command: `python3 -m pyflowchart example.py -f MyClass.add`.
+
+🎉 **Now you are ready to flowchart your code!**
 
-Keep reading this document to learn more usages.
+To learn more about how to use PyFlowchart, keep reading this document.
 
 ## Flowchart in Python
 
-PyFlowchart allows you to write a flowchart in Python which could be translated into the [flowchart.js](https://github.com/adrai/flowchart.js) DSL automatically.
+PyFlowchart lets you write flowcharts in Python, which can be automatically translated into the [flowchart.js](https://github.com/adrai/flowchart.js) DSL.
 
-PyFlowchart supports [flowchart.js](https://github.com/adrai/flowchart.js#node-types) node types:
+The following [flowchart.js node types](https://github.com/adrai/flowchart.js#node-types) are supported:
 
 - StartNode
 - OperationNode
 - ConditionNode
 - InputOutputNode
 - SubroutineNode
 - EndNode
 
-Nodes can be connected by `connect()` method (`connect_{yes|no}` for ConditionNode). An optional second parameter to `connect()` is used to specify the connect_direction.
+To connect nodes, use the `connect()` method. For ConditionNodes, use the `connect_{yes|no}` syntax. You can optionally specify the connect_direction as a second parameter.
 
 Get a Flowchart with your start node and call its `flowchart()` method to generate flowchart.js flowchart DSL：
 
 ```python
 from pyflowchart import *
 
 st = StartNode('a_pyflow_test')
@@ -108,31 +108,37 @@
 cond2->
 cond2(yes)->io3
 io3->e5
 cond2(no)->sub4
 sub4(right)->op1
 ```
 
-Then you can visit http://flowchart.js.org and translate the generated textual representation into SVG flow chart diagrams:
+You can visit http://flowchart.js.org and translate the generated textual representation into SVG flow chart diagrams:
 
 ![screenshot on flowchart.js page](docs/imgs/flowchart-js-org.png)
 
-P.S. Many Markdown editors (for example, Typora) support this flowchart syntax, too (reference: [Typora doc about flowchart](https://support.typora.io/Draw-Diagrams-With-Markdown/#flowcharts)). And if you prefer CLI, see [francoislaberge/diagrams](https://github.com/francoislaberge/diagrams/#flowchart).
+(v0.3.0) You can also use `pyflowchart.output_html` to generate a page similar to the picture above:
+
+```python
+output_html('output.html', 'a_pyflow_test', fc.flowchart())
+```
+
+By the way, many Markdown editors, like Typora, also support this flowchart syntax. For more information, see [the Typora documentation on flowcharts]((https://support.typora.io/Draw-Diagrams-With-Markdown/#flowcharts)). If you prefer the command line, you can use [francoislaberge/diagrams]((https://github.com/francoislaberge/diagrams/#flowchart)).
 
 ### Set Params to Nodes
 
-Since v0.2.0, we support a `Node.set_param(key, value)` method to generate flowchart like this:
+Starting with v0.2.0, you can use the `Node.set_param(key, value)` method to generate flowcharts like this:
 
 ```
 element(param1=value1,param2=value2)=>start: Start
 ```
 
 (See also [adrai/flowchart.js#node-specific-specifiers-by-type](https://github.com/adrai/flowchart.js#node-specific-specifiers-by-type))
 
-And for convenience, there are grammar sugars to set param `align-next=no` for ConditionNodes:
+There is also a shortcut to set the `align-next=no` parameter for ConditionNodes: 
 
 ```python
 cond = ConditionNode("a cond node")
 cond.no_align_next()
 # or do this at __init__:
 cond = ConditionNode("a cond node", align_next=False)
 ```
@@ -144,43 +150,42 @@
 ```
 
 The generated flowchart will look like:
 
 ```
 cond(align-next=no)=>condition: Yes or No?
 ...
-
 cond(yes,right)->op
 ```
 
 ## Python to Flowchart
 
-PyFlowchart can also translate your Python Codes into Flowcharts.
+PyFlowchart can also translate your Python code into flowcharts.
 
-For example, you got a `simple.py`:
+For example, let's say you have a Python file called `simple.py` with the following code:
 
 ```python
 def foo(a, b):
     if a:
         print("a")
     else:
         for i in range(3):
             print("b")
     return a + b
 ```
 
-Run PyFlowchart in CLI to generate flowchart code:
+To generate a flowchart from this code, you can run the following command in the terminal:
 
 ```sh
-$ python3 -m pyflowchart simple.py
+$ python -m pyflowchart simple.py
 
 # output flowchart code.
 ```
 
-Or, in Python
+Or, in Python:
 
 ```python
 >>> from pyflowchart import Flowchart
 >>> with open('simple.py') as f:
 ...     code = f.read()
 ... 
 >>> fc = Flowchart.from_code(code)
@@ -195,26 +200,33 @@
 
 As mentioned above, we use `Flowchart.from_code` to translate Python codes into Flowcharts. The `from_code` is defined as:
 
 ```python
 Flowchart.from_code(code, field="", inner=True, simplify=True, conds_align=False)
 ```
 
-PyFlowchart CLI is a 1:1 interface for this function:
+- `code`: The Python code to be converted into a flowchart.
+- `field`: The name of a field in the code to be converted into a flowchart. If this parameter is not specified, the entire code will be converted.
+- `inner`: If `True`, the body of the field will be parsed as a nested flowchart. If `False`, the body of the field will be parsed as a single node.
+- `simplify`: If `True`, simple If and Loop statements will be simplified. For example, an If statement with a single expression will be converted into a single node.
+- `conds_align`: If `True`, consecutive If statements will be aligned in the flowchart.
+
+PyFlowchart CLI is an interface for this function:
 
 ```sh
-python3 -m pyflowchart [-f FIELD] [-i] [--no-simplify] [--conds-align] code_file
+python -m pyflowchart [-f FIELD] [-i] [--no-simplify] [--conds-align] [-o OUTPUT] code_file
 ```
 
-Let's talk about those three args:
+- `-f FIELD`: The name of the field to be converted into a flowchart.
+- `-i`:  If specified, the body of the field will be parsed as a nested flowchart.
+- `--no-simplify`:  If specified, the If and Loop statements will not be simplified.
+- `--conds-align`: If specified, consecutive If statements will be aligned in the flowchart.
+- `-o OUTPUT`: If specified, output the flowchart to specific file with a format indicating by the extension name. (only support `*.html` for now)
 
-- `field`: str: Specify a field of code to generate a flowchart
-- `inner`: bool:  `True` to parse the body of field; whereas `False` to parse the body as a single object.
-- `simplify`: bool: for If & Loop statements: simplify the one-line-body or not
-- `conds_align`: bool: improve the flowchart of *consecutive If statements* converted from python code. (Beta)
+⚠️ `-o` is not a part of `Flowchart.from_code`. It's `from pyflowchar import output_html`.
 
 ### field
 
 the `field` is the path to a field (i.e. a function) you want to draw a flowchart. 
 
 ```python
 # example.py
@@ -252,113 +264,136 @@
 print(fc.flowchart())
 ```
 
 Or:
 
 ```sh
 # CLI
-python3 -m pyflowchart example.py -f Bar.buzz.g
+python -m pyflowchart example.py -f Bar.buzz.g
 ```
 
 Output result:
 
 ![specify a field](docs/imgs/field.png)
 
 ### inner
 
-`inner` controls parser's behaving. Techly, `inner=True` means parsing `field.body`, while `inner=False` parses `[field]`. So, if  `inner=True`, pyflowchart will look into the field, otherwise, it takes the `field` as a node.
+The `inner` parameter controls how the parser behaves. If `inner=True`, the parser will look into the field and parse its body. If `inner=False`, the parser will take the field as a single node.
 
 ![pyflowchart_inner](docs/imgs/inner.png)
 
-For CLI,  adding an argument `-i`  means `inner=True`, else `inner=False`.
+In CLI, the `-i` argument sets `inner=True`. The absence of `-i` argument implies `inner=False`.
+
+🔧 For developers: Techly, `inner=True` means parsing `field.body`, while `inner=False` parses `[field]`.
 
 ### simplify
 
-simplify is for If & Loop statements: simplify the one-line-body.
+The `simplify` parameter controls whether to simplify If and Loop statements. When `simplify=True`, an If or Loop statements with one-line-body will be simplified into a single node.
 
-For example:
+For example, the following code:
 
 ```python
 # example_simplify.py
 a = 1
 if a == 1:
     print(a)
 while a < 4:
     a = a + 1
 ```
 
-- Default: `simplify=True`:
+Would be converted into the following flowchart when **simplify=True** :
 
 ```python
 flowchart = Flowchart.from_code(example_simplify_py, field="", inner=True)
 print(flowchart.flowchart())
-# SH $ python3 -m pyflowchart example_simplify.py 
+# SH $ python -m pyflowchart example_simplify.py 
 ```
 
 ![simplify result](docs/imgs/simplify.png)
 
-- `simplify=False`:
+And with `simplify=False`:
 
 ```python
 flowchart = Flowchart.from_code(example_simplify_py, field="", inner=True, simplify=False)
 print(flowchart.flowchart())
-# SH $ python3 -m pyflowchart --no-simplify example_simplify.py 
+# SH $ python -m pyflowchart --no-simplify example_simplify.py 
 ```
 
 ![no simplify result](docs/imgs/no-simplify.png)
 
 ### conds-align (Beta)
 
-Improve the flowchart of *consecutive If statements* converted from python code with the new feature of  `v0.2.0`.
+The `conds-align` parameter controls whether consecutive If statements are aligned in the flowchart. When `conds-align=True`, consecutive If statements are aligned in the flowchart.
 
 ```python
 # example-conds-align.py
 if cond1:
 	op1
 if cond2:
 	op2
 if cond3:
 	op3
 op_end
 ```
 
 ![conds-align-result](docs/imgs/conds-align.png)
 
+**Note:** This feature is still in beta and may not work perfectly in all cases.
+
+### output html and images
+
+You can also directly ouput the generated flowchart.js DSL into an html by adding the parameter ```-o output.html``` where you specify an output filename ending in `.html` or `.htm`.
+
+![output-html](docs/imgs/output-html.png)
+
+Opening the `output.html` in your browser will let you visualize the diagrams. You can tweak the code and click run to update the diagram. There are also links to download the current visuals as a  `.svg` or `.png` image.
+
+⚠️ The output file specified will overwrite any file that already has that name.
+
+🐍 To use this feature via Python instead of CLI, call `output_html(output_name: str, field_name: str, flowchart: str) -> None`:
+
+```py
+>>> import pyflowchart
+>>> help(pyflowchart.output_html)
+```
+
 ## Beautify Flowcharts
 
-Sometimes, the generated flowchart is awful. In those cases, you are encouraged to modify the generated flowchart code by yourself OR consider making your python source code at bottom more clear if it's exceedingly complex.
+The flowcharts generated by PyFlowchart may not always be perfect. In these cases, you can modify the generated flowchart code yourself or consider making your Python source code more clear. Clear and beautiful Python source code will result in more beautiful flowcharts generated by PyFlowchart.
+
+An example: If you don't like the flowchart flow direction you can tweak a condition by modifying with with directions such as:
+
+![beautify-flowchart-example](docs/imgs/beautify-example.png)
 
 ## TODOs
 
 - [ ] Directly generate flowchart SVG/HTML:
 
 ```sh
 $ pyflowchart example.py -o flowchart.svg
 ```
 
 Depends on `node.js` and `flowchart.js`.
 
 - [ ] PyFlowchart GUI
 
-Well, I guess a **GUI** for PyFlowchart may be remarkable. Pasting your code into it, the flowchart DSL will be generated just in time, and the flowchart will be shown aside.
+A **GUI** for PyFlowchart would be amazing. You could paste your Python code into it, and the flowchart DSL would be generated in real time, with the flowchart displayed alongside it. You could clearly see how the two are related.
 
 - [ ] ~~The Chinese README your buddies waiting for!~~ 希望有同学帮助贡献个中文 README 呀。
-- [ ] Tests automation.
+- [x] Tests automation.
 
 ----
 
-Sadly, I am too busy (pronounced as `[ˈlеizi]`——lazy) to code these ideas. Please [submit an issue](https://github.com/cdfmlr/pyflowchart/issues/new) to push me on. Or, PR to make it by yourself. I cannot wait to appreciate your great contribution!
+Unfortunately, I am too busy (pronounced as `[ˈlеizi]`——lazy) to code these ideas myself. Please [submit an issue](https://github.com/cdfmlr/pyflowchart/issues/new) to push me on. Or, PR to make it by yourself. I cannot wait to appreciate your great contribution!
 
 ## References
 
 - Inspired by [Vatsha/code_to_flowchart](https://github.com/Vatsha/code_to_flowchart)
 - Based on [adrai/flowchart.js](http://flowchart.js.org), [python ast](https://docs.python.org/3/library/ast.html), [simonpercivall/astunparse](https://github.com/simonpercivall/astunparse)
 - [A blog about this project](https://clownote.github.io/2020/10/24/blog/PyFlowchart/)
 
 ## License
 
-Copyright 2020-2022 CDFMLR. All rights reserved.
+Copyright 2020-2023 CDFMLR. All rights reserved.
 
 Licensed under the MIT License.
 
-
-
```

### Comparing `pyflowchart-0.2.3/pyflowchart/ast_node.py` & `pyflowchart-0.3.0/pyflowchart/ast_node.py`

 * *Files identical despite different names*

### Comparing `pyflowchart-0.2.3/pyflowchart/flowchart.py` & `pyflowchart-0.3.0/pyflowchart/flowchart.py`

 * *Files identical despite different names*

### Comparing `pyflowchart-0.2.3/pyflowchart/node.py` & `pyflowchart-0.3.0/pyflowchart/node.py`

 * *Files identical despite different names*

### Comparing `pyflowchart-0.2.3/pyflowchart.egg-info/PKG-INFO` & `pyflowchart-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,95 @@
 Metadata-Version: 2.1
 Name: pyflowchart
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python codes to Flowcharts.
 Home-page: https://github.com/cdfmlr/pyflowchart
 Author: CDFMLR
 Author-email: cdfmlr@outlook.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyFlowchart
 
-PyFlowchart is a package to:
+English | [机翻中文](README_zh-CN.md)
 
-- write flowcharts in the Python language,
-- translate Python source codes into flowcharts.
+PyFlowchart is a Python package that lets you:
 
-PyFlowchart produces flowcharts in [flowchart.js](https://github.com/adrai/flowchart.js) flowchart DSL, a widely used flow chart textual representation. It's easy to convert these flowcharts text into a picture via [flowchart.js.org](http://flowchart.js.org), [francoislaberge/diagrams](https://github.com/francoislaberge/diagrams/#flowchart), or some markdown editors. 
+- Write flowcharts in Python.
+- Translate Python source code into flowcharts.
+
+PyFlowchart produces flowcharts in the [flowchart.js](https://github.com/adrai/flowchart.js)  flowchart DSL, a widely used textual representation of flowcharts. You can convert these flowcharts to images using [flowchart.js.org](http://flowchart.js.org), [francoislaberge/diagrams](https://github.com/francoislaberge/diagrams/#flowchart), or some markdown editors. Alternatively, we  also support an option to output the generated flowchart into a interactive HTML page.
 
 ## Get PyFlowchart
 
 ```sh
-$ pip3 install pyflowchart
+$ pip install pyflowchart
 ```
 
 ## Quick Start
 
-To flowchartlize your python codes in `example.py`，run:
+Want to **flowchart your Python code in `example.py`?** Run this:
+
+```sh
+$ python -m pyflowchart example.py
+```
+
+> ⚠️ PyFlowchart works with **Python 3.7+**. To check your Python version, run [`python --version`](https://docs.python.org/3/using/cmdline.html#cmdoption-version).
+>
+> If you have both Python 2 and Python 3 installed, you may need to use `python3` instead of `python`. This is becoming less common as [Python 2 is sunsetting](https://www.python.org/doc/sunset-python-2/).
+
+PyFlowchart will output the generated flowchart.js DSL. You can convert the output code to a rendered diagram by going to http://flowchart.js.org or using editors like Typora.
+
+**To output a HTML file** containing the generated flowchart:
 
 ```sh
-$ python3 -m pyflowchart example.py
+$ python -m pyflowchart example.py -o example.html
+$ # open example.html
 ```
 
-PyFlowchart will output the generated flowchart.js DSL. Go to http://flowchart.js.org or use editors like [Typora](https://support.typora.io/Draw-Diagrams-With-Markdown/#flowcharts) to turn the output code into a rendered diagram.
+Open `example.html` in your browser to see the output in graphical representation.
+
+**To specify a function (or a method in a class) to flowchartlize:**
 
-To specify a function (or a method in a class) to flowchartlize:
+- Use the `-f` flag to specify the function or method name.
 
 ```sh
-$ python3 -m pyflowchart example.py -f function_name
+$ python -m pyflowchart example.py -f function_name
 # or
-$ python3 -m pyflowchart example.py -f ClassName.method_name
+$ python -m pyflowchart example.py -f ClassName.method_name
 ```
 
-🎉 Now you are ready to enjoy the flowchartlization.
+For example, to flowchartlize the `add()` function in the `MyClass` class, you would use the following command: `python3 -m pyflowchart example.py -f MyClass.add`.
 
-Keep reading this document to learn more usages.
+🎉 **Now you are ready to flowchart your code!**
+
+To learn more about how to use PyFlowchart, keep reading this document.
 
 ## Flowchart in Python
 
-PyFlowchart allows you to write a flowchart in Python which could be translated into the [flowchart.js](https://github.com/adrai/flowchart.js) DSL automatically.
+PyFlowchart lets you write flowcharts in Python, which can be automatically translated into the [flowchart.js](https://github.com/adrai/flowchart.js) DSL.
 
-PyFlowchart supports [flowchart.js](https://github.com/adrai/flowchart.js#node-types) node types:
+The following [flowchart.js node types](https://github.com/adrai/flowchart.js#node-types) are supported:
 
 - StartNode
 - OperationNode
 - ConditionNode
 - InputOutputNode
 - SubroutineNode
 - EndNode
 
-Nodes can be connected by `connect()` method (`connect_{yes|no}` for ConditionNode). An optional second parameter to `connect()` is used to specify the connect_direction.
+To connect nodes, use the `connect()` method. For ConditionNodes, use the `connect_{yes|no}` syntax. You can optionally specify the connect_direction as a second parameter.
 
 Get a Flowchart with your start node and call its `flowchart()` method to generate flowchart.js flowchart DSL：
 
 ```python
 from pyflowchart import *
 
 st = StartNode('a_pyflow_test')
@@ -108,31 +126,37 @@
 cond2->
 cond2(yes)->io3
 io3->e5
 cond2(no)->sub4
 sub4(right)->op1
 ```
 
-Then you can visit http://flowchart.js.org and translate the generated textual representation into SVG flow chart diagrams:
+You can visit http://flowchart.js.org and translate the generated textual representation into SVG flow chart diagrams:
 
 ![screenshot on flowchart.js page](docs/imgs/flowchart-js-org.png)
 
-P.S. Many Markdown editors (for example, Typora) support this flowchart syntax, too (reference: [Typora doc about flowchart](https://support.typora.io/Draw-Diagrams-With-Markdown/#flowcharts)). And if you prefer CLI, see [francoislaberge/diagrams](https://github.com/francoislaberge/diagrams/#flowchart).
+(v0.3.0) You can also use `pyflowchart.output_html` to generate a page similar to the picture above:
+
+```python
+output_html('output.html', 'a_pyflow_test', fc.flowchart())
+```
+
+By the way, many Markdown editors, like Typora, also support this flowchart syntax. For more information, see [the Typora documentation on flowcharts]((https://support.typora.io/Draw-Diagrams-With-Markdown/#flowcharts)). If you prefer the command line, you can use [francoislaberge/diagrams]((https://github.com/francoislaberge/diagrams/#flowchart)).
 
 ### Set Params to Nodes
 
-Since v0.2.0, we support a `Node.set_param(key, value)` method to generate flowchart like this:
+Starting with v0.2.0, you can use the `Node.set_param(key, value)` method to generate flowcharts like this:
 
 ```
 element(param1=value1,param2=value2)=>start: Start
 ```
 
 (See also [adrai/flowchart.js#node-specific-specifiers-by-type](https://github.com/adrai/flowchart.js#node-specific-specifiers-by-type))
 
-And for convenience, there are grammar sugars to set param `align-next=no` for ConditionNodes:
+There is also a shortcut to set the `align-next=no` parameter for ConditionNodes: 
 
 ```python
 cond = ConditionNode("a cond node")
 cond.no_align_next()
 # or do this at __init__:
 cond = ConditionNode("a cond node", align_next=False)
 ```
@@ -144,43 +168,42 @@
 ```
 
 The generated flowchart will look like:
 
 ```
 cond(align-next=no)=>condition: Yes or No?
 ...
-
 cond(yes,right)->op
 ```
 
 ## Python to Flowchart
 
-PyFlowchart can also translate your Python Codes into Flowcharts.
+PyFlowchart can also translate your Python code into flowcharts.
 
-For example, you got a `simple.py`:
+For example, let's say you have a Python file called `simple.py` with the following code:
 
 ```python
 def foo(a, b):
     if a:
         print("a")
     else:
         for i in range(3):
             print("b")
     return a + b
 ```
 
-Run PyFlowchart in CLI to generate flowchart code:
+To generate a flowchart from this code, you can run the following command in the terminal:
 
 ```sh
-$ python3 -m pyflowchart simple.py
+$ python -m pyflowchart simple.py
 
 # output flowchart code.
 ```
 
-Or, in Python
+Or, in Python:
 
 ```python
 >>> from pyflowchart import Flowchart
 >>> with open('simple.py') as f:
 ...     code = f.read()
 ... 
 >>> fc = Flowchart.from_code(code)
@@ -195,26 +218,33 @@
 
 As mentioned above, we use `Flowchart.from_code` to translate Python codes into Flowcharts. The `from_code` is defined as:
 
 ```python
 Flowchart.from_code(code, field="", inner=True, simplify=True, conds_align=False)
 ```
 
-PyFlowchart CLI is a 1:1 interface for this function:
+- `code`: The Python code to be converted into a flowchart.
+- `field`: The name of a field in the code to be converted into a flowchart. If this parameter is not specified, the entire code will be converted.
+- `inner`: If `True`, the body of the field will be parsed as a nested flowchart. If `False`, the body of the field will be parsed as a single node.
+- `simplify`: If `True`, simple If and Loop statements will be simplified. For example, an If statement with a single expression will be converted into a single node.
+- `conds_align`: If `True`, consecutive If statements will be aligned in the flowchart.
+
+PyFlowchart CLI is an interface for this function:
 
 ```sh
-python3 -m pyflowchart [-f FIELD] [-i] [--no-simplify] [--conds-align] code_file
+python -m pyflowchart [-f FIELD] [-i] [--no-simplify] [--conds-align] [-o OUTPUT] code_file
 ```
 
-Let's talk about those three args:
+- `-f FIELD`: The name of the field to be converted into a flowchart.
+- `-i`:  If specified, the body of the field will be parsed as a nested flowchart.
+- `--no-simplify`:  If specified, the If and Loop statements will not be simplified.
+- `--conds-align`: If specified, consecutive If statements will be aligned in the flowchart.
+- `-o OUTPUT`: If specified, output the flowchart to specific file with a format indicating by the extension name. (only support `*.html` for now)
 
-- `field`: str: Specify a field of code to generate a flowchart
-- `inner`: bool:  `True` to parse the body of field; whereas `False` to parse the body as a single object.
-- `simplify`: bool: for If & Loop statements: simplify the one-line-body or not
-- `conds_align`: bool: improve the flowchart of *consecutive If statements* converted from python code. (Beta)
+⚠️ `-o` is not a part of `Flowchart.from_code`. It's `from pyflowchar import output_html`.
 
 ### field
 
 the `field` is the path to a field (i.e. a function) you want to draw a flowchart. 
 
 ```python
 # example.py
@@ -252,113 +282,136 @@
 print(fc.flowchart())
 ```
 
 Or:
 
 ```sh
 # CLI
-python3 -m pyflowchart example.py -f Bar.buzz.g
+python -m pyflowchart example.py -f Bar.buzz.g
 ```
 
 Output result:
 
 ![specify a field](docs/imgs/field.png)
 
 ### inner
 
-`inner` controls parser's behaving. Techly, `inner=True` means parsing `field.body`, while `inner=False` parses `[field]`. So, if  `inner=True`, pyflowchart will look into the field, otherwise, it takes the `field` as a node.
+The `inner` parameter controls how the parser behaves. If `inner=True`, the parser will look into the field and parse its body. If `inner=False`, the parser will take the field as a single node.
 
 ![pyflowchart_inner](docs/imgs/inner.png)
 
-For CLI,  adding an argument `-i`  means `inner=True`, else `inner=False`.
+In CLI, the `-i` argument sets `inner=True`. The absence of `-i` argument implies `inner=False`.
+
+🔧 For developers: Techly, `inner=True` means parsing `field.body`, while `inner=False` parses `[field]`.
 
 ### simplify
 
-simplify is for If & Loop statements: simplify the one-line-body.
+The `simplify` parameter controls whether to simplify If and Loop statements. When `simplify=True`, an If or Loop statements with one-line-body will be simplified into a single node.
 
-For example:
+For example, the following code:
 
 ```python
 # example_simplify.py
 a = 1
 if a == 1:
     print(a)
 while a < 4:
     a = a + 1
 ```
 
-- Default: `simplify=True`:
+Would be converted into the following flowchart when **simplify=True** :
 
 ```python
 flowchart = Flowchart.from_code(example_simplify_py, field="", inner=True)
 print(flowchart.flowchart())
-# SH $ python3 -m pyflowchart example_simplify.py 
+# SH $ python -m pyflowchart example_simplify.py 
 ```
 
 ![simplify result](docs/imgs/simplify.png)
 
-- `simplify=False`:
+And with `simplify=False`:
 
 ```python
 flowchart = Flowchart.from_code(example_simplify_py, field="", inner=True, simplify=False)
 print(flowchart.flowchart())
-# SH $ python3 -m pyflowchart --no-simplify example_simplify.py 
+# SH $ python -m pyflowchart --no-simplify example_simplify.py 
 ```
 
 ![no simplify result](docs/imgs/no-simplify.png)
 
 ### conds-align (Beta)
 
-Improve the flowchart of *consecutive If statements* converted from python code with the new feature of  `v0.2.0`.
+The `conds-align` parameter controls whether consecutive If statements are aligned in the flowchart. When `conds-align=True`, consecutive If statements are aligned in the flowchart.
 
 ```python
 # example-conds-align.py
 if cond1:
 	op1
 if cond2:
 	op2
 if cond3:
 	op3
 op_end
 ```
 
 ![conds-align-result](docs/imgs/conds-align.png)
 
+**Note:** This feature is still in beta and may not work perfectly in all cases.
+
+### output html and images
+
+You can also directly ouput the generated flowchart.js DSL into an html by adding the parameter ```-o output.html``` where you specify an output filename ending in `.html` or `.htm`.
+
+![output-html](docs/imgs/output-html.png)
+
+Opening the `output.html` in your browser will let you visualize the diagrams. You can tweak the code and click run to update the diagram. There are also links to download the current visuals as a  `.svg` or `.png` image.
+
+⚠️ The output file specified will overwrite any file that already has that name.
+
+🐍 To use this feature via Python instead of CLI, call `output_html(output_name: str, field_name: str, flowchart: str) -> None`:
+
+```py
+>>> import pyflowchart
+>>> help(pyflowchart.output_html)
+```
+
 ## Beautify Flowcharts
 
-Sometimes, the generated flowchart is awful. In those cases, you are encouraged to modify the generated flowchart code by yourself OR consider making your python source code at bottom more clear if it's exceedingly complex.
+The flowcharts generated by PyFlowchart may not always be perfect. In these cases, you can modify the generated flowchart code yourself or consider making your Python source code more clear. Clear and beautiful Python source code will result in more beautiful flowcharts generated by PyFlowchart.
+
+An example: If you don't like the flowchart flow direction you can tweak a condition by modifying with with directions such as:
+
+![beautify-flowchart-example](docs/imgs/beautify-example.png)
 
 ## TODOs
 
 - [ ] Directly generate flowchart SVG/HTML:
 
 ```sh
 $ pyflowchart example.py -o flowchart.svg
 ```
 
 Depends on `node.js` and `flowchart.js`.
 
 - [ ] PyFlowchart GUI
 
-Well, I guess a **GUI** for PyFlowchart may be remarkable. Pasting your code into it, the flowchart DSL will be generated just in time, and the flowchart will be shown aside.
+A **GUI** for PyFlowchart would be amazing. You could paste your Python code into it, and the flowchart DSL would be generated in real time, with the flowchart displayed alongside it. You could clearly see how the two are related.
 
 - [ ] ~~The Chinese README your buddies waiting for!~~ 希望有同学帮助贡献个中文 README 呀。
-- [ ] Tests automation.
+- [x] Tests automation.
 
 ----
 
-Sadly, I am too busy (pronounced as `[ˈlеizi]`——lazy) to code these ideas. Please [submit an issue](https://github.com/cdfmlr/pyflowchart/issues/new) to push me on. Or, PR to make it by yourself. I cannot wait to appreciate your great contribution!
+Unfortunately, I am too busy (pronounced as `[ˈlеizi]`——lazy) to code these ideas myself. Please [submit an issue](https://github.com/cdfmlr/pyflowchart/issues/new) to push me on. Or, PR to make it by yourself. I cannot wait to appreciate your great contribution!
 
 ## References
 
 - Inspired by [Vatsha/code_to_flowchart](https://github.com/Vatsha/code_to_flowchart)
 - Based on [adrai/flowchart.js](http://flowchart.js.org), [python ast](https://docs.python.org/3/library/ast.html), [simonpercivall/astunparse](https://github.com/simonpercivall/astunparse)
 - [A blog about this project](https://clownote.github.io/2020/10/24/blog/PyFlowchart/)
 
 ## License
 
-Copyright 2020-2022 CDFMLR. All rights reserved.
+Copyright 2020-2023 CDFMLR. All rights reserved.
 
 Licensed under the MIT License.
 
-
-
```

### Comparing `pyflowchart-0.2.3/setup.py` & `pyflowchart-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setuptools.setup(
     name='pyflowchart',
-    version='0.2.3',
+    version='0.3.0',
     url='https://github.com/cdfmlr/pyflowchart',
     license='MIT',
     author='CDFMLR',
     author_email='cdfmlr@outlook.com',
     description='Python codes to Flowcharts.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```


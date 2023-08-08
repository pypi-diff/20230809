# Comparing `tmp/autobound-0.1.2.tar.gz` & `tmp/autobound-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobound-0.1.2.tar", last modified: Wed Apr  5 16:47:26 2023, max compression
+gzip compressed data, was "autobound-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `autobound-0.1.2.tar` & `autobound-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2022-12-06 23:12:00.712500 autobound-0.1.2/LICENSE
--rw-r--r--   0        0        0     3517 2023-04-05 16:31:22.647094 autobound-0.1.2/README.md
--rw-r--r--   0        0        0     1173 2023-04-05 16:31:28.543108 autobound-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      609 2023-04-05 16:47:04.437354 autobound-0.1.2/src/autobound/__init__.py
--rw-r--r--   0        0        0    12784 2023-04-05 16:28:01.022621 autobound-0.1.2/src/autobound/elementwise_functions.py
--rw-r--r--   0        0        0    17866 2023-04-05 16:28:01.022621 autobound-0.1.2/src/autobound/enclosure_arithmetic.py
--rw-r--r--   0        0        0     5201 2023-04-05 16:28:01.022621 autobound-0.1.2/src/autobound/graph_editor.py
--rw-r--r--   0        0        0    13170 2023-04-05 16:28:01.022621 autobound-0.1.2/src/autobound/interval_arithmetic.py
--rw-r--r--   0        0        0      703 2023-04-05 16:28:30.182689 autobound-0.1.2/src/autobound/jax/__init__.py
--rw-r--r--   0        0        0    19379 2023-04-05 16:28:30.182689 autobound-0.1.2/src/autobound/jax/jax_bound.py
--rw-r--r--   0        0        0     9113 2023-04-05 16:28:30.182689 autobound-0.1.2/src/autobound/jax/jaxpr_editor.py
--rw-r--r--   0        0        0     9810 2023-04-05 16:28:01.022621 autobound-0.1.2/src/autobound/polynomials.py
--rw-r--r--   0        0        0    11915 2023-04-05 16:28:01.022621 autobound-0.1.2/src/autobound/primitive_enclosures.py
--rw-r--r--   0        0        0     3849 2023-04-05 16:28:01.026621 autobound-0.1.2/src/autobound/test_utils.py
--rw-r--r--   0        0        0    23170 2023-04-05 16:28:01.026621 autobound-0.1.2/src/autobound/types.py
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 autobound-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-06 23:12:00.712500 autobound-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3517 2023-04-05 16:31:22.647094 autobound-0.1.3/README.md
+-rw-r--r--   0        0        0     1173 2023-04-05 16:31:28.543108 autobound-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      609 2023-08-08 21:47:54.956526 autobound-0.1.3/src/autobound/__init__.py
+-rw-r--r--   0        0        0    12784 2023-04-05 16:28:01.022621 autobound-0.1.3/src/autobound/elementwise_functions.py
+-rw-r--r--   0        0        0    17904 2023-08-08 21:48:06.856568 autobound-0.1.3/src/autobound/enclosure_arithmetic.py
+-rw-r--r--   0        0        0     5201 2023-04-05 16:28:01.022621 autobound-0.1.3/src/autobound/graph_editor.py
+-rw-r--r--   0        0        0    13170 2023-04-05 16:28:01.022621 autobound-0.1.3/src/autobound/interval_arithmetic.py
+-rw-r--r--   0        0        0      703 2023-04-05 16:28:30.182689 autobound-0.1.3/src/autobound/jax/__init__.py
+-rw-r--r--   0        0        0    19379 2023-04-05 16:28:30.182689 autobound-0.1.3/src/autobound/jax/jax_bound.py
+-rw-r--r--   0        0        0     9113 2023-04-05 16:28:30.182689 autobound-0.1.3/src/autobound/jax/jaxpr_editor.py
+-rw-r--r--   0        0        0     9810 2023-04-05 16:28:01.022621 autobound-0.1.3/src/autobound/polynomials.py
+-rw-r--r--   0        0        0    11915 2023-04-05 16:28:01.022621 autobound-0.1.3/src/autobound/primitive_enclosures.py
+-rw-r--r--   0        0        0     3849 2023-04-05 16:28:01.026621 autobound-0.1.3/src/autobound/test_utils.py
+-rw-r--r--   0        0        0    23170 2023-04-05 16:28:01.026621 autobound-0.1.3/src/autobound/types.py
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 autobound-0.1.3/PKG-INFO
```

### Comparing `autobound-0.1.2/LICENSE` & `autobound-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/README.md` & `autobound-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/pyproject.toml` & `autobound-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/__init__.py` & `autobound-0.1.3/src/autobound/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `autobound-0.1.2/src/autobound/elementwise_functions.py` & `autobound-0.1.3/src/autobound/elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/enclosure_arithmetic.py` & `autobound-0.1.3/src/autobound/enclosure_arithmetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,15 +324,16 @@
       x_ndim = self.np_like.ndim(self.trust_region[0])
       term_product_coefficient = functools.partial(
           _elementwise_term_product_coefficient, x_ndim=x_ndim,
           np_like=self.np_like)
       term_power_coefficient = functools.partial(
           _elementwise_term_power_coefficient, x_ndim=x_ndim,
           np_like=self.np_like)
-      multiplicative_identity = self.np_like.ones_like(self.trust_region[0])
+      a0 = a[0][0] if isinstance(a[0], tuple) else a[0]
+      multiplicative_identity = self.np_like.ones_like(a0)
       result = polynomials.integer_power(  # pytype: disable=wrong-arg-types
           a,
           p,
           self.set_arithmetic.add,
           self.np_like.asarray(0),
           multiplicative_identity,
           term_product_coefficient,
```

### Comparing `autobound-0.1.2/src/autobound/graph_editor.py` & `autobound-0.1.3/src/autobound/graph_editor.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/interval_arithmetic.py` & `autobound-0.1.3/src/autobound/interval_arithmetic.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/jax/__init__.py` & `autobound-0.1.3/src/autobound/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/jax/jax_bound.py` & `autobound-0.1.3/src/autobound/jax/jax_bound.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/jax/jaxpr_editor.py` & `autobound-0.1.3/src/autobound/jax/jaxpr_editor.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/polynomials.py` & `autobound-0.1.3/src/autobound/polynomials.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/primitive_enclosures.py` & `autobound-0.1.3/src/autobound/primitive_enclosures.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/test_utils.py` & `autobound-0.1.3/src/autobound/test_utils.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/src/autobound/types.py` & `autobound-0.1.3/src/autobound/types.py`

 * *Files identical despite different names*

### Comparing `autobound-0.1.2/PKG-INFO` & `autobound-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobound
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Keywords: 
 Author-email: AutoBound authors <autobound@google.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```


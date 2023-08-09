# Comparing `tmp/thebestllmever-0.0.2.tar.gz` & `tmp/thebestllmever-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thebestllmever-0.0.2.tar", max compression
+gzip compressed data, was "thebestllmever-0.0.3.tar", max compression
```

## Comparing `thebestllmever-0.0.2.tar` & `thebestllmever-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-05-05 17:46:22.150156 thebestllmever-0.0.2/LICENSE
--rw-r--r--   0        0        0    10794 2023-08-08 21:32:25.786828 thebestllmever-0.0.2/README.md
--rw-r--r--   0        0        0     7031 2023-08-08 21:30:21.813558 thebestllmever-0.0.2/andromeda/README.md
--rw-r--r--   0        0        0       93 2023-08-04 03:53:46.512786 thebestllmever-0.0.2/andromeda/__init__.py
--rw-r--r--   0        0        0     2738 2023-08-01 01:00:20.391101 thebestllmever-0.0.2/andromeda/configs.py
--rw-r--r--   0        0        0      210 2023-07-31 23:42:02.232928 thebestllmever-0.0.2/andromeda/core/__init__.py
--rw-r--r--   0        0        0     7922 2023-08-04 03:56:45.104636 thebestllmever-0.0.2/andromeda/core/attend.py
--rw-r--r--   0        0        0     4449 2023-07-27 23:19:59.076649 thebestllmever-0.0.2/andromeda/core/autoregressive_wrapper.py
--rw-r--r--   0        0        0    10224 2023-08-04 03:51:30.012907 thebestllmever-0.0.2/andromeda/core/flash.py
--rw-r--r--   0        0        0    47128 2023-08-08 21:30:21.855431 thebestllmever-0.0.2/andromeda/core/transformer.py
--rw-r--r--   0        0        0        0 2023-07-24 15:55:44.000080 thebestllmever-0.0.2/andromeda/dataset_prep/__init__.py
--rw-r--r--   0        0        0      326 2023-08-01 02:16:28.826494 thebestllmever-0.0.2/andromeda/dataset_prep/books.py
--rw-r--r--   0        0        0     5593 2023-07-27 23:19:59.078716 thebestllmever-0.0.2/andromeda/inference.py
--rw-r--r--   0        0        0     4265 2023-08-08 21:30:21.791149 thebestllmever-0.0.2/andromeda/model.py
--rw-r--r--   0        0        0        0 2023-07-24 15:46:11.793907 thebestllmever-0.0.2/andromeda/old/__init__.py
--rw-r--r--   0        0        0     7385 2023-07-27 23:19:59.072801 thebestllmever-0.0.2/andromeda/old/sophia.py
--rw-r--r--   0        0        0     9763 2023-08-08 21:30:21.875051 thebestllmever-0.0.2/andromeda/old/training.py
--rw-r--r--   0        0        0    11280 2023-08-08 21:30:21.833994 thebestllmever-0.0.2/andromeda/old/training_1.py
--rw-r--r--   0        0        0    11666 2023-08-08 21:30:21.815182 thebestllmever-0.0.2/andromeda/old/training_sophia.py
--rw-r--r--   0        0        0        0 2023-07-24 15:45:54.396085 thebestllmever-0.0.2/andromeda/utils/__init__.py
--rw-r--r--   0        0        0     6256 2023-07-24 18:38:28.724015 thebestllmever-0.0.2/andromeda/utils/decoupled_optimizer.py
--rw-r--r--   0        0        0      487 2023-06-03 19:26:38.101050 thebestllmever-0.0.2/andromeda/utils/helpers.py
--rw-r--r--   0        0        0     5025 2023-06-05 17:22:50.120473 thebestllmever-0.0.2/andromeda/utils/rf_utils.py
--rw-r--r--   0        0        0     3307 2023-07-27 23:19:59.079840 thebestllmever-0.0.2/andromeda/utils/stable_adamw.py
--rw-r--r--   0        0        0      961 2023-08-08 21:36:25.810882 thebestllmever-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    11853 1970-01-01 00:00:00.000000 thebestllmever-0.0.2/setup.py
--rw-r--r--   0        0        0    11983 1970-01-01 00:00:00.000000 thebestllmever-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-05 17:46:22.150156 thebestllmever-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10798 2023-08-09 01:46:20.471431 thebestllmever-0.0.3/README.md
+-rw-r--r--   0        0        0     7031 2023-08-08 21:30:21.813558 thebestllmever-0.0.3/andromeda/README.md
+-rw-r--r--   0        0        0      134 2023-08-09 03:00:33.206420 thebestllmever-0.0.3/andromeda/__init__.py
+-rw-r--r--   0        0        0     2738 2023-08-01 01:00:20.391101 thebestllmever-0.0.3/andromeda/configs.py
+-rw-r--r--   0        0        0      210 2023-07-31 23:42:02.232928 thebestllmever-0.0.3/andromeda/core/__init__.py
+-rw-r--r--   0        0        0     7922 2023-08-04 03:56:45.104636 thebestllmever-0.0.3/andromeda/core/attend.py
+-rw-r--r--   0        0        0     4449 2023-07-27 23:19:59.076649 thebestllmever-0.0.3/andromeda/core/autoregressive_wrapper.py
+-rw-r--r--   0        0        0    10224 2023-08-04 03:51:30.012907 thebestllmever-0.0.3/andromeda/core/flash.py
+-rw-r--r--   0        0        0    46938 2023-08-08 21:37:51.627754 thebestllmever-0.0.3/andromeda/core/transformer.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:55:44.000080 thebestllmever-0.0.3/andromeda/dataset_prep/__init__.py
+-rw-r--r--   0        0        0      326 2023-08-01 02:16:28.826494 thebestllmever-0.0.3/andromeda/dataset_prep/books.py
+-rw-r--r--   0        0        0     5593 2023-07-27 23:19:59.078716 thebestllmever-0.0.3/andromeda/inference.py
+-rw-r--r--   0        0        0     4288 2023-08-08 22:13:19.910408 thebestllmever-0.0.3/andromeda/model.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:46:11.793907 thebestllmever-0.0.3/andromeda/old/__init__.py
+-rw-r--r--   0        0        0     7385 2023-07-27 23:19:59.072801 thebestllmever-0.0.3/andromeda/old/sophia.py
+-rw-r--r--   0        0        0     9763 2023-08-08 21:30:21.875051 thebestllmever-0.0.3/andromeda/old/training.py
+-rw-r--r--   0        0        0    11280 2023-08-08 21:30:21.833994 thebestllmever-0.0.3/andromeda/old/training_1.py
+-rw-r--r--   0        0        0    11666 2023-08-08 21:30:21.815182 thebestllmever-0.0.3/andromeda/old/training_sophia.py
+-rw-r--r--   0        0        0    24590 2023-08-09 03:01:17.410539 thebestllmever-0.0.3/andromeda/train.py
+-rw-r--r--   0        0        0        0 2023-07-24 15:45:54.396085 thebestllmever-0.0.3/andromeda/utils/__init__.py
+-rw-r--r--   0        0        0     6256 2023-07-24 18:38:28.724015 thebestllmever-0.0.3/andromeda/utils/decoupled_optimizer.py
+-rw-r--r--   0        0        0      487 2023-06-03 19:26:38.101050 thebestllmever-0.0.3/andromeda/utils/helpers.py
+-rw-r--r--   0        0        0     5025 2023-06-05 17:22:50.120473 thebestllmever-0.0.3/andromeda/utils/rf_utils.py
+-rw-r--r--   0        0        0     3307 2023-07-27 23:19:59.079840 thebestllmever-0.0.3/andromeda/utils/stable_adamw.py
+-rw-r--r--   0        0        0      961 2023-08-09 03:01:28.368331 thebestllmever-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11859 1970-01-01 00:00:00.000000 thebestllmever-0.0.3/setup.py
+-rw-r--r--   0        0        0    11987 1970-01-01 00:00:00.000000 thebestllmever-0.0.3/PKG-INFO
```

### Comparing `thebestllmever-0.0.2/LICENSE` & `thebestllmever-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/README.md` & `thebestllmever-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 # Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌
 
+![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)
+
 <div align="center">
 
 [![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)
 [![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)
 [![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) 
 [![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) 
 [![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) 
@@ -16,19 +18,18 @@
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
 [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
 [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
 [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)
 
 </div>
 
----
 
-![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)
 
-Welcome to Andromeda, a high-performance language model that offers exciting possibilities in the realm of natural language understanding and generation. Built for efficiency and speed, Andromeda rivals leading models like OpenAI's GPT-4 and PALM. Features include:
+Welcome to Andromeda, The Fastest, Most Creative, and Reliable Language Model Ever Built, train your own verison, conduct inference, and finetune your own verison with simple plug in and play scripts get started in 10 seconds, and:
+
 
 - 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)
 - ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)
 - 🎓 Superior Reasoning Capabilities
 
 ---
 
@@ -43,17 +44,19 @@
 ## Hiring
 We're hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`
 
 ----------
 
 ## 💻 Usage
 
-There are two methods to use Andromeda but pip does not work now.
+There are two methods to use Andromeda 
+
+1. `pip install TheBestLLMEver`
 
-1. Clone the repository.
+2. `git clone https://github.com/kyegomez/Andromeda.git` 
 
 For detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).
 
 ### Method 1
 
 To get started:
```

### Comparing `thebestllmever-0.0.2/andromeda/README.md` & `thebestllmever-0.0.3/andromeda/README.md`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/configs.py` & `thebestllmever-0.0.3/andromeda/configs.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/core/attend.py` & `thebestllmever-0.0.3/andromeda/core/attend.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/core/autoregressive_wrapper.py` & `thebestllmever-0.0.3/andromeda/core/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/core/flash.py` & `thebestllmever-0.0.3/andromeda/core/flash.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/core/transformer.py` & `thebestllmever-0.0.3/andromeda/core/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1189,18 +1189,14 @@
                 attn_intermediates = intermediates
             )
 
             return x, intermediates
 
         return x
 
-class Encoder(AttentionLayers):
-    def __init__(self, **kwargs):
-        assert 'causal' not in kwargs, 'cannot set causality on encoder'
-        super().__init__(causal = False, **kwargs)
 
 class Decoder(AttentionLayers):
     def __init__(self, **kwargs):
         assert 'causal' not in kwargs, 'cannot set causality on decoder'
         super().__init__(causal = True, **kwargs)
```

### Comparing `thebestllmever-0.0.2/andromeda/inference.py` & `thebestllmever-0.0.3/andromeda/inference.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/model.py` & `thebestllmever-0.0.3/andromeda/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 
 class Andromeda(Module):
     """
     Andromeda is a transformer-based model architecture. It initializes with 
     a Transformer and AutoregressiveWrapper with default or user-specified parameters.
     """
     def __init__(self, 
-                num_tokens=50432, 
+                 num_tokens=50432, 
                  max_seq_len=8192, 
-                 dim=2560, depth=32, 
+                 dim=2560, 
+                 depth=32, 
                  dim_head=128, 
                  heads=24,
                  use_abs_pos_emb=False, 
                  alibi_pos_bias=True, 
                  alibi_num_heads=12, 
                  rotary_xpos=True,
                  attn_flash=True, 
-                 shift_tokens=1, 
+                #  shift_tokens=1, 
                  attn_one_kv_head=True,  # multiquery attention
                  qk_norm=True, 
                  attn_qk_norm=True, 
                  attn_qk_norm_dim_scale=True, 
                  embedding_provider=AndromedaEmbedding()):
         """
         Initialize the model with specified or default parameters.
@@ -82,15 +83,15 @@
                     dim_head=dim_head,
                     heads=heads,
                     alibi_pos_bias=alibi_pos_bias,
                     alibi_num_heads=alibi_num_heads,
                     rotary_xpos=rotary_xpos,
                     attn_flash=attn_flash,
                     # deepnorm=deepnorm,
-                    shift_tokens=shift_tokens,
+                    # shift_tokens=shift_tokens,
                     attn_one_kv_head=attn_one_kv_head,
                     qk_norm=qk_norm,
                     attn_qk_norm=attn_qk_norm,
                     attn_qk_norm_dim_scale=attn_qk_norm_dim_scale
                 )
             )
```

### Comparing `thebestllmever-0.0.2/andromeda/old/sophia.py` & `thebestllmever-0.0.3/andromeda/old/sophia.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/old/training.py` & `thebestllmever-0.0.3/andromeda/old/training.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/old/training_1.py` & `thebestllmever-0.0.3/andromeda/old/training_1.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/old/training_sophia.py` & `thebestllmever-0.0.3/andromeda/old/training_sophia.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/utils/decoupled_optimizer.py` & `thebestllmever-0.0.3/andromeda/utils/decoupled_optimizer.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/utils/rf_utils.py` & `thebestllmever-0.0.3/andromeda/utils/rf_utils.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/andromeda/utils/stable_adamw.py` & `thebestllmever-0.0.3/andromeda/utils/stable_adamw.py`

 * *Files identical despite different names*

### Comparing `thebestllmever-0.0.2/pyproject.toml` & `thebestllmever-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TheBestLLMEver"
-version = "0.0.2"
+version = "0.0.3"
 description = "andromeda - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # assuming you have a README.md file
 homepage = "https://github.com/kyegomez/Andromeda"
 keywords = ["artificial intelligence", "attention mechanism", "transformers"]
 classifiers = [
```

### Comparing `thebestllmever-0.0.2/setup.py` & `thebestllmever-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'matplotlib',
  'numpy',
  'torch',
  'transformers']
 
 setup_kwargs = {
     'name': 'thebestllmever',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'andromeda - Pytorch',
-    'long_description': '\n# Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌\n\n<div align="center">\n\n[![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)\n[![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) \n[![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) \n[![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) \n[![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)\n[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) \n[![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) \n[![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)\n![Discord](https://img.shields.io/discord/999382051935506503)\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)\n\n</div>\n\n---\n\n![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)\n\nWelcome to Andromeda, a high-performance language model that offers exciting possibilities in the realm of natural language understanding and generation. Built for efficiency and speed, Andromeda rivals leading models like OpenAI\'s GPT-4 and PALM. Features include:\n\n- 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)\n- ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)\n- 🎓 Superior Reasoning Capabilities\n\n---\n\n## 🔄 Updates\n\n- [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)\n- [And, here is the WANDB link to watch Andromeda train live!](https://wandb.ai/apacai/Andromeda/overview?)\n\n---\n\n-----\n## Hiring\nWe\'re hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`\n\n----------\n\n## 💻 Usage\n\nThere are two methods to use Andromeda but pip does not work now.\n\n1. Clone the repository.\n\nFor detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).\n\n### Method 1\n\nTo get started:\n\n1. Clone the repository and install the required packages:\n\n```bash\ngit clone https://github.com/kyegomez/Andromeda\ncd Andromeda\npip3 install -r requirements.txt\ncd Andromeda\npython3 train.py\n```\n\nFor further instructions, refer to the [Training SOP](DOCs/TRAINING.md).\n\n---\n\n## 📚 Training\n\n1. Set the environment variables:\n   - `ENTITY_NAME`: Your wandb project name\n   - `OUTPUT_DIR`: Directory to save the weights (e.g., `./weights`)\n   - `MASTER_ADDR`: For distributed training\n   - `MASTER_PORT` For master port distributed training\n   - `RANK`- Number of nodes services\n   - `WORLD_SIZE` Number of gpus\n\n2. Configure the training:\n   - Accelerate Config\n   - Enable Deepspeed 3\n   - Accelerate launch train_distributed_accelerate.py\n\nFor more information, refer to the [Training SOP](DOCs/TRAINING.md).\n\n---\n\n## 🗃️ Dataset Building\n\nTo preprocess a\n\n different dataset similar to the C4 or Falcon dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.\n\nExample command:\n\n```bash\npython3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"\n```\n\n---\n\n## 🚀 Why Andromeda?\n\nAndromeda offers several advantages:\n- Andromeda offers reliable processing of 100,000+ sequence lengths extremely fast under 300ms\n- Andromeda\'s dataset strategy was crafted with atomic precision and attention to detail for creativity and quantitative reasoning.\n- Andromeda is extremely intelligent with the ability to think like a poet or make API Calls to your favorite apps.\n\nFor detailed information about the model architecture and methods, refer to the [Model Architecture](DOCs/MODEL_ARCHITECTURE.md) documentation.\n\n---\n\n# 🎯 Andromeda Principles\n\n- **Efficiency**: Optimize with techniques like attention flashing, rotary position encodings, and deep normalization.\n- **Flexibility**: Adapt to various tasks and domains for wide applications.\n- **Scalability**: Designed to scale with resources and data sizes.\n- **Community-Driven**: Thrives on contributions from the open-source community.\n\n---\n\n## 🚀 Get Involved\n\nWe\'re just at the beginning of our journey. As we continue to develop and refine Andromeda, we invite you to join us. Whether you\'re a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Andromeda.\n\n---\n\n# 🤝 Contributing to Andromeda\n\nWe are thrilled to invite you to be a part of the Andromeda project. This is not just an open-source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.\n\n## 🌟 Why Contribute\n\nContributing to Andromeda not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Andromeda project, you are adding value. As such, we believe it\'s only fair that you share in the rewards.\n\n## 💰 Rewards Program\n\nHere\'s how the Andromeda Rewards Program works:\n\n1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.\n\n2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.\n\n3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution.\n\nThis means you\'re not just contributing to an open-source project; you\'re becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.\n\n## 🚀 Becoming a Paid API\n\nAs part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project but also fund the rewards program. If you contribute anything to make Andromeda, you will receive recurring revenue from paid API requests!\n\n## 🚀 How to Start Contributing\n\nIf you\'re ready to become a part of Andromeda and contribute to the future of multimodal embeddings, here\'s what you need to do:\n\n1. Fork the repository.\n\n2. Make your improvements or additions in your forked repository.\n\n3. Submit a pull request detailing the changes you\'ve made.\n\n4. Our team will review your submission. If it\'s approved, it will be merged into the main repository, and you will become part of the Andromeda Rewards Program.\n\nThank you for considering contributing to Andromeda. Your expertise and commitment to this project are what make it thrive. Let\'s build the future of multimodal embeddings together.\n\n---\n\n## 🗺️ Roadmap\n\n1. **Training phase**: Train Andromeda on a large-scale dataset to achieve SOTA performance in various natural language processing tasks.\n\n2. **World-class inference infrastructure**: Establish a robust and efficient infrastructure that leverages techniques such as:\n\n   - Model quantization: Reduce memory and computational requirements without significant loss in performance.\n   - Distillation: Train smaller, faster models that retain the knowledge of the larger model.\n   - Optimized serving frameworks: Deploy Andromeda using efficient serving frameworks, such as NVIDIA Triton or TensorFlow Serving, for rapid inference.\n\n3. **Continuous improvement**: Continuously fine-tune Andromeda on diverse data sources and adapt it to new tasks and domains.\n\n4. **Community-driven development**: Encourage open-source contributions, including pre-processing improvements, advanced training techniques, and novel use cases.\n\n---\n\n## 📈 Benchmarks\n\n### Speed\n- Andromeda utilizes one of the most reliable Attentions ever, flash attention 2.0 Triton. It consumes 50x less memory than GPT-3 and 10x less than LLAMA.\n\n![AndromedaBanner](images/andromeda_performance.png)\n\n- We can speed this up even more with dynamic sparse flash attention 2.0.\n\n---\n\n# 🔮 Join the Journey\n\nWe\'re just getting started, and we invite you to join the journey. Let\'s revolutionize the NLP landscape together! 🚀🌟\n\n- Join Agora and work with 2,000+ AI Engineers to implement all new features.\n- Provide compute and help train Andromeda.\n- Share the message on how we\'re liberating this superintelligent AI and seizing the power from the corrupt, providing it back to you.\n',
+    'long_description': '\n# Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌\n\n![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)\n\n<div align="center">\n\n[![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)\n[![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) \n[![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) \n[![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) \n[![GitHub license](https://img.shields.io/github/license/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/blob/main/LICENSE)\n[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/Andromeda)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20Andromeda&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) \n[![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda) \n[![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=&summary=&source=)\n![Discord](https://img.shields.io/discord/999382051935506503)\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) \n[![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)\n\n</div>\n\n\n\nWelcome to Andromeda, The Fastest, Most Creative, and Reliable Language Model Ever Built, train your own verison, conduct inference, and finetune your own verison with simple plug in and play scripts get started in 10 seconds, and:\n\n\n- 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)\n- ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)\n- 🎓 Superior Reasoning Capabilities\n\n---\n\n## 🔄 Updates\n\n- [READY FOR TRAINING, help us with the strategy!](https://www.figma.com/file/pfaU8Nhyw0EdXuT6z4Hutw/Andromeda-Strategy?type=whiteboard&node-id=0%3A1&t=Tub1wIzaPAXt2i86-1)\n- [And, here is the WANDB link to watch Andromeda train live!](https://wandb.ai/apacai/Andromeda/overview?)\n\n---\n\n-----\n## Hiring\nWe\'re hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`\n\n----------\n\n## 💻 Usage\n\nThere are two methods to use Andromeda \n\n1. `pip install TheBestLLMEver`\n\n2. `git clone https://github.com/kyegomez/Andromeda.git` \n\nFor detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).\n\n### Method 1\n\nTo get started:\n\n1. Clone the repository and install the required packages:\n\n```bash\ngit clone https://github.com/kyegomez/Andromeda\ncd Andromeda\npip3 install -r requirements.txt\ncd Andromeda\npython3 train.py\n```\n\nFor further instructions, refer to the [Training SOP](DOCs/TRAINING.md).\n\n---\n\n## 📚 Training\n\n1. Set the environment variables:\n   - `ENTITY_NAME`: Your wandb project name\n   - `OUTPUT_DIR`: Directory to save the weights (e.g., `./weights`)\n   - `MASTER_ADDR`: For distributed training\n   - `MASTER_PORT` For master port distributed training\n   - `RANK`- Number of nodes services\n   - `WORLD_SIZE` Number of gpus\n\n2. Configure the training:\n   - Accelerate Config\n   - Enable Deepspeed 3\n   - Accelerate launch train_distributed_accelerate.py\n\nFor more information, refer to the [Training SOP](DOCs/TRAINING.md).\n\n---\n\n## 🗃️ Dataset Building\n\nTo preprocess a\n\n different dataset similar to the C4 or Falcon dataset used during training, use the `build_dataset.py` script. This script pre-tokenizes the data, chunks it into blocks of a specified sequence length, and uploads it to the Huggingface hub.\n\nExample command:\n\n```bash\npython3 Andromeda/build_dataset.py --seed 42 --seq_len 8192 --hf_account "HUGGINGFACE APIKEY" --tokenizer "EleutherAI/gpt-neox-20b" --dataset_name "EleutherAI/the_pile_deduplicated"\n```\n\n---\n\n## 🚀 Why Andromeda?\n\nAndromeda offers several advantages:\n- Andromeda offers reliable processing of 100,000+ sequence lengths extremely fast under 300ms\n- Andromeda\'s dataset strategy was crafted with atomic precision and attention to detail for creativity and quantitative reasoning.\n- Andromeda is extremely intelligent with the ability to think like a poet or make API Calls to your favorite apps.\n\nFor detailed information about the model architecture and methods, refer to the [Model Architecture](DOCs/MODEL_ARCHITECTURE.md) documentation.\n\n---\n\n# 🎯 Andromeda Principles\n\n- **Efficiency**: Optimize with techniques like attention flashing, rotary position encodings, and deep normalization.\n- **Flexibility**: Adapt to various tasks and domains for wide applications.\n- **Scalability**: Designed to scale with resources and data sizes.\n- **Community-Driven**: Thrives on contributions from the open-source community.\n\n---\n\n## 🚀 Get Involved\n\nWe\'re just at the beginning of our journey. As we continue to develop and refine Andromeda, we invite you to join us. Whether you\'re a developer, researcher, or simply an enthusiast, your insights and contributions can help shape the future of Andromeda.\n\n---\n\n# 🤝 Contributing to Andromeda\n\nWe are thrilled to invite you to be a part of the Andromeda project. This is not just an open-source project but a community initiative, and we value your expertise and creativity. To show our appreciation, we have instituted a unique rewards system that directly compensates contributors from the revenue generated by the Andromeda API.\n\n## 🌟 Why Contribute\n\nContributing to Andromeda not only enhances your skills and profile but also comes with financial rewards. When you contribute code, documentation, or any form of improvement to the Andromeda project, you are adding value. As such, we believe it\'s only fair that you share in the rewards.\n\n## 💰 Rewards Program\n\nHere\'s how the Andromeda Rewards Program works:\n\n1. **Submit a Pull Request:** This can be a code enhancement, bug fix, documentation update, new feature, or any improvement to the project.\n\n2. **Review and Approval:** Our team will review your contribution. If it gets approved and merged, you become eligible for the rewards program.\n\n3. **Revenue Share:** Once your pull request is merged, you will receive a percentage of the revenue generated by the Andromeda API. The percentage will be determined based on the significance and impact of your contribution.\n\nThis means you\'re not just contributing to an open-source project; you\'re becoming a part of the Andromeda ecosystem. Your efforts can yield ongoing benefits as the Andromeda API grows and evolves.\n\n## 🚀 Becoming a Paid API\n\nAs part of our growth strategy, we will be deploying Andromeda as a Paid API. The revenue generated from this API will not only sustain and further the project but also fund the rewards program. If you contribute anything to make Andromeda, you will receive recurring revenue from paid API requests!\n\n## 🚀 How to Start Contributing\n\nIf you\'re ready to become a part of Andromeda and contribute to the future of multimodal embeddings, here\'s what you need to do:\n\n1. Fork the repository.\n\n2. Make your improvements or additions in your forked repository.\n\n3. Submit a pull request detailing the changes you\'ve made.\n\n4. Our team will review your submission. If it\'s approved, it will be merged into the main repository, and you will become part of the Andromeda Rewards Program.\n\nThank you for considering contributing to Andromeda. Your expertise and commitment to this project are what make it thrive. Let\'s build the future of multimodal embeddings together.\n\n---\n\n## 🗺️ Roadmap\n\n1. **Training phase**: Train Andromeda on a large-scale dataset to achieve SOTA performance in various natural language processing tasks.\n\n2. **World-class inference infrastructure**: Establish a robust and efficient infrastructure that leverages techniques such as:\n\n   - Model quantization: Reduce memory and computational requirements without significant loss in performance.\n   - Distillation: Train smaller, faster models that retain the knowledge of the larger model.\n   - Optimized serving frameworks: Deploy Andromeda using efficient serving frameworks, such as NVIDIA Triton or TensorFlow Serving, for rapid inference.\n\n3. **Continuous improvement**: Continuously fine-tune Andromeda on diverse data sources and adapt it to new tasks and domains.\n\n4. **Community-driven development**: Encourage open-source contributions, including pre-processing improvements, advanced training techniques, and novel use cases.\n\n---\n\n## 📈 Benchmarks\n\n### Speed\n- Andromeda utilizes one of the most reliable Attentions ever, flash attention 2.0 Triton. It consumes 50x less memory than GPT-3 and 10x less than LLAMA.\n\n![AndromedaBanner](images/andromeda_performance.png)\n\n- We can speed this up even more with dynamic sparse flash attention 2.0.\n\n---\n\n# 🔮 Join the Journey\n\nWe\'re just getting started, and we invite you to join the journey. Let\'s revolutionize the NLP landscape together! 🚀🌟\n\n- Join Agora and work with 2,000+ AI Engineers to implement all new features.\n- Provide compute and help train Andromeda.\n- Share the message on how we\'re liberating this superintelligent AI and seizing the power from the corrupt, providing it back to you.\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/Andromeda',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `thebestllmever-0.0.2/PKG-INFO` & `thebestllmever-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thebestllmever
-Version: 0.0.2
+Version: 0.0.3
 Summary: andromeda - Pytorch
 Home-page: https://github.com/kyegomez/Andromeda
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.6,<4.0
@@ -31,14 +31,16 @@
 Requires-Dist: torch
 Requires-Dist: transformers
 Description-Content-Type: text/markdown
 
 
 # Andromeda: Ultra-Fast and Ultra-Intelligent SOTA Language Model 🚀🌌
 
+![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)
+
 <div align="center">
 
 [![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)
 [![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)
 [![GitHub issues](https://img.shields.io/github/issues/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/issues) 
 [![GitHub forks](https://img.shields.io/github/forks/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/network) 
 [![GitHub stars](https://img.shields.io/github/stars/kyegomez/Andromeda)](https://github.com/kyegomez/Andromeda/stargazers) 
@@ -50,19 +52,18 @@
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&title=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
 [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&t=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
 [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Andromeda%20-%20the%20next%20generation%20AI%20shields) 
 [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Andromeda%20-%20the%20next%20generation%20AI%20shields%20%23Andromeda%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2FAndromeda)
 
 </div>
 
----
 
-![Andromeda Next Generation Open Source Language Model](images/andromeda-banner.png)
 
-Welcome to Andromeda, a high-performance language model that offers exciting possibilities in the realm of natural language understanding and generation. Built for efficiency and speed, Andromeda rivals leading models like OpenAI's GPT-4 and PALM. Features include:
+Welcome to Andromeda, The Fastest, Most Creative, and Reliable Language Model Ever Built, train your own verison, conduct inference, and finetune your own verison with simple plug in and play scripts get started in 10 seconds, and:
+
 
 - 💼 Handle Ultra Long Sequences (32,000-200,000+ context lengths)
 - ⚡ Ultra Fast Processing (32,000+ tokens in under 100ms)
 - 🎓 Superior Reasoning Capabilities
 
 ---
 
@@ -77,17 +78,19 @@
 ## Hiring
 We're hiring: Engineers, Researchers, Interns, And, Customer Success Professionals to work on democratizing Andromeda, email me at with your story `kye@apac.ai`
 
 ----------
 
 ## 💻 Usage
 
-There are two methods to use Andromeda but pip does not work now.
+There are two methods to use Andromeda 
+
+1. `pip install TheBestLLMEver`
 
-1. Clone the repository.
+2. `git clone https://github.com/kyegomez/Andromeda.git` 
 
 For detailed instructions, refer to the [Training SOP](DOCs/TRAINING.md) and [Documentation](https://github.com/kyegomez/Andromeda/blob/master/DOCs/DOCUMENTATION.md).
 
 ### Method 1
 
 To get started:
```


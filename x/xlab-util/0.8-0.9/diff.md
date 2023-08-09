# Comparing `tmp/xlab-util-0.8.tar.gz` & `tmp/xlab-util-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlab-util-0.8.tar", last modified: Tue Aug  8 03:08:18 2023, max compression
+gzip compressed data, was "xlab-util-0.9.tar", last modified: Tue Aug  8 03:53:03 2023, max compression
```

## Comparing `xlab-util-0.8.tar` & `xlab-util-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:08:18.394149 xlab-util-0.8/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 03:08:18.394149 xlab-util-0.8/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.8/README.md
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-08 03:08:18.394149 xlab-util-0.8/setup.cfg
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-08 03:08:06.000000 xlab-util-0.8/setup.py
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:08:18.386150 xlab-util-0.8/xlab_util.egg-info/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:08:18.390149 xlab-util-0.8/xlabutil/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      255 2023-08-08 02:40:03.000000 xlab-util-0.8/xlabutil/__init__.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.8/xlabutil/base.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.8/xlabutil/inference.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     2771 2023-08-08 03:07:32.000000 xlab-util-0.8/xlabutil/result.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.8/xlabutil/type.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      967 2023-08-08 02:35:38.000000 xlab-util-0.8/xlabutil/util.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:53:03.297002 xlab-util-0.9/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 03:53:03.297002 xlab-util-0.9/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.9/README.md
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-08 03:53:03.297002 xlab-util-0.9/setup.cfg
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-08 03:52:54.000000 xlab-util-0.9/setup.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:53:03.297002 xlab-util-0.9/xlab_util.egg-info/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 03:53:03.000000 xlab-util-0.9/xlab_util.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-08 03:53:03.000000 xlab-util-0.9/xlab_util.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-08 03:53:03.000000 xlab-util-0.9/xlab_util.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-08 03:53:03.000000 xlab-util-0.9/xlab_util.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:53:03.297002 xlab-util-0.9/xlabutil/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      271 2023-08-08 03:42:41.000000 xlab-util-0.9/xlabutil/__init__.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      692 2023-08-08 03:21:14.000000 xlab-util-0.9/xlabutil/base.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     2201 2023-08-08 03:44:42.000000 xlab-util-0.9/xlabutil/inference.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     2954 2023-08-08 03:34:01.000000 xlab-util-0.9/xlabutil/result.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.9/xlabutil/type.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1041 2023-08-08 03:32:41.000000 xlab-util-0.9/xlabutil/util.py
```

### Comparing `xlab-util-0.8/xlabutil/inference.py` & `xlab-util-0.9/xlabutil/inference.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 from typing import Union, Any
 
 from openxlab.model import Inference
 from openxlab.model.clients.modelapi_client import Result 
 from .type import ImageType
 
 
-class InferenceResult():
+class Input():
+
+    @staticmethod
+    def input(img) -> Image.Image:
+        return Image.open("./demo.png").convert("RGB")
+
+
+class Output():
     
     def __init__(self, raw_result: Result) -> None:
         self._raw_result = raw_result
         self._content_type = self._raw_result.content_type
         self._content = self._raw_result.original
 
 
@@ -28,34 +35,53 @@
 
     
     def pred(self) -> Any:
         if self._content_type == "application/json":
             return json.loads(self._content)
 
 
-class InstanceSegInference(Inference, InferenceResult):
+class InstanceSegInference(Inference, Input, Output):
+
+    def __init__(self, model_repo):
+        super().__init__(model_repo)
+
+
+    def __call__(self, img: ImageType, 
+                       return_visualization: bool=False, 
+                       **kwargs) -> Output:
+        if return_visualization:
+            kwargs["return_visualization"] = True
+
+        result = super().inference([img], **kwargs)
+
+        return Output(result)
+
+
+class PoseEstimationInference(Inference, Input, Output):
 
     def __init__(self, model_repo):
         super().__init__(model_repo)
 
 
     def __call__(self, img: ImageType, 
                        return_visualization: bool=False, 
-                       **kwargs) -> InferenceResult:
+                       **kwargs) -> Output:
         if return_visualization:
             kwargs["return_visualization"] = True
 
         result = super().inference([img], **kwargs)
 
-        return InferenceResult(result)
+        return Output(result)
 
 
 class RemoteInference():
 
     def from_remote(model_repo: str, 
                     task_type: str="instance-seg"):
         if "instance-seg" == task_type:
             return InstanceSegInference(model_repo)
+        elif "pose-estimation" == task_type:
+            return PoseEstimationInference(model_repo)
```

### Comparing `xlab-util-0.8/xlabutil/result.py` & `xlab-util-0.9/xlabutil/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import base64
-import dataclasses
 
 from PIL import Image
 from io import BytesIO
 from dataclasses import dataclass, field
 from typing import Optional, List, Union
 
 import numpy as np
 
+from .util import array_to_base64
+
 
 @dataclass
 class Visual():
 
     # visualization
     visualization: Optional[str] = field(default_factory=lambda: "")
 
-    def set_visual(self, input: Union[List, Image.Image]):
-        if isinstance(input, List):
-            img_byte = BytesIO()
-            img = Image.fromarray(input)
-            img.save(img_byte, format="jpeg")
-            visual = base64.b64encode(img_byte.getvalue()).decode('utf-8')
+    def set_visual(self, input: Union[np.ndarray, Image.Image], format: str="jpeg"):
+        """设置可视化结果"""
+        if isinstance(input, np.ndarray):
+            visual = array_to_base64(input, format=format)
         elif isinstance(input, Image.Image):
             img_byte = BytesIO()
             input.save(img_byte, format="jpeg")
             visual = base64.b64encode(img_byte.getvalue()).decode('utf-8')
         else:
             visual = input if isinstance(input, str) else None
 
@@ -80,8 +79,15 @@
 class PoseEstimationResult(Visual):
     """The result of object detection."""
     # The bounding boxes of all detected objects
     bboxes: Optional[List[List[int]]] = field(default_factory=lambda: [])
     # The scores of all detected objects
     scores: Optional[List[float]] = field(default_factory=lambda: [])
     # The pose estimation results of all detected objects
-    poses: Optional[List[InstancePose]] = field(default_factory=lambda: [])
+    poses: Optional[List[InstancePose]] = field(default_factory=lambda: [])
+
+
+    def set_pred(self, bbox, score, keypoints, keypoint_scores):
+        """设置预测结果"""
+        self.bboxes.append(bbox)
+        self.scores.append(score)
+        self.poses.append(InstancePose(keypoints, keypoint_scores))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xlab-util-0.8/xlabutil/util.py` & `xlab-util-0.9/xlabutil/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,39 +4,41 @@
 
 from PIL import Image
 from io import BytesIO
 from dataclasses import _is_dataclass_instance
 
 import numpy as np
 
+from .base import NumpyJSONEncoder
+
 
 def save_base64(base64_str: str, img_path: str):
     """保存base64为图片"""
     img_bytes = base64.b64decode(base64_str)
     img_bytes = BytesIO(img_bytes)
     Image.open(img_bytes).save(img_path)
 
 
 def img_to_array(img: Image.Image):
     """图片转ndarray"""
     return np.asarray(img)
 
 
-def array_to_base64(img_array):
+def array_to_base64(array: np.ndarray, format: str="jpeg"):
     """ndarray转为图片（base64）"""
     img_byte = BytesIO()
-    img = Image.fromarray(img_array)
-    img.save(img_byte, format="jpeg")
+    img = Image.fromarray(array)
+    img.save(img_byte, format=format)
 
     return base64.b64encode(img_byte.getvalue()).decode('utf-8')
 
 
 def array_to_img(img_array) -> Image.Image:
     """ndarray转为图片"""
     return Image.fromarray(img_array.astype(np.uint8))
 
 
 def to_json(array):
     if _is_dataclass_instance(array):
         array = dataclasses.asdict(array)
-        
-    return json.dumps(array)
+
+    return json.dumps(array, cls=NumpyJSONEncoder)
```


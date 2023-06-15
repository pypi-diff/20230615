# Comparing `tmp/rapid_layout-0.0.9-py3-none-any.whl.zip` & `tmp/rapid_layout-3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6834192 bytes, number of entries: 10
--rw-r--r--  2.0 unx      646 b- defN 23-Jan-09 01:19 rapid_layout/__init__.py
--rw-r--r--  2.0 unx      517 b- defN 23-Jan-09 01:19 rapid_layout/config.yaml
--rw-r--r--  2.0 unx     2998 b- defN 23-Jan-09 01:19 rapid_layout/rapid_layout.py
--rw-r--r--  2.0 unx    15141 b- defN 23-Jan-09 01:19 rapid_layout/utils.py
+Zip file size: 6835695 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-15 14:14 rapid_layout/__init__.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Jun-15 14:14 rapid_layout/config.yaml
+-rw-r--r--  2.0 unx     3390 b- defN 23-Jun-15 14:14 rapid_layout/rapid_layout.py
+-rw-r--r--  2.0 unx    18231 b- defN 23-Jun-15 14:14 rapid_layout/utils.py
 -rw-r--r--  2.0 unx  7423528 b- defN 22-Nov-19 19:32 rapid_layout/models/layout_cdla.onnx
--rw-r--r--  2.0 unx     1742 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      838 b- defN 23-Jan-09 01:19 rapid_layout-0.0.9.dist-info/RECORD
-10 files, 7445580 bytes uncompressed, 6832758 bytes compressed:  8.2%
+-rw-r--r--  2.0 unx     3179 b- defN 23-Jun-15 14:15 rapid_layout-3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 14:15 rapid_layout-3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-15 14:15 rapid_layout-3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jun-15 14:15 rapid_layout-3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-Jun-15 14:15 rapid_layout-3.6.dist-info/RECORD
+10 files, 7450487 bytes uncompressed, 6834281 bytes compressed:  8.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: rapid_layout/utils.py
 Comment: 
 
 Filename: rapid_layout/models/layout_cdla.onnx
 Comment: 
 
-Filename: rapid_layout-0.0.9.dist-info/METADATA
+Filename: rapid_layout-3.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_layout-0.0.9.dist-info/WHEEL
+Filename: rapid_layout-3.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_layout-0.0.9.dist-info/entry_points.txt
+Filename: rapid_layout-3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_layout-0.0.9.dist-info/top_level.txt
+Filename: rapid_layout-3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_layout-0.0.9.dist-info/RECORD
+Filename: rapid_layout-3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_layout/config.yaml

```diff
@@ -1,8 +1,8 @@
-model_path: models/layout_table.onnx
+model_path: models/layout_cdla.onnx
 
 use_cuda: false
 CUDAExecutionProvider:
     device_id: 0
     arena_extend_strategy: kNextPowerOfTwo
     cudnn_conv_algo_search: EXHAUSTIVE
     do_copy_in_default_stream: true
```

## rapid_layout/rapid_layout.py

```diff
@@ -7,86 +7,93 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import argparse
 import time
 from pathlib import Path
+from typing import Union
+
+import cv2
 import numpy as np
 
 from .utils import (OrtInferSession, PicoDetPostProcess, create_operators,
-                    read_yaml, transform)
+                    read_yaml, transform, vis_layout, LoadImage)
 
 root_dir = Path(__file__).resolve().parent
 
 
 class RapidLayout():
     def __init__(self,
                  model_path: str = None):
         config_path = str(root_dir / 'config.yaml')
         config = read_yaml(config_path)
         if model_path is None:
             model_path = str(root_dir / 'models' / 'layout_cdla.onnx')
         config['model_path'] = model_path
 
-        session_instance = OrtInferSession(config)
-        self.predictor = session_instance.session
-        self.input_name = session_instance.get_input_name()
-        labels = session_instance.get_metadata()['character'].splitlines()
+        self.session = OrtInferSession(config)
+        labels = self.session.get_metadata()['character'].splitlines()
 
         self.preprocess_op = create_operators(config['pre_process'])
         self.postprocess_op = PicoDetPostProcess(labels,
                                                  **config['post_process'])
+        self.load_img = LoadImage()
+
+    def __call__(self, img_content: Union[str, np.ndarray, bytes, Path]):
+        img = self.load_img(img_content)
 
-    def __call__(self, img):
         ori_im = img.copy()
         data = {'image': img}
         data = transform(data, self.preprocess_op)
         img = data[0]
 
         if img is None:
             return None, 0
 
         img = np.expand_dims(img, axis=0)
         img = img.copy()
 
         preds, elapse = 0, 1
         starttime = time.time()
 
-        input_dict = {self.input_name: img}
-        preds_onnx = self.predictor.run(None, input_dict)
+        preds = self.session(img)
 
-        np_score_list, np_boxes_list = [], []
-        num_outs = int(len(preds_onnx) / 2)
+        score_list, boxes_list = [], []
+        num_outs = int(len(preds) / 2)
         for out_idx in range(num_outs):
-            np_score_list.append(preds_onnx[out_idx])
-            np_boxes_list.append(preds_onnx[out_idx + num_outs])
-        preds = dict(boxes=np_score_list, boxes_num=np_boxes_list)
-
+            score_list.append(preds[out_idx])
+            boxes_list.append(preds[out_idx + num_outs])
+        preds = dict(boxes=score_list, boxes_num=boxes_list)
         post_preds = self.postprocess_op(ori_im, img, preds)
         elapse = time.time() - starttime
         return post_preds, elapse
 
 
 def main():
-    import argparse
-    import cv2
-
     parser = argparse.ArgumentParser()
-    parser.add_argument('--img_path', type=str, required=True)
-    parser.add_argument('--model_path', type=str,
-                        default=str(root_dir / 'models' / 'layout_cdla.onnx'))
+    parser.add_argument('-v', '--vis', action='store_true',
+                        help='Wheter to visualize the layout results.')
+    parser.add_argument('-img', '--img_path', type=str, required=True,
+                        help='Path to image for layout.')
+    parser.add_argument('-m', '--model_path', type=str,
+                        default=str(root_dir / 'models' / 'layout_cdla.onnx'),
+                        help='The model path used for inference.')
     args = parser.parse_args()
 
     layout_engine = RapidLayout(args.model_path)
 
     img = cv2.imread(args.img_path)
-
     layout_res, elapse = layout_engine(img)
-
     print(layout_res)
 
+    if args.vis:
+        img_path = Path(args.img_path)
+        save_path = img_path.resolve().parent / f'vis_{img_path.name}'
+        vis_layout(img, layout_res, str(save_path))
+
 
 if __name__ == '__main__':
     main()
```

## rapid_layout/utils.py

```diff
@@ -1,18 +1,24 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+import copy
 import warnings
+from io import BytesIO
+from pathlib import Path
+from typing import Union
 
-import yaml
 import cv2
 import numpy as np
-from onnxruntime import (get_available_providers, get_device,
-                         SessionOptions, InferenceSession,
-                         GraphOptimizationLevel)
+import yaml
+from onnxruntime import (GraphOptimizationLevel, InferenceSession,
+                         SessionOptions, get_available_providers, get_device)
+from PIL import Image, UnidentifiedImageError
+
+InputType = Union[str, np.ndarray, bytes, Path]
 
 
 class OrtInferSession():
     def __init__(self, config):
         sess_opt = SessionOptions()
         sess_opt.log_severity_level = 4
         sess_opt.enable_cpu_mem_arena = False
@@ -24,63 +30,144 @@
 
         EP_list = []
         if config['use_cuda'] and get_device() == 'GPU' \
                 and cuda_ep in get_available_providers():
             EP_list = [(cuda_ep, config[cuda_ep])]
         EP_list.append((cpu_ep, cpu_provider_options))
 
+        self._verify_model(config['model_path'])
         self.session = InferenceSession(config['model_path'],
                                         sess_options=sess_opt,
                                         providers=EP_list)
 
         if config['use_cuda'] and cuda_ep not in self.session.get_providers():
             warnings.warn(f'{cuda_ep} is not avaiable for current env, the inference part is automatically shifted to be executed under {cpu_ep}.\n'
                           'Please ensure the installed onnxruntime-gpu version matches your cuda and cudnn version, '
                           'you can check their relations from the offical web site: '
                           'https://onnxruntime.ai/docs/execution-providers/CUDA-ExecutionProvider.html',
                           RuntimeWarning)
 
-    def get_input_name(self, input_idx=0):
-        return self.session.get_inputs()[input_idx].name
+    def __call__(self, input_content: np.ndarray) -> np.ndarray:
+        input_dict = dict(zip(self.get_input_names(), [input_content]))
+        try:
+            return self.session.run(self.get_output_names(), input_dict)
+        except Exception as e:
+            raise ONNXRuntimeError('ONNXRuntime inferece failed.') from e
+
+    def get_input_names(self, ):
+        return [v.name for v in self.session.get_inputs()]
 
-    def get_output_name(self, output_idx=0):
-        return self.session.get_outputs()[output_idx].name
+    def get_output_names(self,):
+        return [v.name for v in self.session.get_outputs()]
 
     def get_metadata(self):
         meta_dict = self.session.get_modelmeta().custom_metadata_map
         return meta_dict
 
+    @staticmethod
+    def _verify_model(model_path):
+        model_path = Path(model_path)
+        if not model_path.exists():
+            raise FileNotFoundError(f'{model_path} does not exists.')
+        if not model_path.is_file():
+            raise FileExistsError(f'{model_path} is not a file.')
+
+
+class ONNXRuntimeError(Exception):
+    pass
+
+
+class LoadImage():
+    def __init__(self, ):
+        pass
+
+    def __call__(self, img: InputType) -> np.ndarray:
+        if not isinstance(img, InputType.__args__):
+            raise LoadImageError(
+                f'The img type {type(img)} does not in {InputType.__args__}')
+
+        img = self.load_img(img)
+
+        if img.ndim == 2:
+            return cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+
+        if img.ndim == 3 and img.shape[2] == 4:
+            return self.cvt_four_to_three(img)
+
+        return img
+
+    def load_img(self, img: InputType) -> np.ndarray:
+        if isinstance(img, (str, Path)):
+            self.verify_exist(img)
+            try:
+                img = np.array(Image.open(img))
+                img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+            except UnidentifiedImageError as e:
+                raise LoadImageError(
+                    f'cannot identify image file {img}') from e
+            return img
+
+        if isinstance(img, bytes):
+            img = np.array(Image.open(BytesIO(img)))
+            img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+            return img
+
+        if isinstance(img, np.ndarray):
+            return img
+
+        raise LoadImageError(f'{type(img)} is not supported!')
+
+    @staticmethod
+    def cvt_four_to_three(img: np.ndarray) -> np.ndarray:
+        '''RGBA → RGB
+        '''
+        r, g, b, a = cv2.split(img)
+        new_img = cv2.merge((b, g, r))
+
+        not_a = cv2.bitwise_not(a)
+        not_a = cv2.cvtColor(not_a, cv2.COLOR_GRAY2BGR)
+
+        new_img = cv2.bitwise_and(new_img, new_img, mask=a)
+        new_img = cv2.add(new_img, not_a)
+        return new_img
+
+    @staticmethod
+    def verify_exist(file_path: Union[str, Path]):
+        if not Path(file_path).exists():
+            raise LoadImageError(f'{file_path} does not exist.')
+
+
+class LoadImageError(Exception):
+    pass
+
 
 def transform(data, ops=None):
     """ transform """
     if ops is None:
         ops = []
 
     for op in ops:
         data = op(data)
         if data is None:
             return None
     return data
 
 
 def create_operators(op_param_dict):
-    """
-    create operators based on the config
-    """
     ops = []
     for op_name, param in op_param_dict.items():
         if param is None:
             param = {}
         op = eval(op_name)(**param)
         ops.append(op)
     return ops
 
 
 class Resize():
-    def __init__(self, size=(640, 640), **kwargs):
+    def __init__(self, size=(640, 640)):
         self.size = size
 
     def resize_image(self, img):
         resize_h, resize_w = self.size
         ori_h, ori_w = img.shape[:2]  # (h, w, c)
         ratio_h = float(resize_h) / ori_h
         ratio_w = float(resize_w) / ori_w
@@ -102,20 +189,18 @@
                 new_boxes.append(new_box)
             data['polys'] = np.array(new_boxes, dtype=np.float32)
         data['image'] = img_resize
         return data
 
 
 class NormalizeImage():
-    """ normalize image such as substract mean, divide std
-    """
-
-    def __init__(self, scale=None, mean=None, std=None, order='chw', **kwargs):
+    def __init__(self, scale=None, mean=None, std=None, order='chw'):
         if isinstance(scale, str):
             scale = eval(scale)
+
         self.scale = np.float32(scale if scale is not None else 1.0 / 255.0)
         mean = mean if mean is not None else [0.485, 0.456, 0.406]
         std = std if std is not None else [0.229, 0.224, 0.225]
 
         shape = (3, 1, 1) if order == 'chw' else (1, 1, 3)
         self.mean = np.array(mean).reshape(shape).astype('float32')
         self.std = np.array(std).reshape(shape).astype('float32')
@@ -126,27 +211,25 @@
                           np.ndarray), "invalid input 'img' in NormalizeImage"
         data['image'] = (
             img.astype('float32') * self.scale - self.mean) / self.std
         return data
 
 
 class ToCHWImage():
-    """ convert hwc image to chw image
-    """
     def __init__(self, **kwargs):
         pass
 
     def __call__(self, data):
         img = np.array(data['image'])
         data['image'] = img.transpose((2, 0, 1))
         return data
 
 
 class KeepKeys():
-    def __init__(self, keep_keys, **kwargs):
+    def __init__(self, keep_keys):
         self.keep_keys = keep_keys
 
     def __call__(self, data):
         data_list = []
         for key in self.keep_keys:
             data_list.append(data[key])
         return data_list
@@ -155,21 +238,14 @@
 def read_yaml(yaml_path):
     with open(yaml_path, 'rb') as f:
         data = yaml.load(f, Loader=yaml.Loader)
     return data
 
 
 class PicoDetPostProcess():
-    """
-    Args:
-        input_shape (int): network input image size
-        ori_shape (int): ori image shape of before padding
-        scale_factor (float): scale factor of ori image
-        enable_mkldnn (bool): whether to open MKLDNN
-    """
     def __init__(self,
                  labels,
                  strides=[8, 16, 32, 64],
                  score_threshold=0.4,
                  nms_threshold=0.5,
                  nms_top_k=1000,
                  keep_top_k=100):
@@ -405,7 +481,32 @@
             left_top (N, 2): left top corner.
             right_bottom (N, 2): right bottom corner.
         Returns:
             area (N): return the area.
         """
         hw = np.clip(right_bottom - left_top, 0.0, None)
         return hw[..., 0] * hw[..., 1]
+
+
+def vis_layout(img: np.ndarray, layout_res: list, save_path: str) -> None:
+    font = cv2.FONT_HERSHEY_COMPLEX
+    font_scale = 1
+    font_color = (0, 0, 255)
+    font_thickness = 1
+
+    tmp_img = copy.deepcopy(img)
+    for v in layout_res:
+        bbox = np.round(v['bbox']).astype(np.int32)
+        label = v['label']
+
+        start_point = (bbox[0], bbox[1])
+        end_point = (bbox[2], bbox[3])
+
+        cv2.rectangle(tmp_img, start_point, end_point, (0, 255, 0), 2)
+
+        (w, h), _ = cv2.getTextSize(label, font, font_scale, font_thickness)
+        put_point = start_point[0], start_point[1] + h
+        cv2.putText(tmp_img, label, put_point, font, font_scale,
+                    font_color, font_thickness)
+
+    cv2.imwrite(save_path, tmp_img)
+    print(f'The infer result has saved in {save_path}')
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


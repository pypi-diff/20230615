# Comparing `tmp/mlcvzoo_mmocr-5.0.1.tar.gz` & `tmp/mlcvzoo_mmocr-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmocr-5.0.1.tar", max compression
+gzip compressed data, was "mlcvzoo_mmocr-6.0.0.tar", max compression
```

## Comparing `mlcvzoo_mmocr-5.0.1.tar` & `mlcvzoo_mmocr-6.0.0.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0      393 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/README.md
--rw-r--r--   0        0        0      177 2023-05-11 11:10:51.233392 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/__init__.py
--rw-r--r--   0        0        0     3449 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/configuration.py
--rw-r--r--   0        0        0     3228 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/mlcvzoo_mmocr_dataset.py
--rw-r--r--   0        0        0     4719 2023-05-11 08:05:29.657505 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/model.py
--rw-r--r--   0        0        0      154 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/py.typed
--rw-r--r--   0        0        0      379 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/structs.py
--rw-r--r--   0        0        0     4828 2023-05-11 08:05:29.657505 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_detection_model.py
--rw-r--r--   0        0        0     3947 2023-05-11 08:05:29.657505 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_recognition_model.py
--rw-r--r--   0        0        0    11416 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/LICENSE
--rw-r--r--   0        0        0      103 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/README.md
--rw-r--r--   0        0        0      154 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-10 13:07:55.992709 mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/mmocr.py
--rw-r--r--   0        0        0     3988 2023-05-11 14:03:20.820970 mlcvzoo_mmocr-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-5.0.1/setup.py
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/LICENSE
+-rw-r--r--   0        0        0      393 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/README.md
+-rw-r--r--   0        0        0      244 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/__init__.py
+-rw-r--r--   0        0        0     3491 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/configuration.py
+-rw-r--r--   0        0        0     2578 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/model.py
+-rw-r--r--   0        0        0        0 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/py.typed
+-rw-r--r--   0        0        0      421 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/structs.py
+-rw-r--r--   0        0        0     6068 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/text_detection_model.py
+-rw-r--r--   0        0        0     6010 2023-06-14 10:11:10.051267 mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/text_recognition_model.py
+-rw-r--r--   0        0        0     4048 2023-06-14 14:38:28.877095 mlcvzoo_mmocr-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-6.0.0/setup.py
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 mlcvzoo_mmocr-6.0.0/PKG-INFO
```

### Comparing `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/configuration.py` & `mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of the MMOCRConfig that is used to configure the MMOCRModel (and subclasses).
 """
 
 from __future__ import annotations
```

### Comparing `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/text_detection_model.py` & `mlcvzoo_mmocr-6.0.0/mlcvzoo_mmocr/text_detection_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for defining the model classes that are used to wrap the mmocr framework.
 """
 
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from mlcvzoo_base.api.data.annotation_class_mapper import AnnotationClassMapper
 from mlcvzoo_base.api.data.class_identifier import ClassIdentifier
-from mlcvzoo_base.api.data.segmentation import PolygonType, Segmentation
+from mlcvzoo_base.api.data.segmentation import Segmentation
 from mlcvzoo_base.api.model import SegmentationModel
+from mlcvzoo_mmdetection.model import MMDetectionModel
+from mmocr.apis.inferencers import TextDetInferencer
+from mmocr.structures.textdet_data_sample import TextDetDataSample
 from nptyping import Int, NDArray, Shape
 
 from mlcvzoo_mmocr.configuration import MMOCRConfig
 from mlcvzoo_mmocr.model import MMOCRModel
 
 logger = logging.getLogger(__name__)
 
@@ -32,14 +36,16 @@
         self,
         from_yaml: Optional[str] = None,
         configuration: Optional[MMOCRConfig] = None,
         string_replacement_map: Optional[Dict[str, str]] = None,
         init_for_inference: bool = False,
         is_multi_gpu_instance: bool = False,
     ) -> None:
+        self.inferencer: Optional[TextDetInferencer] = None
+
         MMOCRModel.__init__(
             self,
             from_yaml=from_yaml,
             configuration=configuration,
             string_replacement_map=string_replacement_map,
             init_for_inference=init_for_inference,
             is_multi_gpu_instance=is_multi_gpu_instance,
@@ -49,91 +55,118 @@
             configuration=self.configuration,
             init_for_inference=init_for_inference,
             mapper=AnnotationClassMapper(
                 class_mapping=self.configuration.class_mapping,
             ),
         )
 
+    def _init_inference_model(self) -> None:
+        if self.net is None:
+            self.inferencer = TextDetInferencer(self.cfg, None)
+
+            self.net = self.inferencer.model
+
+            if self.configuration.inference_config.checkpoint_path != "":
+                self.restore(
+                    checkpoint_path=self.configuration.inference_config.checkpoint_path
+                )
+
     @property
     def num_classes(self) -> int:
         return self.mapper.num_classes
 
     def get_classes_id_dict(self) -> Dict[int, str]:
         return self.mapper.annotation_class_id_to_model_class_name_map
 
-    @staticmethod
-    def __decode_mmocr_result_to_list_of_points(
-        text_detection_result: List[float],
-    ) -> PolygonType:
-        """
-        Converts MMOCR result to list of tuples. MMOCR stores the result as
-        [x,y,x,y,x,y,x,y, ..., score]. This function takes all but the last
-        element (the score) of the MMOCR result and reshapes them.
-        The returned format is [(x, y), (x, y), ...].
-        """
-
-        # we skip last entry because this is a confidence value
-        return list(zip(text_detection_result[:-1:2], text_detection_result[1:-1:2]))
-
-    def __process_text_detection_result(
-        self, result: Dict[str, Any]
+    def __decode_mmocr_result(
+        self, prediction: TextDetDataSample
     ) -> List[Segmentation]:
-        segmentations: List[Segmentation] = list()
-
-        for text_detection_result in result["boundary_result"]:
-            score: float = text_detection_result[-1]
-
-            polygon: PolygonType = (
-                MMOCRTextDetectionModel.__decode_mmocr_result_to_list_of_points(
-                    text_detection_result=text_detection_result
+        segmentations: List[Segmentation] = []
+        for polygons, score in zip(
+            prediction.pred_instances.polygons, prediction.pred_instances.scores
+        ):
+            float_score = float(score)
+            if float_score < self.configuration.inference_config.score_threshold:
+                continue
+
+            polygon_iterator = iter(polygons)
+
+            segmentations.extend(
+                self.build_segmentations(
+                    class_identifiers=[
+                        ClassIdentifier(
+                            class_id=MMOCRConfig.__text_class_id__,
+                            class_name=MMOCRConfig.__text_class_name__,
+                        )
+                    ],
+                    score=score,
+                    polygon=list(zip(polygon_iterator, polygon_iterator)),
                 )
             )
 
-            if score >= self.configuration.inference_config.score_threshold:
-                segmentations.extend(
-                    self.build_segmentations(
-                        class_identifiers=[
-                            ClassIdentifier(
-                                class_id=MMOCRConfig.__text_class_id__,
-                                class_name=MMOCRConfig.__text_class_name__,
-                            )
-                        ],
-                        score=score,
-                        polygon=polygon,
-                    )
-                )
-
-                if self.configuration.inference_config.to_rect_polygon:
-                    for segmentation in segmentations:
-                        segmentation.to_rect_polygon()
+            # TODO: Move directly into the "build_segmentation" method?
+            if self.configuration.inference_config.to_rect_polygon:
+                for segmentation in segmentations:
+                    segmentation.to_rect_polygon()
 
         return segmentations
 
     def predict(
         self, data_item: Union[str, ImageType]
     ) -> Tuple[Union[str, ImageType], List[Segmentation]]:
-        assert self.net is not None
+        if self.net is None:
+            raise ValueError(
+                "The 'net' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
+        if self.inferencer is None:
+            raise ValueError(
+                "The 'inferencer' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
 
-        return data_item, self.__process_text_detection_result(
-            result=self._predict(data_item=data_item)
+        # For a single data_item we only have one prediction
+        return data_item, self.__decode_mmocr_result(
+            self.inferencer(
+                data_item, return_datasamples=True, batch_size=1, progress_bar=False
+            )["predictions"][0]
         )
 
     def predict_many(
         self, data_items: List[Union[str, ImageType]]
     ) -> List[Tuple[Union[str, ImageType], List[Segmentation]]]:
-        assert self.net is not None
+        if self.net is None:
+            raise ValueError(
+                "The 'net' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
+        if self.inferencer is None:
+            raise ValueError(
+                "The 'inferencer' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
 
         prediction_list: List[Tuple[Union[str, ImageType], List[Segmentation]]] = []
 
-        results = self._predict(data_item=data_items)
+        # TODO: add batch-size as parameter
+        predictions: List[TextDetDataSample] = self.inferencer(
+            data_items,
+            return_datasamples=True,
+            batch_size=len(data_items),
+            progress_bar=False,
+        )["predictions"]
 
-        for data_item, result in zip(data_items, results):
-            segmentations = self.__process_text_detection_result(result=result)
+        for data_item, prediction in zip(data_items, predictions):
+            segmentations = self.__decode_mmocr_result(prediction=prediction)
 
             prediction_list.append(
                 (
                     data_item,
                     segmentations,
                 )
             )
 
         return prediction_list
+
+
+if __name__ == "__main__":
+    MMDetectionModel.run(MMOCRTextDetectionModel)
```

### Comparing `mlcvzoo_mmocr-5.0.1/mlcvzoo_mmocr/third_party/LICENSE` & `mlcvzoo_mmocr-6.0.0/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,203 +1,220 @@
-Copyright (c) MMOCR Authors. All rights reserved.
+Open Logistics Foundation License
+Version 1.3, January 2023
+https://www.openlogisticsfoundation.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION AND DISTRIBUTION
+
+§1 Definitions
+
+(1) "Subject Matter of the License" shall mean the works of software components
+in Source or Object form as well as any other components protected under
+copyright, design and/or patent law which are made available under this License.
+
+(2) "License" shall mean the terms and conditions for the use, reproduction and
+distribution of the Subject Matter of the License in accordance with the
+provisions of this document.
+
+(3) "Licensor(s)" shall mean the copyright holder(s) or the entity authorized by
+law or contract by the copyright holder(s) to grant the License.
+
+(4) "You" (or "Your") shall mean a natural or legal person exercising the
+permissions granted by this License.
+
+(5) "Source" form shall mean the preferred form for making modifications,
+including but not limited to software source code, documentation source, and
+configuration files.
+
+(6) "Object" form shall mean any form resulting from mechanical transformation
+or translation of a Source form, including but not limited to compiled object
+code, generated documentation, and conversions to other media types.
+
+(7) "Derivative Works" shall mean any work, whether in Source or Object form or
+any other form, that is based on (or derived from) the Subject Matter of the
+License and for which the editorial revisions, annotations, elaborations, or
+other modifications represent, as a whole, an original work of authorship. For
+the purposes of this License, Derivative Works shall not include works that
+remain separable from, or merely link (or bind by name) to the interfaces of,
+the Subject Matter of the License and Derivative Works thereof.
+
+(8) "Contribution" shall mean any proprietary work, including the original
+version of the Subject Matter of the License and any changes or additions to
+such work, or Derivative Works of such work, that the rights holder, or a
+natural or legal person authorized to make submissions, intentionally submits to
+a Licensor to be incorporated into the Subject Matter of the License. For the
+purposes of this definition, "submit" shall mean any form of electronic or
+written communication which is sent to a Licensor or its representatives for the
+purpose of discussing or improving the Subject Matter of the License, including
+but not limited to communications sent via electronic mailing lists, source code
+control systems and issue tracking systems; however, communications that are
+clearly marked by the copyright holder as "not a contribution" or otherwise
+identified as such in writing are excluded.
+
+(9) "Contributor" shall mean the Licensor(s) and/or any natural or legal person
+on whose behalf the Licensor(s) receive(s) any Contribution subsequently
+incorporated into the Subject Matter of the License.
+
+§2 Grant of usage rights
+
+Subject to the terms and conditions of this License and compliance with the
+provisions of this License, You are hereby granted by each Contributor, insofar
+as applicable to the respective Subject Matter of the License the
+
+- royalty-free and non-exclusive,
+- sub-licensable for commercial and non-commercial purposes,
+- worldwide and perpetual,
+- irrevocable and non-terminable
+
+right to reproduce, prepare Derivative Works of, publicly display, publicly
+perform, and distribute the Subject Matter of the License and such Derivative
+Works in any form. This right of use includes but is not limited to the right
+
+- to use the Subject Matter of the License in any hardware and software
+  environment (with regard to the software and data components), in particular
+  to store or load it permanently or temporarily, to display it and run it,
+  including to the extent reproductions are necessary to that end,
+- to otherwise modify, interpret, edit or redesign it,
+- to store, reproduce, exhibit, publish, distribute it in tangible or intangible
+  form, on any medium or in any other way, for commercial and non-commercial
+  purposes, in particular to communicate it privately or publicly, including via
+  image, audio and other information carriers, irrespective of whether by wire
+  or wireless means,
+- to use it in databases, data networks and online services, including the right
+  to make the software and data components of the Subject Matter of the License
+  available in Source or Object form to users of the aforementioned databases,
+  networks and online services for research and retrieval purposes,
+- to allow third parties to use or operate it,
+- to use it for own purposes but also to provide services to third parties,
+- to distribute it
+
+in its original or modified, interpreted, edited or redesigned form.
+
+The foregoing right of use relates to the Subject Matter of the License, in
+particular to its Source and Object form of software components (including
+design rights, where applicable).
+
+§3 Grant of patent license
+
+Subject to the terms and conditions of this License and compliance with the
+provisions of this License, You are hereby granted by each Contributor a
+- royalty-free and non-exclusive,
+- worldwide and perpetual,
+- irrevocable (with the exception of the restrictions set out in this Section 3)
+
+patent license in all rights deriving from the patents, owned and licensable by
+the Contributor at the time of the submission of the Contribution, to
+
+- produce,
+- have produced,
+- use,
+- offer for sale,
+- sell,
+- import and otherwise transfer
+
+the Subject Matter of the License.
+
+However, said patent license shall cover only those rights deriving from the
+patents of the respective Contributors which are indispensable in order not to
+infringe that patent and only to the extent that the use of the Contributor’s
+respective Contributions, whether alone or in combination with other
+Contributions of the Contributors or any third parties together with the Subject
+Matter of the License for which these Contributions were submitted, would
+otherwise infringe that patent. The grant of license shall not include rights
+deriving from the patents which may in future become necessary for their lawful
+use due to subsequent modifications to the Subject Matter or Contributions made
+by third parties after the original submission.
+
+In the event that You institute patent litigation against any entity or person
+(including a counterclaim or countersuit in a legal action), alleging that the
+Subject Matter of the License or a Contribution incorporated or contained
+therein constitutes patent infringement or indirect infringement, all patent
+licenses which have been granted to You under this License for the Subject
+Matter of the License as well as this License itself shall be deemed terminated
+as of the date on which the action is filed.
+
+§4 Distribution
+
+You may reproduce and distribute copies of the Subject Matter of the License or
+Derivative Works on any medium, with or without modifications (with regard to
+software components in Source or Object form), provided that You comply with
+the following rules:
+
+- You must provide all other recipients of the Subject Matter of the License or
+  of Derivative Works with a copy of this License and inform them that the
+  Subject Matter of the License was originally licensed under this License.
+- You must ensure that modified files contain prominent notices indicating that
+  You have modified the files.
+- You must retain all copyright, patent, trademark and attribution notices in
+  the Subject Matter of the License in the Source form of any Derivative Works
+  You distribute, with the exception of those notices that do not pertain to any
+  part of the Derivative Works.
+
+You may add Your own copyright notices to Your modifications and state any
+additional or different license conditions and conditions for the use,
+reproduction or distribution of Your modifications or for those Derivative Works
+as a whole, provided that Your use, reproduction and distribution of the work
+complies with the terms and conditions set out in this License in all other
+respects.
+
+§5 Submission of Contributions
+
+Unless expressly stated otherwise, every Contribution that You have
+intentionally submitted for inclusion in the Subject Matter of the License is
+subject to this License without any additional terms or conditions applying.
+Irrespective of the above, none of the terms or conditions contained herein may
+be interpreted to supersede or modify the terms or conditions of any separate
+licensing agreement that You may have concluded with a Licensor for such
+Contributions, such as a so-called "Contributor License Agreement" (CLA).
+
+§6 Trademarks
+
+This License does not grant permission to use the trade names, trademarks,
+service marks or product names of the Licensor(s) or of a Contributor.
+
+§7 Limited warranty
+
+This License is granted free of charge and thus constitutes a gift. Accordingly,
+any warranty is excluded. The Subject Matter of the License is a work in
+progress; it is constantly being improved by countless Contributors. The Subject
+Matter of the License is not complete and may therefore contain errors ("bugs")
+or additional patents of Contributors or third parties, as is inherent in this
+type of development.
+
+§8 Limitation of liability
+
+Except in cases of intentional and grossly negligent conduct, the Contributors,
+their legal representatives, trustees, officers and employees shall not be
+liable for direct or indirect, material or immaterial loss or damage of any kind
+arising from the License or the use of the Subject Matter of the License; this
+applies, among other things, but not exclusively, to loss of goodwill, loss of
+production, computer failures or errors, loss of data or economic loss or
+damage, even if the Contributor has been notified of the possibility of such
+loss or damage. Irrespective of the above, the Licensor shall only be liable
+within the scope of statutory product liability to the extent that the
+respective provisions are applicable to the Subject Matter of the License or the
+Contribution.
+
+Except in cases of intentional conduct, the Contributors, their legal
+representatives, trustees, officers and employees shall not be liable for any
+infringement of third-party patent or intellectual property rights arising from
+the Contributions nor do they warrant that the Contributions are accurate,
+devoid of mistakes, complete and/or fit for any particular purpose.
+
+§9 Provision of warranties or assumption of additional liability in the event of
+distribution of the Subject Matter of the License
+
+In the event of distribution of the Subject Matter of the License or Derivative
+Works, You are free to accept support, warranty, indemnity or other liability
+obligations and/or rights consistent with this License and to charge a fee in
+return. However, in accepting such obligations, You may act only on Your own
+behalf and on Your sole responsibility, not on behalf of any other Contributor,
+and You hereby agree to indemnify, defend, and hold each Contributor harmless
+for any liability incurred by, or claims asserted against, such Contributor by
+reason of Your accepting any such warranty or additional liability.
+
+§10 Applicable law
+
+This License is governed by German law, excluding its conflict of laws
+provisions and the provisions of the UN Convention on Contracts for the
+International Sale of Goods (CISG).
 
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2021 MMOCR Authors. All rights reserved.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+END OF TERMS AND CONDITIONS
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlcvzoo_mmocr-5.0.1/pyproject.toml` & `mlcvzoo_mmocr-6.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "mlcvzoo_mmocr"
-version = "5.0.1"
-license = "Open Logistics License Version 1.0"
 description = "MLCVZoo MMOCR Package"
+version = "6.0.0"
+license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -31,40 +31,39 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 yaml-config-builder = { version = "^8" }
 related-mltoolbox = { version = "^1" }
 mlcvzoo_base = { version = "^5" }
-mlcvzoo_mmdetection = { version = "^5" }
+mlcvzoo_mmdetection = { version = "^6" }
 
-attrs = { version = ">=20" }
 # 4.6.0.66 leads to errors when building mmcv-full
-opencv-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
-opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
-mmocr = { version=">=0.3,<=0.6.3" }
-mmdet = { version="^2.11.0" }
-# mmocr 0.6 has <= 1.6.0
-mmcv-full = { version=">=1.3.4,!=1.3.18" }
+opencv-python = { version = ">=4.5,!=4.5.5.64,!=4.6.0.66" }
+opencv-contrib-python = { version = ">=4.5,!=4.5.5.64,!=4.6.0.66" }
+attrs = { version = ">=20" }
+mmocr = { version = "^1.0" }
 pycocotools = { version=">=2.0.2", markers = "platform_machine == 'x86_64'" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
 nptyping = { version = ">=2.0" }
-torch = { version = ">=1.9" }
+# torch 2.0.1 has missing cuda dependencies https://github.com/pytorch/pytorch/issues/100974
+torch = { version = ">=1.9,!=2.0.1" }
 torchvision = { version = ">=0.10" }
 
 [tool.poetry.dev-dependencies]
 mock = { version = ">=4.0" }
 pytest = { version = ">=7.0" }
 pytest-cov = { version = ">=3.0.0" }
 black = { version = ">=22" }
 mypy = { version = ">=0.961" }
 pylint = { version = ">=2.9.6" }
-isort = { version = ">=5.9" }
-pytest-mock = ">=3.7"
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
+pytest-mock = { version = ">=3.7" }
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_mmocr-5.0.1/setup.py` & `mlcvzoo_mmocr-6.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mlcvzoo_mmocr', 'mlcvzoo_mmocr.third_party']
+['mlcvzoo_mmocr']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
  'mlcvzoo_base>=5,<6',
- 'mlcvzoo_mmdetection>=5,<6',
- 'mmcv-full>=1.3.4,!=1.3.18',
- 'mmdet>=2.11.0,<3.0.0',
- 'mmocr>=0.3,<=0.6.3',
+ 'mlcvzoo_mmdetection>=6,<7',
+ 'mmocr>=1.0,<2.0',
  'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
- 'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
- 'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
+ 'opencv-contrib-python>=4.5,!=4.5.5.64,!=4.6.0.66',
+ 'opencv-python>=4.5,!=4.5.5.64,!=4.6.0.66',
  'related-mltoolbox>=1,<2',
- 'torch>=1.9',
+ 'torch>=1.9,!=2.0.1',
  'torchvision>=0.10',
  'yaml-config-builder>=8,<9']
 
 extras_require = \
 {':platform_machine == "x86_64"': ['pycocotools>=2.0.2']}
 
 setup_kwargs = {
     'name': 'mlcvzoo-mmocr',
-    'version': '5.0.1',
+    'version': '6.0.0',
     'description': 'MLCVZoo MMOCR Package',
     'long_description': '# MLCVZoo MMOCR\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_mmocr** is the wrapper module for\nthe [mmocr framework](https://github.com/open-mmlab/mmocr).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-mmocr\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_mmocr-5.0.1/PKG-INFO` & `mlcvzoo_mmocr-6.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmocr
-Version: 5.0.1
+Version: 6.0.0
 Summary: MLCVZoo MMOCR Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
-License: Open Logistics License Version 1.0
+License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20)
 Requires-Dist: mlcvzoo_base (>=5,<6)
-Requires-Dist: mlcvzoo_mmdetection (>=5,<6)
-Requires-Dist: mmcv-full (>=1.3.4,!=1.3.18)
-Requires-Dist: mmdet (>=2.11.0,<3.0.0)
-Requires-Dist: mmocr (>=0.3,<=0.6.3)
+Requires-Dist: mlcvzoo_mmdetection (>=6,<7)
+Requires-Dist: mmocr (>=1.0,<2.0)
 Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
-Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: opencv-python (>=4.5,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: pycocotools (>=2.0.2) ; platform_machine == "x86_64"
 Requires-Dist: related-mltoolbox (>=1,<2)
-Requires-Dist: torch (>=1.9)
+Requires-Dist: torch (>=1.9,!=2.0.1)
 Requires-Dist: torchvision (>=0.10)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo MMOCR
```


# Comparing `tmp/prodiapy-2.6.tar.gz` & `tmp/prodiapy-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-2.6.tar", last modified: Thu May 18 10:11:04 2023, max compression
+gzip compressed data, was "prodiapy-3.0.tar", last modified: Thu Jun 15 13:06:08 2023, max compression
```

## Comparing `prodiapy-2.6.tar` & `prodiapy-3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:11:04.680724 prodiapy-2.6/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-2.6/LICENSE
--rw-rw-rw-   0        0        0     1039 2023-05-18 10:11:04.679238 prodiapy-2.6/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-05-17 08:01:08.000000 prodiapy-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 10:11:04.666673 prodiapy-2.6/prodia/
--rw-rw-rw-   0        0        0      132 2023-05-17 08:01:33.000000 prodiapy-2.6/prodia/__init__.py
--rw-rw-rw-   0        0        0     2290 2023-05-16 11:51:42.000000 prodiapy-2.6/prodia/data.py
--rw-rw-rw-   0        0        0    15009 2023-05-17 08:47:07.000000 prodiapy-2.6/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:11:04.679238 prodiapy-2.6/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1039 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 10:11:04.000000 prodiapy-2.6/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 10:11:04.681228 prodiapy-2.6/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-05-17 08:45:42.000000 prodiapy-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:06:08.005341 prodiapy-3.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.0/LICENSE
+-rw-rw-rw-   0        0        0     1050 2023-06-15 13:06:08.003862 prodiapy-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-06-15 13:03:38.000000 prodiapy-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:06:07.994346 prodiapy-3.0/prodia/
+-rw-rw-rw-   0        0        0      240 2023-06-15 12:59:58.000000 prodiapy-3.0/prodia/__init__.py
+-rw-rw-rw-   0        0        0     4226 2023-06-14 12:51:44.000000 prodiapy-3.0/prodia/ext.py
+-rw-rw-rw-   0        0        0    12226 2023-06-15 12:59:11.000000 prodiapy-3.0/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:06:08.003862 prodiapy-3.0/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1050 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-15 13:06:07.000000 prodiapy-3.0/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:06:08.005341 prodiapy-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-06-15 13:01:38.000000 prodiapy-3.0/setup.py
```

### Comparing `prodiapy-2.6/LICENSE` & `prodiapy-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-2.6/PKG-INFO` & `prodiapy-3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 2.6
+Version: 3.0
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==2.5
+pip install prodiapy==3.0
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-prodia.Client(api_key=key)
+client = prodia.Client(api_key=key)
 
 image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 [Full Documentation](https://prodiapy.readme.io/)
 
-Feel free to join out [Discord server](https://discord.gg/eAcrtqaE) and ask question!
+Feel free to join out [Discord server](https://discord.gg/qX5dwV3HEp) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodiapy-2.6/README.md` & `prodiapy-3.0/prodiapy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+Metadata-Version: 2.1
+Name: prodiapy
+Version: 3.0
+Summary: Prodia API Python Wrapper
+Author: yoou3-cyber
+Author-email: zenafey@eugw.ru
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==2.5
+pip install prodiapy==3.0
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-prodia.Client(api_key=key)
+client = prodia.Client(api_key=key)
 
 image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 [Full Documentation](https://prodiapy.readme.io/)
 
-Feel free to join out [Discord server](https://discord.gg/eAcrtqaE) and ask question!
+Feel free to join out [Discord server](https://discord.gg/qX5dwV3HEp) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```

### Comparing `prodiapy-2.6/prodia/main.py` & `prodiapy-3.0/prodia/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,423 +1,318 @@
 import requests
 import time
 import os
 import asyncio
+from prodia import endpoint, names
 
 
-api_key = None
 
-def Client(api_key:str=None):
-    if api_key is None:
-        print("No API key provided")
-        return
-    else:
-        global key
-        key = api_key
-
-def models():
-    print('Available models:')
-    print(Models.mlist)
-
-def samplers():
-    print('Available samplers:')
-    print(Samplers.slist)
-
-def aspect_ratios():
-    print('Available ratios:')
-    print(ar.alist)
-
-
-def txt2img(
-        prompt:str=None,
-        negative_prompt:str="badly draw",
-        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
-        sampler:str="Heun",
-        aspect_ratio:str="square",
-        steps:int=25,
-        cfg_scale:int=7,
-        seed:int=-1,
-        upscale:bool=False):
-    if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
-    else:
-        if prompt == None:
-            print("LOG: Prompt was not defined, used default (kittens on cloud)")
-            prompt = "kittens on cloud"
-        url = "https://api.prodia.com/v1/job"
+async def one_txt2img(key:str = None,
+                      prompt: str = None,
+                      negative_prompt: str = "badly drawn",
+                      model: str = names.realisticvs14,
+                      sampler: str = "DDIM",
+                      aspect_ratio: str = "square",
+                      steps: int = 30,
+                      cfg_scale: int = 7,
+                      seed: int = -1,
+                      upscale: bool = False):
+    payload = {
+        "prompt": prompt,
+        "model": model,
+        "sampler": sampler,
+        "negative_prompt": negative_prompt,
+        "steps": steps,
+        "cfg_scale": cfg_scale,
+        "seed": seed,
+        "upscale": upscale,
+        "aspect_ratio": aspect_ratio
+    }
+    headers = {
+        "accept": "application/json",
+        "content-type": "application/json",
+        "X-Prodia-Key": key
+    }
+    headers2 = {
+        "accept": "application/json",
+        "X-Prodia-Key": key
+    }
+    print(f"txt2img image with params:\n{payload}")
+    response = requests.post(endpoint.txt2img, json=payload, headers=headers)
+    job_id = response.json()['job']
+    await asyncio.sleep(3)
+
+    stt = True
+    while stt is True:
+        rec = requests.get(endpoint.retrieve.format(job_id=job_id), headers=headers2)
+        status = rec.json()['status']
+        if status == "succeeded":
+            print(f"Image {job_id} generated!")
+            image_url = rec.json()['imageUrl']
+            stt = False
+            return image_url
+        elif status == "queued":
+            print("Still working...")
+            await asyncio.sleep(2)
+        elif status == "generating":
+            print("Still working...")
+            await asyncio.sleep(2)
+        else:
+            print(f"Something went wrong! Please try later, error: {status}")
+            stt = False
+            return status
+
+async def one_img2img(key:str = None,
+                      image_url:str = None,
+                      prompt: str = None,
+                      negative_prompt: str = "badly drawn",
+                      model: str = names.realisticvs14,
+                      sampler: str = "DDIM",
+                      denoising_strength: float=0.6,
+                      steps: int = 30,
+                      cfg_scale: int = 7,
+                      seed: int = -1,
+                      upscale: bool = False):
+    payload = {
+        "steps": steps,
+        "sampler": sampler,
+        "imageUrl": image_url,
+        "model": model,
+        "prompt": prompt,
+        "denoising_strength": denoising_strength,
+        "negative_prompt": negative_prompt,
+        "cfg_scale": cfg_scale,
+        "seed": seed,
+        "upscale": upscale
+    }
+    headers = {
+        "accept": "application/json",
+        "content-type": "application/json",
+        "X-Prodia-Key": key
+    }
+    headers2 = {
+        "accept": "application/json",
+        "X-Prodia-Key": key
+    }
+    print(f"img2img image with params:\n{payload}")
+    response = requests.post(endpoint.img2img, json=payload, headers=headers)
+    job_id = response.json()['job']
+    await asyncio.sleep(3)
+
+    stt = True
+    while stt is True:
+        rec = requests.get(endpoint.retrieve.format(job_id=job_id), headers=headers2)
+        status = rec.json()['status']
+        if status == "succeeded":
+            print(f"Image {job_id} generated!")
+            image_url = rec.json()['imageUrl']
+            stt = False
+            return image_url
+        elif status == "queued":
+            print("Still working...")
+            await asyncio.sleep(2)
+        elif status == "generating":
+            print("Still working...")
+            await asyncio.sleep(2)
+        else:
+            print(f"Something went wrong! Please try later, error: {status}")
+            stt = False
+            return status
+
+
+
+async def gather(mode:str ="txt2img", key:str = None, image_url:str = None, prompt: str = None,
+                             negative_prompt: str = "badly drawn",
+                             model: str = names.realisticvs14,
+                             sampler: str = "DDIM",
+                             denoising_strength:float=0.6,
+                             aspect_ratio: str = "square",
+                             steps: int = 30,
+                             cfg_scale: int = 7,
+                             seed: int = -1,
+                             upscale: bool = False,
+                             number_outputs: int = 1, images: list = None):
+        if mode == "txt2img":
+            images = await asyncio.gather(*[one_txt2img(key=key, prompt=prompt, negative_prompt=negative_prompt, model=model, sampler=sampler, aspect_ratio=aspect_ratio, steps=steps, cfg_scale=cfg_scale, seed=seed, upscale=upscale) for _ in range(number_outputs)])
+            return images
+        elif mode == "img2img":
+            images = await asyncio.gather(*[
+                one_img2img(key=key, image_url=image_url, prompt=prompt, negative_prompt=negative_prompt, model=model, sampler=sampler,
+                            denoising_strength=denoising_strength, steps=steps, cfg_scale=cfg_scale, seed=seed, upscale=upscale) for
+                _ in range(number_outputs)])
+            return images
+        elif mode == "save":
+            await asyncio.gather(*[one_save(images=images) for _ in range(len(images))])
+
+
+
+class Client:
+    def __init__(self, api_key:str) -> None:
+        self.api_key = api_key
+
+    def txt2img(self,
+                          prompt: str = None,
+                          negative_prompt: str = "badly drawn",
+                          model: str = names.realisticvs14,
+                          sampler: str = "DDIM",
+                          aspect_ratio: str = "square",
+                          steps: int = 30,
+                          cfg_scale: int = 7,
+                          seed: int = -1,
+                          upscale: bool = False):
+        if prompt is None:
+            print("Prompt cant be empty")
+            return
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
             "cfg_scale": cfg_scale,
             "seed": seed,
             "upscale": upscale,
             "aspect_ratio": aspect_ratio
         }
         headers = {
             "accept": "application/json",
             "content-type": "application/json",
-            "X-Prodia-Key": key
+            "X-Prodia-Key": self.api_key
         }
         headers2 = {
             "accept": "application/json",
-            "X-Prodia-Key": key
+            "X-Prodia-Key": self.api_key
         }
-        print(f"LOG: txt2img image with params:\n{payload}")
-        response = requests.post(url, json=payload, headers=headers)
-        job_id = response.json()['job']
+        print(f"txt2img image with params:\n{payload}")
+        response = requests.post(endpoint.txt2img, json=payload, headers=headers)
+        try:
+            job_id = response.json()['job']
+        except ValueError:
+            print(f"Invalid generation parameters || {response.status_code} || {response.content}")
+            return
         time.sleep(3)
 
-        retrieve_url = f'https://api.prodia.com/v1/job/{job_id}'
         stt = True
         while stt is True:
-            rec = requests.get(retrieve_url, headers=headers2)
+            rec = requests.get(endpoint.retrieve.format(job_id=job_id), headers=headers2)
             status = rec.json()['status']
             if status == "succeeded":
                 print(f"Image {job_id} generated!")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
                 time.sleep(2)
             elif status == "generating":
                 print("Still working...")
                 time.sleep(2)
             else:
-                print(f"ERROR: Something went wrong! Please try later, error: {status}")
+                print(f"Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
-
-def img2img(
-        imageUrl:str=None,
-        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
-        prompt:str=None,
-        denoising_strength:float=0.7,
-        negative_prompt:str="badly drawn",
-        steps:int=25,
-        cfg_scale:int=7,
-        seed:int=-1,
-        upscale:bool=False,
-        sampler:str="Heun"):
-
-    if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API key at https://app.prodia.com/api\nto define api key use:\nprodia.Client(api_key='your-key')")
-    elif imageUrl is None:
-        print("ERROR: Image URL is required and cannot be empty")
-    elif prompt is None:
-        print("ERROR: Prompt is required and cannot be empty")
-    else:
-        url = "https://api.prodia.com/v1/transform"
-
+    def img2img(self, image_url: str = None,
+                          prompt: str = None,
+                          negative_prompt: str = "badly drawn",
+                          model: str = names.realisticvs14,
+                          sampler: str = "DDIM",
+                          denoising_strength: float = 0.6,
+                          steps: int = 30,
+                          cfg_scale: int = 7,
+                          seed: int = -1,
+                          upscale: bool = False):
+        if image_url is None:
+            print("image_url cant be none")
+            return
+        if prompt is None:
+            print("Prompt cant be empty")
+            return
         payload = {
             "steps": steps,
             "sampler": sampler,
-            "imageUrl": imageUrl,
+            "imageUrl": image_url,
             "model": model,
             "prompt": prompt,
             "denoising_strength": denoising_strength,
             "negative_prompt": negative_prompt,
             "cfg_scale": cfg_scale,
             "seed": seed,
             "upscale": upscale
         }
         headers = {
             "accept": "application/json",
             "content-type": "application/json",
-            "X-Prodia-Key": key
+            "X-Prodia-Key": self.api_key
         }
-        headersrecieve = {
+        headers2 = {
             "accept": "application/json",
-            "X-Prodia-Key": key
+            "X-Prodia-Key": self.api_key
         }
-        print(f"LOG: img2img image with params:\n{payload}")
-        response = requests.post(url, json=payload, headers=headers)
-        job_id = response.json()['job']
-        time.sleep(5)
+        print(f"img2img image with params:\n{payload}")
+        response = requests.post(endpoint.txt2img, json=payload, headers=headers)
+        try:
+            job_id = response.json()['job']
+        except ValueError:
+            print(f"Invalid generation parameters || {response.status_code} || {response.content}")
+            return
+        time.sleep(3)
 
-        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
         stt = True
         while stt is True:
-            rec = requests.get(rec_url, headers=headersrecieve)
+            rec = requests.get(endpoint.retrieve.format(job_id=job_id), headers=headers2)
             status = rec.json()['status']
             if status == "succeeded":
-                print(f"LOG: Image {job_id} generated!")
+                print(f"Image {job_id} generated!")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
-                time.sleep(3)
+                time.sleep(2)
             elif status == "generating":
                 print("Still working...")
-                time.sleep(3)
+                time.sleep(2)
             else:
-                print(f"ERROR: Something went wrong! Please try later, error: {status}")
+                print(f"Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
-def control_net_scribble(
-        imageUrl:str=None,
-        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
-        prompt:str=None,
-        negative_prompt:str="badly drawn",
-        steps:int=25,
-        cfg_scale:int=7,
-        seed:int=-1,
-        sampler:str="Heun"):
-
-    if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API key at https://app.prodia.com/api\nto define api key use:\nprodia.Client(api_key='your-key')")
-    elif imageUrl is None:
-        print("ERROR: Image URL is required and cannot be empty")
-    elif prompt is None:
-        print("ERROR: Prompt is required and cannot be empty")
-    else:
-        url = "https://api.prodia.com/v1/controlnet/scribble"
-
-        payload = {
-            "steps": steps,
-            "sampler": sampler,
-            "imageUrl": imageUrl,
-            "model": model,
-            "prompt": prompt,
-            "negative_prompt": negative_prompt,
-            "cfg_scale": cfg_scale,
-            "seed": seed
-        }
-        headers = {
-            "accept": "application/json",
-            "content-type": "application/json",
-            "X-Prodia-Key": key
-        }
-        headersrecieve = {
-            "accept": "application/json",
-            "X-Prodia-Key": key
-        }
-        print(f"LOG: control_net image with params:\n{payload}")
-        response = requests.post(url, json=payload, headers=headers)
-        job_id = response.json()['job']
-        time.sleep(5)
-
-        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
-        stt = True
-        while stt is True:
-            rec = requests.get(rec_url, headers=headersrecieve)
-            status = rec.json()['status']
-            if status == "succeeded":
-                print(f"LOG: Image {job_id} generated!")
-                image_url = rec.json()['imageUrl']
-                stt = False
-                return image_url
-            elif status == "queued":
-                print("Still working...")
-                time.sleep(3)
-            elif status == "generating":
-                print("Still working...")
-                time.sleep(3)
-            else:
-                print(f"ERROR: Something went wrong! Please try later, error: {status}")
-                stt = False
-                return status
+class AsyncClient:
+    def __init__(self, api_key:str) -> None:
+        self.api_key = api_key
 
-async def arunv1(
-        prompt:str="kittens on cloud",
+    async def txt2img(self, prompt:str=None,
         negative_prompt:str="badly drawn",
-        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
-        sampler:str="Heun",
+        model:str=names.realisticvs14,
+        sampler:str="DDIM",
         aspect_ratio:str="square",
-        steps:int=25,
-        cfg_scale:int=7,
-        seed:int=-1,
-        upscale:bool=False):
-    if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.Client(api_key='your-key')")
-    else:
-        if prompt == "kittens on cloud" or prompt == "" or prompt == " ":
-            print("LOG: Prompt was not defined or empty, used default (kittens on cloud)")
-        url = "https://api.prodia.com/v1/job"
-        payload = {
-            "prompt": prompt,
-            "model": model,
-            "sampler": sampler,
-            "negative_prompt": negative_prompt,
-            "steps": steps,
-            "cfg_scale": cfg_scale,
-            "seed": seed,
-            "upscale": upscale,
-            "aspect_ratio": aspect_ratio
-        }
-        headers = {
-            "accept": "application/json",
-            "content-type": "application/json",
-            "X-Prodia-Key": key
-        }
-        headersrecieve = {
-            "accept": "application/json",
-            "X-Prodia-Key": key
-        }
-        print(f"LOG: txt2img image with params:\n{payload}")
-        response = requests.post(url, json=payload, headers=headers)
-        job_id = response.json()['job']
-        await asyncio.sleep(3)
-
-        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
-        stt = True
-        while stt is True:
-            rec = requests.get(rec_url, headers=headersrecieve)
-            status = rec.json()['status']
-            if status == "succeeded":
-                print(f"Image {job_id} generated!")
-                image_url = rec.json()['imageUrl']
-                stt = False
-                return image_url
-            elif status == "queued":
-                print("Still working...")
-                await asyncio.sleep(2)
-            elif status == "generating":
-                print("Still working...")
-                await asyncio.sleep(2)
-            else:
-                print(f"ERROR: Something went wrong! Please try later, error: {status}")
-                stt = False
-                return status
-
-
-async def arunv2(
-        imageUrl:str=None,
-        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
-        prompt:str=None,
-        denoising_strength:float=0.7,
-        negative_prompt:str="badly drawn, low detailed, ugly, mutated, unralistic",
-        steps:int=25,
+        steps:int=30,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False,
-        sampler:str="Heun"):
-
-    if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
-    elif imageUrl is None:
-        print("ERROR: Image URL is required and cannot be empty")
-    elif prompt is None:
-        print("ERROR: Prompt is required and cannot be empty")
-    else:
-        url = "https://api.prodia.com/v1/transform"
-
-        payload = {
-            "steps": steps,
-            "sampler": sampler,
-            "imageUrl": imageUrl,
-            "model": model,
-            "prompt": prompt,
-            "denoising_strength": denoising_strength,
-            "negative_prompt": negative_prompt,
-            "cfg_scale": cfg_scale,
-            "seed": seed,
-            "upscale": upscale
-        }
-        headers = {
-            "accept": "application/json",
-            "content-type": "application/json",
-            "X-Prodia-Key": key
-        }
-        headersrecieve = {
-            "accept": "application/json",
-            "X-Prodia-Key": key
-        }
-        print(f"LOG: img2img image with params:\n{payload}")
-        response = requests.post(url, json=payload, headers=headers)
-        job_id = response.json()['job']
-        await asyncio.sleep(4)
-
-        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
-        stt = True
-        while stt is True:
-            rec = requests.get(rec_url, headers=headersrecieve)
-            status = rec.json()['status']
-            if status == "succeeded":
-                print(f"LOG: Image {job_id} generated!")
-                image_url = rec.json()['imageUrl']
-                stt = False
-                return image_url
-            elif status == "queued":
-                print("Still working...")
-                await asyncio.sleep(2)
-            elif status == "generating":
-                print("Still working...")
-                await asyncio.sleep(2)
-            else:
-                print(f"ERROR: Something went wrong! Please try later, error: {status}")
-                stt = False
-                return status
+        number_outputs:int=1):
+        if prompt is None:
+            print("Prompt cant be empty")
+            return
+        images = await gather(mode="txt2img", key=self.api_key, prompt=prompt, negative_prompt=negative_prompt, model=model, sampler=sampler, aspect_ratio=aspect_ratio, steps=steps, cfg_scale=cfg_scale, seed=seed, upscale=upscale, number_outputs=number_outputs)
+        return images
 
-async def arunv3(
-        imageUrl:str=None,
-        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
-        prompt:str=None,
-        negative_prompt:str="badly drawn, low detailed, ugly, mutated, unralistic",
-        steps:int=25,
+    async def img2img(self, image_url:str = None, prompt:str=None,
+        negative_prompt:str="badly drawn",
+        model:str=names.realisticvs14,
+        sampler:str="DDIM",
+        denoising_strength:float=0.6,
+        steps:int=30,
         cfg_scale:int=7,
         seed:int=-1,
-        sampler:str="Heun"):
-
-    if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
-    elif imageUrl is None:
-        print("ERROR: Image URL is required and cannot be empty")
-    elif prompt is None:
-        print("ERROR: Prompt is required and cannot be empty")
-    else:
-        url = "https://api.prodia.com/v1/controlnet/scribble"
-
-        payload = {
-            "steps": steps,
-            "sampler": sampler,
-            "imageUrl": imageUrl,
-            "model": model,
-            "prompt": prompt,
-            "negative_prompt": negative_prompt,
-            "cfg_scale": cfg_scale,
-            "seed": seed
-        }
-        headers = {
-            "accept": "application/json",
-            "content-type": "application/json",
-            "X-Prodia-Key": key
-        }
-        headersrecieve = {
-            "accept": "application/json",
-            "X-Prodia-Key": key
-        }
-        print(f"LOG: img2img image with params:\n{payload}")
-        response = requests.post(url, json=payload, headers=headers)
-        job_id = response.json()['job']
-        await asyncio.sleep(4)
-
-        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
-        stt = True
-        while stt is True:
-            rec = requests.get(rec_url, headers=headersrecieve)
-            status = rec.json()['status']
-            if status == "succeeded":
-                print(f"LOG: Image {job_id} generated!")
-                image_url = rec.json()['imageUrl']
-                stt = False
-                return image_url
-            elif status == "queued":
-                print("Still working...")
-                await asyncio.sleep(2)
-            elif status == "generating":
-                print("Still working...")
-                await asyncio.sleep(2)
-            else:
-                print(f"ERROR: Something went wrong! Please try later, error: {status}")
-                stt = False
-                return status
-
-
-
+        upscale:bool=False,
+        number_outputs:int=1):
+        if image_url is None:
+            print("image_url cant be none")
+            return
+        if prompt is None:
+            print("Prompt cant be empty")
+            return
+        images = await gather(mode="img2img", key=self.api_key, image_url=image_url, prompt=prompt, negative_prompt=negative_prompt, model=model, sampler=sampler, denoising_strength=denoising_strength, steps=steps, cfg_scale=cfg_scale, seed=seed, upscale=upscale, number_outputs=number_outputs)
+        return images
```

### Comparing `prodiapy-2.6/prodiapy.egg-info/PKG-INFO` & `prodiapy-3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-Metadata-Version: 2.1
-Name: prodiapy
-Version: 2.6
-Summary: Prodia API Python Wrapper
-Author: yoou3-cyber
-Author-email: zenafey@eugw.ru
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==2.5
+pip install prodiapy==3.0
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
 
 key = "your-prodia-key"
 
-prodia.Client(api_key=key)
+client = prodia.Client(api_key=key)
 
 image = prodia.txt2img(prompt="kittens on cloud", model="dreamlike-diffusion-2.0.safetensors [fdcf65e7]")
 print(image)
 ```
 `image` variable will be a url of your image
 
 [Full Documentation](https://prodiapy.readme.io/)
 
-Feel free to join out [Discord server](https://discord.gg/eAcrtqaE) and ask question!
+Feel free to join out [Discord server](https://discord.gg/qX5dwV3HEp) and ask question!
 
 ![7eacddcb-3a45-4114-b731-3cd7af9522e1](https://user-images.githubusercontent.com/118455214/233359979-80274381-10dd-4ced-b7fa-d45437ef5bce.png)
```


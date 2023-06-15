# Comparing `tmp/qsm-forward-0.5.tar.gz` & `tmp/qsm-forward-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm-forward-0.5.tar", last modified: Wed Jun 14 06:57:44 2023, max compression
+gzip compressed data, was "qsm-forward-0.6.tar", last modified: Thu Jun 15 07:31:27 2023, max compression
```

## Comparing `qsm-forward-0.5.tar` & `qsm-forward-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.5/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 06:57:44.977896 qsm-forward-0.5/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm-forward-0.5/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-14 06:55:50.000000 qsm-forward-0.5/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      465 2023-06-14 05:36:03.000000 qsm-forward-0.5/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    19754 2023-06-14 06:54:44.000000 qsm-forward-0.5/qsm_forward/qsm_forward.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-14 06:57:44.000000 qsm-forward-0.5/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-14 06:57:44.977896 qsm-forward-0.5/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-14 06:55:36.000000 qsm-forward-0.5/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-14 06:57:44.977896 qsm-forward-0.5/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.5/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm-forward-0.6/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-15 07:31:27.754525 qsm-forward-0.6/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     5541 2023-06-15 07:31:12.000000 qsm-forward-0.6/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-15 07:22:16.000000 qsm-forward-0.6/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      429 2023-06-15 07:28:11.000000 qsm-forward-0.6/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    21162 2023-06-15 07:27:02.000000 qsm-forward-0.6/qsm_forward/qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     6312 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      292 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       19 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-15 07:31:27.000000 qsm-forward-0.6/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-15 07:31:27.754525 qsm-forward-0.6/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      812 2023-06-15 07:22:21.000000 qsm-forward-0.6/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-15 07:31:27.754525 qsm-forward-0.6/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm-forward-0.6/tests/test_qsm_forward.py
```

### Comparing `qsm-forward-0.5/LICENSE` & `qsm-forward-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm-forward-0.5/pyproject.toml` & `qsm-forward-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm-forward"
-version = "0.5"
+version = "0.6"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `qsm-forward-0.5/qsm_forward/qsm_forward.py` & `qsm-forward-0.6/qsm_forward/qsm_forward.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,149 +8,221 @@
 from nilearn.image import resample_img
 
 import json
 import os
 import nibabel as nib
 import numpy as np
 
-# Default parameters for tissue
-default_tissue_params = {
-    "chi_path" : "ChiModelMIX_noCalc.nii.gz",
-    "M0_path" : "M0.nii.gz",
-    "R1_path" : "R1.nii.gz",
-    "R2star_path" : "R2star.nii.gz",
-    "mask_path" : "BrainMask.nii.gz",
-    "seg_path" : "SegmentedModel.nii.gz"
-}
-
-# Default parameters for reconstruction
-default_recon_params = {
-    "Subject" : "1",                # Subject ID
-    "Session" : "1",                # Session ID
-    "Run" : 1,                      # Run number
-    "TR" : 50e-3,                   # Repetition time (in seconds)
-    "TEs" : np.array([ 4e-3, 12e-3, 20e-3, 28e-3 ]), # Echo times (in seconds)
-    "flip_angle" : 15,              # Flip angle (in degrees)
-    "B0" : 7,                       # Magnetic field strength (in Tesla)
-    "B0_dir" : np.array([0, 0, 1]), # B0 field direction
-    "phase_offset" : 0,             # Phase offset (in radians)
-    "generate_phase_offset": True,  # Boolean to control phase offset generation
-    "generate_shim_field" : True,   # Boolean to control shim field generation
-    "voxel_size" : np.array([1.0, 1.0, 1.0]), # Voxel size (in mm)
-    "peak_snr" : np.inf             # Peak signal-to-noise ratio
-}
+class TissueParams:
+    """
+    A class used to represent tissue parameters.
+
+    Attributes
+    ----------
+    chi_path : str
+        The path to the Chi file.
+    M0_path : str
+        The path to the M0 file.
+    R1_path : str
+        The path to the R1 file.
+    R2star_path : str
+        The path to the R2* file.
+    mask_path : str
+        The path to the brain mask file.
+    seg_path : str
+        The path to the segmentation file.
+    """
+
+    def __init__(
+            self,
+            root_dir = "",
+            chi_fname = "ChiModelMIX_noCalc.nii.gz",
+            M0_fname = "M0.nii.gz",
+            R1_fname = "R1.nii.gz",
+            R2star_fname = "R2star.nii.gz",
+            mask_fname = "BrainMask.nii.gz",
+            seg_fname = "SegmentedModel.nii.gz"
+    ):
+        self.chi_path = os.path.join(root_dir, chi_fname)
+        self.M0_path = os.path.join(root_dir, M0_fname)
+        self.R1_path = os.path.join(root_dir, R1_fname)
+        self.R2star_path = os.path.join(root_dir, R2star_fname)
+        self.mask_path = os.path.join(root_dir, mask_fname)
+        self.seg_path = os.path.join(root_dir, seg_fname)
+        
+
+class ReconParams:
+    """
+    A class used to represent reconstruction parameters.
+
+    Attributes
+    ----------
+    subject : str
+        The ID of the subject.
+    session : str
+        The ID of the session.
+    run : int
+        The run number.
+    TR : float
+        Repetition time (in seconds).
+    TEs : np.array
+        Echo times (in seconds).
+    flip_angle : int
+        Flip angle (in degrees).
+    B0 : int
+        Magnetic field strength (in Tesla).
+    B0_dir : np.array
+        B0 field direction.
+    phase_offset : int
+        Phase offset (in radians).
+    generate_phase_offset : bool
+        Boolean to control phase offset generation.
+    generate_shim_field : bool
+        Boolean to control shim field generation.
+    voxel_size : np.array
+        Voxel size (in mm).
+    peak_snr : float
+        Peak signal-to-noise ratio.
+    """
+
+    def __init__(
+            self,
+            subject="1",
+            session="1",
+            run="1",
+            TR=50e3,
+            TEs=np.array([ 4e-3, 12e-3, 20e-3, 28e-3 ]),
+            flip_angle=15,
+            B0=7,
+            B0_dir=np.array([0, 0, 1]),
+            phase_offset=0,
+            generate_phase_offset=True,
+            generate_shim_field=True,
+            voxel_size=np.array([1.0, 1.0, 1.0]),
+            peak_snr=np.inf
+        ):
+        self.subject = subject
+        self.session = session
+        self.run = run
+        self.TR = TR
+        self.TEs = TEs
+        self.flip_angle = flip_angle
+        self.B0 = B0
+        self.B0_dir = B0_dir
+        self.phase_offset = phase_offset
+        self.generate_phase_offset = generate_phase_offset
+        self.generate_shim_field = generate_shim_field
+        self.voxel_size = voxel_size
+        self.peak_snr = peak_snr
 
 def generate_bids(tissue_params, recon_params, bids_dir):
     """
-    Generate T2*-weighted MRI signals and save the outputs in the BIDS-compliant format.
+    Simulate T2*-weighted magnitude and phase images and save the outputs in the BIDS-compliant format.
 
     This function simulates a T2*-weighted MRI signal based on a ground truth susceptibility map,
-    computes the necessary parameters, and saves the outputs (images, JSON headers) in the BIDS-compliant
-    format in the specified directory.
+    and saves the outputs (images, JSON headers) in the BIDS-compliant format in the specified
+    directory.
 
     Parameters:
-    tissue_params (dict): A dictionary containing paths to different tissue parameter files.
-        Keys are: "chi_path", "M0_path", "R1_path", "R2star_path", "mask_path", and "seg_path".
+    tissue_params (TissueParams): Provides paths to different tissue parameter files.
 
-    recon_params (dict): A dictionary containing the parameters for the reconstruction simulation.
-        Keys are: "Subject", "Session", "Run", "TR", "TEs", "flip_angle", "B0", "B0_dir",
-        "phase_offset", "shimm", "voxel_size", "peak_snr".
+    recon_params (ReconParams): Provides parameters for the simulated reconstruction.
 
     bids_dir (str): The directory where the BIDS-formatted outputs will be saved.
 
     Returns:
     None. Outputs are saved as files in the bids_dir directory.
 
     """
 
     # create output directories
     print("Creating output directory...")
     os.makedirs(bids_dir, exist_ok=True)
     
     # recon name
-    recon_name = f"sub-{recon_params['Subject']}_ses-{recon_params['Session']}_run-{recon_params['Run']}"
-    session_dir = os.path.join(bids_dir, f"sub-{recon_params['Subject']}", f"ses-{recon_params['Session']}")
+    recon_name = f"sub-{recon_params.subject}_ses-{recon_params.session}_run-{recon_params.run}"
+    session_dir = os.path.join(bids_dir, f"sub-{recon_params.subject}", f"ses-{recon_params.session}")
     os.makedirs(os.path.join(session_dir, 'anat'), exist_ok=True)
     os.makedirs(os.path.join(session_dir, 'extra_data'), exist_ok=True)
 
     # image-space resizing
-    chi_nii = nib.load(tissue_params['chi_path'])
+    chi_nii = nib.load(tissue_params.chi_path)
     print("Image-space resizing of chi...")
-    chi_downsampled_nii = resize(chi_nii, recon_params['voxel_size'])
+    chi_downsampled_nii = resize(chi_nii, recon_params.voxel_size)
     nib.save(chi_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_chi.nii"))
-    if os.path.exists(str(tissue_params['mask_path'])):
+    if os.path.exists(str(tissue_params.mask_path)):
         print("Image-space cropping of mask...")
-        mask_downsampled_nii = resize(nib.load(tissue_params['mask_path']), recon_params['voxel_size'], 'nearest')
+        mask_downsampled_nii = resize(nib.load(tissue_params.mask_path), recon_params.voxel_size, 'nearest')
         nib.save(mask_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_mask.nii"))
         del mask_downsampled_nii
-    if os.path.exists(str(tissue_params['seg_path'])):
+    if os.path.exists(str(tissue_params.seg_path)):
         print("Image-space cropping of segmentation...")
-        seg_downsampled_nii = resize(nib.load(tissue_params['seg_path']), recon_params['voxel_size'], 'nearest')
+        seg_downsampled_nii = resize(nib.load(tissue_params.seg_path), recon_params.voxel_size, 'nearest')
         nib.save(seg_downsampled_nii, filename=os.path.join(session_dir, "extra_data", f"{recon_name}_segmentation.nii"))
         del seg_downsampled_nii
 
     # calculate field
     print("Computing field model...")
     chi = chi_nii.get_fdata()
     field = generate_field(chi)
     del chi
 
     # simulate shim field
-    mask = nib.load(tissue_params['mask_path']).get_fdata() if os.path.exists(tissue_params['mask_path']) else np.ones(field.shape)
-    if recon_params['generate_shim_field']:
+    mask = nib.load(tissue_params.mask_path).get_fdata() if os.path.exists(tissue_params.mask_path) else np.ones(field.shape)
+    if recon_params.generate_shim_field:
         print("Computing shim fields...")
         _, field, _ = generate_shimmed_field(field, mask, order=2)
 
     # phase offset
-    M0 = nib.load(tissue_params['M0_path']).get_fdata() if os.path.exists(tissue_params['M0_path']) else np.ones(field.shape) * mask
-    if recon_params['generate_phase_offset']:
+    M0 = nib.load(tissue_params.M0_path).get_fdata() if os.path.exists(tissue_params.M0_path) else np.ones(field.shape) * mask
+    if recon_params.generate_phase_offset:
         print("Computing phase offset...")
-        phase_offset = recon_params['phase_offset'] + generate_phase_offset(M0, mask, M0.shape)
+        phase_offset = recon_params.phase_offset + generate_phase_offset(M0, mask, M0.shape)
 
     # signal model
-    multiecho = len(recon_params['TEs']) > 1
-    R1 = nib.load(tissue_params['R1_path']).get_fdata() if os.path.exists(tissue_params['R1_path']) else np.ones(field.shape) * mask
-    R2star = nib.load(tissue_params['R2star_path']).get_fdata() if os.path.exists(tissue_params['R2star_path']) else np.ones(field.shape) * mask
+    multiecho = len(recon_params.TEs) > 1
+    R1 = nib.load(tissue_params.R1_path).get_fdata() if os.path.exists(tissue_params.R1_path) else np.ones(field.shape) * mask
+    R2star = nib.load(tissue_params.R2star_path).get_fdata() if os.path.exists(tissue_params.R2star_path) else np.ones(field.shape) * mask
     del mask
-    for i in range(len(recon_params['TEs'])):
+    for i in range(len(recon_params.TEs)):
         print(f"Computing MR signal for echo {i+1}...")
         recon_name_i = f"{recon_name}_echo-{i+1}" if multiecho else recon_name
 
         sigHR = generate_signal(
             field=field,
-            B0=recon_params['B0'],
-            TR=recon_params['TR'],
-            TE=recon_params['TEs'][i],
-            flip_angle=recon_params['flip_angle'],
+            B0=recon_params.B0,
+            TR=recon_params.TR,
+            TE=recon_params.TEs[i],
+            flip_angle=recon_params.flip_angle,
             phase_offset=phase_offset,
             R1=R1,
             R2star=R2star,
             M0=M0
         )
     
         # k-space cropping of sigHR
         print(f"k-space cropping of MR signal for echo {i+1}...")
-        resolution = np.array(np.round((np.array(chi_nii.header.get_zooms()) / recon_params['voxel_size']) * np.array(chi_nii.header.get_data_shape())), dtype=int)
+        resolution = np.array(np.round((np.array(chi_nii.header.get_zooms()) / recon_params.voxel_size) * np.array(chi_nii.header.get_data_shape())), dtype=int)
         sigHR_cropped = crop_kspace(sigHR, resolution)
         del sigHR
 
         # noise
         print(f"Simulating noise for echo {i+1}...")
-        sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params['peak_snr'])
+        sigHR_cropped_noisy = add_noise(sigHR_cropped, peak_snr=recon_params.peak_snr)
         del sigHR_cropped
 
         # save nifti images
         mag_filename = f"{recon_name_i}_part-mag" + ("_MEGRE" if multiecho else "_T2starw")
         phs_filename = f"{recon_name_i}_part-phase" + ("_MEGRE" if multiecho else "_T2starw")
         nib.save(nib.Nifti1Image(dataobj=np.abs(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{mag_filename}.nii"))
         nib.save(nib.Nifti1Image(dataobj=np.angle(sigHR_cropped_noisy), affine=chi_downsampled_nii.affine, header=chi_downsampled_nii.header), filename=os.path.join(session_dir, "anat", f"{phs_filename}.nii"))
 
         # json header
         print(f"Creating JSON headers...")
-        json_dict = { 'EchoTime': recon_params['TEs'][i], 'MagneticFieldStrength': recon_params['B0'], 'EchoNumber': i+1, 'ProtocolName': 'T2starw', 'ConversionSoftware': 'qsm-forward' }
+        json_dict = { 'EchoTime': recon_params.TEs[i], 'MagneticFieldStrength': recon_params.B0, 'EchoNumber': i+1, 'ProtocolName': 'T2starw', 'ConversionSoftware': 'qsm-forward' }
 
         json_dict_phs = json_dict.copy()
         json_dict_phs['ImageType'] = ['P', 'PHASE']
         json_dict_mag = json_dict.copy()
         json_dict_mag['ImageType'] = ['M', 'MAGNITUDE']
 
         with open(os.path.join(session_dir, "anat", f"{mag_filename}.json"), 'w') as mag_json_file:
```

### Comparing `qsm-forward-0.5/setup.py` & `qsm-forward-0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm-forward',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```


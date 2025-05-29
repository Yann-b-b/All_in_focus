# All-in-Focus Pipeline

This repository contains focal stack image sets and Jupyter notebooks for generating all-in-focus images using different alignment strategies.

## Folder Structure

- `photos1/`  
- `photos2/`  
- `photos3/`  
- `photos4/`  
- `photos_synthetic/`  
  > Each folder contains a set of images taken at different focus levels to be used in the all-in-focus image synthesis pipeline.

## Notebooks

- `THISONE_ALIGN.ipynb`  
  This notebook performs the full pipeline **with alignment**, including:
  - Loading and preprocessing focal stacks
  - Optical flow alignment
  - Focus measure calculation
  - Graph cuts-based depth map estimation
  - Image fusion

- `THISONE_NOALIGN.ipynb`  
  This notebook runs the same pipeline **without alignment**, useful when the input images are synthetically generated or already aligned.

## Usage

1. Place your focal stack images into one of the `photos*` folders.
2. Open and run either notebook depending on whether alignment is required.
3. The final output will be an all-in-focus image generated from the stack.

---

Feel free to fork or contribute!

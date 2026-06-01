# Image Stitching - Computer Vision Assignment 1

This project contains an image stitching pipeline for the Computer Vision 2026 first assignment. The notebook implements Harris corner detection, patch descriptors, descriptor matching, RANSAC-based affine estimation, panorama stitching, sensitivity analyses, and a SIFT comparison.

## Project Layout

```text
Assignment 1/
  notebooks/
    Image_Stitching_CV2026.ipynb
  data/
    images/
      leftImage.png
      rightImage.png
      pair*_left.jpg
      pair*_right.jpg
      ...
  outputs/
    cell-11/
    cell-12-15/
    cell-16/
    cell-17/
  reports/
    Computer_Vision_report.pdf
  docs/
    assignment-brief-image-stitching.pdf
  archives/
    images-1.zip
    Cezar_Ceausescu_First_Assignment_CV2026.zip
  requirements.txt
```

The `Code/` directory is left in place only for existing local environment/editor files. The active project files are in the directories above.

## Setup

From this directory:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Run The Notebook

Start Jupyter from the project root so paths resolve cleanly:

```powershell
jupyter lab notebooks\Image_Stitching_CV2026.ipynb
```

The first code cell locates `data/images` automatically. The default grader cell uses `leftImage.png` and `rightImage.png`; add new image pairs to `GRADER_PAIRS` in that cell to test other inputs.

## Outputs

Generated figures from previous runs are stored in `outputs/` by notebook cell group. The final report is in `reports/`, and the original assignment brief is in `docs/`.

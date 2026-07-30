# Atmospheric and Oceanic Controls of Coastal Upwelling in the Northern Gulf of Guinea: Insights from Keta, Ghana
_Reproducible code, data processing, and notebooks for the paper: “Atmospheric and Oceanic Controls of Coastal Upwelling in the Northern Gulf of Guinea: Insights from Keta, Ghana”_

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17534972.svg)](https://doi.org/10.5281/zenodo.17534972)




## Overview
This repository reproduces the full analysis pipeline:
- Compute Ekman (ECUI) and geostrophic (GCUI) upwelling indices
- Process SST, SSH, monthly anomalies on a common grid
- Correlation & lag–longitude diagnostics
- EOF/PCA across ECUI, GCUI, SST, SSH
- Plot figures used in the manuscript

**Study window:** 2010–2022  
**Focus region:** Eastern Ghana–Togo shelf near Keta (≈ 0–2°E, 4–6°N)

## Quick start (Binder)
Click the Binder badge above to open the environment in your browser and run:
- `notebooks/REFINED_EKMAN_CORRECTED.ipynb` → end-to-end processing and figures


## Local installation
```bash
# 1) Create the conda env (uses conda-forge)
mamba env create -f environment.yml   # or: conda env create -f environment.yml
conda activate gog-upwelling

# 2) (Optional) Register the kernel
python -m ipykernel install --user --name gog-upwelling

# Synergistic Drivers of Coastal Upwelling in the Gulf of Guinea (Insights from Keta, Ghana)
_Reproducible code, data processing, and notebooks for the paper: “Synergistic Atmospheric–Oceanic Controls of Coastal Upwelling in the Northern Gulf of Guinea: Insights from Keta, Ghana”_

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17534972.svg)](https://doi.org/10.5281/zenodo.17534972)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ORG/REPO/TAG?labpath=notebooks%2Frun_analysis.ipynb)

> 🔧 Replace `17534972`, `ORG/REPO`, and `TAG` after you mint your Zenodo DOI and GitHub release.

## Overview
This repository reproduces the full analysis pipeline:
- Compute Ekman (ECUI) and geostrophic (GCUI) upwelling indices
- Process SST, SSH, SSS monthly anomalies on a common grid
- Correlation & lag–longitude diagnostics
- Joint EOF/PCA across ECUI, GCUI, SST, SSH, SSS
- Plot figures used in the manuscript

**Study window:** 2010–2017  
**Focus region:** Eastern Ghana–Togo shelf near Keta (≈ 0–2°E, 2–6°N)

## Quick start (Binder)
Click the Binder badge above to open the environment in your browser and run:
- `notebooks/run_analysis.ipynb` → end-to-end processing and figures
- `notebooks/reproduce_eof_pca.ipynb` → joint EOF/PCA with saved outputs

## Local installation
```bash
# 1) Create the conda env (uses conda-forge)
mamba env create -f environment.yml   # or: conda env create -f environment.yml
conda activate gog-upwelling

# 2) (Optional) Register the kernel
python -m ipykernel install --user --name gog-upwelling

# Excess Heat Factor Based Analysis of Heatwave in Ghana

Companion code repository for:

> Yamba, E. I., Amponsah, D., Pinkrah, N. O., Oppong, S., Adjei, M. J., Ablerdu, A. K., Wemegah, C. S. **Excess Heat Factor Based Analysis of Heatwave Prevalence, Frequency, Duration and Intensity in Ghana.**

## Overview

This repository contains the analysis code used to characterize heatwaves across the five climatic zones of Ghana (Sudan Savannah, Guinea Savannah, Transition, Forest, Coastal) over 1960–2022. Heatwaves are detected using the Excess Heat Factor (EHF) framework, and their return periods are estimated using a Peaks-Over-Threshold (POT) approach with the Generalized Pareto Distribution (GPD).

## Contents

All analysis code is in a single script — **`EHF--CODES.ipynb`** — organised in five sections in the order results appear in the paper:

| # | Section | Paper | Output |
|---|---------|-------|--------|
| 1 | Standardized Temperature Anomaly Index (STAI) | §3.1 | Fig. 2 |
| 2 | Heatwave detection via the Excess Heat Factor | §3.2 | Figs. 3–7 |
| 3 | Total heatwave days & 5-year rolling mean | §3.3 | Fig. 8 |
| 4 | Station-level trends in annual heatwave days | §3.3 | Table 3 |
| 5 | Return levels of intensity & duration (POT + GPD) | §3.4 | Fig. 9 |

Cell markers (`# %%`) allow each section to be run interactively in VS Code, Spyder, or PyCharm.

## Data

Daily minimum and maximum temperature records (1960–2022) from 24 synoptic stations of the **Ghana Meteorological Agency (GMet)**, quality-controlled and gap-filled with the **ERA5 reanalysis**. Raw station data are not redistributed here and should be requested from GMet. The scripts expect station-level daily files of the form `<Station>_1960_2022_dTx_complete.txt` and `<Station>_1960_2022_dTn_complete.txt`.

## Requirements

Python 3.9+ with `numpy`, `pandas`, `scipy`, `matplotlib`, `seaborn`, and `pymannkendall`:

```bash
pip install numpy pandas scipy matplotlib seaborn pymannkendall
```

## Citation

If you use this code, please cite the paper above.

## Contact

Corresponding author: **Edmund I. Yamba** — eiyamba@knust.edu.gh

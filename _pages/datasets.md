---
layout: page
permalink: /datasets/
title: datasets
description: Open datasets from my research, free to download and reuse.
nav: true
nav_order: 2
---

## High-Resolution Daily PM<sub>2.5</sub> for the Contiguous US (2005–2021)

<p>
  <a href="https://doi.org/10.5281/zenodo.20402757"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.20402757.svg" alt="DOI 10.5281/zenodo.20402757"></a>
  <img src="https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey.svg" alt="License: CC BY 4.0">
</p>

Daily surface PM<sub>2.5</sub> estimates at **1 km** across the contiguous United States, from **August 2005 to December 2021**. The estimates come from a bidirectional LSTM with attention that combines EPA ground monitors, satellite remote sensing, and wildfire smoke density observations. It does especially well on high-pollution days, such as wildfire smoke events, where many existing products underestimate.

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/pm25_dataset_map.jpg" class="img-fluid rounded z-depth-1" zoomable=true alt="Model predictions during the 2020 California August Complex Fire" %}
  </div>
</div>
<div class="caption">
  Predictions during the 2020 August Complex Fire in California: (1) CONUS-wide predictions, (2) zoomed-in predictions, (3) NOAA smoke density polygons, and (4) bias at EPA monitors.
</div>

| | |
|---|---|
| **Coverage** | Contiguous United States |
| **Resolution** | 1 km, daily |
| **Period** | Aug 25, 2005 – Dec 31, 2021 |
| **Variable** | Surface PM<sub>2.5</sub> concentration (µg/m³) |
| **Format** | One ZIP per year (monthly files inside), about 85 GB in total |
| **License** | CC BY 4.0 |

<p class="mt-3">
  <a class="btn btn-sm z-depth-0" role="button" href="https://doi.org/10.5281/zenodo.20402757">Download (Zenodo)</a>
  <a class="btn btn-sm z-depth-0" role="button" href="https://doi.org/10.3390/rs17010126">Paper</a>
  <a class="btn btn-sm z-depth-0" role="button" href="https://github.com/geohai/pm2.5_conus_lstm">Code</a>
</p>

**Citation.** If you use this dataset, please cite the paper:

> Wang, Z., Crooks, J. L., Regan, E. A., & Karimzadeh, M. (2025). High-Resolution Estimation of Daily PM<sub>2.5</sub> Levels in the Contiguous US Using Bi-LSTM with Attention. *Remote Sensing*, 17(1), 126. [https://doi.org/10.3390/rs17010126](https://doi.org/10.3390/rs17010126)

```bibtex
@article{wang2025pm25,
  author  = {Wang, Zhongying and Crooks, James L. and Regan, Elizabeth A. and Karimzadeh, Morteza},
  title   = {High-Resolution Estimation of Daily {PM2.5} Levels in the Contiguous {US} Using Bi-{LSTM} with Attention},
  journal = {Remote Sensing},
  year    = {2025},
  volume  = {17},
  number  = {1},
  pages   = {126},
  doi     = {10.3390/rs17010126}
}
```

Questions or ideas for using the data? Email me at [zywang16@mit.edu](mailto:zywang16@mit.edu).

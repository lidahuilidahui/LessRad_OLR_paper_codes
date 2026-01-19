# LessRad_OLR_paper_codes
This repository contains the Python (Jupyter Notebook) code used to generate specific figures 
(Figure 4 in the manuscript, corresponding to Figures 4 in the notebook execution, respectively) 
for the ESSD paper titled: "LessRad OLR: A New High-Resolution (0.05°, Hourly) Outgoing Longwave Radiation Dataset for Climate Monitoring from MODIS".

The code performs comparative analysis of various Outgoing Longwave Radiation (OLR) products, 
including the newly developed LessRad OLR, CERES SYN OLR, ERA5 OLR, CLARA-A3 OLR, and HIRS OLR, against the CERES EBAF OLR benchmark. 
Analyses focus on global and regional (Global Land/Ocean, Deserts, Deep Convective Regions, Polar Regions, Tibetan Plateau) monthly mean Bias and RMSE.

The primary input data for these specific plotting scripts are pre-processed monthly mean OLR data for each product, resampled to a common 1°x1° grid,
 covering the period 2001-2023. The notebook utilizes Xarray for data handling, Pandas for data structuring, NumPy for numerical operations, 
 and Ultraplot (a custom plotting library, likely based on Matplotlib) for generating the bar charts.
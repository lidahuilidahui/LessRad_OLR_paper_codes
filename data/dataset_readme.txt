# Data Files for LessRad OLR Paper Figure Generation

This directory (`data/`) contains the pre-processed input data files required by the Jupyter Notebook (`Fig5_Fig10to12_plot_codes.ipynb`)
to generate Figures 5, and 10-12 as presented in the Earth System Science Data (ESSD) manuscript : 
"LessRad OLR: A New High-Resolution (0.05°, Hourly) Outgoing Longwave Radiation Dataset for Climate Monitoring from MODIS".

All data files provided here are:
-   Monthly mean Outgoing Longwave Radiation (OLR) values.
-   Resampled to a common 1°x1° global grid (180 latitudes, 360 longitudes).
-   Covering the period from January 2001 to December 2023 (23 years * 12 months = 276 time steps).
-   Stored in NetCDF (.nc) format.
-   The dimensions of the OLR variable in each file are (time: 276, latitude: 180, longitude: 360).

## Files Included:

1.  **`LessRad_monthly_OLR_2001to2023_1degree.nc`**:
    * Description: Monthly mean LessRad OLR product, resampled to 1°x1° resolution.
    * Original Resolution: 0.05°, hourly.
    * Variable name within NetCDF: `LessRad OLR`

2.  **`CERES_SYN_monthly_OLR_2001to2023_1degree.nc`**:
    * Description: Monthly mean CERES SYN1deg OLR product (Edition 4.2).
    * Original Resolution: 1°x1°, hourly.
    * Variable name within NetCDF: `CERES SYN OLR`

3.  **`ERA5_monthly_OLR_2001to2023_1degree.nc`**:
    * Description: Monthly mean ERA5 OLR, resampled from its native resolution to 1°x1°.
    * Original Resolution: Approx. 0.25°, hourly.
    * Variable name within NetCDF: `ERA5 OLR`

4.  **`CLARA_A3_monthly_OLR_2001to2023_1degree.nc`**:
    * Description: Monthly mean EUMETSAT CM SAF CLARA-A3 OLR, resampled from its native resolution to 1°x1°.
    * Original Resolution: 0.25°, daily.
    * Variable name within NetCDF: `CLARA-A3 OLR`

5.  **`HIRS_monthly_OLR_2001to2023_1degree.nc`**:
    * Description: Monthly mean NOAA HIRS OLR CDR (v01r02).
    * Original Resolution: 1°x1°, daily (as per manuscript; some versions might be 2.5°).
    * Variable name within NetCDF: `HIRS OLR`

6.  **`CERES_EBAF_monthly_OLR_2001to2023_1degree.nc`**:
    * Description: Monthly mean CERES EBAF OLR product (Edition 4.2.1), used as the benchmark.
    * Original Resolution: 1°x1°, monthly.
    * Variable name within NetCDF: `CERES EBAF OLR`

7.  **`land_sea_mask_1degree.nc`**:
    * Description: Land-sea mask on a 1°x1° global grid. Used for regional analysis (separating land and ocean statistics).
    * Variable name within NetCDF: `lsm` (1 for land, 0 for ocean).

## Notes:
* These files are specifically prepared for the plotting script in this repository. 
* For access to the full, native resolution LessRad OLR dataset, 
* please refer to the data availability section in the main manuscript (DOI: https://doi.org/10.11888/Atmos.tpdc.301403).
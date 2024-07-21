# MCD19A2_MAIAC_AOD_Processing
This project processes MODIS (Moderate Resolution Imaging Spectroradiometer) Aerosol Optical Depth (AOD) data from the MCD19A2 product and creates a NetCDF file containing daily averaged AOD values. The script filters the data based on quality assurance flags, calculates daily averages, and stores the results in a structured NetCDF file.

## MODIS Product Details

- **Product**: MCD19A2 (MODIS Terra and Aqua Combined Multi-Angle Implementation of Atmospheric Correction (MAIAC) Land Aerosol Optical Depth Daily 1km)
- **Version**: 6
- **Parameters Used**:
  - Optical_Depth_055 (AOD at 550 nm)
  - Optical_Depth_047 (AOD at 470 nm)
  - AOD_QA (Quality assurance flags)

## Features

- Processes MODIS MCD19A2 AOD data for multiple orbits within a day
- Filters data based on quality assurance flags (values 1, 9, 8193, and 8201)
- Calculates daily averages for AOD at 550nm and 470nm
- Creates a structured NetCDF file with proper dimensions and attributes

## Requirements

- Python 3.x
- NumPy
- netCDF4
- pyproj


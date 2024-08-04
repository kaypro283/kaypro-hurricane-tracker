# Kaypro MBASIC-80 Hurricane Tracker

A comprehensive hurricane tracking and prediction program written in MBASIC-80 for Kaypro computers.

## About This Project

This hurricane tracker was a fun way for me to revisit BASIC programming and apply some interesting forecasting concepts on vintage hardware. While it uses real meteorological principles, it's important to understand that this is a hobby project and not meant for actual weather prediction. For real hurricane information, always refer to NOAA and the National Hurricane Center. They're the experts with the most up-to-date and accurate forecasts. This project is great for learning about weather modeling and enjoying some retro computing.

## Overview

This program allows users to track and predict the path of hurricanes based on manual entry or loaded data files. It uses advanced techniques such as Kalman filtering and weighted averaging to provide predictions.

## Features

- **Data Input**: Manual entry of hurricane data or loading from data files
- **Predictive Model**: Combines linear and exponential weighting for accurate forecasting
- **Visual Representation**: ASCII map showing projected and historic paths
- **Kalman Filter**: Enhances accuracy of projected positions
- **Wind Speed Projections**: Estimates wind speeds for up to 3 days
- **Wind Radii Calculations**: Projects 34, 50, and 64 kt wind radii for 3 days
- **Distance Calculations**: Uses Haversine formula for accurate distance measurements
- **Multiple Reporting Options**: Various data visualization and reporting features

## ASCII Map

The program generates a dynamic ASCII map to visualize hurricane paths and key locations. The map includes:

- Hurricane intensity symbols (D, S, 1-5)
- Projected path of storm
- Various major cities/locations

This visual representation allows for quick understanding of the hurricane's path and its relation to important geographical points.

## Kalman Filter

The program implements a Kalman filter to improve the accuracy of projected positions. This advanced technique:

- Predicts future states based on previous estimates
- Updates predictions using actual measurements
- Dynamically adapts to changing conditions
- Provides more reliable forecasts, especially for longer-term predictions

## Additional Notes

- The lines of code responsible for loading and saving files have been commented out (REM). You can restore this functionality by removing the REM statements.
- Sample .DAT files for historical hurricanes are included in the repository for testing and demonstration purposes.

## Usage

1. Run the program on a Kaypro computer or compatible emulator
2. Choose to enter new hurricane data or load existing data
3. Use the main menu to access various features and reports
4. Generate ASCII maps, view projections, and analyze wind speed data

## Creating and Uploading Data Files

The program provides pre-defined tracking data for Tropical Storm Debby (as of August 4, 2024). You are provided an option to use these data, upload a data file (*.dat), or manually input the hurricane storm data (you will be promoted to save the manually entered data after completing input). The repository includes a README.TXT file, which covers the requried format for data files. The format is very specific, so please follow it carefully. To upload a file:

1. Select option 2 from the initial menu to load from a file
2. Enter the filename (e.g., ALPHA.DAT) when prompted

THe repository contains an example data file (ALPHA.DAT) for uploading. Rememeber you have "un-rem" the lines of code associated with data loading/saving. This data file includes:

Number of days (10)

For each day:

Storm direction (degrees)
Storm speed (knots)
Latitude (degrees North)
Longitude (degrees West, negative)
Central pressure (millibars)
Maximum sustained wind speed (knots)

Hurricane Alpha in this example:

Starts north of Hispaniola
Moves through the Bahamas
Crosses the Florida Keys
Enters the Gulf of Mexico
Weakens as it approaches the northern Gulf Coast

## Contributing

Contributions, bug reports, and feature requests are welcome! Feel free to open an issue or submit a pull request.

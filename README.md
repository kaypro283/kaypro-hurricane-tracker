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

The program generates an ASCII map to visualize hurricane paths and key locations. The map legend includes:

- Hurricane intensity symbols (D, S, 1-5)
- Projected path markers (X)
- Key location markers (H, R, C, B, M, T, K, J, P, A)

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

## Data Files

The repository includes sample .DAT files for historical hurricanes. To use these:

1. Select option 2 from the initial menu to load from a file
2. Enter the filename (e.g., ELENA.DAT) when prompted

## Contributing

Contributions, bug reports, and feature requests are welcome! Feel free to open an issue or submit a pull request.

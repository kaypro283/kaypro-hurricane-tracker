Storm Data Format Instructions
This file explains the format for uploading storm data to the Kaypro Hurricane Tracker program.

File Format
Each storm data file should be a plain text file with the following structure:

First line: Number of days of data (integer, 2-20)
Subsequent lines: Data for each day, with 6 values per day, one value per line

Data values for each day:

Storm direction in degrees (0-360)
Storm speed in knots
Latitude (positive for North, negative for South)
Longitude (positive for East, negative for West)
Central pressure in millibars
Maximum sustained wind speed in knots

Example
Here's an example of a properly formatted storm data file:

5
315
14
24.1
-83.3
1005
40
290
14
20.9
-76.6
1012
25
290
14
21.4
-78.3
1012
25
285
12
21.4
-79.7
1010
25
285
14
22.0
-80.7
1009
25

This example represents 5 days of storm data.

Notes

Ensure each value is on a new line
Use decimal points for fractional values (e.g., 24.1 for latitude)
Use negative values for South latitude and West longitude
The file should have no empty lines between values
Save the file with a .DAT extension (e.g., STORM.DAT)

When loading data in the program, enter the filename exactly as it is saved, including the .DAT extension.
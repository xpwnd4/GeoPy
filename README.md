# GeoPy

GeoPy is a Python-based geocoding utility that processes company address data from an Excel file and converts it into latitude and longitude coordinates. This can be useful for mapping, location analysis, and data enrichment workflows.

## Features

- Reads address data from an Excel file
- Converts registered addresses into geographic coordinates
- Outputs the processed results into a new Excel file
- Simple and easy to run in a local Python environment

## Prerequisites

Before running the script, make sure you have the following installed:

- **Python 3**
- **Visual Studio Code** or any Python-compatible IDE

## Required Libraries

This project requires the following Python libraries:

- `pandas`
- `requests`

The following modules are included in Python by default, so no separate installation is needed:

- `json`
- `time`

To install the required libraries, run:

```bash
pip install pandas requests

Input File Requirements

Your Excel file must contain the following exact column headers:

Registered_Address
Company_name

These column names must match exactly, including capitalization and underscores.

Configuration
1. Set the input file name

Locate the following line in the script:

df = pd.read_excel("FILE-NAME.xlsx")

Replace "FILE-NAME.xlsx" with the name of your actual Excel input file.

Example:

df = pd.read_excel("companies.xlsx")
2. Set the output file name

Locate the line used to save the processed file:

df.to_excel("FILE-NAME.xlsx")

Replace "FILE-NAME.xlsx" with the name you want for the output file.

Example:

df.to_excel("companies_output.xlsx")
How to Run

Open your terminal in the project folder and run:

py geo.py
Example Workflow
Prepare an Excel file with the required headers:
Registered_Address
Company_name
Place the Excel file in the same folder as the script
Update the input file name in the script
Update the output file name in the script
Run the script using:
py geo.py
Output

The script will generate a new Excel file containing the processed results, including the corresponding latitude and longitude values for each registered address.

Notes
Make sure the Excel file is in the same directory as the script unless you specify the full file path.
Ensure the column headers are written exactly as required.
File names in the code must be enclosed in double quotes.
Incorrect column names may cause the script to fail during execution.
Use Case

This project is useful for:

Geocoding business address data
Supporting mapping and visualization projects
Automating coordinate lookups from spreadsheet-based records
Enriching datasets with location information
Author

Created as a simple geocoding utility for processing address-based Excel data using Python.


If you want, I can also make this README look more like a **professional portfolio project README** with 

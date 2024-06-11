# Statewide Longitudinal Data Systems Scraper

## Overview

The **Statewide Longitudinal Data Systems Scraper** is a Python script designed to scrape data from a specific webpage containing information about Statewide Longitudinal Data Systems. The script extracts the data, cleans it, and exports it to an Excel file with two sheets: one containing plain URLs and another with formatted hyperlinks. Additionally, it formats the headers and a specified row for better readability.

## Features

- **Web Scraping**: Extracts data from [Statewide Longitudinal Data Systems 2024](https://reports.ecs.org/comparisons/statewide-longitudinal-data-systems-2024).
- **Data Cleaning**: Removes unwanted text from headers.
- **Excel Export**: Creates an Excel file with two sheets:
  - **URL**: Contains the extracted URLs in plain text.
  - **Original**: Contains the original text with hyperlinks formatted in Excel.
- **Formatting**: Bolds the header rows and a specified row (row 51) in each sheet.
- **Dynamic File Saving**: Saves the Excel file to the user's desktop, regardless of the user running the script.

## Requirements

- `requests`
- `beautifulsoup4`
- `pandas`
- `openpyxl`
- `os` (standard library)

## Installation

Install the required packages using pip:

```bash
pip install requests beautifulsoup4 pandas openpyxl

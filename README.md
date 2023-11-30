# Challenge 5 README

## Athelic Sales Analysis

[Provide a clear and concise title for your assignment]

## Overview

[Provide a brief overview of the assignment, its purpose, and what it aims to achieve]

## Table of Contents

- [Data File](#data-files)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Dependencies](#dependencies)
- [Usage](#usage)

## Data Files

- [athletic_sales_2020.csv](link_to_athletic_sales_2020.csv)
- [athletic_sales_2021.csv](link_to_athletic_sales_2021.csv)

## Project Structure

```plaintext
athletic_sales_analysis/
│
├── Resources/
│   ├── athletic_sales_2020.csv
│   ├── athletic_sales_2021.csv
│
├── notebooks/
│   ├── athletic_sales_analysis.ipynb
│
└── README.md
```

## Getting Started

### Combine and Clean the Data

1. Import the CSV files, `athletic_sales_2020.csv` and `athletic_sales_2021.csv`.
2. Ensure similar column names and data types.
3. Combine the two DataFrames using an inner join and reset the index.

### Determine which Retailer had the Most Sales

1. Create a multi-index DataFrame with "retailer," "region," "state," and "city."
2. Rename the aggregated column and sort the results to show the top five retailers.

## Dependencies

Ensure the following dependencies are installed:

- [Pandas](https://pandas.pydata.org/)
- [Jupyter Notebooks](https://jupyter.org/)

## Usage

### Determine which Region Sold the Most Products

1. Use either `groupby` or `pivot_table` to create a multi-index DataFrame with "region," "state," and "city."
2. Rename the aggregated column and sort the results to show the top five regions with the greatest number of products sold.

### Determine which Region had the Most Sales

1. Similar to the previous section, focus on total sales.

### Determine which Retailer had the Most Sales

1. Create a multi-index DataFrame with "retailer," "region," "state," and "city."
2. Rename the aggregated column and sort the results to show the top five retailers.

### Determine which Retailer Sold the Most Women's Athletic Footwear

1. Filter the combined DataFrame for women's athletic footwear sales.
2. Create a multi-index DataFrame with "retailer," "region," "state," and "city."
3. Rename the aggregated column and sort the results to show the top five retailers.

### Determine the Day with the Most Women's Athletic Footwear Sales

1. Create a pivot table with "invoice_date" as the index and "total_sales" as the values.
2. Rename the aggregated column and use the `resample` function to place the data into daily bins.
3. Sort the resampled DataFrame to show the top 10 days.

### Determine the Week with the Most Women's Athletic Footwear Sales

1. Apply `resample` to the pivot table, placing the data into weekly bins.
2. Sort the resampled DataFrame to show the top 10 weeks.
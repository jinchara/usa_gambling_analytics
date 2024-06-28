# README

## Project Overview

This project is focused on extracting and analyzing data related to commercial gaming revenue by state for the year 2023. The data is sourced from the [Gambling Industry News website](https://gamblingindustrynews.com/usa-gambling-statistics/). The project involves web scraping, data cleaning, and visualization to provide insights into the US gambling industry's performance in 2023.

## Code Functionality

### Dependencies

The project requires the following Python libraries:
- `requests`: For sending HTTP requests to fetch the web page.
- `BeautifulSoup` from `bs4`: For parsing HTML content.
- `pandas`: For data manipulation and analysis.
- `csv`: For writing data to a CSV file.
- `matplotlib`: For data visualization.

### Steps

1. **Web Scraping**:
    - The code sends a GET request to the specified URL to fetch the webpage content.
    - It parses the HTML content using BeautifulSoup to find the relevant table containing commercial gaming revenue data.

2. **Data Extraction**:
    - The table headers and rows are extracted from the HTML and stored in a DataFrame.
    - Headers are obtained from `<th>` elements, and data rows are obtained from `<td>` elements.

3. **Data Cleaning**:
    - A function `convert_to_numeric` is defined to convert revenue values from string format (with currency symbols and units) to numeric format.
    - Rows with missing or invalid revenue data are dropped.
    - The 'Annual Change %' column is cleaned by removing the '%' symbol and converting the values to floats.

4. **Data Storage**:
    - The cleaned data is written to a CSV file named `table.csv` using the `csv` module.

5. **Data Visualization**:
    - Two bar charts are created using `matplotlib`:
        - **Commercial Gaming Revenue by State**: Displays the revenue for each state in millions of dollars.
        - **Annual Change Percentage by State**: Shows the annual percentage change in revenue for each state.

## Contact

For any questions or issues, please contact [Your Name] at [Your Email].

---

This README provides an overview of the project, instructions for setup and usage, and context for the analysis. Adjust the contact information as necessary.

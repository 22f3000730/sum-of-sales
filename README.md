# Sales Summary Single Page Application

## Overview
This is a simple single-page application that reads sales data from a CSV file encoded in base64 format, sums the sales column, and displays the total on the page.

## Requirements
- A valid CSV file containing sales data with a header named `sales`.
- Bootstrap 5 for styling.

## Implementation Details
1. The application fetches the `data.csv` data from an embedded data URI.
2. It decodes the base64 encoded CSV data and parses it into rows and columns.
3. The first row is treated as the header to locate the `sales` column.
4. It sums up all the values in the `sales` column.
5. The title of the document is set according to a specified format.
6. The total sales amount is displayed in an HTML element with the ID `total-sales`.

## How to Run
You can simply load this HTML page in a web browser to see the application in action.

## Testing
The implementation includes the following checks:
- Verify that the document title is set correctly.
- Check that Bootstrap is loaded from jsdelivr.
- Assert that the calculated total sales is congruent with the expected result.

## Error Handling
The application includes error handling for the following cases:
- If the sales column is not found in the CSV data.
- Parsing errors while converting CSV values to numbers.
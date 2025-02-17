
# Data Cleaning in Pandas

This script demonstrates basic data cleaning operations using Python's Pandas library. The operations performed include reading an Excel file, removing duplicates, dropping unnecessary columns, handling missing values, standardizing string formats, splitting address data, and filtering out records based on conditions.

## Overview

The data cleaning process involves the following steps:

1. **Read Data:**  
   The script starts by loading data from an Excel file (`Customer Call List.xlsx`) into a Pandas DataFrame.

2. **Remove Duplicates:**  
   Duplicate rows are removed from the DataFrame.

3. **Drop Unwanted Column:**  
   A column named `Not_Useful_Column` is dropped as it is not needed for analysis.

4. **Handle Missing Values:**  
   - All missing values (`NaN`) are filled with the placeholder `'-'`.
   - Specific string representations like `'N/a'` and `'NaN'` are replaced with `'-'`.

5. **Clean and Format Data:**  
   - The `Last_Name` column is cleaned by stripping unwanted characters (e.g., numbers and punctuation).
   - The `Phone_Number` column is standardized by replacing certain characters (`'/'` and `'|'`) with `'-'`.

6. **Split Address Data:**  
   The full address string is split into three separate columns: `Street_Address`, `State`, and `Zip_Code`.

7. **Standardize Binary Columns:**  
   Values in `Do_Not_Contact` and `Paying Customer` columns are standardized to:
   - `'Y'` for "Yes"
   - `'N'` for "No"

8. **Filter Records:**  
   - Records with `Do_Not_Contact` set to `'Y'` are removed.
   - Records with missing phone numbers (indicated by `'-'`) are also removed.

9. **Reset DataFrame Index:**  
   After filtering, the DataFrame index is reset to maintain consistency.

## How to Run the Script

1. **Install Pandas:**  
   Ensure that Pandas is installed in your Python environment:
   ```bash
   pip install pandas
   ```

2. **Adjust the File Path:**  
   Modify the file path in the script to point to the correct location of your `Customer Call List.xlsx` file:
   ```python
   df = pd.read_excel(r"C:\Users\Admin\Downloads\Customer Call List.xlsx")
   ```

3. **Run the Script:**  
   Execute the script in your Python environment (e.g., using an IDE, Jupyter Notebook, or the command line).


## Conclusion

This script provides a straightforward example of how to clean and preprocess data using Pandas. Adjust the file paths and column names as needed for your specific dataset.

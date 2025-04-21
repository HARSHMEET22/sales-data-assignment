## sales-data-assignment

# End-to-End Data Cleaning & Transformation Summary
- Overview of the Dataset
- The dataset contains three main sheets:
- Order File: Sales transaction details
- Product File: Product-level information
   Customer File: Customer demographic and identity data

#  This is a sales dataset, and the goal is to clean, structure, and analyze it using Excel and Power Query.

# 1) Initial Review & Format Check
- Checked all three sheets for inconsistent formatting, missing values, and incorrect data types.
-   Identified issues such as:
-   Mixed or incorrect date formats
-   Duplicate entries
-   Extra spaces or unclean font/text
-   Blank rows and columns

# 2) Date Column Cleaning (Excel Formulas)
- Used =TEXT() or =DATEVALUE() formula where necessary to standardize date columns
- Ensured all date columns (like Order Date, Delivery Date) were converted to a consistent format.

# 3)  Text Formatting & Font Cleanup 
- Used formulas like:
- =TRIM() – to remove extra spaces
- =PROPER() or =UPPER()/=LOWER() – for consistent casing
- =CLEAN() – to remove non-printable characters

# 4) Loaded Data into Power Query
- Imported all three sheets into Power Query Editor.
- This allowed better control over cleaning, transforming, and merging data.

# 5) Cleaning in Power Query
- Removed Duplicates: Used Remove Duplicates to clean records from all sheets.
- Removed Blank Rows: Applied filters or conditional logic to remove rows with missing critical info (e.g., blank Customer ID, Product ID).
- Split Columns: Used Split Column (by delimiter or position) to separate values (like names or addresses if needed).
- Changed Data Types: Ensured all columns had appropriate data types (e.g., text, date, number).
- Renamed Columns: Gave proper, readable names to columns for clarity.

# 6) Data Integration
- Merged tables:
- Order File joined with Customer File on Customer ID
- Order File joined with Product File on Product ID

#  7)  Output & Final Touch
- Loaded the cleaned and merged data back to Excel for analysis.
- Created meaningful tables with:
- Clean column headers
- Filtered views (no blanks or error values)
- Easy-to-read format
- Ensured relationships were correctly defined to avoid mismatches.

# Final Result
- A clean, de-duplicated, readable dataset
- Structured in a way that allows easy analysis and dashboard creation
- Ready for pivot tables, charts, and Power BI visualizations



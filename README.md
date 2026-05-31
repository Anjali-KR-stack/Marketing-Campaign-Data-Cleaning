Marketing Campaign Data Cleaning
Project Objective

The objective of this project is to clean and prepare a marketing campaign dataset for analysis.

Rows: 2240

Columns: 29

Cleaning Steps Performed
Converted the dataset into an Excel Table for easier filtering, sorting, and analysis.
All the data was initially loaded into a single column. Used Data → Text to Columns with Tab delimiter to split the data into separate columns.
Applied AutoFit Column Width and AutoFit Row Height to improve readability.
Checked for blank values and found missing data only in the Income column. Calculated the median Income value (58138) and filled all blank Income records using Go To Special → Blanks and Ctrl + Enter.
Checked for duplicate records and found no duplicate rows.
Converted the Dt_Customer column into proper Date format.
Identified outliers in the Year_Birth column. A few records had birth years around 1900, which were considered unrealistic for this analysis. Since there were only 3 such records, they were removed.

Removed the following columns:

Z_CostContact
Z_Revenue

These columns contained constant values and would not provide meaningful insights during analysis or visualization.

Standardized the Marital_Status column by replacing:
Absurd → Single
Alone → Single
YOLO → Single

Created a new column called Age using:

=YEAR(TODAY())-B2

Created a new column called Total_Children using:

=[@Kidhome]+[@Teenhome]

Created a new column called Total_Spending using:

=SUM(J2)

Created a new column called Total_Purchases using:

=P2+Q2+R2

New Columns Created
Age
Total_Children
Total_Spending
Total_Purchases
Final Outcome

The dataset was successfully cleaned by handling missing values, removing unnecessary columns, standardizing categorical values, and creating new analytical features. The final dataset is ready for analysis, reporting, and dashboard creation.

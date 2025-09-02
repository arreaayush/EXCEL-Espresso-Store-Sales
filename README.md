# EXCEL-Espresso-Store-Sales

📌 Project Overview

This project demonstrates various Excel data analysis techniques using an e-commerce dataset (espresso store).
The tasks cover formatting, sorting, filtering, conditional labeling, string & date functions, pivot tables, and goal-seek.
The file contains multiple sheets, each dedicated to a specific task.

📂 Contents & Example Formulas

espresso store
Base dataset containing customer, product, and order details (Order ID, Customer ID, Gender, Age, Date, Channel, Amount, Shipping Info, etc.).

** Q1_Format

Applied formatting techniques to clean and present raw data.

Conditional formatting for highlighting values.

Currency formatting for Amount.

Example:

Format → Number → Currency

Conditional Format: Highlight Amount > 1000

** Q2_SortFilter

Sorted and filtered records to analyze specific subsets of data.

Sort by Amount (Largest to Smallest).

Filter orders shipped only to Punjab.

Example:

Sort: Data → Sort by Amount

Filter: Data → Filter → Select ship-state = PUNJAB

** Q3_ShipState

Extracted and validated shipping state information.

Used formulas to clean or extract state data.

Example formula:

=PROPER(TRIM([@ship-state]))

** Q4_DemandLabel

Created demand categories based on conditions.

Used IF function to label demand.

Example:

=IF(Amount>1000,"High Demand","Least Demanded")

** Q5_CountExtract

Extracted parts of text and counted specific records.

Extracted middle part of Order ID.

Counted customers in a specific age group.

Example:

=MID(A2,5,7)      → Extract middle digits of Order ID
=COUNTIFS(Gender,"Men",Age,">=30",Age,"<=40")

** Q6_ReplaceCategory

Updated product categories using Find & Replace or formulas.

Example:

=SUBSTITUTE(Category,"kurta","kurta sets")

** Q7_DateAfter3Months

Added 3 months to each order date.

Example:

=EDATE(Date,3)

** Q8_OneWayTable

Built a one-way data table for mortgage loan calculations.

Explored how changing interest rate impacts monthly payments.

Example:

=PMT(InterestRate/12,LoanTerm,LoanAmount)

** Q9_GoalSeek

Applied Goal Seek to determine required values.

Example case: What sales amount gives $125 commission at 2.4%?

Steps:

Formula: =Sales*Commission%

Goal Seek → Set Commission Value = 125 by changing Sales

** Q10_Pivot & Chart

Created pivot tables and charts to summarize sales trends.

Summarized monthly sales (Sum of Amount).

Counted total orders per month.

Added Pivot Chart for visualization.

Example Steps:

Insert → Pivot Table → Rows = Month, Values = Amount (Sum)

Insert → Chart (Column/Line)

🛠 Skills Practiced

Data formatting & cleaning

Sorting and filtering records

Text extraction & string manipulation (MID, COUNTIFS)

Conditional logic and labeling (IF)

Find & Replace transformations (SUBSTITUTE)

Date manipulation in Excel (EDATE)

One-way data tables (PMT)

Goal Seek (What-if Analysis)

Pivot Tables & Charts

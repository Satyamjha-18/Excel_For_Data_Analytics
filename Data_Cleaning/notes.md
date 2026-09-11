# 🧹 Data Cleaning in Excel - Notes

## 📅 Day 14 - Data Cleaning

Data Cleaning is the process of finding and correcting inaccurate, incomplete, duplicate, inconsistent, or improperly formatted data.

The main goal is to convert **Raw Data → Clean Data → Analysis-Ready Data**.

---

# 📖 1. What is Data Cleaning?

Raw data often contains problems such as:

- Missing values
- Blank cells
- Extra spaces
- Duplicate records
- Inconsistent text
- Incorrect capitalization
- Different date formats
- Missing IDs
- Incorrect product names
- Invalid values
- Unnecessary columns

Before performing analysis, these problems should be identified and handled properly.

---

# 🎯 2. Data Cleaning Workflow

A basic data cleaning workflow is:

```text
Raw Data
   ↓
Identify Problems
   ↓
Handle Missing Values
   ↓
Remove Extra Spaces
   ↓
Standardize Text
   ↓
Standardize Dates
   ↓
Remove Duplicates
   ↓
Validate Data
   ↓
Transform Data
   ↓
Analyze Data
   ↓
Create Charts
```

---

# 📊 3. Inspecting Raw Data

Before cleaning data, first understand the dataset.

Check:

- Number of rows
- Number of columns
- Column names
- Data types
- Missing values
- Duplicate values
- Incorrect values
- Inconsistent formatting

### Important Rule

Do not directly modify the raw dataset.

Keep the original data as a reference and create a cleaned version.

---

# 🧹 4. Identifying Missing Values

Missing values occur when a cell does not contain any value.

Example:

| Employee ID | Name | City |
|-------------|------|------|
| 101 | Rahul | Delhi |
| 102 | Amit | |
| 103 | Priya | Mumbai |

Here, the City value for Amit is missing.

---

## Excel Method 1: Filter

### Process

```text
Select Data
   ↓
Data
   ↓
Filter
   ↓
Select Column Filter
   ↓
Select Blanks
```

This helps identify rows containing missing values.

---

## Excel Method 2: Go To Special

### Process

```text
Home
   ↓
Find & Select
   ↓
Go To Special
   ↓
Blanks
   ↓
OK
```

Excel will select blank cells.

---

# 🆔 5. Handling Missing IDs

IDs are important because they uniquely identify records.

For example:

```text
Employee ID
101
102
(blank)
104
```

Do not randomly create an ID.

### Correct approach

1. Check the original source.
2. Check whether the ID can be recovered.
3. If it is available, enter the correct ID.
4. If it cannot be determined, keep it blank or flag it.

### Important

Never invent business data just to remove blanks.

---

# ✂️ 6. Removing Extra Spaces

Raw data may contain unnecessary spaces.

Example:

```text
"  Rahul Kumar  "
```

This can create problems while searching, matching, or comparing data.

### Formula

```excel
=TRIM(A2)
```

### TRIM()

`TRIM()` removes unnecessary spaces from text.

Example:

```text
Before:
"  Rahul Kumar  "

After:
"Rahul Kumar"
```

---

# 🧹 7. Removing Non-Printable Characters

Sometimes data copied from external sources contains hidden or non-printable characters.

Use:

```excel
=CLEAN(A2)
```

### CLEAN()

`CLEAN()` removes non-printable characters from text.

It is useful when data is copied from:

- Websites
- External software
- Reports
- Other databases

---

# 🔤 8. Standardizing Text

The same value can appear in different formats.

Example:

```text
rahul
RAHUL
Rahul
```

For analysis, it is better to maintain a consistent format.

---

## PROPER()

Converts text into proper case.

```excel
=PROPER(A2)
```

Example:

```text
rahul kumar
```

Output:

```text
Rahul Kumar
```

---

## UPPER()

Converts text into uppercase.

```excel
=UPPER(A2)
```

Example:

```text
Rahul
```

Output:

```text
RAHUL
```

---

## LOWER()

Converts text into lowercase.

```excel
=LOWER(A2)
```

Example:

```text
RAHUL
```

Output:

```text
rahul
```

---

# 🔄 9. Cleaning Inconsistent Product Names

The same product may appear in different formats.

Example:

```text
Antacids
AnTACids
ANTACIDS
```

All three represent the same product.

They should be standardized into one consistent value.

---

## Method 1: Find & Replace

Shortcut:

```text
Ctrl + H
```

### Process

```text
Ctrl + H
   ↓
Find what
   ↓
Enter incorrect value
   ↓
Replace with
   ↓
Enter correct value
   ↓
Replace All
```

Example:

```text
Find:
AnTACids

Replace with:
Antacids
```

---

# 🔄 10. Standardizing Product Names

Another example:

```text
Blood THINners
```

can be standardized as:

```text
Blood Thinners
```

Consistency is important because inconsistent values can produce incorrect analysis.

For example:

```text
Antacids
AnTACids
```

may be counted as two different categories by Excel.

---

# 📅 11. Date Formatting

Dates can appear in different formats.

Example:

```text
01/02/2024
2024-02-01
1-Feb-2024
```

For analysis, dates should ideally be stored as actual Excel dates and displayed consistently.

---

## Excel Process

1. Select the date column.
2. Right-click.
3. Select **Format Cells**.
4. Select **Date**.
5. Choose the required format.
6. Click **OK**.

Example:

```text
01-Feb-2024
```

---

# 🔍 12. Checking Whether a Date is a Real Date

Sometimes a date may actually be stored as text.

A real Excel date is generally stored as a number internally.

You can test a value using:

```excel
=ISNUMBER(A2)
```

If the result is:

```text
TRUE
```

the value is numeric and may be a valid Excel date.

If:

```text
FALSE
```

the value may be stored as text.

---

# 🗑️ 13. Removing Duplicate Records

Duplicate records occur when the same record appears more than once.

Example:

| Employee ID | Name | City |
|-------------|------|------|
| 101 | Rahul | Delhi |
| 102 | Amit | Mumbai |
| 101 | Rahul | Delhi |

The first and third rows are duplicates.

---

## Excel Process

```text
Select Dataset
   ↓
Data
   ↓
Remove Duplicates
   ↓
Select Columns
   ↓
OK
```

Excel will show the number of duplicate values removed.

---

# ⚠️ 14. Important Rule for Duplicates

Do not remove duplicates blindly.

Before removing them, ask:

- Is the record actually duplicated?
- Is the repeated record valid?
- Is the same customer allowed to have multiple transactions?
- Is the same employee allowed to appear multiple times?

For example, in a sales dataset, the same customer appearing multiple times may be completely valid.

---

# 🔢 15. Zero vs Blank Values

Zero and blank values are different.

### Zero

```text
Sales = 0
```

This may mean that no sale occurred.

### Blank

```text
Sales = blank
```

This may mean:

- Data was not recorded
- Information is unavailable
- Value is missing

Therefore:

```text
0 ≠ Blank
```

Do not automatically replace zero values with blanks.

---

# 📊 16. Handling Missing Sales Values

Suppose the dataset contains:

| Product | Sales |
|---------|------:|
| Product A | 500 |
| Product B | |
| Product C | 300 |
| Product D | 0 |

Here:

- Blank = missing/unavailable
- 0 = possibly no sales

The correct treatment depends on the business requirement.

---

# 🔄 17. Data Transformation

Data Transformation means converting cleaned data into a useful structure for analysis.

Common transformations include:

- Standardizing text
- Formatting dates
- Creating calculated columns
- Renaming columns
- Removing unnecessary columns
- Replacing incorrect values
- Converting data types
- Creating analysis-ready tables

---

# 🧮 18. Useful Excel Functions for Data Cleaning

## SUM()

Calculates total.

```excel
=SUM(B2:B10)
```

---

## AVERAGE()

Calculates average.

```excel
=AVERAGE(B2:B10)
```

---

## COUNT()

Counts numeric values.

```excel
=COUNT(B2:B10)
```

---

## COUNTA()

Counts non-empty cells.

```excel
=COUNTA(A2:A10)
```

---

## COUNTIF()

Counts values based on a condition.

```excel
=COUNTIF(B2:B10,"Antacids")
```

---

## SUMIF()

Calculates the sum based on a condition.

```excel
=SUMIF(A2:A10,"Antacids",B2:B10)
```

---

# 🎨 19. Conditional Formatting for Data Checking

Conditional Formatting can help identify unusual or problematic values.

### Excel Process

```text
Select Data
   ↓
Home
   ↓
Conditional Formatting
```

Useful options include:

- Highlight Cell Rules
- Duplicate Values
- Greater Than
- Less Than
- Blank cells
- Data Bars

---

## Example: Finding Duplicates

```text
Select Column
   ↓
Home
   ↓
Conditional Formatting
   ↓
Highlight Cells Rules
   ↓
Duplicate Values
```

This makes duplicate values easier to identify before removing them.

---

# 🔎 20. Find & Replace

Find & Replace is useful for correcting inconsistent data.

Shortcut:

```text
Ctrl + H
```

Example:

```text
Find:
AnTACids

Replace:
Antacids
```

It can also be used for:

- Incorrect spellings
- Inconsistent capitalization
- Unwanted characters
- Incorrect category names

---

# 📋 21. Sorting Data

Sorting helps identify unusual or inconsistent records.

### Excel Process

```text
Select Dataset
   ↓
Data
   ↓
Sort
```

You can sort:

- A to Z
- Z to A
- Smallest to Largest
- Largest to Smallest
- Oldest to Newest
- Newest to Oldest

---

# 🔍 22. Filtering Data

Filtering displays only the records that satisfy a condition.

### Excel Process

```text
Select Dataset
   ↓
Data
   ↓
Filter
```

Examples:

- Show only blank cities
- Show only one product
- Show sales greater than 500
- Show a particular employee
- Show records from a particular date

---

# 📊 23. Creating a Clean Table

After cleaning, the dataset should have:

- Clear column names
- Consistent formatting
- Correct data types
- No unnecessary spaces
- Standardized text
- Correct dates
- Properly handled missing values
- Properly handled duplicates

The cleaned dataset becomes suitable for analysis.

---

# 📈 24. Basic Analysis After Cleaning

Once the data is cleaned, analysis can be performed.

Examples:

### Total

```excel
=SUM(B2:B100)
```

### Average

```excel
=AVERAGE(B2:B100)
```

### Minimum

```excel
=MIN(B2:B100)
```

### Maximum

```excel
=MAX(B2:B100)
```

### Number of Records

```excel
=COUNTA(A2:A100)
```

---

# 📊 25. Creating Basic Charts

Charts help visualize the cleaned data.

Common charts:

- Column Chart
- Bar Chart
- Line Chart
- Pie Chart

### Excel Process

```text
Select Clean Data
   ↓
Insert
   ↓
Charts
   ↓
Select Required Chart
```

Always create charts from the **cleaned dataset**.

---

# 🧪 26. Raw Data vs Clean Data

A major purpose of this practice is to understand the difference between raw and cleaned data.

### Raw Data

May contain:

```text
Missing Values
Extra Spaces
Inconsistent Text
Duplicate Records
Different Date Formats
Incorrect Values
```

### Clean Data

Should contain:

```text
Consistent Values
Correct Formatting
Proper Data Types
Handled Missing Values
Standardized Text
Validated Records
```

---

# 📝 27. Data Cleaning Checklist

Before considering the dataset ready for analysis, check:

- [ ] Column names are clear
- [ ] Missing values are identified
- [ ] Blank cells are reviewed
- [ ] Extra spaces are removed
- [ ] Text is standardized
- [ ] Product names are consistent
- [ ] Dates are correctly formatted
- [ ] Duplicate records are reviewed
- [ ] IDs are checked
- [ ] Zero and blank values are understood
- [ ] Data types are correct
- [ ] Unnecessary columns are removed
- [ ] Cleaned data is validated
- [ ] Analysis is performed
- [ ] Charts are created

---

# 🎯 28. Key Learning

The most important lesson from Data Cleaning is:

> **Good analysis starts with clean data.**

If the input data is incorrect or inconsistent, the final analysis and visualization can also be incorrect.

Therefore, before creating reports, dashboards, or charts, the dataset should always be checked and cleaned properly.

---

# 🚀 29. Final Data Cleaning Workflow

```text
Raw Dataset
     ↓
Understand Dataset
     ↓
Identify Data Problems
     ↓
Handle Missing Values
     ↓
Clean Extra Spaces
     ↓
Standardize Text
     ↓
Standardize Dates
     ↓
Check IDs
     ↓
Review Duplicates
     ↓
Handle Zero / Blank Values
     ↓
Transform Data
     ↓
Validate Data
     ↓
Perform Analysis
     ↓
Create Charts
     ↓
Analysis-Ready Dataset
```

---

# 🎓 Day 14 Learning Outcome

After completing Data Cleaning in Excel, I learned how to:

- Understand raw datasets
- Identify data quality problems
- Handle missing values
- Handle blank cells
- Remove extra spaces using `TRIM()`
- Clean non-printable characters using `CLEAN()`
- Standardize text using `PROPER()`, `UPPER()`, and `LOWER()`
- Handle inconsistent product names
- Standardize date formats
- Identify and remove duplicate records
- Understand the difference between zero and blank values
- Perform data transformation
- Validate cleaned data
- Perform basic analysis
- Create basic charts
- Prepare data for further Data Analytics

---
## 📌 Important Excel Shortcuts

| Shortcut   | Purpose        |
|------------|----------------|
| `Ctrl + H` | Find & Replace |
| `Ctrl + F` | Find           |
| `Ctrl + Z` | Undo           |
| `Ctrl + Y` | Redo           |
| `Ctrl + C` | Copy           |
| `Ctrl + V` | Paste          |
| `Ctrl + X` | Cut            |
| `Ctrl + S` | Save           |
| `Ctrl + A` | Select All     |

---

# 📚 Conclusion

Data Cleaning is one of the most important steps in Data Analytics.

The purpose is not simply to remove blank cells or duplicates. The real goal is to make sure that the data is:

```text
Accurate
Consistent
Complete
Valid
Structured
Analysis-Ready
```
After cleaning the data, it can be safely used for:

- Excel Analysis
- Pivot Tables
- Dashboards
- Power BI
- SQL Analysis
- Data Visualization
- Machine Learning
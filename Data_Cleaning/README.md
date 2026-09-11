# 📊 Data Cleaning in Excel

## 📖 Introduction

Data Cleaning is the process of identifying, correcting, removing, and standardizing incorrect, incomplete, duplicate, or inconsistent data.

Clean data is important because it improves:

- Data Accuracy
- Data Consistency
- Data Analysis
- Reporting
- Visualization
- Decision Making

This project demonstrates practical **Data Cleaning and Transformation using Microsoft Excel**.

---

## 🎯 Objective

The main objective of this project is to clean raw datasets and transform them into structured and analysis-ready data.

This project covers:

- Missing Values
- Blank Cells
- Inconsistent Text
- Extra Spaces
- Different Date Formats
- Missing IDs
- Inconsistent Product Names
- Zero and Missing Values
- Data Transformation
- Basic Analysis
- Basic Charts

---

## 📁 Workbook Structure

The Excel workbook contains the following sheets:

1. **Un Clean Data**
2. **claened data_01**
3. **Unclean Data**
4. **Clean data_02**
5. **Clean and Tranformed table**
6. **Basic chart**

The workbook contains both raw and cleaned datasets to compare the data before and after cleaning.

---

## 🧹 Data Cleaning Techniques

### 1. Handling Missing Values

Missing values occur when some cells do not contain any data.

Example:

| Employee ID | Name | City |
|-------------|------|------|
| 101 | Rahul | Delhi |
| 102 | Amit | |
| | Priya | Mumbai |

### Common Approaches

- Identify missing values
- Filter blank cells
- Fill values when reliable information is available
- Remove rows when appropriate
- Keep blanks when the value is genuinely unknown

### Excel Process

```text
Data → Filter
```

Then filter the required column and select **Blanks**.

Another method:

```text
Home → Find & Select → Go To Special → Blanks
```

---

## ✂️ 2. Removing Extra Spaces

Sometimes text contains unnecessary spaces.

Example:

```text
"  Rahul Kumar  "
```

Use:

```excel
=TRIM(A2)
```

### TRIM()

The `TRIM()` function removes unnecessary spaces from text.

---

## 🧹 3. Cleaning Non-Printable Characters

The `CLEAN()` function removes non-printable characters from text.

```excel
=CLEAN(A2)
```

It is useful when data is copied from external systems.

---

## 🔤 4. Standardizing Text

Text may appear in different formats.

Example:

```text
rahul
RAHUL
Rahul
```

These values can be standardized using Excel text functions.

### PROPER()

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

### UPPER()

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

### LOWER()

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

## 🔄 5. Handling Inconsistent Data

The same value may be written in different ways.

Example:

```text
Antacids
AnTACids
ANTACIDS
```

These values represent the same product but have inconsistent formatting.

They should be standardized into one format.

### Excel Process

1. Select the dataset.
2. Go to **Home**.
3. Select **Find & Replace** or press `Ctrl + H`.
4. Enter the incorrect value.
5. Enter the standardized value.
6. Click **Replace All**.

---

## 📅 6. Standardizing Date Formats

Dates may appear in different formats.

Example:

```text
01/02/2024
2024-02-01
1-Feb-2024
```

For proper analysis, dates should follow a consistent format.

### Excel Process

1. Select the date column.
2. Right-click → **Format Cells**.
3. Select **Date**.
4. Choose the required format.
5. Click **OK**.

A consistent date format makes sorting, filtering, and date calculations easier.

---

## 🆔 7. Handling Missing Employee IDs

Employee IDs are important identifiers.

If an Employee ID is missing:

- Do not randomly create an ID.
- Check the original source.
- If the correct ID is available, update it.
- If the value cannot be determined, keep it blank or flag it based on the business requirement.

Data should never be changed without a valid reason.

---

## 🗑️ 8. Removing Duplicate Records

Duplicate records can affect analysis and produce incorrect results.

### Excel Process

1. Select the dataset.
2. Go to **Data**.
3. Click **Remove Duplicates**.
4. Select the columns to check.
5. Click **OK**.

Excel will identify and remove duplicate records.

---

## 🔢 9. Handling Zero and Missing Values

Zero and blank values are not always the same.

### Zero

A zero can represent an actual value.

Example:

```text
Sales = 0
```

This may mean that no sale occurred.

### Blank

A blank may mean:

- Data is missing
- Data was not recorded
- Information is unavailable

Therefore, zero values should not automatically be replaced with blanks or vice versa.

---

## 🧪 10. Data Transformation

Data transformation means converting cleaned data into a useful structure for analysis.

Common transformations include:

- Standardizing text
- Formatting dates
- Creating calculated columns
- Removing unnecessary columns
- Renaming columns
- Replacing incorrect values
- Converting data types
- Creating analysis-ready tables

---

## 📊 11. Basic Data Analysis

After cleaning the dataset, basic analysis can be performed.

Examples:

- Total Records
- Total Sales
- Average Sales
- Minimum Value
- Maximum Value
- Number of Products
- Number of Employees
- Category-wise Analysis

Common Excel functions:

```excel
=SUM()
=AVERAGE()
=COUNT()
=COUNTA()
=MIN()
=MAX()
=COUNTIF()
=SUMIF()
```

---

## 📈 12. Basic Charts

Charts help visualize cleaned data.

Common charts include:

- Column Chart
- Bar Chart
- Line Chart
- Pie Chart

### Excel Process

1. Select the cleaned data.
2. Go to **Insert**.
3. Select the required chart.
4. Add a suitable chart title.
5. Format the chart if required.

Charts should be created from clean and structured data.

---

## 🛠️ Excel Tools Used

The following Excel features are useful for data cleaning:

- Sort
- Filter
- Find & Replace
- Go To Special
- Remove Duplicates
- Format Cells
- Text Functions
- Date Functions
- Conditional Formatting
- Excel Formulas
- Charts

---

## 🔍 Data Cleaning Workflow

```text
Raw Data
   ↓
Identify Data Issues
   ↓
Handle Missing Values
   ↓
Remove Extra Spaces
   ↓
Standardize Text
   ↓
Standardize Dates
   ↓
Handle Duplicates
   ↓
Transform Data
   ↓
Validate Cleaned Data
   ↓
Perform Analysis
   ↓
Create Charts
```

---

## 📌 Key Excel Functions

| Function | Purpose |
|----------|---------|
| `TRIM()` | Removes extra spaces |
| `CLEAN()` | Removes non-printable characters |
| `PROPER()` | Converts text to proper case |
| `UPPER()` | Converts text to uppercase |
| `LOWER()` | Converts text to lowercase |
| `SUM()` | Calculates total |
| `AVERAGE()` | Calculates average |
| `COUNT()` | Counts numeric values |
| `COUNTA()` | Counts non-empty cells |
| `MIN()` | Finds minimum value |
| `MAX()` | Finds maximum value |
| `COUNTIF()` | Counts values based on a condition |
| `SUMIF()` | Calculates sum based on a condition |

---

## 🎯 Learning Outcomes

After completing this project, I learned how to:

- Identify problems in raw data
- Handle missing and blank values
- Remove unnecessary spaces
- Standardize text values
- Clean inconsistent product names
- Handle date formatting
- Identify duplicate records
- Understand zero vs missing values
- Transform raw data into structured data
- Perform basic data analysis
- Create basic charts
- Prepare data for further analytics

---

## 🚀 Project Goal

The goal of this project is to build a strong foundation in **Excel Data Cleaning and Data Preparation** for Data Analytics.

Clean and structured data is the first step toward creating reliable:

- Reports
- Dashboards
- Business Analysis
- Data Visualizations
- Data Analytics Projects

---
## 👨‍💻 Author

**Satyam Kumar**

B.Tech CSE (AIML) | Aspiring Data Analyst & Data Scientist

GitHub: **Satyamjha-18**
# 📊 Excel for Data Analytics - Complete Notes

These notes cover my daily practical learning of Microsoft Excel for Data Analytics.

The topics are organized day-wise from Excel fundamentals to lookup functions, including INDEX & MATCH.

---

# 📅 Day 01 - Introduction to Excel & Data Formatting

## 📖 What is Microsoft Excel?

Microsoft Excel is a spreadsheet application used to store, organize, calculate, analyze, and visualize data.

Excel is widely used in:

- Data Analytics
- Finance
- Business Intelligence
- Reporting
- Sales Analysis
- HR Analytics
- Financial Analysis
- Data Cleaning

---

## 📌 Excel Interface

Important components of Excel:

### Workbook

A workbook is an Excel file that contains one or more worksheets.

Example:

`Sales_Analysis.xlsx`

### Worksheet

A worksheet is an individual sheet inside a workbook.

Example:

- Sales
- Customers
- Products

### Rows

Rows are identified by numbers.

Example:

`1, 2, 3, 4...`

### Columns

Columns are identified by letters.

Example:

`A, B, C, D...`

### Cell

The intersection of a row and a column is called a cell.

Example:

`A1`

### Name Box

The Name Box displays the address of the selected cell.

Example:

`B5`

It can also be used to quickly select a cell or range.

### Formula Bar

The Formula Bar displays or allows editing of the content/formula of the selected cell.

### Ribbon

The Ribbon contains Excel tools and commands organized into tabs.

Examples:

- Home
- Insert
- Page Layout
- Formulas
- Data
- Review
- View

### Status Bar

The Status Bar displays information about the selected data.

It can show:

- Average
- Count
- Sum

---

# 🎨 Data Formatting

Formatting means changing the appearance of data to make it clear and professional.

## Font Formatting

Common options:

- Font type
- Font size
- Bold
- Italic
- Underline

Example:

```text
Product Name
```

can be made bold for a table heading.

---

## Alignment

Alignment controls the position of content inside a cell.

Types:

- Left
- Center
- Right
- Top
- Middle
- Bottom

---

## Borders

Borders help separate data and improve table readability.

Common borders:

- All Borders
- Outside Borders
- Bottom Border
- Thick Borders

---

## Fill Color

Fill Color adds background color to cells.

It is commonly used for:

- Headers
- Important values
- KPI sections
- Categories

---

## Merge & Center

Merge & Center combines multiple cells into one cell and centers the content.

Example:

```text
A1:D1
```

can be merged to create a report title.

---

## Wrap Text

Wrap Text displays long text on multiple lines inside the same cell.

Useful when:

- Column width is limited
- Headers are long
- Descriptions contain large text

---

## Number Formatting

Number formatting controls how numbers are displayed.

Examples:

- Number
- Currency
- Percentage
- Date
- Time

Example:

```text
1000
```

can be displayed as:

```text
₹1,000
```

or:

```text
1,000.00
```

---

## 🎯 Day 01 Learning Outcomes

After completing Day 01, I can:

- Understand the Excel interface
- Understand workbook and worksheet
- Work with rows, columns, and cells
- Format data professionally
- Apply borders and alignment
- Use number formatting
- Create and save Excel workbooks

---

# 📅 Day 02 - Workbook, Worksheet, Cells & Data Entry

## 📖 Workbook

A workbook is the complete Excel file.

Example:

```text
Employee_Data.xlsx
```

A workbook can contain multiple worksheets.

---

## 📖 Worksheet

A worksheet is a single working area inside a workbook.

Example:

```text
Workbook
│
├── Employees
├── Sales
└── Products
```

---

## 📌 Creating a Worksheet

A new worksheet can be created using the `+` button at the bottom of Excel.

Worksheets can also be:

- Renamed
- Moved
- Copied
- Deleted
- Hidden

---

## 📌 Rows and Columns

Rows are horizontal and identified by numbers.

Columns are vertical and identified by letters.

Example:

```text
       A       B       C
1    Name    Age     City
2    Rahul   22      Delhi
3    Aman    24      Pune
```

---

## 📌 Cell and Cell Range

A single cell:

```text
A1
```

A range:

```text
A1:C5
```

A range represents multiple cells.

---

## 📥 Data Entry

Excel allows different types of data:

- Text
- Numbers
- Dates
- Time
- Percentages
- Currency

Example:

| Name | Age | Salary |
|---|---:|---:|
| Rahul | 22 | 25000 |
| Aman | 24 | 30000 |

---

## ✏️ Editing Data

Data can be edited by:

- Double-clicking a cell
- Using the Formula Bar
- Selecting the cell and pressing `F2`

---

## 📋 Copy and Paste

Common shortcuts:

```text
Ctrl + C → Copy
Ctrl + V → Paste
Ctrl + X → Cut
```

---

## ➕ Insert Rows and Columns

Rows and columns can be inserted when additional data is required.

---

## ❌ Delete Rows and Columns

Unnecessary rows and columns can be deleted without deleting the entire worksheet.

---

## 🎯 Day 02 Learning Outcomes

- Create and manage workbooks
- Create and manage worksheets
- Work with cells and ranges
- Enter and edit data
- Copy and paste data
- Insert and delete rows and columns
- Apply basic formatting

---

# 📅 Day 03 - Sorting, Filtering & Data Types

## 📊 Sorting

Sorting means arranging data in a particular order.

Common sorting types:

- Ascending
- Descending

---

## 🔼 Ascending Order

For numbers:

```text
10
20
30
40
```

For text:

```text
Aman
Rahul
Satyam
```

---

## 🔽 Descending Order

For numbers:

```text
40
30
20
10
```

For text:

```text
Satyam
Rahul
Aman
```

---

## 📌 Custom Sorting

Custom Sort allows sorting using multiple columns.

Example:

First sort by:

```text
Department
```

Then by:

```text
Salary
```

---

## 🔎 Filtering

Filtering displays only the records that satisfy a condition.

Example:

If a dataset contains employees from:

```text
Delhi
Mumbai
Pune
Bangalore
```

we can filter only:

```text
Delhi
```

---

## 📌 Data Types

Common Excel data types:

### Text

Example:

```text
Rahul
Sales
Delhi
```

### Number

Example:

```text
100
2500
99.5
```

### Date

Example:

```text
01/08/2026
```

### Time

Example:

```text
10:30 AM
```

### Percentage

Example:

```text
75%
```

### Currency

Example:

```text
₹50,000
```

---

## 🎯 Day 03 Learning Outcomes

- Sort data
- Apply ascending and descending sorting
- Apply filters
- Use custom sorting
- Understand Excel data types
- Apply suitable data formatting
- Prepare data for analysis

---

# 📅 Day 04 - Basic Formulas & Arithmetic Functions

## 📖 What is a Formula?

A formula is an expression used to perform calculations in Excel.

Every formula starts with:

```text
=
```

Example:

```excel
=A1+B1
```

---

# ➕ Arithmetic Operators

## Addition

```excel
=A1+B1
```

## Subtraction

```excel
=A1-B1
```

## Multiplication

```excel
=A1*B1
```

## Division

```excel
=A1/B1
```

---

## 📌 SUM Function

SUM calculates the total of numbers.

### Syntax

```excel
=SUM(A1:A10)
```

Example:

```excel
=SUM(B2:B10)
```

---

## 📌 AVERAGE Function

AVERAGE calculates the average value.

### Syntax

```excel
=AVERAGE(A1:A10)
```

Example:

```excel
=AVERAGE(B2:B10)
```

---

## 📌 MIN Function

MIN returns the smallest value.

### Syntax

```excel
=MIN(A1:A10)
```

---

## 📌 MAX Function

MAX returns the largest value.

### Syntax

```excel
=MAX(A1:A10)
```

---

## 🧮 Example

| Product | Sales |
|---|---:|
| A | 100 |
| B | 200 |
| C | 300 |

Total:

```excel
=SUM(B2:B4)
```

Average:

```excel
=AVERAGE(B2:B4)
```

Minimum:

```excel
=MIN(B2:B4)
```

Maximum:

```excel
=MAX(B2:B4)
```

---

## 🎯 Day 04 Learning Outcomes

- Create Excel formulas
- Perform arithmetic calculations
- Use SUM
- Use AVERAGE
- Find minimum values
- Find maximum values

---

# 📅 Day 05 - Text Functions

Text functions are used to extract, modify, clean, and combine text data.

---

## 📌 LEFT Function

LEFT returns characters from the beginning of a text string.

### Syntax

```excel
=LEFT(text,num_chars)
```

Example:

```excel
=LEFT("Satyam",3)
```

Result:

```text
Sat
```

---

## 📌 RIGHT Function

RIGHT returns characters from the end of a text string.

### Syntax

```excel
=RIGHT(text,num_chars)
```

Example:

```excel
=RIGHT("Satyam",3)
```

Result:

```text
yam
```

---

## 📌 MID Function

MID extracts characters from the middle of a text string.

### Syntax

```excel
=MID(text,start_num,num_chars)
```

Example:

```excel
=MID("Analytics",2,4)
```

---

## 📌 LEN Function

LEN returns the number of characters in a text string.

### Syntax

```excel
=LEN(text)
```

Example:

```excel
=LEN("Excel")
```

Result:

```text
5
```

---

## 📌 UPPER Function

Converts text into uppercase.

```excel
=UPPER("excel")
```

Result:

```text
EXCEL
```

---

## 📌 LOWER Function

Converts text into lowercase.

```excel
=LOWER("EXCEL")
```

Result:

```text
excel
```

---

## 📌 TRIM Function

TRIM removes unnecessary spaces from text.

```excel
=TRIM(A2)
```

Useful for cleaning datasets.

---

## 📌 CONCAT Function

CONCAT combines text values.

```excel
=CONCAT(A2,B2)
```

---

## 📌 CONCATENATE Function

CONCATENATE combines multiple text values.

```excel
=CONCATENATE(A2," ",B2)
```

Example:

```text
First Name = Rahul
Last Name = Kumar
```

Formula:

```excel
=CONCATENATE(A2," ",B2)
```

Result:

```text
Rahul Kumar
```

---

## 🎯 Day 05 Learning Outcomes

- Extract text
- Modify text
- Change text case
- Remove unnecessary spaces
- Combine text values
- Clean text-based datasets

---

# 📅 Day 06 - Count Functions & Cell Referencing

# 🔢 Count Functions

## 📌 COUNT

COUNT counts cells containing numbers.

### Syntax

```excel
=COUNT(A1:A10)
```

Example:

```text
10
20
Rahul
30
```

COUNT returns:

```text
3
```

---

## 📌 COUNTA

COUNTA counts non-empty cells.

### Syntax

```excel
=COUNTA(A1:A10)
```

It counts:

- Numbers
- Text
- Dates
- Other non-empty values

---

## 📌 COUNTBLANK

COUNTBLANK counts empty cells.

### Syntax

```excel
=COUNTBLANK(A1:A10)
```

---

## 📌 COUNTIF

COUNTIF counts cells based on one condition.

### Syntax

```excel
=COUNTIF(range,criteria)
```

Example:

```excel
=COUNTIF(B2:B20,">50000")
```

This counts salaries greater than 50,000.

---

## 📌 COUNTIFS

COUNTIFS counts cells based on multiple conditions.

### Syntax

```excel
=COUNTIFS(range1,criteria1,range2,criteria2)
```

Example:

```excel
=COUNTIFS(B2:B20,"Sales",C2:C20,">50000")
```

---

# 📌 Cell Referencing

Cell referencing defines which cells are used in a formula.

There are three major types:

1. Relative Reference
2. Absolute Reference
3. Mixed Reference

---

## 🔹 Relative Reference

Example:

```excel
=A1+B1
```

When copied down, it changes automatically.

```excel
=A2+B2
```

---

## 🔒 Absolute Reference

An absolute reference remains fixed when copied.

Example:

```excel
=$A$1
```

The `$` symbol locks the row and column.

---

## 🔀 Mixed Reference

A mixed reference locks either the row or the column.

### Fixed Column

```excel
=$A1
```

Column A is fixed.

### Fixed Row

```excel
=A$1
```

Row 1 is fixed.

---

## 🎯 Day 06 Learning Outcomes

- Use COUNT
- Use COUNTA
- Use COUNTBLANK
- Use COUNTIF
- Use COUNTIFS
- Understand relative references
- Understand absolute references
- Understand mixed references
- Use `$` in formulas

---

# 📅 Day 07 - Date & Time Functions

Excel provides functions to work with dates and times.

---

## 📌 TODAY

TODAY returns the current date.

```excel
=TODAY()
```

Example result:

```text
01/09/2026
```

The actual result changes according to the current date.

---

## 📌 NOW

NOW returns the current date and time.

```excel
=NOW()
```

---

## 📌 DATE

DATE creates a date from year, month, and day.

### Syntax

```excel
=DATE(year,month,day)
```

Example:

```excel
=DATE(2026,9,1)
```

---

## 📌 DAY

DAY extracts the day from a date.

```excel
=DAY(A2)
```

---

## 📌 MONTH

MONTH extracts the month.

```excel
=MONTH(A2)
```

---

## 📌 YEAR

YEAR extracts the year.

```excel
=YEAR(A2)
```

---

## 📅 Date Formatting

Dates can be displayed in different formats.

Example:

```text
01/09/2026
1-Sep-2026
September 1, 2026
```

---

## ⏰ Time Formatting

Time can be displayed as:

```text
10:30 AM
10:30:45 AM
22:30
```

---

## 📌 Basic Date Calculation

Example:

```excel
=B2-A2
```

This can calculate the number of days between two dates.

---

## 🎯 Day 07 Learning Outcomes

- Work with dates
- Work with time
- Use TODAY
- Use NOW
- Create dates using DATE
- Extract day, month, and year
- Format dates and times
- Perform basic date calculations

---

# 📅 Day 08 - IF, IFS & Nested IF

Logical functions are used to make decisions based on conditions.

---

# 📌 IF Function

IF checks a condition and returns one value if TRUE and another if FALSE.

### Syntax

```excel
=IF(logical_test,value_if_true,value_if_false)
```

Example:

```excel
=IF(B2>=40,"Pass","Fail")
```

If marks are 40 or above:

```text
Pass
```

Otherwise:

```text
Fail
```

---

# 📌 IFS Function

IFS evaluates multiple conditions.

### Syntax

```excel
=IFS(condition1,result1,condition2,result2,...)
```

Example:

```excel
=IFS(
B2>=90,"A",
B2>=75,"B",
B2>=60,"C",
B2>=40,"D",
B2<40,"Fail"
)
```

---

# 📌 Nested IF

Nested IF means using one IF function inside another IF function.

Example:

```excel
=IF(B2>=90,"A",
IF(B2>=75,"B",
IF(B2>=60,"C",
IF(B2>=40,"D","Fail"))))
```

---

## 📌 Conditional Calculation

Example:

```excel
=IF(C2="Yes",B2*10%,0)
```

If condition is TRUE, the calculation is performed.

---

## 🎯 Day 08 Learning Outcomes

- Use IF
- Use IFS
- Create Nested IF
- Apply conditional calculations
- Work with multiple conditions
- Perform decision-making using Excel formulas

---

# 📅 Day 09 - Logical Operators & Functions

Logical functions are used to evaluate multiple conditions.

---

# 📌 AND Function

AND returns TRUE when all conditions are TRUE.

### Syntax

```excel
=AND(condition1,condition2,...)
```

Example:

```excel
=AND(B2>=40,C2>=40)
```

Both conditions must be TRUE.

---

# 📌 OR Function

OR returns TRUE when at least one condition is TRUE.

### Syntax

```excel
=OR(condition1,condition2,...)
```

Example:

```excel
=OR(B2>=40,C2>=40)
```

Only one condition needs to be TRUE.

---

# 📌 NOT Function

NOT reverses a logical result.

### Syntax

```excel
=NOT(condition)
```

Example:

```excel
=NOT(B2="Yes")
```

---

# 📌 Combining Logical Functions with IF

AND with IF:

```excel
=IF(AND(B2>=40,C2>=40),"Pass","Fail")
```

OR with IF:

```excel
=IF(OR(B2>=40,C2>=40),"Eligible","Not Eligible")
```

NOT with IF:

```excel
=IF(NOT(B2="No"),"Approved","Rejected")
```

---

## 📌 Logical Operators

Excel supports:

| Operator | Meaning |
|---|---|
| `=` | Equal to |
| `<>` | Not equal to |
| `>` | Greater than |
| `<` | Less than |
| `>=` | Greater than or equal to |
| `<=` | Less than or equal to |

---

## 🎯 Day 09 Learning Outcomes

- Understand logical operators
- Use AND
- Use OR
- Use NOT
- Combine logical functions with IF
- Work with multiple conditions

---

# 📅 Day 10 - Lookup Functions

Lookup functions are used to search for a value in a dataset and return related information.

Main lookup functions:

- VLOOKUP
- HLOOKUP
- LOOKUP

---

# 🔎 VLOOKUP

VLOOKUP means Vertical Lookup.

It searches for a value vertically in the first column of a table and returns a value from another column.

### Syntax

```excel
=VLOOKUP(lookup_value,table_array,col_index_num,[range_lookup])
```

---

## 📌 Example

Suppose we have:

| ID | Name | Salary |
|---|---|---:|
| 101 | Rahul | 30000 |
| 102 | Aman | 35000 |
| 103 | Ravi | 40000 |

Formula:

```excel
=VLOOKUP(102,A2:C4,2,FALSE)
```

Result:

```text
Aman
```

---

## 📌 Exact Match

Use:

```excel
FALSE
```

or:

```excel
0
```

Example:

```excel
=VLOOKUP(102,A2:C4,2,FALSE)
```

---

## 📌 Approximate Match

Use:

```excel
TRUE
```

or:

```excel
1
```

Approximate match is generally used with sorted lookup data.

---

# 🔎 HLOOKUP

HLOOKUP means Horizontal Lookup.

It searches for a value horizontally across the first row of a table.

### Syntax

```excel
=HLOOKUP(lookup_value,table_array,row_index_num,[range_lookup])
```

---

## 📌 Example

```text
        A       B       C
1      Jan     Feb     Mar
2      100     200     300
```

Formula:

```excel
=HLOOKUP("Feb",A1:C2,2,FALSE)
```

Result:

```text
200
```

---

# 🔎 LOOKUP

LOOKUP searches for a value in one row or column and returns the corresponding value from another row or column.

### Syntax

```excel
=LOOKUP(lookup_value,lookup_vector,result_vector)
```

Example:

```excel
=LOOKUP(102,A2:A4,B2:B4)
```

---

## 📌 Lookup Functions Comparison

| Function | Search Direction |
|---|---|
| VLOOKUP | Vertical |
| HLOOKUP | Horizontal |
| LOOKUP | Vector-based |

---

## 🎯 Day 10 Learning Outcomes

- Understand lookup functions
- Use VLOOKUP
- Use HLOOKUP
- Use LOOKUP
- Understand exact match
- Understand approximate match
- Retrieve information from datasets

---

# 📅 Day 11 - XLOOKUP

## 📖 What is XLOOKUP?

XLOOKUP is a modern Excel lookup function used to search for a value in one range and return the corresponding value from another range.

It is more flexible than traditional VLOOKUP and HLOOKUP.

---

## 📌 XLOOKUP Syntax

```excel
=XLOOKUP(lookup_value,lookup_array,return_array)
```

---

## 📌 Parameters

### lookup_value

The value that we want to search.

Example:

```text
102
```

### lookup_array

The range where Excel searches for the value.

Example:

```excel
=A2:A10
```

### return_array

The range from which Excel returns the result.

Example:

```excel
=B2:B10
```

---

## 📌 Basic Example

Dataset:

| ID | Name | Salary |
|---|---|---:|
| 101 | Rahul | 30000 |
| 102 | Aman | 35000 |
| 103 | Ravi | 40000 |

Formula:

```excel
=XLOOKUP(102,A2:A4,B2:B4)
```

Result:

```text
Aman
```

---

## 📌 XLOOKUP with Not Found Message

XLOOKUP allows a custom message when the lookup value is not found.

### Syntax

```excel
=XLOOKUP(lookup_value,lookup_array,return_array,"Not Found")
```

Example:

```excel
=XLOOKUP(105,A2:A4,B2:B4,"Employee Not Found")
```

Result:

```text
Employee Not Found
```

---

## 📌 Exact Match

XLOOKUP uses exact match by default.

Example:

```excel
=XLOOKUP(102,A2:A4,B2:B4)
```

---

## 📌 Vertical Lookup

XLOOKUP can perform vertical lookup.

```excel
=XLOOKUP(E2,A2:A10,B2:B10)
```

---

## 📌 Horizontal Lookup

XLOOKUP can also perform horizontal lookup.

Example:

```excel
=XLOOKUP("Feb",B1:D1,B2:D2)
```

---

## 📌 XLOOKUP Advantages

Compared with VLOOKUP:

- Can lookup to the left
- Does not require column index number
- Exact match is default
- Supports custom not-found messages
- Can perform vertical lookup
- Can perform horizontal lookup
- More flexible lookup structure

---

## 🎯 Day 11 Learning Outcomes

- Understand XLOOKUP
- Understand lookup value
- Understand lookup array
- Understand return array
- Perform exact-match lookup
- Handle missing values
- Perform vertical lookup
- Perform horizontal lookup
- Retrieve data efficiently

---

# 📅 Day 12 - INDEX & MATCH Functions

INDEX and MATCH are powerful Excel functions used together for flexible data lookup.

They are commonly used as an alternative to traditional VLOOKUP.

---

# 🔎 INDEX Function

INDEX returns a value from a specific position in a range.

### Syntax

```excel
=INDEX(array,row_num)
```

For a two-dimensional range:

```excel
=INDEX(array,row_num,column_num)
```

---

## 📌 Basic INDEX Example

Suppose:

| A |
|---|
| Rahul |
| Aman |
| Ravi |

Formula:

```excel
=INDEX(A2:A4,2)
```

Result:

```text
Aman
```

Because Aman is the second value in the range.

---

## 📌 INDEX with Row and Column

Suppose:

| Name | City | Salary |
|---|---|---:|
| Rahul | Delhi | 30000 |
| Aman | Pune | 35000 |
| Ravi | Mumbai | 40000 |

Formula:

```excel
=INDEX(A2:C4,2,3)
```

Result:

```text
35000
```

Explanation:

- Row 2 → Aman
- Column 3 → Salary
- Result → 35000

---

# 🔎 MATCH Function

MATCH searches for a value in a range and returns its position.

### Syntax

```excel
=MATCH(lookup_value,lookup_array,match_type)
```

---

## 📌 Match Type

### Exact Match

Use:

```excel
0
```

Example:

```excel
=MATCH("Aman",A2:A4,0)
```

If Aman is the second item, the result is:

```text
2
```

---

## 📌 Approximate Match

MATCH also supports:

```text
1
0
-1
```

For most exact lookup situations, use:

```excel
0
```

---

# 🔗 INDEX + MATCH

INDEX and MATCH can be combined to perform a flexible lookup.

Suppose:

| ID | Name | Salary |
|---|---|---:|
| 101 | Rahul | 30000 |
| 102 | Aman | 35000 |
| 103 | Ravi | 40000 |

We want to find the salary of ID `102`.

Formula:

```excel
=INDEX(C2:C4,MATCH(102,A2:A4,0))
```

---

## 📌 How INDEX + MATCH Works

First MATCH finds the position:

```excel
=MATCH(102,A2:A4,0)
```

Result:

```text
2
```

Then INDEX uses that position:

```excel
=INDEX(C2:C4,2)
```

Result:

```text
35000
```

So the complete formula is:

```excel
=INDEX(C2:C4,MATCH(102,A2:A4,0))
```

---

# 📌 INDEX + MATCH for Name Lookup

To find the name for ID `103`:

```excel
=INDEX(B2:B4,MATCH(103,A2:A4,0))
```

Result:

```text
Ravi
```

---

# 📌 Two-Way Lookup

INDEX + MATCH can be used for two-way lookup.

Two-way lookup means finding a value using both:

- Row
- Column

Example:

| Product | Jan | Feb | Mar |
|---|---:|---:|---:|
| A | 100 | 200 | 300 |
| B | 150 | 250 | 350 |
| C | 120 | 220 | 320 |

A two-way lookup can find the value based on:

```text
Product = B
Month = Feb
```

Formula:

```excel
=INDEX(B2:D4,MATCH("B",A2:A4,0),MATCH("Feb",B1:D1,0))
```

Result:

```text
250
```

---

# 📌 Dynamic Data Lookup

INDEX + MATCH is useful when the lookup column and return column are separate and may change.

It provides more flexibility than traditional VLOOKUP.

---

# 📌 INDEX + MATCH vs VLOOKUP

| Feature | VLOOKUP | INDEX + MATCH |
|---|---|---|
| Vertical lookup | Yes | Yes |
| Lookup to left | No | Yes |
| Flexible lookup | Limited | High |
| Column index required | Yes | No |
| Two-way lookup | Limited | Yes |
| Dynamic lookup | Limited | Yes |

---

# 📌 INDEX + MATCH vs XLOOKUP

| Feature | INDEX + MATCH | XLOOKUP |
|---|---|---|
| Flexible lookup | Yes | Yes |
| Left lookup | Yes | Yes |
| Exact match | Yes | Yes |
| Two-way lookup | Yes | Yes |
| Easy syntax | Moderate | Easy |
| Modern Excel | Works | Works |

---

# 🧠 Important Points to Remember

## INDEX

INDEX returns a value based on its position.

```excel
=INDEX(range,row_num)
```

---

## MATCH

MATCH returns the position of a value.

```excel
=MATCH(lookup_value,lookup_array,0)
```

---

## INDEX + MATCH

MATCH finds the position and INDEX returns the value from that position.

```excel
=INDEX(return_range,MATCH(lookup_value,lookup_range,0))
```

---

# 🎯 Day 12 Learning Outcomes

After completing Day 12, I can:

- Understand INDEX
- Understand MATCH
- Use INDEX independently
- Use MATCH independently
- Combine INDEX and MATCH
- Perform exact-match lookup
- Perform two-way lookup
- Perform flexible data lookup
- Use INDEX + MATCH as an alternative to VLOOKUP

---

# 📈 Excel Learning Progress

- [x] Day 01 - Introduction & Data Formatting
- [x] Day 02 - Workbook, Worksheet & Data Entry
- [x] Day 03 - Sorting, Filtering & Data Types
- [x] Day 04 - Basic Formulas & Functions
- [x] Day 05 - Text Functions
- [x] Day 06 - Count Functions & Cell Referencing
- [x] Day 07 - Date & Time Functions
- [x] Day 08 - IF, IFS & Nested IF
- [x] Day 09 - Logical Operators & Functions
- [x] Day 10 - VLOOKUP, HLOOKUP & LOOKUP
- [x] Day 11 - XLOOKUP
- [x] Day 12 - INDEX & MATCH

---

# 📂 Workbook Structure

All practical Excel exercises are maintained in a single Excel workbook.

The workbook contains daily practical exercises based on the topics covered during the learning process.

---

# 🛠️ Tools Used

- Microsoft Excel
- Visual Studio Code
- Git
- GitHub

---
# 🎯 Goal

The goal of this learning series is to develop practical Excel skills for Data Analytics and build a strong foundation for working with real-world datasets, reports, dashboards, and business analysis.

⭐ Learning Excel one day at a time with practical implementation.
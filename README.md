# Data-Cleaning-Projects
# 🧹 Data Cleaning Project — U.S. Presidents Dataset

## 📌 Project Overview

This project demonstrates a real-world data cleaning workflow applied to a U.S. Presidents dataset containing historical records of all 45 presidents, including their prior roles, political party, vice president, and salary.

The raw dataset contained several quality issues — duplicates, encoding errors, typos, and improperly formatted dates — that were identified, documented, and resolved to produce a clean, analysis-ready Excel file.

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `US_Presidents_Raw.xlsx` | Original dataset before cleaning |
| `US_Presidents_Cleaned_v2.xlsx` | Final cleaned dataset (with ReadMe sheet) |
| `README.md` | Project documentation (this file) |

---

## 🔍 Issues Found in the Raw Data

| # | Issue | Details |
|---|-------|---------|
| 1 | **Unnamed index column** | Auto-generated column with no analytical value |
| 2 | **Empty row** | Row 47 contained null values across all fields |
| 3 | **Duplicate rows** | Woodrow Wilson (#28) and Barack Obama (#44) each appeared twice |
| 4 | **Encoding artifacts** | Text encoding errors (e.g., `â€"`) appeared in date ranges within the `prior` column |
| 5 | **Excess whitespace** | Multiple consecutive spaces in `president`, `prior`, `party`, and `vice` columns |
| 6 | **Inconsistent casing** | President names stored in ALL CAPS |
| 7 | **Party column errors** | 4 distinct issues: extra spacing, typo (`Demorcatic`), wrong plural (`Republicans`), and embedded date data in Whig entry |
| 8 | **Date formatting** | `date updated` and `date created` stored as Excel serial numbers (e.g., `44391`) instead of readable dates |

---

## ✅ Cleaning Steps Applied

### Step 1 — Removed Unnamed Index Column
Deleted the redundant auto-generated index column that duplicated the `S.No.` field.

### Step 2 — Deleted Empty Rows
Removed 1 empty row (former row 47) with null values to ensure the dataset is continuous — equivalent to manually deleting blank rows in Excel.

### Step 3 — Fixed Text Encoding Errors
Replaced garbled character sequences (e.g., `â€"`) with proper dashes (`–`) across all text columns — equivalent to using **Find & Replace (Ctrl+H)** in Excel.

### Step 4 — Cleaned Excess Whitespace
Collapsed multiple consecutive spaces into single spaces and stripped leading/trailing spaces across all text fields.

### Step 5 — Standardised President Names
Converted ALL-CAPS names to Title Case (e.g., `GEORGE WASHINGTON` → `George Washington`).

### Step 6 — Corrected Party Name Errors
Fixed 4 issues:
- `Democratic-  Republican` → `Democratic-Republican` (extra spaces)
- `Demorcatic` → `Democratic` (typo)
- `Republicans` → `Republican` (wrong plural)
- Removed embedded date text from John Tyler's `Whig` entry

### Step 7 — Removed Duplicate Rows
Removed 2 duplicate rows using Excel's **Data > Remove Duplicates** logic. Duplicates were detected *after* text cleaning to ensure typo variations (e.g., `Demorcatic` vs `Democratic`) didn't mask identical records.

### Step 8 — Converted Date Columns
Converted Excel serial numbers in `date updated` and `date created` to readable calendar dates (e.g., `44391` → `2021-07-14`).

---

## 📊 Before vs. After

| Metric | Raw Data | Cleaned Data |
|--------|----------|--------------|
| Rows | 47 | 45 |
| Columns | 9 | 8 |
| Duplicate rows | 2 | 0 |
| Empty rows | 1 | 0 |
| Encoding errors | Yes | No |
| Readable dates | No | Yes |
| Standardised casing | No | Yes |

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data inspection and structure review,# 🧹 Data Cleaning Project — U.S. Presidents Dataset

## 📌 Project Overview

This project demonstrates a real-world data cleaning workflow applied to a U.S. Presidents dataset containing historical records of all 45 presidents, including their prior roles, political party, vice president, and salary.

The raw dataset contained several quality issues — duplicates, encoding errors, typos, and improperly formatted dates — that were identified, documented, and resolved to produce a clean, analysis-ready Excel file.

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `US_Presidents_Raw.xlsx` | Original dataset before cleaning |
| `US_Presidents_Cleaned_v2.xlsx` | Final cleaned dataset (with ReadMe sheet) |
| `README.md` | Project documentation (this file) |

---

## 🔍 Issues Found in the Raw Data

| # | Issue | Details |
|---|-------|---------|
| 1 | **Unnamed index column** | Auto-generated column with no analytical value |
| 2 | **Empty row** | Row 47 contained null values across all fields |
| 3 | **Duplicate rows** | Woodrow Wilson (#28) and Barack Obama (#44) each appeared twice |
| 4 | **Encoding artifacts** | Text encoding errors (e.g., `â€"`) appeared in date ranges within the `prior` column |
| 5 | **Excess whitespace** | Multiple consecutive spaces in `president`, `prior`, `party`, and `vice` columns |
| 6 | **Inconsistent casing** | President names stored in ALL CAPS |
| 7 | **Party column errors** | 4 distinct issues: extra spacing, typo (`Demorcatic`), wrong plural (`Republicans`), and embedded date data in Whig entry |
| 8 | **Date formatting** | `date updated` and `date created` stored as Excel serial numbers (e.g., `44391`) instead of readable dates |

---

## ✅ Cleaning Steps Applied

### Step 1 — Removed Unnamed Index Column
Deleted the redundant auto-generated index column that duplicated the `S.No.` field.

### Step 2 — Deleted Empty Rows
Removed 1 empty row (former row 47) with null values to ensure the dataset is continuous — equivalent to manually deleting blank rows in Excel.

### Step 3 — Fixed Text Encoding Errors
Replaced garbled character sequences (e.g., `â€"`) with proper dashes (`–`) across all text columns — equivalent to using **Find & Replace (Ctrl+H)** in Excel.

### Step 4 — Cleaned Excess Whitespace
Collapsed multiple consecutive spaces into single spaces and stripped leading/trailing spaces across all text fields.

### Step 5 — Standardised President Names
Converted ALL-CAPS names to Title Case (e.g., `GEORGE WASHINGTON` → `George Washington`).

### Step 6 — Corrected Party Name Errors
Fixed 4 issues:
- `Democratic-  Republican` → `Democratic-Republican` (extra spaces)
- `Demorcatic` → `Democratic` (typo)
- `Republicans` → `Republican` (wrong plural)
- Removed embedded date text from John Tyler's `Whig` entry

### Step 7 — Removed Duplicate Rows
Removed 2 duplicate rows using Excel's **Data > Remove Duplicates** logic. Duplicates were detected *after* text cleaning to ensure typo variations (e.g., `Demorcatic` vs `Democratic`) didn't mask identical records.

### Step 8 — Converted Date Columns
Converted Excel serial numbers in `date updated` and `date created` to readable calendar dates (e.g., `44391` → `2021-07-14`).

---

## 📊 Before vs. After

| Metric | Raw Data | Cleaned Data |
|--------|----------|--------------|
| Rows | 47 | 45 |
| Columns | 9 | 8 |
| Duplicate rows | 2 | 0 |
| Empty rows | 1 | 0 |
| Encoding errors | Yes | No |
| Readable dates | No | Yes |
| Standardised casing | No | Yes |

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data inspection, structure review, Automated cleaning and formatted output
  
---
## 👤 Author

**Seyi Oyediran Data Analyst | 3MTT Fellow

- 🔗 [LinkedIn](https://www.linkedin.com/in/) 
- 💼 [Upwork Profile](https://www.upwork.com/)

---

*This project is part of my ongoing data analytics portfolio. Feel free to fork, use, or reach out with feedback!*

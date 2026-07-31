# 📊 Power BI DAX Calculated Tables - Adventure Works Analysis

Welcome to the **Power BI DAX Calculated Tables** project! This repository contains a practical data modeling project built using **Power BI Desktop** and **DAX (Data Analysis Expressions)** applied to the standard **Adventure Works** dataset.

---

## 📌 Project Overview
The main objective of this project is to demonstrate the use of **Calculated Tables (`New Table`)** in Power BI for custom data segmentation, cloned table references, and optimized data summaries without altering the original source data structure.

---

## 🛠️ Key DAX Calculated Tables Implemented

### 1. Table Cloning (`ALL`)
* **Syntax:**
  ```dax
  Sales Clone = ALL(Sales)
  ```
* **Description:** Creates an exact duplicate of the `Sales` table while ignoring any active filter contexts. Useful for comparative analysis and reference tables.

---

### 2. Segmented Data Table (`FILTER`)
* **Syntax:**
  ```dax
  Canada Sales = FILTER(Sales, Sales[Sales Country] = "Canada")
  ```
* **Description:** Generates a filtered table containing only transactions from **Canada**, streamlining focused regional analysis.

---

### 3. Summarized & Aggregated Table (`SUMMARIZE`)
* **Syntax:**
  ```dax
  Anual Sales = 
  SUMMARIZE(
      Sales, 
      Sales[Sales Country], 
      Products[Category], 
      "Sales", SUM(Sales[Total Price])
  )
  ```
* **Description:** Builds a summary matrix grouping total revenue by `Sales Country` and `Category`.

---

## 📁 Repository Files
```text
├── AdventureWorksData.xlsx                 # Raw Source Data (Excel)
├── 1.pbix                                  # Power BI Data Model & Dashboard
└── README.md                               # Project Documentation
```



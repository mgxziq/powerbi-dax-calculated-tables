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

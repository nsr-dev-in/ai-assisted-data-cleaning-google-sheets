# AI-Assisted Data Cleaning with Google Sheets

## 📊 Project Overview

This project is a practical data cleaning exercise completed as part of my **Data Analyst with AI Internship – Masterclass 1**.

The goal was to transform a messy e-commerce dataset containing **1,000+ order records** into a cleaner, consistent, and analysis-ready dataset using **Google Sheets, AI-assisted prompts, and manual validation**.

---

## 🎯 Objectives

- Identify and handle missing values
- Detect duplicate records
- Standardize inconsistent data
- Clean and convert currency values into numeric format
- Standardize date formats
- Clean city names
- Standardize payment methods
- Standardize order statuses
- Handle negative quantity values
- Validate AI-generated cleaning results manually

---

## 🛠️ Tools & Technologies

- **Google Sheets**
- **AI-assisted prompting**
- **Data Cleaning**
- **Data Validation**
- **Manual Data Quality Checks**

---

## 🧹 Data Cleaning Performed

### 1. Missing Values

Identified missing values across important columns such as:

- Customer_ID
- Email
- Order_Date
- Quantity
- Unit_Price

Where possible, values were recovered using reliable information from other columns. Values that could not be reliably determined were not randomly invented.

### 2. Date Standardization

Converted inconsistent date formats into a consistent:

`DD/MM/YYYY`

format.

### 3. Currency Cleaning

Cleaned values containing:

- `₹`
- `INR`
- Commas

and converted them into numeric values.

Example:

`₹1,299` → `1299`

`INR 1,599` → `1599`

### 4. City Standardization

Standardized inconsistent city names and capitalization.

Examples:

`delhi` → `Delhi`

`mumbai` → `Mumbai`

`pune` → `Pune`

`Bengaluru` / `Bangalore` → `Bengaluru`

### 5. Payment Method Standardization

Standardized variations such as:

`upi` → `UPI`

`credit card` → `Credit Card`

`COD` / `cod` → `Cash on Delivery`

### 6. Order Status Standardization

Standardized variations such as:

`delivered` / `DELIVERED` → `Delivered`

`shipped` → `Shipped`

`pending` → `Pending`

`cancelled` → `Cancelled`

### 7. Quantity Cleaning

Negative quantities were converted to their positive equivalent.

Example:

`-3` → `3`

Positive quantities were left unchanged.

---

## 🤖 Role of AI

AI was used to assist with repetitive data-cleaning tasks through structured prompts.

However, the cleaning process was **not fully automated**.

I manually reviewed and validated the results to ensure that:

- Data was not unnecessarily modified
- Missing information was not invented
- Standardization rules were applied consistently
- Cleaned values remained logically correct

### Key Learning

> **AI can make data cleaning faster, but it cannot replace an analyst's judgment.**

---

## 📈 Dataset

The project uses a messy e-commerce orders dataset containing:

- **1,000+ records**
- **13 columns**

### Main Columns

| Column | Description |
|---|---|
| Order_ID | Unique order identifier |
| Customer_ID | Customer identifier |
| Customer_Name | Customer name |
| Email | Customer email |
| Order_Date | Order date |
| Product | Purchased product |
| Category | Product category |
| Quantity | Number of units |
| Unit_Price | Price per unit |
| Total_Amount | Total order amount |
| City | Customer city |
| Payment_Method | Payment method |
| Order_Status | Order fulfillment status |

---

## 📂 Project Structure

```text
ai-assisted-data-cleaning-google-sheets/
│
├── Raw_Data.csv
├── Cleaned_Data.csv
├── README.md
└── Cleaning_Log

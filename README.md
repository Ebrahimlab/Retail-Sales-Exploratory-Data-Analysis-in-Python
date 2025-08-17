# Retail-Sales-Exploratory-Data-Analysis-in-Python

This project analyzes a fictional but realistic retail sales dataset to uncover customer purchasing patterns, category preferences, and seasonal spending trends.
The dataset includes:
**Transaction ID, Date, Customer ID, Gender, Age, Product Category, Quantity, Price per Unit, Total Amount**

Although the data is synthetic, the analysis methods and insights are directly applicable to real-world retail data, helping businesses optimize marketing, inventory, and customer engagement strategies.

**Business Questions Addressed**
1. **Customer Demographics & Spending** — How does age and gender influence total purchase amounts?
2. **Product Category Preferences** — Which category is most purchased by each age-gender group?
3. **Time-Based Spending Trends** — How do sales vary by day and month across product categories, customer counts, and gender?

**Dataset Overview**:
- **Rows**: 1,000
- **Columns**: 9
- **Unique Transactions**: 1,000
- **Unique Customers**: 1,000
- **Unique Dates**: 345 (multiple customers purchased on the same dates)
- **Categories**: Beauty, Clothing, Electronics
- **Missing Values**: None

**Data Preparation**
- Converted Date to datetime format
- Verified column uniqueness
- Confirmed no missing values


**Analysis 1 — Spending by Age & Gender**
Grouped data by **Age** and **Gender** to calculate total spending.

**Example Pattern**:

- Females aged 18 spent more than males of the same age
- Males aged 22 outspent females significantly

**Visualization**:

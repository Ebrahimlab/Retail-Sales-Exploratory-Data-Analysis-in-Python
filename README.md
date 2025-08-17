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
("C:\Users\mebrh\OneDrive\Desktop\Retail-Sales-EDA-in-Python-main\Barplot of Total Spending by Age and Gender.png" )



**Analysis 2 — Top Product Category by Age & Gender**
Examined **category-level spending** for each demographic segment.

**Key Findings**:

- Younger shoppers (18–25) prefer Beauty & Clothing
- Older demographics lean towards Electronics
- Males dominate Electronics spending, females lead in Beauty purchases



**Analysis 3 — Monthly Spending Patterns**
Grouped transactions by month to assess seasonal and category-specific trends.

**Findings**:

1. **Spending Fluctuations**:
- Peak in May (53,150) — 42% above average
- Low in September (23,620) — seasonal dip
- Q4 surge (Oct–Dec) above 35K

2. **Category Shifts**:
- Electronics led in 8 of 12 months
- Beauty peaked in Jan & Jul
- Clothing dominated Feb–Apr

3. **Customer Traffic**:
- Highest: May (105 customers)
- Lowest: September (65 customers)

4. **Gender Trends**:
- Females outspent males in 7 months
- Males led during Electronics-heavy months

**Visualization**:

("C:\Users\mebrh\OneDrive\Desktop\Retail-Sales-EDA-in-Python-main\Lineplot of Total Monthly Spending Trend by Gender.png")




**Conclusion**
Three core findings:

1. **Gender-Driven Behavior** — clear category preferences by gender
2. **Age Influence** — younger buyers focus on Beauty/Clothing, older on Electronics
3. **Seasonality** — predictable peaks in May and Q4, dips in September



